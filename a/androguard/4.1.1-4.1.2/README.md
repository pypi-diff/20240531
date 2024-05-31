# Comparing `tmp/androguard-4.1.1.tar.gz` & `tmp/androguard-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "androguard-4.1.1.tar", max compression
+gzip compressed data, was "androguard-4.1.2.tar", max compression
```

## Comparing `androguard-4.1.1.tar` & `androguard-4.1.2.tar`

### file list

```diff
@@ -1,120 +1,120 @@
--rw-r--r--   0        0        0    10174 2024-03-14 22:24:40.735909 androguard-4.1.1/LICENCE-2.0
--rw-r--r--   0        0        0     3967 2024-03-14 22:24:40.735909 androguard-4.1.1/README.md
--rw-r--r--   0        0        0      156 2024-03-14 22:24:40.735909 androguard-4.1.1/androguard/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 22:24:40.735909 androguard-4.1.1/androguard/cli/__init__.py
--rwxr-xr-x   0        0        0    16794 2024-03-14 22:24:40.735909 androguard-4.1.1/androguard/cli/cli.py
--rw-r--r--   0        0        0    17413 2024-03-14 22:24:40.735909 androguard-4.1.1/androguard/cli/main.py
--rw-r--r--   0        0        0        0 2024-03-14 22:24:40.735909 androguard-4.1.1/androguard/core/__init__.py
--rw-r--r--   0        0        0        1 2024-03-14 22:24:40.735909 androguard-4.1.1/androguard/core/analysis/__init__.py
--rw-r--r--   0        0        0    77072 2024-03-14 22:24:40.735909 androguard-4.1.1/androguard/core/analysis/analysis.py
--rw-r--r--   0        0        0     7007 2024-03-14 22:24:40.735909 androguard-4.1.1/androguard/core/androconf.py
--rw-r--r--   0        0        0     3267 2024-03-14 22:24:40.735909 androguard-4.1.1/androguard/core/api_specific_resources/__init__.py
--rw-r--r--   0        0        0    72874 2024-03-14 22:24:40.735909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_10.json
--rw-r--r--   0        0        0    74153 2024-03-14 22:24:40.735909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_13.json
--rw-r--r--   0        0        0    83838 2024-03-14 22:24:40.735909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_14.json
--rw-r--r--   0        0        0    85210 2024-03-14 22:24:40.735909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_15.json
--rw-r--r--   0        0        0    92149 2024-03-14 22:24:40.735909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_16.json
--rw-r--r--   0        0        0   107091 2024-03-14 22:24:40.735909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_17.json
--rw-r--r--   0        0        0   111302 2024-03-14 22:24:40.735909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_18.json
--rw-r--r--   0        0        0   121871 2024-03-14 22:24:40.735909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_19.json
--rw-r--r--   0        0        0   138882 2024-03-14 22:24:40.739909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_21.json
--rw-r--r--   0        0        0   142552 2024-03-14 22:24:40.739909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_22.json
--rw-r--r--   0        0        0   109896 2024-03-14 22:24:40.739909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_23.json
--rw-r--r--   0        0        0   120102 2024-03-14 22:24:40.739909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_24.json
--rw-r--r--   0        0        0   120261 2024-03-14 22:24:40.739909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_25.json
--rw-r--r--   0        0        0   130585 2024-03-14 22:24:40.739909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_26.json
--rw-r--r--   0        0        0   136413 2024-03-14 22:24:40.739909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_27.json
--rw-r--r--   0        0        0   152916 2024-03-14 22:24:40.739909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_28.json
--rw-r--r--   0        0        0   179247 2024-03-14 22:24:40.739909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_29.json
--rw-r--r--   0        0        0   195808 2024-03-14 22:24:40.739909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_30.json
--rw-r--r--   0        0        0   227446 2024-03-14 22:24:40.743909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_31.json
--rw-r--r--   0        0        0   228655 2024-03-14 22:24:40.743909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_32.json
--rw-r--r--   0        0        0   254150 2024-03-14 22:24:40.743909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_33.json
--rw-r--r--   0        0        0   303365 2024-03-14 22:24:40.743909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_34.json
--rw-r--r--   0        0        0    61160 2024-03-14 22:24:40.743909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_4.json
--rw-r--r--   0        0        0    64832 2024-03-14 22:24:40.743909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_5.json
--rw-r--r--   0        0        0    64832 2024-03-14 22:24:40.743909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_6.json
--rw-r--r--   0        0        0    64832 2024-03-14 22:24:40.743909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_7.json
--rw-r--r--   0        0        0    70158 2024-03-14 22:24:40.743909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_8.json
--rw-r--r--   0        0        0    71331 2024-03-14 22:24:40.743909 androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_9.json
--rw-r--r--   0        0        0   179196 2024-03-14 22:24:40.743909 androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_16.json
--rw-r--r--   0        0        0   214407 2024-03-14 22:24:40.743909 androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_17.json
--rw-r--r--   0        0        0   224135 2024-03-14 22:24:40.743909 androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_18.json
--rw-r--r--   0        0        0   220470 2024-03-14 22:24:40.743909 androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_19.json
--rw-r--r--   0        0        0   334121 2024-03-14 22:24:40.747909 androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_21.json
--rw-r--r--   0        0        0   310636 2024-03-14 22:24:40.747909 androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_22.json
--rw-r--r--   0        0        0   246635 2024-03-14 22:24:40.747909 androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_23.json
--rw-r--r--   0        0        0   369549 2024-03-14 22:24:40.747909 androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_24.json
--rw-r--r--   0        0        0   377172 2024-03-14 22:24:40.747909 androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_25.json
--rw-r--r--   0        0        0    79921 2024-03-14 22:24:40.747909 androguard-4.1.1/androguard/core/apk/__init__.py
--rw-r--r--   0        0        0   116375 2024-03-14 22:24:40.747909 androguard-4.1.1/androguard/core/axml/__init__.py
--rw-r--r--   0        0        0     1980 2024-03-14 22:24:40.747909 androguard-4.1.1/androguard/core/axml/types.py
--rw-r--r--   0        0        0    28131 2024-03-14 22:24:40.747909 androguard-4.1.1/androguard/core/bytecode.py
--rw-r--r--   0        0        0   264541 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/core/dex/__init__.py
--rw-r--r--   0        0        0     5971 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/core/dex/dex_types.py
--rw-r--r--   0        0        0      121 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/core/mutf8/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/core/resources/__init__.py
--rw-r--r--   0        0        0   106820 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/core/resources/public.json
--rw-r--r--   0        0        0     2011 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/core/resources/public.py
--rw-r--r--   0        0        0   191207 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/core/resources/public.xml
--rw-r--r--   0        0        0       40 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/decompiler/__init__.py
--rw-r--r--   0        0        0    10902 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/decompiler/basic_blocks.py
--rw-r--r--   0        0        0    15110 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/decompiler/control_flow.py
--rw-r--r--   0        0        0    23613 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/decompiler/dast.py
--rw-r--r--   0        0        0    20008 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/decompiler/dataflow.py
--rw-r--r--   0        0        0    20838 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/decompiler/decompile.py
--rw-r--r--   0        0        0     2802 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/decompiler/decompiler.py
--rw-r--r--   0        0        0    18344 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/decompiler/graph.py
--rw-r--r--   0        0        0    38005 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/decompiler/instruction.py
--rw-r--r--   0        0        0     4788 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/decompiler/node.py
--rw-r--r--   0        0        0    61404 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/decompiler/opcode_ins.py
--rw-r--r--   0        0        0     6103 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/decompiler/util.py
--rw-r--r--   0        0        0    26421 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/decompiler/writer.py
--rw-r--r--   0        0        0     6936 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/misc.py
--rw-r--r--   0        0        0    10596 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/pentest/__init__.py
--rw-r--r--   0        0        0      210 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/pentest/adb.py
--rw-r--r--   0        0        0    22842 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/pentest/internal/utils.js
--rw-r--r--   0        0        0     8549 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/pentest/modules/binder/intercept_binder.js
--rw-r--r--   0        0        0     2857 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/pentest/modules/code_loading/dex.js
--rw-r--r--   0        0        0     4153 2024-03-14 22:24:40.751909 androguard-4.1.1/androguard/pentest/modules/code_loading/dyndex.js
--rw-r--r--   0        0        0      841 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/code_loading/load_class.js
--rw-r--r--   0        0        0      723 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/code_loading/native.js
--rw-r--r--   0        0        0     1011 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/compression/gzip.js
--rw-r--r--   0        0        0     1076 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/encoding/base64.js
--rw-r--r--   0        0        0     3353 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/encryption/cipher.js
--rw-r--r--   0        0        0     2945 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/file_system/shared_preferences.js
--rw-r--r--   0        0        0      432 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/framework/cordova.js
--rw-r--r--   0        0        0     1768 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/framework/flutter/disable_cert_chain_bypass_v7a.js
--rw-r--r--   0        0        0     1749 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/framework/flutter/disable_cert_chain_bypass_v8a.js
--rw-r--r--   0        0        0     1786 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/framework/flutter/disable_cert_chain_bypass_x86_64.js
--rw-r--r--   0        0        0     2351 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/helpers/antidebug/binaries.js
--rw-r--r--   0        0        0      358 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/helpers/antidebug/debug.js
--rw-r--r--   0        0        0     3976 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/helpers/antidebug/environment.js
--rw-r--r--   0        0        0     2752 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/helpers/antidebug/package.js
--rw-r--r--   0        0        0     9174 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/helpers/antidebug/process.js
--rw-r--r--   0        0        0     4317 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/helpers/dump/dexdump.js
--rw-r--r--   0        0        0    30140 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/helpers/pinning/ssl.js
--rw-r--r--   0        0        0     1816 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/http_communications/uri.js
--rw-r--r--   0        0        0     5507 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/intents/intents.js
--rw-r--r--   0        0        0     6236 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/intents/intents_creation.js
--rw-r--r--   0        0        0     1892 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/intents/pending_intents.js
--rw-r--r--   0        0        0     5888 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/ipc/ipc.js
--rw-r--r--   0        0        0     4216 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/sockets/sockets.js
--rw-r--r--   0        0        0     3281 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/pentest/modules/webviews/webviews.js
--rw-r--r--   0        0        0    13655 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/session.py
--rw-r--r--   0        0        0     8494 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/ui/__init__.py
--rw-r--r--   0        0        0     2743 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/ui/data_types.py
--rw-r--r--   0        0        0     2110 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/ui/filter.py
--rw-r--r--   0        0        0     5311 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/ui/selection.py
--rw-r--r--   0        0        0    24274 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/ui/table.py
--rw-r--r--   0        0        0      204 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/ui/util.py
--rw-r--r--   0        0        0        0 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/ui/widget/__init__.py
--rw-r--r--   0        0        0     1990 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/ui/widget/details.py
--rw-r--r--   0        0        0     2399 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/ui/widget/filters.py
--rw-r--r--   0        0        0     3999 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/ui/widget/frame.py
--rw-r--r--   0        0        0     1291 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/ui/widget/help.py
--rw-r--r--   0        0        0      981 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/ui/widget/toolbar.py
--rw-r--r--   0        0        0     4681 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/ui/widget/transactions.py
--rw-r--r--   0        0        0     3103 2024-03-14 22:24:40.755909 androguard-4.1.1/androguard/util.py
--rw-r--r--   0        0        0     1032 2024-03-14 22:24:40.763909 androguard-4.1.1/pyproject.toml
--rw-r--r--   0        0        0     5099 1970-01-01 00:00:00.000000 androguard-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10174 2024-05-31 05:25:37.874580 androguard-4.1.2/LICENCE-2.0
+-rw-r--r--   0        0        0     3967 2024-05-31 05:25:37.878580 androguard-4.1.2/README.md
+-rw-r--r--   0        0        0      156 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/cli/__init__.py
+-rwxr-xr-x   0        0        0    16999 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/cli/cli.py
+-rw-r--r--   0        0        0    17914 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/cli/main.py
+-rw-r--r--   0        0        0        0 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/core/__init__.py
+-rw-r--r--   0        0        0        1 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/core/analysis/__init__.py
+-rw-r--r--   0        0        0    81620 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/core/analysis/analysis.py
+-rw-r--r--   0        0        0     7397 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/core/androconf.py
+-rw-r--r--   0        0        0     3378 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/core/api_specific_resources/__init__.py
+-rw-r--r--   0        0        0    72874 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_10.json
+-rw-r--r--   0        0        0    74153 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_13.json
+-rw-r--r--   0        0        0    83838 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_14.json
+-rw-r--r--   0        0        0    85210 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_15.json
+-rw-r--r--   0        0        0    92149 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_16.json
+-rw-r--r--   0        0        0   107091 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_17.json
+-rw-r--r--   0        0        0   111302 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_18.json
+-rw-r--r--   0        0        0   121871 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_19.json
+-rw-r--r--   0        0        0   138882 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_21.json
+-rw-r--r--   0        0        0   142552 2024-05-31 05:25:37.878580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_22.json
+-rw-r--r--   0        0        0   109896 2024-05-31 05:25:37.882580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_23.json
+-rw-r--r--   0        0        0   120102 2024-05-31 05:25:37.882580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_24.json
+-rw-r--r--   0        0        0   120261 2024-05-31 05:25:37.882580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_25.json
+-rw-r--r--   0        0        0   130585 2024-05-31 05:25:37.882580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_26.json
+-rw-r--r--   0        0        0   136413 2024-05-31 05:25:37.882580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_27.json
+-rw-r--r--   0        0        0   152916 2024-05-31 05:25:37.882580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_28.json
+-rw-r--r--   0        0        0   179247 2024-05-31 05:25:37.882580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_29.json
+-rw-r--r--   0        0        0   195808 2024-05-31 05:25:37.882580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_30.json
+-rw-r--r--   0        0        0   227446 2024-05-31 05:25:37.882580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_31.json
+-rw-r--r--   0        0        0   228655 2024-05-31 05:25:37.882580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_32.json
+-rw-r--r--   0        0        0   254150 2024-05-31 05:25:37.886580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_33.json
+-rw-r--r--   0        0        0   303365 2024-05-31 05:25:37.886580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_34.json
+-rw-r--r--   0        0        0    61160 2024-05-31 05:25:37.886580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_4.json
+-rw-r--r--   0        0        0    64832 2024-05-31 05:25:37.886580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_5.json
+-rw-r--r--   0        0        0    64832 2024-05-31 05:25:37.886580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_6.json
+-rw-r--r--   0        0        0    64832 2024-05-31 05:25:37.886580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_7.json
+-rw-r--r--   0        0        0    70158 2024-05-31 05:25:37.886580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_8.json
+-rw-r--r--   0        0        0    71331 2024-05-31 05:25:37.886580 androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_9.json
+-rw-r--r--   0        0        0   179196 2024-05-31 05:25:37.886580 androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_16.json
+-rw-r--r--   0        0        0   214407 2024-05-31 05:25:37.886580 androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_17.json
+-rw-r--r--   0        0        0   224135 2024-05-31 05:25:37.886580 androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_18.json
+-rw-r--r--   0        0        0   220470 2024-05-31 05:25:37.886580 androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_19.json
+-rw-r--r--   0        0        0   334121 2024-05-31 05:25:37.890580 androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_21.json
+-rw-r--r--   0        0        0   310636 2024-05-31 05:25:37.890580 androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_22.json
+-rw-r--r--   0        0        0   246635 2024-05-31 05:25:37.890580 androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_23.json
+-rw-r--r--   0        0        0   369549 2024-05-31 05:25:37.890580 androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_24.json
+-rw-r--r--   0        0        0   377172 2024-05-31 05:25:37.890580 androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_25.json
+-rw-r--r--   0        0        0    83683 2024-05-31 05:25:37.890580 androguard-4.1.2/androguard/core/apk/__init__.py
+-rw-r--r--   0        0        0   121101 2024-05-31 05:25:37.890580 androguard-4.1.2/androguard/core/axml/__init__.py
+-rw-r--r--   0        0        0     1980 2024-05-31 05:25:37.890580 androguard-4.1.2/androguard/core/axml/types.py
+-rw-r--r--   0        0        0    29198 2024-05-31 05:25:37.890580 androguard-4.1.2/androguard/core/bytecode.py
+-rw-r--r--   0        0        0   277084 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/core/dex/__init__.py
+-rw-r--r--   0        0        0     5971 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/core/dex/dex_types.py
+-rw-r--r--   0        0        0      121 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/core/mutf8/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/core/resources/__init__.py
+-rw-r--r--   0        0        0   106820 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/core/resources/public.json
+-rw-r--r--   0        0        0     2011 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/core/resources/public.py
+-rw-r--r--   0        0        0   191207 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/core/resources/public.xml
+-rw-r--r--   0        0        0       40 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/decompiler/__init__.py
+-rw-r--r--   0        0        0    10972 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/decompiler/basic_blocks.py
+-rw-r--r--   0        0        0    15110 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/decompiler/control_flow.py
+-rw-r--r--   0        0        0    23652 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/decompiler/dast.py
+-rw-r--r--   0        0        0    20008 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/decompiler/dataflow.py
+-rw-r--r--   0        0        0    21447 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/decompiler/decompile.py
+-rw-r--r--   0        0        0     3321 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/decompiler/decompiler.py
+-rw-r--r--   0        0        0    18344 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/decompiler/graph.py
+-rw-r--r--   0        0        0    38005 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/decompiler/instruction.py
+-rw-r--r--   0        0        0     4788 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/decompiler/node.py
+-rw-r--r--   0        0        0    61404 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/decompiler/opcode_ins.py
+-rw-r--r--   0        0        0     6463 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/decompiler/util.py
+-rw-r--r--   0        0        0    26436 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/decompiler/writer.py
+-rw-r--r--   0        0        0     7361 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/misc.py
+-rw-r--r--   0        0        0    10596 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/__init__.py
+-rw-r--r--   0        0        0      210 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/adb.py
+-rw-r--r--   0        0        0    22842 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/internal/utils.js
+-rw-r--r--   0        0        0     8549 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/modules/binder/intercept_binder.js
+-rw-r--r--   0        0        0     2857 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/modules/code_loading/dex.js
+-rw-r--r--   0        0        0     4153 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/modules/code_loading/dyndex.js
+-rw-r--r--   0        0        0      841 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/modules/code_loading/load_class.js
+-rw-r--r--   0        0        0      723 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/modules/code_loading/native.js
+-rw-r--r--   0        0        0     1011 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/modules/compression/gzip.js
+-rw-r--r--   0        0        0     1076 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/modules/encoding/base64.js
+-rw-r--r--   0        0        0     3353 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/modules/encryption/cipher.js
+-rw-r--r--   0        0        0     2945 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/modules/file_system/shared_preferences.js
+-rw-r--r--   0        0        0      432 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/modules/framework/cordova.js
+-rw-r--r--   0        0        0     1768 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/modules/framework/flutter/disable_cert_chain_bypass_v7a.js
+-rw-r--r--   0        0        0     1749 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/modules/framework/flutter/disable_cert_chain_bypass_v8a.js
+-rw-r--r--   0        0        0     1786 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/modules/framework/flutter/disable_cert_chain_bypass_x86_64.js
+-rw-r--r--   0        0        0     2351 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/modules/helpers/antidebug/binaries.js
+-rw-r--r--   0        0        0      358 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/modules/helpers/antidebug/debug.js
+-rw-r--r--   0        0        0     3976 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/modules/helpers/antidebug/environment.js
+-rw-r--r--   0        0        0     2752 2024-05-31 05:25:37.894580 androguard-4.1.2/androguard/pentest/modules/helpers/antidebug/package.js
+-rw-r--r--   0        0        0     9174 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/pentest/modules/helpers/antidebug/process.js
+-rw-r--r--   0        0        0     4317 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/pentest/modules/helpers/dump/dexdump.js
+-rw-r--r--   0        0        0    30140 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/pentest/modules/helpers/pinning/ssl.js
+-rw-r--r--   0        0        0     1816 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/pentest/modules/http_communications/uri.js
+-rw-r--r--   0        0        0     5507 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/pentest/modules/intents/intents.js
+-rw-r--r--   0        0        0     6236 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/pentest/modules/intents/intents_creation.js
+-rw-r--r--   0        0        0     1892 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/pentest/modules/intents/pending_intents.js
+-rw-r--r--   0        0        0     5888 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/pentest/modules/ipc/ipc.js
+-rw-r--r--   0        0        0     4216 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/pentest/modules/sockets/sockets.js
+-rw-r--r--   0        0        0     3281 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/pentest/modules/webviews/webviews.js
+-rw-r--r--   0        0        0    14414 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/session.py
+-rw-r--r--   0        0        0     8494 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/ui/__init__.py
+-rw-r--r--   0        0        0     2743 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/ui/data_types.py
+-rw-r--r--   0        0        0     2110 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/ui/filter.py
+-rw-r--r--   0        0        0     5311 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/ui/selection.py
+-rw-r--r--   0        0        0    24274 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/ui/table.py
+-rw-r--r--   0        0        0      204 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/ui/util.py
+-rw-r--r--   0        0        0        0 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/ui/widget/__init__.py
+-rw-r--r--   0        0        0     1990 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/ui/widget/details.py
+-rw-r--r--   0        0        0     2399 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/ui/widget/filters.py
+-rw-r--r--   0        0        0     3999 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/ui/widget/frame.py
+-rw-r--r--   0        0        0     1291 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/ui/widget/help.py
+-rw-r--r--   0        0        0      981 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/ui/widget/toolbar.py
+-rw-r--r--   0        0        0     4681 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/ui/widget/transactions.py
+-rw-r--r--   0        0        0     3284 2024-05-31 05:25:37.898580 androguard-4.1.2/androguard/util.py
+-rw-r--r--   0        0        0      989 2024-05-31 05:25:37.902580 androguard-4.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5053 1970-01-01 00:00:00.000000 androguard-4.1.2/PKG-INFO
```

### Comparing `androguard-4.1.1/LICENCE-2.0` & `androguard-4.1.2/LICENCE-2.0`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/README.md` & `androguard-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/cli/cli.py` & `androguard-4.1.2/androguard/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,14 +252,15 @@
     help='output directory. If the output folder already exsist, '
          'it will be overwritten!',
 )
 @click.option(
     '--format', '-f', 'format_',
     help='Additionally write control flow graphs for each method, specify '
          'the format for example png, jpg, raw (write dot file), ...',
+    type=click.Choice(['png', 'jpg', 'raw'])
 )
 @click.option(
     '--jar', '-j',
     is_flag=True,
     default=False,
     help='Use DEX2JAR to create a JAR file',
 )
@@ -547,15 +548,14 @@
     Create a call graph based on the data of Analysis and export it into a graph format.
     """
     from androguard.core.bytecode import FormatClassToJava
     from androguard.misc import AnalyzeAPK
     from androguard.core.analysis.analysis import ExternalMethod
 
     import matplotlib.pyplot as plt
-    import networkx as nx
 
     a, d, dx = AnalyzeAPK(file_)
 
     entry_points = map(FormatClassToJava,
                        a.get_activities() + a.get_providers() +
                        a.get_services() + a.get_receivers())
     entry_points = list(entry_points)
@@ -564,16 +564,21 @@
         classname,
         methodname,
         descriptor,
         accessflag,
         no_isolated,
         entry_points
     )
-        
+
     if show:
+        try:
+            import PyQt5
+        except ImportError:
+            print("PyQt5 is not installed. In most OS you can install it by running 'pip install PyQt5'.\n")
+            exit()
         pos = nx.spring_layout(callgraph)
         internal = []
         external = []
 
         for n in callgraph:
             if isinstance(n, ExternalMethod):
                 external.append(n)
```

### Comparing `androguard-4.1.1/androguard/cli/main.py` & `androguard-4.1.2/androguard/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 # core modules
 import os
 import re
 import shutil
 import sys
+from typing import Union
 
 # 3rd party modules
 from lxml import etree
 from loguru import logger
 from pygments import highlight
 from pygments.lexers import get_lexer_by_name
 from pygments.formatters.terminal import TerminalFormatter
+from oscrypto import asymmetric
 
 # internal modules
+from androguard.core.axml import ARSCParser
+from androguard.session import Session
 from androguard.core import androconf
 from androguard.core import apk
 from androguard.core.axml import AXMLPrinter
 from androguard.core.dex import get_bytecodes_method
 from androguard.util import readFile
 from androguard.ui import DynamicUI
 
-
-def androaxml_main(inp, outp=None, resource=None):
+def androaxml_main(
+        inp:str,
+        outp:Union[str,None]=None,
+        resource:Union[str,None]=None) -> None:
+    
     ret_type = androconf.is_android(inp)
     if ret_type == "APK":
         a = apk.APK(inp)
         if resource:
             if resource not in a.files:
                 logger.error("The APK does not contain a file called '{}'".format(resource), file=sys.stderr)
                 sys.exit(1)
@@ -42,15 +49,21 @@
     if outp:
         with open(outp, "wb") as fd:
             fd.write(buff)
     else:
         sys.stdout.write(highlight(buff.decode("UTF-8"), get_lexer_by_name("xml"), TerminalFormatter()))
 
 
-def androarsc_main(arscobj, outp=None, package=None, typ=None, locale=None):
+def androarsc_main(
+        arscobj: ARSCParser,
+        outp:Union[str,None]=None,
+        package:Union[str,None]=None,
+        typ:Union[str,None]=None,
+        locale:Union[str,None]=None) -> None:
+    
     package = package or arscobj.get_packages_names()[0]
     ttype = typ or "public"
     locale = locale or '\x00\x00'
 
     # TODO: be able to dump all locales of a specific type
     # TODO: be able to recreate the structure of files when developing, eg a
     # res folder with all the XML files
@@ -70,21 +83,23 @@
     if outp:
         with open(outp, "wb") as fd:
             fd.write(buff)
     else:
         sys.stdout.write(highlight(buff.decode("UTF-8"), get_lexer_by_name("xml"), TerminalFormatter()))
 
 
-def export_apps_to_format(filename,
-                          s,
-                          output,
-                          methods_filter=None,
-                          jar=None,
-                          decompiler_type=None,
-                          form=None):
+def export_apps_to_format(
+        filename:str,
+        s: Session,
+        output: str,
+        methods_filter:Union[str,None]=None,
+        jar:bool=False,
+        decompiler_type:Union[str,None]=None,
+        form:Union[str,None]=None) -> None:
+    
     from androguard.misc import clean_file_name
     from androguard.core.bytecode import method2dot, method2format
     from androguard.decompiler import decompiler
     print("Dump information {} in {}".format(filename, output))
 
     if not os.path.exists(output):
         print("Create directory %s" % output)
@@ -140,15 +155,15 @@
             print("jar ...", end=' ')
             filenamejar = decompiler.Dex2Jar(vm,
                                              androconf.CONF["BIN_DEX2JAR"],
                                              androconf.CONF["TMP_DIRECTORY"]).get_jar()
             shutil.move(filenamejar, os.path.join(output, "classes.jar"))
             print("End")
 
-        for method in vm.get_methods():
+        for method in vm.get_encoded_methods():
             if methods_filter_expr:
                 msig = "{}{}{}".format(method.get_class_name(), method.get_name(),
                                        method.get_descriptor())
                 if not methods_filter_expr.search(msig):
                     continue
 
             # Current Folder to write to
@@ -183,26 +198,26 @@
             print("bytecodes ...", end=' ')
             bytecode_buff = get_bytecodes_method(vm, vmx, method)
             with open(filename + ".ag", "w") as fd:
                 fd.write(bytecode_buff)
             print()
 
 
-def valid_class_name(class_name):
+def valid_class_name(class_name:str) -> str:
     if class_name[-1] == ";":
         class_name = class_name[1:-1]
     return os.path.join(*class_name.split("/"))
 
 
-def create_directory(pathdir):
+def create_directory(pathdir:str) -> None:
     if not os.path.exists(pathdir):
         os.makedirs(pathdir)
 
 
-def androlyze_main(session, filename):
+def androlyze_main(session:Session, filename:str) -> None:
     """
     Start an interactive shell
 
     :param session: Session file to load
     :param filename: File to analyze, can be APK or DEX (or ODEX)
     """
     from colorama import Fore
@@ -270,15 +285,15 @@
                         break
                 print(">>> d")
                 print(d)
                 print(">>> dx")
                 print(dx)
                 print()
 
-    def shutdown_hook():
+    def shutdown_hook() -> None:
         """Save the session on exit, if wanted"""
         if not s.isOpen():
             return
 
         try:
             res = input("Do you want to save the session? (y/[n])?").lower()
         except (EOFError, KeyboardInterrupt):
@@ -293,15 +308,15 @@
     cfg = Config()
     _version_string = "Androguard version {}".format(ANDROGUARD_VERSION)
     ipshell = embed(config=cfg, banner1="{} started".format(_version_string))
     atexit.register(shutdown_hook)
     ipshell()
 
 
-def androsign_main(args_apk, args_hash, args_all, show):
+def androsign_main(args_apk:list[str], args_hash:str, args_all:bool, show:bool) -> None:
     from androguard.core.apk import APK
     from androguard.util import get_certificate_name_string
 
     import hashlib
     import binascii
     import traceback
     from colorama import Fore, Style
@@ -356,35 +371,35 @@
                 print()
 
             if len(certs) > 0:
                 print("Found {} unique public keys associated with the certs".format(len(pkeys)))
 
             for public_key in pkeys:
                 if show:
-                    x509_public_key = keys.PublicKeyInfo.load(public_key)
+                    x509_public_key = asymmetric.load_public_key(public_key)
                     print("PublicKey Algorithm:", x509_public_key.algorithm)
                     print("Bit Size:", x509_public_key.bit_size)
                     print("Fingerprint:", binascii.hexlify(x509_public_key.fingerprint))
                     try:
-                        print("Hash Algorithm:", x509_public_key.hash_algo)
+                        print("Hash Algorithm:", x509_public_key.asn1.hash_algo)
                     except ValueError as ve:
-                        # RSA pkey does not have an hash algorithm
+                        # RSA pkey does not have a hash algorithm
                         pass
                 print()
 
 
         except:
             print(Fore.RED + "Error in {}".format(os.path.basename(path)) + Style.RESET_ALL, file=sys.stderr)
             traceback.print_exc(file=sys.stderr)
 
         if len(args_apk) > 1:
             print()
 
 
-def androdis_main(offset, size, dex_file):
+def androdis_main(offset:int, size:int, dex_file:str) -> None:
     from androguard.core.dex import DEX
 
     with open(dex_file, "rb") as fp:
         buf = fp.read()
 
     d = DEX(buf)
 
@@ -409,15 +424,15 @@
                 print("%-8d(%08x)" % (nb, idx), end=' ')
                 i.show(idx)
                 print()
 
                 idx += i.get_length()
 
 
-def androtrace_main(apk_file, list_modules, live=False, enable_ui=False):
+def androtrace_main(apk_file:str, list_modules:list[str], live:bool=False, enable_ui:bool=False) -> None:
     from androguard.pentest import Pentest
     from androguard.session import Session
 
     s = Session()
 
     if not live:
         with open(apk_file, "rb") as fp:
@@ -454,15 +469,15 @@
     else:
         logger.warning("Type 'e' to exit the strace ")
         s = ""
         while (s != 'e') and (not p.is_detached()):
             s = input("Type 'e' to exit:")
 
 
-def androdump_main(package_name, list_modules):
+def androdump_main(package_name:str, list_modules:list[str]) -> None:
     from androguard.pentest import Pentest
     from androguard.session import Session
 
     s = Session()
 
     p = Pentest()
     p.print_devices()
```

### Comparing `androguard-4.1.1/androguard/core/analysis/analysis.py` & `androguard-4.1.2/androguard/core/analysis/analysis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-from androguard.core.androconf import is_ascii_problem, load_api_specific_resource_module
-from androguard.core import bytecode, mutf8, dex
+# Allows type hinting of types not-yet-declared
+# in Python >= 3.7
+# see https://peps.python.org/pep-0563/
+from __future__ import annotations
 
-import re
-import sys
 import collections
+from enum import IntEnum
 from operator import itemgetter
+import re
 import time
-from enum import IntEnum
+from typing import Union, Iterator
+
+from androguard.core.androconf import is_ascii_problem, load_api_specific_resource_module
+from androguard.core import bytecode, dex
 
 from loguru import logger
 import networkx as nx
 
 BasicOPCODES = set()
 for i in dex.BRANCH_DEX_OPCODES:
     p = re.compile(i)
     for op, items in dex.DALVIK_OPCODES_FORMAT.items():
         if p.match(items[1][0]):
             BasicOPCODES.add(op)
 
-
 class REF_TYPE(IntEnum):
     """
     Stores the opcodes for the type of usage in an XREF.
 
     Used in :class:`ClassAnalysis` to store the type of reference to the class.
     """
     REF_NEW_INSTANCE = 0x22
@@ -34,23 +38,144 @@
     INVOKE_INTERFACE = 0x72
     INVOKE_VIRTUAL_RANGE = 0x74
     INVOKE_SUPER_RANGE = 0x75
     INVOKE_DIRECT_RANGE = 0x76
     INVOKE_STATIC_RANGE = 0x77
     INVOKE_INTERFACE_RANGE = 0x78
 
+class ExceptionAnalysis:
+    def __init__(self, exception: list, basic_blocks: BasicBlocks):
+        self.start = exception[0]
+        self.end = exception[1]
+        
+        self.exceptions = exception[2:]
+
+        for i in self.exceptions:
+            i.append(basic_blocks.get_basic_block(i[1]))
+
+    def show_buff(self) -> str:
+        buff = "{:x}:{:x}\n".format(self.start, self.end)
+
+        for i in self.exceptions:
+            if i[2] is None:
+                buff += "\t({} -> {:x} {})\n".format(i[0], i[1], i[2])
+            else:
+                buff += "\t({} -> {:x} {})\n".format(i[0], i[1], i[2].get_name())
+
+        return buff[:-1]
+
+    def get(self) -> dict[str, Union[int, list[dict[str, Union[str, int]]]]]:
+        d = {"start": self.start, "end": self.end, "list": []}
+
+        for i in self.exceptions:
+            d["list"].append({"name": i[0], "idx": i[1], "basic_block": i[2].get_name()})
+
+        return d
+
+
+class Exceptions:
+    def __init__(self) -> None:
+        self.exceptions = []
+
+    def add(self, exceptions: list[list], basic_blocks: BasicBlocks) -> None:
+        for i in exceptions:
+            self.exceptions.append(ExceptionAnalysis(i, basic_blocks))
+
+    def get_exception(self, addr_start: int, addr_end: int) -> Union[ExceptionAnalysis,None]:
+        for i in self.exceptions:
+            if i.start >= addr_start and i.end <= addr_end:
+                return i
+
+            elif addr_end <= i.end and addr_start >= i.start:
+                return i
+
+        return None
+
+    def gets(self) -> list[ExceptionAnalysis]:
+        return self.exceptions
+
+    def get(self) -> Iterator[ExceptionAnalysis]:
+        for i in self.exceptions:
+            yield i
+
+class BasicBlocks:
+    """
+    This class represents all basic blocks of a method.
+
+    It is a collection of many :class:`DEXBasicBlock`.
+    """
+    def __init__(self) -> None:
+        self.bb = []
+
+    def push(self, bb: DEXBasicBlock) -> None:
+        """
+        Adds another basic block to the collection
+
+        :param :class:`DEXBasicBlock` bb: the DEXBasicBlock to add
+        """
+        self.bb.append(bb)
+
+    def pop(self, idx: int) -> DEXBasicBlock:
+        return self.bb.pop(idx)
+
+    def get_basic_block(self, idx: int) -> Union[DEXBasicBlock,None]:
+        for i in self.bb:
+            if i.get_start() <= idx < i.get_end():
+                return i
+        return None
+
+    def __len__(self):
+        return len(self.bb)
+
+    def __iter__(self):
+        """
+        :returns: yields each basic block (:class:`DEXBasicBlock` object)
+        :rtype: Iterator[DEXBasicBlock]
+        """
+        yield from self.bb
+
+    def __getitem__(self, item: int):
+        """
+        Get the basic block at the index
+
+        :param item: index
+        :return: The basic block
+        :rtype: DEXBasicBlock
+        """
+        return self.bb[item]
+
+    def gets(self) -> list[DEXBasicBlock]:
+        """
+        :returns: a list of basic blocks (:class:`DEXBasicBlock` objects)
+        """
+        return self.bb
+
+    # Alias for legacy programs
+    get = __iter__
+    get_basic_block_pos = __getitem__
 
 class DEXBasicBlock:
     """
     A simple basic block of a DEX method.
 
-    A basic block consists of a series of :class:`~androguard.core.bytecodes.dvm.Instruction`
+    A basic block consists of a series of :class:`~androguard.core.dex.Instruction`
     which are not interrupted by branch or jump instructions such as `goto`, `if`, `throw`, `return`, `switch` etc.
     """
-    def __init__(self, start, vm, method, context):
+    def __init__(self, start: int, vm: dex.DEX, method: dex.EncodedMethod, context: BasicBlocks):
+        """_summary_
+
+        :param start: _description_
+        :type start: int
+        :param vm: _description_
+        :type vm: dex.DEX
+        :param method: _description_
+        :type method: dex.EncodedMethod
+        :param context: _description_
+        :type context: BasicBlocks
+        """
         self.__vm = vm
         self.method = method
         self.context = context
 
         self.last_length = 0
         self.nb_instructions = 0
 
@@ -69,104 +194,104 @@
         ])
         self.exception_analysis = None
 
         self.notes = []
 
         self.__cached_instructions = None
 
-    def get_notes(self):
+    def get_notes(self) -> list[str]:
         return self.notes
 
-    def set_notes(self, value):
+    def set_notes(self, value: str) -> None:
         self.notes = [value]
 
-    def add_note(self, note):
+    def add_note(self, note: str) -> None:
         self.notes.append(note)
 
-    def clear_notes(self):
+    def clear_notes(self) -> None:
         self.notes = []
 
-    def get_instructions(self):
+    def get_instructions(self) -> Iterator[dex.Instruction]:
         """
         Get all instructions from a basic block.
 
         :returns: Return all instructions in the current basic block
         """
         idx = 0
         for i in self.method.get_instructions():
             if self.start <= idx < self.end:
                 yield i
             idx += i.get_length()
 
-    def get_nb_instructions(self):
+    def get_nb_instructions(self) -> int:
         return self.nb_instructions
 
-    def get_method(self):
+    def get_method(self) -> dex.EncodedMethod:
         """
         Returns the originiating method
 
         :return: the method
-        :rtype: androguard.core.bytecodes.dvm.EncodedMethod
+        :rtype: androguard.core.dex.EncodedMethod
         """
         return self.method
 
-    def get_name(self):
+    def get_name(self) -> str:
         return self.name
 
-    def get_start(self):
+    def get_start(self) -> int:
         """
         Get the starting offset of this basic block
 
         :return: starting offset
         :rtype: int
         """
         return self.start
 
-    def get_end(self):
+    def get_end(self) -> int:
         """
         Get the end offset of this basic block
 
         :return: end offset
         :rtype: int
         """
         return self.end
 
-    def get_last(self):
+    def get_last(self) -> dex.Instruction:
         """
         Get the last instruction in the basic block
 
-        :return: androguard.core.bytecodes.dvm.Instruction
+        :return: androguard.core.dex.Instruction
         """
         return list(self.get_instructions())[-1]
-
-    def get_next(self):
+    
+    def get_next(self) -> DEXBasicBlock:
         """
         Get next basic blocks
 
         :returns: a list of the next basic blocks
         :rtype: DEXBasicBlock
         """
         return self.childs
 
-    def get_prev(self):
+    def get_prev(self) -> DEXBasicBlock:
         """
         Get previous basic blocks
 
         :returns: a list of the previous basic blocks
         :rtype: DEXBasicBlock
         """
         return self.fathers
-
-    def set_fathers(self, f):
+    
+    def set_fathers(self, f: DEXBasicBlock) -> None:
         self.fathers.append(f)
 
-    def get_last_length(self):
+    def get_last_length(self) -> int:
         return self.last_length
 
-    def set_childs(self, values):
+    def set_childs(self, values: list[int]) -> None:
         # print self, self.start, self.end, values
         if not values:
             next_block = self.context.get_basic_block(self.end + 1)
             if next_block is not None:
                 self.childs.append((self.end - self.get_last_length(), self.end,
                                     next_block))
         else:
@@ -177,175 +302,62 @@
                         self.childs.append((self.end - self.get_last_length(),
                                             i, next_block))
 
         for c in self.childs:
             if c[2] is not None:
                 c[2].set_fathers((c[1], c[0], self))
 
-    def push(self, i):
+    def push(self, i: DEXBasicBlock) -> None:
         self.nb_instructions += 1
         idx = self.end
         self.last_length = i.get_length()
         self.end += self.last_length
 
         op_value = i.get_op_value()
 
         if op_value == 0x26 or (0x2b <= op_value <= 0x2c):
             code = self.method.get_code().get_bc()
             self.special_ins[idx] = code.get_ins_off(idx + i.get_ref_off() * 2)
-
-    def get_special_ins(self, idx):
+    
+    def get_special_ins(self, idx: int) -> Union[dex.Instruction,None]:
         """
         Return the associated instruction to a specific instruction (for example a packed/sparse switch)
 
         :param idx: the index of the instruction
 
         :rtype: None or an Instruction
         """
         if idx in self.special_ins:
             return self.special_ins[idx]
         else:
             return None
 
-    def get_exception_analysis(self):
+    def get_exception_analysis(self) -> ExceptionAnalysis:
         return self.exception_analysis
 
-    def set_exception_analysis(self, exception_analysis):
+    def set_exception_analysis(self, exception_analysis: ExceptionAnalysis):
         self.exception_analysis = exception_analysis
 
-    def show(self):
+    def show(self) -> None:
         print("{}: {:04x} - {:04x}".format(self.get_name(), self.get_start(), self.get_end()))
         for note in self.get_notes():
             print(note)
         print('=' * 20)
 
 
-class BasicBlocks:
-    """
-    This class represents all basic blocks of a method.
-
-    It is a collection of many :class:`DEXBasicBlock`.
-    """
-    def __init__(self):
-        self.bb = []
-
-    def push(self, bb):
-        """
-        Adds another basic block to the collection
-
-        :param DVBMBasicBlock bb: the DEXBasicBlock to add
-        """
-        self.bb.append(bb)
-
-    def pop(self, idx):
-        return self.bb.pop(idx)
-
-    def get_basic_block(self, idx):
-        for i in self.bb:
-            if i.get_start() <= idx < i.get_end():
-                return i
-        return None
-
-    def __len__(self):
-        return len(self.bb)
-
-    def __iter__(self):
-        """
-        :returns: yields each basic block (:class:`DEXBasicBlock` object)
-        :rtype: Iterator[DEXBasicBlock]
-        """
-        yield from self.bb
-
-    def __getitem__(self, item):
-        """
-        Get the basic block at the index
-
-        :param item: index
-        :return: The basic block
-        :rtype: DEXBasicBlock
-        """
-        return self.bb[item]
-
-    def gets(self):
-        """
-        :returns: a list of basic blocks (:class:`DEXBasicBlock` objects)
-        """
-        return self.bb
-
-    # Alias for legacy programs
-    get = __iter__
-    get_basic_block_pos = __getitem__
-
-
-class ExceptionAnalysis:
-    def __init__(self, exception, bb):
-        self.start = exception[0]
-        self.end = exception[1]
-
-        self.exceptions = exception[2:]
-
-        for i in self.exceptions:
-            i.append(bb.get_basic_block(i[1]))
-
-    def show_buff(self):
-        buff = "{:x}:{:x}\n".format(self.start, self.end)
-
-        for i in self.exceptions:
-            if i[2] is None:
-                buff += "\t({} -> {:x} {})\n".format(i[0], i[1], i[2])
-            else:
-                buff += "\t({} -> {:x} {})\n".format(i[0], i[1], i[2].get_name())
-
-        return buff[:-1]
-
-    def get(self):
-        d = {"start": self.start, "end": self.end, "list": []}
-
-        for i in self.exceptions:
-            d["list"].append({"name": i[0], "idx": i[1], "bb": i[2].get_name()})
-
-        return d
-
-
-class Exceptions:
-    def __init__(self):
-        self.exceptions = []
-
-    def add(self, exceptions, basic_blocks):
-        for i in exceptions:
-            self.exceptions.append(ExceptionAnalysis(i, basic_blocks))
-
-    def get_exception(self, addr_start, addr_end):
-        for i in self.exceptions:
-            if i.start >= addr_start and i.end <= addr_end:
-                return i
-
-            elif addr_end <= i.end and addr_start >= i.start:
-                return i
-
-        return None
-
-    def gets(self):
-        return self.exceptions
-
-    def get(self):
-        for i in self.exceptions:
-            yield i
-
-
 class MethodAnalysis:
     """
     This class analyses in details a method of a class/dex file
     It is a wrapper around a :class:`EncodedMethod` and enhances it
     by using multiple :class:`DEXBasicBlock` encapsulated in a :class:`BasicBlocks` object.
 
     :type vm: a :class:`DEX` object
     :type method: a :class:`EncodedMethod` object
     """
-    def __init__(self, vm, method):
+    def __init__(self, vm: dex.DEX, method: dex.EncodedMethod):
         logger.debug("Adding new method {} {}".format(method.get_class_name(), method.get_name()))
 
         self.__vm = vm
         self.method = method
 
         self.basic_blocks = BasicBlocks()
         self.exceptions = Exceptions()
@@ -373,50 +385,50 @@
         else:
             self.code = self.method.get_code()
 
         if self.code:
             self._create_basic_block()
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Returns the name of this method"""
         return self.method.get_name()
 
     @property
-    def descriptor(self):
+    def descriptor(self) -> str:
         """Returns the type descriptor for this method"""
         return self.method.get_descriptor()
 
     @property
-    def access(self):
+    def access(self) -> str:
         """Returns the access flags to the method as a string"""
         return self.method.get_access_flags_string()
 
     @property
-    def class_name(self):
+    def class_name(self) -> str:
         """Returns the name of the class of this method"""
         return self.method.class_name
 
     @property
-    def full_name(self):
+    def full_name(self) -> str:
         """Returns classname + name + descriptor, separated by spaces (no access flags)"""
         return self.method.full_name
 
-    def get_class_name(self):
+    def get_class_name(self) -> str:
         """Return the class name of the method"""
         return self.class_name
 
-    def get_access_flags_string(self):
+    def get_access_flags_string(self) -> str:
         """Returns the concatenated access flags string"""
         return self.access
 
-    def get_descriptor(self):
+    def get_descriptor(self) -> str:
         return self.descriptor
 
-    def _create_basic_block(self):
+    def _create_basic_block(self) -> None:
         """
         Internal Method to create the basic block structure
         Parses all instructions and exceptions.
         """
         current_basic = DEXBasicBlock(0, self.__vm, self.method, self.basic_blocks)
         self.basic_blocks.push(current_basic)
 
@@ -465,146 +477,146 @@
         logger.debug("Creating exceptions")
         self.exceptions.add(excepts, self.basic_blocks)
 
         for i in self.basic_blocks.get():
             # setup exception by basic block
             i.set_exception_analysis(self.exceptions.get_exception(i.start, i.end - 1))
 
-    def add_xref_read(self, classobj, fieldobj, offset):
+    def add_xref_read(self, classobj:ClassAnalysis, fieldobj: FieldAnalysis, offset: int) -> None:
         """
         :param ClassAnalysis classobj:
         :param FieldAnalysis fieldobj:
         :param int offset: offset in the bytecode
         """
         self.xrefread.add((classobj, fieldobj, offset))
 
-    def add_xref_write(self, classobj, fieldobj, offset):
+    def add_xref_write(self, classobj: ClassAnalysis, fieldobj: FieldAnalysis, offset: int) -> None:
         """
         :param ClassAnalysis classobj:
         :param FieldAnalysis fieldobj:
         :param int offset: offset in the bytecode
         """
         self.xrefwrite.add((classobj, fieldobj, offset))
 
-    def get_xref_read(self):
+    def get_xref_read(self) -> list[tuple[ClassAnalysis, FieldAnalysis]]:
         """
         Returns a list of xrefs where a field is read by this method.
 
         The list contains tuples of the originating class and methods,
         where the class is represented as a :class:`ClassAnalysis`,
         while the Field is a :class:`FieldAnalysis`.
         """
         return self.xrefread
 
-    def get_xref_write(self):
+    def get_xref_write(self) -> list[tuple[ClassAnalysis, FieldAnalysis]]:
         """
         Returns a list of xrefs where a field is written to by this method.
 
         The list contains tuples of the originating class and methods,
         where the class is represented as a :class:`ClassAnalysis`,
         while the Field is a :class:`FieldAnalysis`.
         """
         return self.xrefwrite
 
-    def add_xref_to(self, classobj, methodobj, offset):
+    def add_xref_to(self, classobj: ClassAnalysis, methodobj: MethodAnalysis, offset: int) -> None:
         """
         Add a crossreference to another method
         (this method calls another method)
 
         :param classobj: :class:`~ClassAnalysis`
         :param methodobj:  :class:`~MethodAnalysis`
         :param offset: integer where in the method the call happens
         """
         self.xrefto.add((classobj, methodobj, offset))
 
-    def add_xref_from(self, classobj, methodobj, offset):
+    def add_xref_from(self, classobj: ClassAnalysis, methodobj: MethodAnalysis, offset: int) -> None:
         """
         Add a crossrefernece from another method
         (this method is called by another method)
 
         :param classobj: :class:`~ClassAnalysis`
         :param methodobj: :class:`~MethodAnalysis`
         :param offset: integer where in the method the call happens
         """
         self.xreffrom.add((classobj, methodobj, offset))
 
-    def get_xref_from(self):
+    def get_xref_from(self) -> list[tuple[ClassAnalysis, MethodAnalysis, int]]:
         """
         Returns a list of tuples containing the class, method and offset of
         the call, from where this object was called.
 
         The list of tuples has the form:
         (:class:`~ClassAnalysis`,
         :class:`~MethodAnalysis`,
         :class:`int`)
         """
         return self.xreffrom
 
-    def get_xref_to(self):
+    def get_xref_to(self) -> list[tuple[ClassAnalysis, MethodAnalysis, int]]:
         """
         Returns a list of tuples containing the class, method and offset of
         the call, which are called by this method.
 
         The list of tuples has the form:
         (:class:`~ClassAnalysis`,
         :class:`~MethodAnalysis`,
         :class:`int`)
         """
         return self.xrefto
 
-    def add_xref_new_instance(self, classobj, offset):
+    def add_xref_new_instance(self, classobj: ClassAnalysis, offset: int) -> None:
         """
         Add a crossreference to another class that is
         instanced within this method.
 
         :param classobj: :class:`~ClassAnalysis`
         :param offset: integer where in the method the instantiation happens
         """
         self.xrefnewinstance.add((classobj, offset))
 
-    def get_xref_new_instance(self):
+    def get_xref_new_instance(self) -> list[tuple[ClassAnalysis, int]]:
         """
         Returns a list of tuples containing the class and offset of
         the creation of a new instance of a class by this method.
 
         The list of tuples has the form:
         (:class:`~ClassAnalysis`,
         :class:`int`)
         """
         return self.xrefnewinstance
 
-    def add_xref_const_class(self, classobj, offset):
+    def add_xref_const_class(self, classobj: ClassAnalysis, offset: int) -> None:
         """
         Add a crossreference to another classtype.
 
         :param classobj: :class:`~ClassAnalysis`
         :param offset: integer where in the method the classtype is referenced
         """
         self.xrefconstclass.add((classobj, offset))
 
-    def get_xref_const_class(self):
+    def get_xref_const_class(self) -> list[tuple[ClassAnalysis, int]]:
         """
         Returns a list of tuples containing the class and offset of
         the references to another classtype by this method.
 
         The list of tuples has the form:
         (:class:`~ClassAnalysis`,
         :class:`int`)
         """
         return self.xrefconstclass
 
-    def is_external(self):
+    def is_external(self) -> bool:
         """
         Returns True if the underlying method is external
 
         :rtype: boolean
         """
         return isinstance(self.method, ExternalMethod)
 
-    def is_android_api(self):
+    def is_android_api(self) -> bool:
         """
         Returns True if the method seems to be an Android API method.
 
         This method might be not very precise unless an list of known API methods
         is given.
 
         :return: boolean
@@ -624,46 +636,46 @@
         else:
             for candidate in api_candidates:
                 if self.method.get_class_name().startswith(candidate):
                     return True
 
         return False
 
-    def get_basic_blocks(self):
+    def get_basic_blocks(self) -> BasicBlocks:
         """
         Returns the :class:`BasicBlocks` generated for this method.
         The :class:`BasicBlocks` can be used to get a control flow graph (CFG) of the method.
 
         :rtype: a :class:`BasicBlocks` object
         """
         return self.basic_blocks
 
-    def get_length(self):
+    def get_length(self) -> int:
         """
         :returns: an integer which is the length of the code
         :rtype: int
         """
         return self.code.get_length() if self.code else 0
 
-    def get_vm(self):
+    def get_vm(self) -> dex.DEX:
         """
-        :rtype: androguard.core.bytecodes.dvm.DEX
+        :rtype: androguard.core.dex.DEX
         :return:
         """
         return self.__vm
 
-    def get_method(self):
+    def get_method(self) -> dex.EncodedMethod:
         """
 
-        :rtype: androguard.core.bytecodes.dvm.EncodedMethod
+        :rtype: androguard.core.dex.EncodedMethod
         :return:
         """
         return self.method
 
-    def show(self):
+    def show(self) -> None:
         """
         Prints the content of this method to stdout.
 
         This will print the method signature and the decompiled code.
         """
         args, ret = self.method.get_descriptor()[1:].split(")")
         if self.code:
@@ -681,15 +693,15 @@
               self.method.get_access_flags_string(),
               self.method.get_name(),
               ", ".join(args), ret))
         
         if not self.is_external():
             bytecode.PrettyShow(self.basic_blocks.gets(), self.method.notes)
 
-    def show_xrefs(self):
+    def show_xrefs(self) -> None:
         data = "XREFto for %s\n" % self.method
         for ref_class, ref_method, offset in self.xrefto:
             data += "in\n"
             data += "{}:{} @0x{:x}\n".format(ref_class.get_vm_class().get_name(), ref_method, offset)
 
         data += "XREFFrom for %s\n" % self.method
         for ref_class, ref_method, offset in self.xreffrom:
@@ -707,71 +719,71 @@
     StringAnalysis contains the XREFs of a string.
 
     As Strings are only used as a source, they only contain
     the XREF_FROM set, i.e. where the string is used.
 
     This Array stores the information in which method the String is used.
     """
-    def __init__(self, value):
+    def __init__(self, value: str) -> None:
         """
 
         :param str value: the original string value
         """
         self.value = value
         self.orig_value = value
         self.xreffrom = set()
 
-    def add_xref_from(self, classobj, methodobj, off):
+    def add_xref_from(self, classobj: ClassAnalysis, methodobj: MethodAnalysis, off: int) -> None:
         """
         Adds a xref from the given method to this string
 
         :param ClassAnalysis classobj:
         :param MethodAnalysis methodobj:
         :param int off: offset in the bytecode of the call
         """
         self.xreffrom.add((classobj, methodobj, off))
 
-    def get_xref_from(self, withoffset=False):
+    def get_xref_from(self, with_offset:bool = False) -> list[tuple[ClassAnalysis, MethodAnalysis]]:
         """
         Returns a list of xrefs accessing the String.
 
         The list contains tuples of the originating class and methods,
         where the class is represented as a :class:`ClassAnalysis`,
         while the method is a :class:`MethodAnalysis`.
         """
-        if withoffset:
+        if with_offset:
             return self.xreffrom
         return set(map(itemgetter(slice(0, 2)), self.xreffrom))
 
-    def set_value(self, value):
+    def set_value(self, value: str) -> None:
         """
         Overwrite the current value of the String with a new value.
         The original value is not lost and can still be retrieved using :meth:`get_orig_value`.
 
         :param str value: new string value
         """
         self.value = value
 
-    def get_value(self):
+    def get_value(self) -> str:
         """
         Return the (possible overwritten) value of the String
 
         :return: the value of the string
         """
         return self.value
 
-    def get_orig_value(self):
+    def get_orig_value(self) -> str:
         """
         Return the original, read only, value of the String
 
         :return: the original value
         """
         return self.orig_value
 
-    def is_overwritten(self):
+    def is_overwritten(self) -> bool:
         """
         Returns True if the string was overwritten
         :return:
         """
         return self.orig_value != self.value
 
     def __str__(self):
@@ -794,76 +806,76 @@
     FieldAnalysis contains the XREFs for a class field.
 
     Instead of using XREF_FROM/XREF_TO, this object has methods for READ and
     WRITE access to the field.
 
     That means, that it will show you, where the field is read or written.
 
-    :param androguard.core.bytecodes.dvm.EncodedField field: `dvm.EncodedField`
+    :param androguard.core.dex.EncodedField field: `dvm.EncodedField`
     """
-    def __init__(self, field):
+    def __init__(self, field: dex.EncodedField) -> None:
         self.field = field
         self.xrefread = set()
         self.xrefwrite = set()
 
     @property
-    def name(self):
+    def name(self) -> str:
         return self.field.get_name()
 
-    def add_xref_read(self, classobj, methodobj, offset):
+    def add_xref_read(self, classobj: ClassAnalysis, methodobj: MethodAnalysis, offset: int) -> None:
         """
         :param ClassAnalysis classobj:
         :param MethodAnalysis methodobj:
         :param int offset: offset in the bytecode
         """
         self.xrefread.add((classobj, methodobj, offset))
 
-    def add_xref_write(self, classobj, methodobj, offset):
+    def add_xref_write(self, classobj: ClassAnalysis, methodobj: MethodAnalysis, offset: int) -> None:
         """
         :param ClassAnalysis classobj:
         :param MethodAnalysis methodobj:
         :param int offset: offset in the bytecode
         """
         self.xrefwrite.add((classobj, methodobj, offset))
 
-    def get_xref_read(self, withoffset=False):
+    def get_xref_read(self, with_offset:bool = False) -> list[tuple[ClassAnalysis, MethodAnalysis]]:
         """
         Returns a list of xrefs where the field is read.
 
         The list contains tuples of the originating class and methods,
         where the class is represented as a :class:`ClassAnalysis`,
         while the method is a :class:`MethodAnalysis`.
 
-        :param bool withoffset: return the xrefs including the offset
+        :param bool with_offset: return the xrefs including the offset
         """
-        if withoffset:
+        if with_offset:
             return self.xrefread
         # Legacy option, might be removed in the future
         return set(map(itemgetter(slice(0, 2)), self.xrefread))
 
-    def get_xref_write(self, withoffset=False):
+    def get_xref_write(self, with_offset:bool = False) -> list[tuple[ClassAnalysis, MethodAnalysis]]:
         """
         Returns a list of xrefs where the field is written to.
 
         The list contains tuples of the originating class and methods,
         where the class is represented as a :class:`ClassAnalysis`,
         while the method is a :class:`MethodAnalysis`.
 
-        :param bool withoffset: return the xrefs including the offset
+        :param bool with_offset: return the xrefs including the offset
         """
-        if withoffset:
+        if with_offset:
             return self.xrefwrite
         # Legacy option, might be removed in the future
         return set(map(itemgetter(slice(0, 2)), self.xrefwrite))
 
-    def get_field(self):
+    def get_field(self) -> dex.EncodedField:
         """
         Returns the actual field object
 
-        :rtype: androguard.core.bytecodes.dvm.EncodedField
+        :rtype: androguard.core.dex.EncodedField
         """
         return self.field
 
     def __str__(self):
         data = "XREFRead for %s\n" % self.field
         for ref_class, ref_method, off in self.xrefread:
             data += "in\n"
@@ -883,29 +895,29 @@
 class ExternalClass:
     """
     The ExternalClass is used for all classes that are not defined in the
     DEX file, thus are external classes.
 
     :param name: Name of the external class
     """
-    def __init__(self, name):
+    def __init__(self, name: str) -> None:
         self.name = name
         self.methods = []
 
-    def get_methods(self):
+    def get_methods(self) -> list[MethodAnalysis]:
         """
         Return the stored methods for this external class
         :return:
         """
         return self.methods
 
-    def add_method(self, method):
+    def add_method(self, method: MethodAnalysis) -> None:
         self.methods.append(method)
 
-    def get_name(self):
+    def get_name(self) -> str:
         """
         Returns the name of the ExternalClass object
         """
         return self.name
 
     def __repr__(self):
         return "<analysis.ExternalClass {}>".format(self.name)
@@ -915,47 +927,47 @@
     """
     ExternalMethod is a stub class for methods that are not part of the current Analysis.
     There are two possibilities for this:
 
     1) The method is defined inside another DEX file which was not loaded into the Analysis
     2) The method is an API method, hence it is defined in the Android system
 
-    External methods should have a similar API to :class:`~androguard.core.bytecodes.dvm.EncodedMethod`
+    External methods should have a similar API to :class:`~androguard.core.dex.EncodedMethod`
     but obviously they have no code attached.
     The only known information about such methods are the class name, the method name and its descriptor.
 
     :param str class_name: name of the class
     :param str name: name of the method
-    :param List[str] descriptor: descriptor string
+    :param str descriptor: descriptor string
     """
-    def __init__(self, class_name, name, descriptor):
+    def __init__(self, class_name: str, name: str, descriptor: str) -> None:
         self.class_name = class_name
         self.name = name
         self.descriptor = descriptor
 
-    def get_name(self):
+    def get_name(self) -> str:
         return self.name
 
-    def get_class_name(self):
+    def get_class_name(self) -> str:
         return self.class_name
 
-    def get_descriptor(self):
+    def get_descriptor(self) -> str:
         return self.descriptor
 
     @property
-    def full_name(self):
+    def full_name(self) -> str:
         """Returns classname + name + descriptor, separated by spaces (no access flags)"""
         return self.class_name + " " + self.name + " " + str(self.get_descriptor())
 
     @property
-    def permission_api_name(self):
+    def permission_api_name(self) -> str:
         """Returns a name which can be used to look up in the permission maps"""
         return self.class_name + "-" + self.name + "-" + str(self.get_descriptor())
 
-    def get_access_flags_string(self):
+    def get_access_flags_string(self) -> str:
         """
         Returns the access flags string.
 
         Right now, this is always an empty strings, as we can not say what
         kind of access flags an external method might have.
         """
         # TODO can we assume that external methods are always public?
@@ -979,15 +991,15 @@
 
     Also external classes will generate xrefs, obviously only XREF_FROM are
     shown for external classes.
 
     :param classobj: class:`~androguard.core.dex.ClassDefItem` or :class:`ExternalClass`
     """
 
-    def __init__(self, classobj):
+    def __init__(self, classobj: Union[dex.ClassDefItem,ExternalClass]) -> None:
         logger.info(f"Adding new ClassAnalysis: {classobj}")
         # Automatically decide if the class is external or not
         self.external = isinstance(classobj, ExternalClass)
 
         self.orig_class = classobj
 
         # Contains EncodedMethod/ExternalMethod -> MethodAnalysis
@@ -1001,70 +1013,70 @@
 
         self.xrefnewinstance = set()
         self.xrefconstclass = set()
 
         # Reserved for further use
         self.apilist = None
 
-    def add_method(self, method_analysis):
+    def add_method(self, method_analysis: MethodAnalysis) -> None:
         """
         Add the given method to this analyis.
         usually only called during Analysis.add and Analysis._resolve_method
 
         :param MethodAnalysis method_analysis:
         """
         self._methods[method_analysis.get_method()] = method_analysis
         if self.external:
             # Propagate ExternalMethod to ExternalClass
             self.orig_class.add_method(method_analysis.get_method())
 
     @property
-    def implements(self):
+    def implements(self) -> list[str]:
         """
         Get a list of interfaces which are implemented by this class
 
         :return: a list of Interface names
         """
         if self.is_external():
             return []
 
         return self.orig_class.get_interfaces()
 
     @property
-    def extends(self):
+    def extends(self) -> str:
         """
         Return the parent class
 
         For external classes, this is not sure, thus we return always Object (which is the parent of all classes)
 
         :return: a string of the parent class name
         """
         if self.is_external():
             return "Ljava/lang/Object;"
 
         return self.orig_class.get_superclassname()
 
     @property
-    def name(self):
+    def name(self) -> str:
         """
         Return the class name
 
         :return:
         """
         return self.orig_class.get_name()
 
-    def is_external(self):
+    def is_external(self) -> bool:
         """
         Tests if this class is an external class
 
         :return: True if the Class is external, False otherwise
         """
         return self.external
 
-    def is_android_api(self):
+    def is_android_api(self) -> bool:
         """
         Tries to guess if the current class is an Android API class.
 
         This might be not very precise unless an apilist is given, with classes that
         are in fact known APIs.
         Such a list might be generated by using the android.jar files.
 
@@ -1084,88 +1096,96 @@
         else:
             for candidate in api_candidates:
                 if self.orig_class.get_name().startswith(candidate):
                     return True
 
         return False
 
-    def get_methods(self):
+    def get_methods(self) -> list[MethodAnalysis]:
         """
         Return all :class:`MethodAnalysis` objects of this class
 
         :rtype: Iterator[MethodAnalysis]
         """
-        return list(self._methods.values())
+        return self._methods.values()
+        # return list(self._methods.values())
 
-    def get_fields(self):
+    def get_fields(self) -> list[FieldAnalysis]:
         """
         Return all `FieldAnalysis` objects of this class
         """
         return self._fields.values()
 
-    def get_nb_methods(self):
+    def get_nb_methods(self) -> int:
         """
         Get the number of methods in this class
         """
         return len(self._methods)
 
-    def get_method_analysis(self, method):
+    def get_method_analysis(self, method: dex.EncodedMethod) -> MethodAnalysis:
         """
         Return the MethodAnalysis object for a given EncodedMethod
 
         :param method: :class:`EncodedMethod`
         :return: :class:`MethodAnalysis`
         :rtype: MethodAnalysis
         """
         return self._methods.get(method)
 
-    def get_field_analysis(self, field):
+    def get_field_analysis(self, field: dex.EncodedMethod) -> FieldAnalysis:
+        """_summary_
+
+        :param field: _description_
+        :type field: dex.EncodedMethod
+        :return: _description_
+        :rtype: FieldAnalysis
+        """
         return self._fields.get(field)
 
-    def add_field(self, field_analysis):
+    def add_field(self, field_analysis: FieldAnalysis) -> None:
         """
         Add the given field to this analyis.
         usually only called during Analysis.add
 
         :param FieldAnalysis field_analysis:
         """
         self._fields[field_analysis.get_field()] = field_analysis
         # if self.external:
         #     # Propagate ExternalField to ExternalClass
         #     self.orig_class.add_method(field_analysis.get_field())
 
-    def add_field_xref_read(self, method, classobj, field, off):
+    def add_field_xref_read(self, method: MethodAnalysis, classobj: ClassAnalysis, field: dex.EncodedField, off: int) -> None:
         """
         Add a Field Read to this class
 
         :param MethodAnalysis method:
         :param ClassAnalysis classobj:
-        :param androguard.code.bytecodes.dvm.EncodedField field:
+        :param androguard.code.dex.EncodedField field:
         :param int off:
         :return:
         """
         if field not in self._fields:
             self._fields[field] = FieldAnalysis(field)
         self._fields[field].add_xref_read(classobj, method, off)
 
-    def add_field_xref_write(self, method, classobj, field, off):
+    def add_field_xref_write(self, method: MethodAnalysis, classobj: ClassAnalysis, field: dex.EncodedField, off: int) -> None:
         """
         Add a Field Write to this class in a given method
 
         :param MethodAnalysis method:
         :param ClassAnalysis classobj:
-        :param androguard.core.bytecodes.dvm.EncodedField field:
+        :param androguard.core.dex.EncodedField field:
         :param int off:
         :return:
         """
         if field not in self._fields:
             self._fields[field] = FieldAnalysis(field)
         self._fields[field].add_xref_write(classobj, method, off)
 
-    def add_method_xref_to(self, method1, classobj, method2, offset):
+    def add_method_xref_to(self, method1: MethodAnalysis, classobj: ClassAnalysis, method2: MethodAnalysis, offset: int) -> None:
         """
 
         :param MethodAnalysis method1: the calling method
         :param ClassAnalysis classobj: the calling class
         :param MethodAnalysis method2: the called method
         :param int offset: offset in the bytecode of calling method
         """
@@ -1173,30 +1193,30 @@
         # FIXME: Not entirely sure why this can happen but usually a multidex issue:
         # The given method was not added before...
         if method1.get_method() not in self._methods:
             self.add_method(method1)
 
         self._methods[method1.get_method()].add_xref_to(classobj, method2, offset)
 
-    def add_method_xref_from(self, method1, classobj, method2, offset):
+    def add_method_xref_from(self, method1: MethodAnalysis, classobj: ClassAnalysis, method2: MethodAnalysis, offset: int) -> None:
         """
 
         :param MethodAnalysis method1:
         :param ClassAnalysis classobj:
         :param MethodAnalysis method2:
         :param int offset:
         """
         # FIXME: Not entirely sure why this can happen but usually a multidex issue:
         # The given method was not added before...
         if method1.get_method() not in self._methods:
             self.add_method(method1)
 
         self._methods[method1.get_method()].add_xref_from(classobj, method2, offset)
 
-    def add_xref_to(self, ref_kind, classobj, methodobj, offset):
+    def add_xref_to(self, ref_kind: REF_TYPE, classobj: ClassAnalysis, methodobj: MethodAnalysis, offset: int) -> None:
         """
         Creates a crossreference to another class.
         XrefTo means, that the current class calls another class.
         The current class should also be contained in the another class' XrefFrom list.
 
         .. warning::
             The implementation of this specific method might not be what you expect!
@@ -1207,28 +1227,28 @@
         :param ClassAnalysis classobj: :class:`ClassAnalysis` object to link
         :param MethodAnalysis methodobj:
         :param int offset: Offset in the Methods Bytecode, where the call happens
         :return:
         """
         self.xrefto[classobj].add((ref_kind, methodobj, offset))
 
-    def add_xref_from(self, ref_kind, classobj, methodobj, offset):
+    def add_xref_from(self, ref_kind: REF_TYPE, classobj: ClassAnalysis, methodobj: MethodAnalysis, offset: int) -> None:
         """
         Creates a crossreference from this class.
         XrefFrom means, that the current class is called by another class.
 
         :param REF_TYPE ref_kind: type of call
         :param ClassAnalysis classobj: :class:`ClassAnalysis` object to link
         :param MethodAnalysis methodobj:
         :param int offset: Offset in the methods bytecode, where the call happens
         :return:
         """
         self.xreffrom[classobj].add((ref_kind, methodobj, offset))
 
-    def get_xref_from(self):
+    def get_xref_from(self) -> dict[ClassAnalysis, tuple[REF_TYPE, MethodAnalysis, int]]:
         """
         Returns a dictionary of all classes calling the current class.
         This dictionary contains also information from which method the class is accessed.
 
         .. note:: this method might contains wrong information about class usage!
 
         The dictionary contains the classes as keys (stored as :class:`ClassAnalysis`)
@@ -1246,15 +1266,15 @@
                         print("    in method {} {}".format(ref_kind, ref_method))
 
 
         :rtype: Iterator[Tuple[REF_TYPE, MethodAnalysis, int]]
         """
         return self.xreffrom
 
-    def get_xref_to(self):
+    def get_xref_to(self) -> dict[ClassAnalysis, tuple[REF_TYPE, MethodAnalysis, int]]:
         """
         Returns a dictionary of all classes which are called by the current class.
         This dictionary contains also information about the method which is called.
 
         .. note:: this method might contains wrong information about class usage!
 
         The dictionary contains the classes as keys (stored as :class:`ClassAnalysis`)
@@ -1271,86 +1291,86 @@
                     for ref_kind, ref_method, ref_offset in refs:
                         print("    calling method {} {}".format(ref_kind, ref_method))
 
         :rtype: Iterator[Tuple[REF_TYPE, MethodAnalysis, int]]
         """
         return self.xrefto
 
-    def add_xref_new_instance(self, methobj, offset):
+    def add_xref_new_instance(self, methobj:  MethodAnalysis, offset: int) -> None:
         """
         Add a crossreference to another method that is
         instancing this class.
 
         :param classobj: :class:`~MethodAnalysis`
         :param offset: integer where in the method the instantiation happens
         """
         self.xrefnewinstance.add((methobj, offset))
 
-    def get_xref_new_instance(self):
+    def get_xref_new_instance(self) -> list[tuple[MethodAnalysis, int]]:
         """
         Returns a list of tuples containing the set of methods
         with offsets that instance this class
 
 
         The list of tuples has the form:
-        (:class:`~MathodAnalysis`,
+        (:class:`~MethodAnalysis`,
         :class:`int`)
         """
         return self.xrefnewinstance
 
-    def add_xref_const_class(self, methobj, offset):
+    def add_xref_const_class(self, methobj: MethodAnalysis, offset: int) -> None:
         """
         Add a crossreference to a method referencing this classtype.
 
         :param classobj: :class:`~MethodAnalysis`
         :param offset: integer where in the method the classtype is referenced
         """
         self.xrefconstclass.add((methobj, offset))
 
-    def get_xref_const_class(self):
+    def get_xref_const_class(self) -> list[tuple[MethodAnalysis, int]]:
         """
         Returns a list of tuples containing the method and offset
         referencing this classtype.
 
         The list of tuples has the form:
         (:class:`~MethodAnalysis`,
         :class:`int`)
         """
         return self.xrefconstclass
 
-    def get_vm_class(self):
+    def get_vm_class(self) -> Union[dex.ClassDefItem,ExternalClass]:
         """
         Returns the original Dalvik VM class or the external class object.
 
         :return:
-        :rtype: Union[androguard.core.bytecodes.dvm.ClassDefItem, ExternalClass]
+        :rtype: Union[androguard.core.dex.ClassDefItem, ExternalClass]
         """
         return self.orig_class
 
-    def set_restriction_flag(self, flag):
+    def set_restriction_flag(self, flag: dex.HiddenApiClassDataItem.RestrictionApiFlag) -> None:
         """
         Set the level of restriction for this class (hidden level, from Android 10)
         (only applicable to internal classes)
 
         :param flag: The flag to set to
-        :type flag: androguard.core.bytecodes.dvm.HiddenApiClassDataItem.RestrictionApiFlag
+        :type flag: androguard.core.dex.HiddenApiClassDataItem.RestrictionApiFlag
         """
         if self.is_external():
             raise RuntimeError(
                 "Can\'t set restriction flag for external class: %s"
                 % (self.orig_class.name,))
         self.restriction_flag = flag
 
-    def set_domain_flag(self, flag):
+    def set_domain_flag(self, flag: dex.HiddenApiClassDataItem.DomapiApiFlag) -> None:
         """
         Set the api domain for this class (hidden level, from Android 10)
         (only applicable to internal classes)
 
         :param flag: The flag to set to
-        :type flag: androguard.core.bytecodes.dvm.HiddenApiClassDataItem.DomainApiFlag
+        :type flag: androguard.core.dex.HiddenApiClassDataItem.DomainApiFlag
         """
         if self.is_external():
             raise RuntimeError(
                 "Can\'t set domain flag for external class: %s"
                 % (self.orig_class.name,))
         self.domain_flag = flag
 
@@ -1398,21 +1418,21 @@
 
     XREFs are created for:
     * classes (`ClassAnalysis`)
     * methods (`MethodAnalysis`)
     * strings (`StringAnalyis`)
     * fields (`FieldAnalysis`)
 
-    The Analysis should be the only object you are using next to the :class:`~androguard.core.bytecodes.apk.APK`.
+    The Analysis should be the only object you are using next to the :class:`~androguard.core.apk.APK`.
     It encapsulates all the Dalvik related functions into a single place, while you have still the ability to use
-    the functions from :class:`~androguard.core.bytecodes.dvm.DEX` and the related classes.
+    the functions from :class:`~androguard.core.dex.DEX` and the related classes.
 
-    :param Optional[androguard.core.dex.DEX] vm: inital DEX object (default None)
+    :param Union[androguard.core.dex.DEX, None] vm: inital DEX object (default None)
     """
-    def __init__(self, vm=None):
+    def __init__(self, vm: Union[dex.DEX, None]=None) -> None:
         # Contains DEX objects
         self.vms = []
         # A dict of {classname: ClassAnalysis}, populated on add(vm)
         self.classes = dict()
         # A dict of {string: StringAnalysis}, populated on add(vm) and create_xref()
         self.strings = dict()
         # A dict of {EncodedMethod: MethodAnalysis}, populated on add(vm)
@@ -1423,19 +1443,19 @@
 
         if vm:
             self.add(vm)
 
         self.__created_xrefs = False
 
     @property
-    def fields(self):
-        """Returns FieldAnalysis list"""
+    def fields(self) -> Iterator[FieldAnalysis]:
+        """Returns FieldAnalysis generator"""
         return self.get_fields()
 
-    def add(self, vm):
+    def add(self, vm: dex.DEX) -> None:
         """
         Add a DEX to this Analysis.
 
         :param androguard.core.dex.DEX vm: :class:`androguard.core.dex.DEX` to add to this Analysis
         """
         
         self.vms.append(vm)
@@ -1474,15 +1494,15 @@
 
         # seed StringAnalysis objects into strings attribute - connect alter using xrefs
         for string_value in vm.get_strings():
             self.strings[string_value] = StringAnalysis(string_value)
 
         logger.info("Added DEX in the analysis took : {:0d}min {:02d}s".format(*divmod(int(time.time() - tic), 60)))
 
-    def create_xref(self):
+    def create_xref(self) -> None:
         """
         Create Class, Method, String and Field crossreferences
         for all classes in the Analysis.
 
         If you are using multiple DEX files, this function must
         be called when all DEX files are added.
         If you call the function after every DEX file, it will only work
@@ -1509,15 +1529,15 @@
 
         # TODO: After we collected all the information, we should add field and
         # string xrefs to each MethodAnalysis
 
         logger.info("End of creating cross references (XREF) "
                  "run time: {:0d}min {:02d}s".format(*divmod(int(time.time() - tic), 60)))
 
-    def _create_xref(self, current_class):
+    def _create_xref(self, current_class: dex.ClassDefItem) -> None:
         """
         Create the xref for `current_class`
 
         There are four steps involved in getting the xrefs:
         * Xrefs for class instantiation and static class usage
         *       for method calls
         *       for string usage
@@ -1628,15 +1648,15 @@
                         self.classes[cur_cls_name].add_field_xref_read(cur_meth, cur_cls, field_item, off)
                         cur_meth.add_xref_read(cur_cls, field_item, off)
                     else:
                         # write access to a field
                         self.classes[cur_cls_name].add_field_xref_write(cur_meth, cur_cls, field_item, off)
                         cur_meth.add_xref_write(cur_cls, field_item, off)
 
-    def get_method(self, method):
+    def get_method(self, method: dex.EncodedMethod) -> Union[MethodAnalysis,None]:
         """
         Get the :class:`MethodAnalysis` object for a given :class:`EncodedMethod`.
         This Analysis object is used to enhance EncodedMethods.
 
         :param method: :class:`EncodedMethod` to search for
         :return: :class:`MethodAnalysis` object for the given method, or None if method was not found
         :rtype: MethodAnalysis
@@ -1644,15 +1664,15 @@
         if method in self.methods:
             return self.methods[method]
         return None
 
     # Alias
     get_method_analysis = get_method
 
-    def _resolve_method(self, class_name, method_name, method_descriptor):
+    def _resolve_method(self, class_name: str, method_name: str, method_descriptor: list[str]) -> MethodAnalysis:
         """
         Resolves the Method and returns MethodAnalysis.
         Will automatically create ExternalMethods if can not resolve and add to the ClassAnalysis etc
 
         :param str class_name:
         :param str method_name:
         :param List[str] method_descriptor: Tuple which has parameters and return type, i.e. ['(I Z)', 'V']
@@ -1673,30 +1693,30 @@
             # add to all the collections we have
             self.__method_hashes[m_hash] = meth_analysis
             self.classes[class_name].add_method(meth_analysis)
             self.methods[meth] = meth_analysis
 
         return self.__method_hashes[m_hash]
 
-    def get_method_by_name(self, class_name, method_name, method_descriptor):
+    def get_method_by_name(self, class_name: str, method_name: str, method_descriptor: str) -> Union[dex.EncodedMethod,None]:
         """
         Search for a :class:`EncodedMethod` in all classes in this analysis
 
         :param class_name: name of the class, for example 'Ljava/lang/Object;'
         :param method_name: name of the method, for example 'onCreate'
         :param method_descriptor: descriptor, for example '(I I Ljava/lang/String)V
         :return: :class:`EncodedMethod` or None if method was not found
-        :rtype: androguard.core.bytecodes.dvm.EncodedMethod
+        :rtype: androguard.core.dex.EncodedMethod
         """
         m_a = self.get_method_analysis_by_name(class_name, method_name, method_descriptor)
         if m_a and not m_a.is_external():
             return m_a.get_method()
         return None
 
-    def get_method_analysis_by_name(self, class_name, method_name, method_descriptor):
+    def get_method_analysis_by_name(self, class_name: str, method_name: str, method_descriptor: str) -> Union[MethodAnalysis,None]:
         """
         Returns the crossreferencing object for a given method.
 
         This function is similar to :meth:`~get_method_analysis`, with the difference
         that you can look up the Method by name
 
         :param class_name: name of the class, for example `'Ljava/lang/Object;'`
@@ -1706,137 +1726,137 @@
         :rtype: MethodAnalysis
         """
         m_hash = (class_name, method_name, method_descriptor)
         if m_hash not in self.__method_hashes:
             return None
         return self.__method_hashes[m_hash]
 
-    def get_field_analysis(self, field):
+    def get_field_analysis(self, field: dex.EncodedField) -> Union[FieldAnalysis,None]:
         """
         Get the FieldAnalysis for a given fieldname
 
-        :param androguard.core.bytecodes.dvm.EncodedField field: the field
+        :param androguard.core.dex.EncodedField field: the field
         :return: :class:`FieldAnalysis`
         :rtype: FieldAnalysis
         """
         class_analysis = self.get_class_analysis(field.get_class_name())
         if class_analysis:
             return class_analysis.get_field_analysis(field)
         return None
 
-    def is_class_present(self, class_name):
+    def is_class_present(self, class_name: str) -> bool:
         """
         Checks if a given class name is part of this Analysis.
 
         :param class_name: classname like 'Ljava/lang/Object;' (including L and ;)
         :return: True if class was found, False otherwise
         :rtype: bool
         """
         return class_name in self.classes
 
-    def get_class_analysis(self, class_name):
+    def get_class_analysis(self, class_name: str) -> ClassAnalysis:
         """
         Returns the :class:`ClassAnalysis` object for a given classname.
 
         :param class_name: classname like 'Ljava/lang/Object;' (including L and ;)
         :return: :class:`ClassAnalysis`
         :rtype: ClassAnalysis
         """
         return self.classes.get(class_name)
 
-    def get_external_classes(self):
+    def get_external_classes(self) -> Iterator[ClassAnalysis]:
         """
         Returns all external classes, that means all classes that are not
         defined in the given set of `DalvikVMObjects`.
 
         :rtype: Iterator[ClassAnalysis]
         """
         for cls in self.classes.values():
             if cls.is_external():
                 yield cls
 
-    def get_internal_classes(self):
+    def get_internal_classes(self) -> Iterator[ClassAnalysis]:
         """
         Returns all external classes, that means all classes that are
         defined in the given set of :class:`~DEX`.
 
         :rtype: Iterator[ClassAnalysis]
         """
         for cls in self.classes.values():
             if not cls.is_external():
                 yield cls
 
-    def get_internal_methods(self):
+    def get_internal_methods(self) -> Iterator[MethodAnalysis]:
         """
         Returns all internal methods, that means all methods that are
         defined in the given set of :class:`~DEX`.
 
         :rtype: Iterator[MethodAnalysis]
         """
         for m in self.methods.values():
             if not m.is_external():
                 yield m
 
-    def get_external_methods(self):
+    def get_external_methods(self) -> Iterator[MethodAnalysis]:
         """
         Returns all external methods, that means all methods that are not
         defined in the given set of :class:`~DEX`.
 
         :rtype: Iterator[MethodAnalysis]
         """
         for m in self.methods.values():
             if m.is_external():
                 yield m
 
-    def get_strings_analysis(self):
+    def get_strings_analysis(self) -> dict[str,StringAnalysis]:
         """
         Returns a dictionary of strings and their corresponding :class:`StringAnalysis`
 
         :rtype: Dict[str, StringAnalysis]
         """
         return self.strings
 
-    def get_strings(self):
+    def get_strings(self) -> list[StringAnalysis]:
         """
         Returns a list of :class:`StringAnalysis` objects
 
         :rtype: Iterator[StringAnalysis]
         """
         return self.strings.values()
 
-    def get_classes(self):
+    def get_classes(self) -> list[ClassAnalysis]:
         """
         Returns a list of :class:`ClassAnalysis` objects
 
         Returns both internal and external classes (if any)
 
         :rtype: Iterator[ClassAnalysis]
         """
         return self.classes.values()
 
-    def get_methods(self):
+    def get_methods(self) -> Iterator[MethodAnalysis]:
         """
-        Returns a list of `MethodAnalysis` objects
+        Returns a generator of `MethodAnalysis` objects
 
         :rtype: Iterator[MethodAnalysis]
 
         """
         yield from self.methods.values()
 
-    def get_fields(self):
+    def get_fields(self) -> Iterator[FieldAnalysis]:
         """
-        Returns a list of `FieldAnalysis` objects
+        Returns a generator of `FieldAnalysis` objects
 
         :rtype: Iterator[FieldAnalysis]
         """
         for c in self.classes.values():
             for f in c.get_fields():
                 yield f
 
-    def find_classes(self, name=".*", no_external=False):
+    def find_classes(self, name:str = ".*", no_external:bool = False) -> Iterator[ClassAnalysis]:
         """
         Find classes by name, using regular expression
         This method will return all ClassAnalysis Object that match the name of
         the class.
 
         :param name: regular expression for class name (default ".*")
         :param no_external: Remove external classes from the output (default False)
@@ -1844,16 +1864,21 @@
         """
         for cname, c in self.classes.items():
             if no_external and isinstance(c.get_vm_class(), ExternalClass):
                 continue
             if re.match(name, cname):
                 yield c
 
-    def find_methods(self, classname=".*", methodname=".*", descriptor=".*",
-            accessflags=".*", no_external=False):
+    def find_methods(
+        self,
+        classname:str=".*", 
+        methodname:str=".*", 
+        descriptor:str=".*",
+        accessflags:str=".*", 
+        no_external:bool=False) -> Iterator[MethodAnalysis]:
         """
         Find a method by name using regular expression.
         This method will return all MethodAnalysis objects, which match the
         classname, methodname, descriptor and accessflags of the method.
 
         :param classname: regular expression for the classname
         :param methodname: regular expression for the method name
@@ -1876,26 +1901,31 @@
                     if no_external and isinstance(z, ExternalMethod):
                         continue
                     if re.match(methodname, z.get_name()) and \
                        re.match(descriptor, z.get_descriptor()) and \
                        re.match(accessflags, z.get_access_flags_string()):
                         yield m
 
-    def find_strings(self, string=".*"):
+    def find_strings(self, string:str=".*") -> Iterator[StringAnalysis]:
         """
         Find strings by regex
 
         :param string: regular expression for the string to search for
         :rtype: Iterator[StringAnalysis]
         """
         for s, sa in self.strings.items():
             if re.match(string, s):
                 yield sa
 
-    def find_fields(self, classname=".*", fieldname=".*", fieldtype=".*", accessflags=".*"):
+    def find_fields(
+        self,
+        classname:str=".*",
+        fieldname:str=".*",
+        fieldtype:str=".*",
+        accessflags:str=".*") -> Iterator[FieldAnalysis]:
         """
         find fields by regex
 
         :param classname: regular expression of the classname
         :param fieldname: regular expression of the fieldname
         :param fieldtype: regular expression of the fieldtype
         :param accessflags: regular expression of the access flags
@@ -1911,20 +1941,20 @@
                         yield f
 
     def __repr__(self):
         return "<analysis.Analysis VMs: {}, Classes: {}, Methods: {}, Strings: {}>".format(len(self.vms), len(self.classes), len(self.methods), len(self.strings))
 
     def get_call_graph(
         self,
-        classname=".*",
-        methodname=".*",
-        descriptor=".*",
-        accessflags=".*",
-        no_isolated=False,
-        entry_points=[]):
+        classname:str=".*",
+        methodname:str=".*",
+        descriptor:str=".*",
+        accessflags:str=".*",
+        no_isolated:bool=False,
+        entry_points:list=[]) -> nx.DiGraph:
         """
         Generate a directed graph based on the methods found by the filters applied.
         The filters are the same as in
         :meth:`~androguard.core.analysis.analysis.Analysis.find_methods`
 
         A networkx.DiGraph is returned, containing all edges only once!
         that means, if a method calls some method twice or more often, there will
@@ -1991,15 +2021,15 @@
                 # check if the edge is already in the edge set.
                 # If you need all calls, you probably want to check out MultiDiGraph
                 if not CG.has_edge(orig_method, callee_method.method):
                     CG.add_edge(orig_method, callee_method.method)
 
         return CG
 
-    def create_ipython_exports(self):
+    def create_ipython_exports(self) -> None:
         """
         .. warning:: this feature is experimental and is currently not enabled by default! Use with caution!
 
         Creates attributes for all classes, methods and fields on the Analysis object itself.
         This makes it easier to work with Analysis module in an iPython shell.
 
         Classes can be search by typing :code:`dx.CLASS_<tab>`, as each class is added via this attribute name.
@@ -2034,19 +2064,19 @@
             # If the field name is the same in the parent as in the syntetic one, we can only add one!
             for field in cls.get_fields():
                 mname = "FIELD_" + bytecode.FormatNameToPython(field.name)
                 if hasattr(cls, mname):
                     logger.warning("already existing field: {} at class {}".format(mname, name))
                 setattr(cls, mname, field)
 
-    def get_permissions(self, apilevel=None):
+    def get_permissions(self, apilevel:Union[str,int,None]=None) -> Iterator[MethodAnalysis, list[str]]:
         """
         Returns the permissions and the API method based on the API level specified.
         This can be used to find usage of API methods which require a permission.
-        Should be used in combination with an :class:`~androguard.core.bytecodes.apk.APK`.
+        Should be used in combination with an :class:`~androguard.core.apk.APK`.
 
         The returned permissions are a list, as some API methods require multiple permissions at once.
 
         The following example shows the usage and how to get the calling methods using XREF:
 
         example::
             from androguard.misc import AnalyzeAPK
@@ -2079,15 +2109,15 @@
 
         for cls in self.get_external_classes():
             for meth_analysis in cls.get_methods():
                 meth = meth_analysis.get_method()
                 if meth.permission_api_name in permmap:
                     yield meth_analysis, permmap[meth.permission_api_name]
 
-    def get_permission_usage(self, permission, apilevel=None):
+    def get_permission_usage(self, permission:str, apilevel:Union[str,int,None]=None) -> Iterator[MethodAnalysis]:
         """
         Find the usage of a permission inside the Analysis.
 
         example::
             from androguard.misc import AnalyzeAPK
             a, d, dx = AnalyzeAPK("somefile.apk")
 
@@ -2118,33 +2148,33 @@
 
         for cls in self.get_external_classes():
             for meth_analysis in cls.get_methods():
                 meth = meth_analysis.get_method()
                 if meth.permission_api_name in apis:
                     yield meth_analysis
 
-    def get_android_api_usage(self):
+    def get_android_api_usage(self) -> Iterator[MethodAnalysis]:
         """
         Get all usage of the Android APIs inside the Analysis.
 
         :return: yields :class:`MethodAnalysis` objects for all Android APIs methods
         """
 
         for cls in self.get_external_classes():
             for meth_analysis in cls.get_methods():
                 if meth_analysis.is_android_api():
                     yield meth_analysis
 
 
-def is_ascii_obfuscation(vm):
+def is_ascii_obfuscation(vm: dex.DEX) -> bool:
     """
     Tests if any class inside a DalvikVMObject
     uses ASCII Obfuscation (e.g. UTF-8 Chars in Classnames)
 
-    :param androguard.core.bytecodes.dvm.DEX vm: `DalvikVMObject`
+    :param androguard.core.dex.DEX vm: `DalvikVMObject`
     :return: True if ascii obfuscation otherwise False
     :rtype: bool
     """
     for classe in vm.get_classes():
         if is_ascii_problem(classe.get_name()):
             return True
         for method in classe.get_methods():
```

### Comparing `androguard-4.1.1/androguard/core/androconf.py` & `androguard-4.1.2/androguard/core/androconf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-import sys
+# Allows type hinting of types not-yet-declared
+# in Python >= 3.7
+# see https://peps.python.org/pep-0563/
+from __future__ import annotations
+
+
 import os
-import logging
+import sys
 import tempfile
-from colorama import init, Fore
-from loguru import logger
+from typing import Union
 
 from androguard import __version__
 from androguard.core.api_specific_resources import load_permission_mappings, load_permissions
 ANDROGUARD_VERSION = __version__
 
+from colorama import init, Fore
+from loguru import logger
 
 # initialize colorama, only has an effect on windows
 init()
 
 
 class InvalidResourceError(Exception):
     """
     Invalid Resource Erorr is thrown by load_api_specific_resource_module
     """
     pass
 
 
-def is_ascii_problem(s):
+def is_ascii_problem(s: str) -> bool:
     """
     Test if a string contains other chars than ASCII
 
     :param androguard.core.mutf8.MUTF8String s: a string to test
     :return: True if string contains other chars than ASCII, False otherwise
     :rtype: bool
     """
@@ -81,15 +87,15 @@
     },
 }
 
 
 class Configuration:
     instance = None
 
-    def __init__(self):
+    def __init__(self) -> None:
         """
         A Wrapper for the CONF object
         This creates a singleton, which has the same attributes everywhere.
         """
         if not Configuration.instance:
             Configuration.instance = default_conf
 
@@ -108,30 +114,30 @@
     def __repr__(self):
         return repr(self.instance)
 
 
 CONF = Configuration()
 
 
-def is_android(filename):
+def is_android(filename: str) -> str:
     """
     Return the type of the file
 
     :param filename : the filename
     :returns: "APK", "DEX", None
     """
     if not filename:
         return None
 
     with open(filename, "rb") as fd:
         f_bytes = fd.read()
         return is_android_raw(f_bytes)
 
 
-def is_android_raw(raw):
+def is_android_raw(raw: bytes) -> str:
     """
     Returns a string that describes the type of file, for common Android
     specific formats
     """
     val = None
 
     # We do not check for META-INF/MANIFEST.MF,
@@ -151,29 +157,29 @@
     elif raw[0:4] == b"\x03\x00\x08\x00" or raw[0:4] == b"\x00\x00\x08\x00":
         val = "AXML"
     elif raw[0:4] == b"\x02\x00\x0C\x00":
         val = "ARSC"
 
     return val
 
-def rrmdir(directory):
+def rrmdir(directory: str) -> None:
     """
     Recursivly delete a directory
 
     :param directory: directory to remove
     """
     for root, dirs, files in os.walk(directory, topdown=False):
         for name in files:
             os.remove(os.path.join(root, name))
         for name in dirs:
             os.rmdir(os.path.join(root, name))
     os.rmdir(directory)
 
 
-def make_color_tuple(color):
+def make_color_tuple(color: str) -> tuple[int,int,int]:
     """
     turn something like "#000000" into 0,0,0
     or "#FFFFFF into "255,255,255"
     """
     R = color[1:3]
     G = color[3:5]
     B = color[5:7]
@@ -181,15 +187,15 @@
     R = int(R, 16)
     G = int(G, 16)
     B = int(B, 16)
 
     return R, G, B
 
 
-def interpolate_tuple(startcolor, goalcolor, steps):
+def interpolate_tuple(startcolor: tuple[int,int,int], goalcolor: tuple[int,int,int], steps: int) -> list[str]:
     """
     Take two RGB color sets and mix them over a specified number of steps.  Return the list
     """
     # white
 
     R = startcolor[0]
     G = startcolor[1]
@@ -224,25 +230,25 @@
 
         color = str.upper("#" + hR + hG + hB)
         buffer.append(color)
 
     return buffer
 
 
-def color_range(startcolor, goalcolor, steps):
+def color_range(startcolor: tuple[int,int,int], goalcolor: tuple[int,int,int], steps: int) -> list[str]:
     """
     wrapper for interpolate_tuple that accepts colors as html ("#CCCCC" and such)
     """
     start_tuple = make_color_tuple(startcolor)
     goal_tuple = make_color_tuple(goalcolor)
 
     return interpolate_tuple(start_tuple, goal_tuple, steps)
 
 
-def load_api_specific_resource_module(resource_name, api=None):
+def load_api_specific_resource_module(resource_name: str, api:Union[str,int,None]=None) -> dict:
     """
     Load the module from the JSON files and return a dict, which might be empty
     if the resource could not be loaded.
 
     If no api version is given, the default one from the CONF dict is used.
 
     :param resource_name: Name of the resource to load
```

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/__init__.py` & `androguard-4.1.2/androguard/core/api_specific_resources/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+
 import json
 import os
 import re
+from typing import Union
 
 from loguru import logger
 
 
 class APILevelNotFoundError(Exception):
     pass
 
-
-def load_permissions(apilevel, permtype='permissions'):
+def load_permissions(apilevel:Union[str,int], permtype:str='permissions') -> dict[str, dict[str,str]]:
     """
     Load the Permissions for the given apilevel.
 
     The permissions lists are generated using this tool: https://github.com/U039b/aosp_permissions_extraction
 
     Has a fallback to select the maximum or minimal available API level.
     For example, if 28 is requested but only 26 is available, 26 is returned.
@@ -60,15 +61,15 @@
         logger.warning("Requested API Level could not be found, using {} instead".format(lower_level))
         return load_permissions(lower_level, permtype)
 
     with open(permissions_file, "r") as fp:
         return json.load(fp)[permtype]
 
 
-def load_permission_mappings(apilevel):
+def load_permission_mappings(apilevel:Union[str,int]) -> dict[str, list[str]]:
     """
     Load the API/Permission mapping for the requested API level.
     If the requetsed level was not found, None is returned.
 
     :param apilevel: integer value of the API level, i.e. 24 for Android 7.0
     :return: a dictionary of {MethodSignature: [List of Permissions]}
     """
```

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_10.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_10.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_13.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_13.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_14.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_14.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_15.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_15.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_16.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_16.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_17.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_17.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_18.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_18.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_19.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_19.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_21.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_21.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_22.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_22.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_23.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_23.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_24.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_24.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_25.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_25.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_26.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_26.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_27.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_27.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_28.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_28.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_29.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_29.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_30.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_30.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_31.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_31.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_32.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_32.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_33.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_33.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_34.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_34.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_4.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_4.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_5.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_5.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_6.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_6.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_7.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_7.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_8.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_8.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/aosp_permissions/permissions_9.json` & `androguard-4.1.2/androguard/core/api_specific_resources/aosp_permissions/permissions_9.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_16.json` & `androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_16.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_17.json` & `androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_17.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_18.json` & `androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_18.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_19.json` & `androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_19.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_21.json` & `androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_21.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_22.json` & `androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_22.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_23.json` & `androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_23.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_24.json` & `androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_24.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/api_specific_resources/api_permission_mappings/permissions_25.json` & `androguard-4.1.2/androguard/core/api_specific_resources/api_permission_mappings/permissions_25.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/apk/__init__.py` & `androguard-4.1.2/androguard/core/apk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,83 @@
-# Androguard
-from androguard.core import androconf
-from androguard.util import get_certificate_name_string
-from apkInspector.headers import ZipEntry
-
-from androguard.core.axml import ARSCParser, AXMLPrinter, ARSCResTableConfig, AXMLParser, format_value, START_TAG, END_TAG, TEXT, END_DOCUMENT
+# Allows type hinting of types not-yet-declared
+# in Python >= 3.7
+# see https://peps.python.org/pep-0563/
+from __future__ import annotations
 
 # Python core
+import binascii
+import hashlib
 import io
-from zlib import crc32
 import os
 import re
-import binascii
-import zipfile
-import logging
 from struct import unpack
-import hashlib
-import warnings
+from typing import Iterator, Union
+import zipfile
+from zlib import crc32
+
+# Androguard
+from androguard.core import androconf
+from androguard.util import get_certificate_name_string
+from apkInspector.headers import ZipEntry
+
+from androguard.core.axml import (ARSCParser,
+    AXMLPrinter,
+    ARSCResTableConfig,
+    AXMLParser,
+    format_value, 
+    START_TAG,
+    END_TAG,
+    TEXT,
+    END_DOCUMENT)
 
 # External dependecies
+from lxml.etree import Element
 import lxml.sax
 from xml.dom.pulldom import SAX2DOM
 # Used for reading Certificates
 from asn1crypto import cms, x509, keys
+
 from loguru import logger
 
 NS_ANDROID_URI = 'http://schemas.android.com/apk/res/android'
 NS_ANDROID = '{{{}}}'.format(NS_ANDROID_URI)  # Namespace as used by etree
 
-
+# Dictionary of the different protection levels mapped to their corresponding attribute names as described in
+# https://android.googlesource.com/platform/frameworks/base/+/master/core/java/android/content/pm/PermissionInfo.java
+protection_flags_to_attributes = {
+    "0x00000000": "normal",
+    "0x00000001": "dangerous",
+    "0x00000002": "signature",
+    "0x00000003": "signature or system",
+    "0x00000004": "internal",
+    "0x00000010": "privileged",
+    "0x00000020": "development",
+    "0x00000040": "appop",
+    "0x00000080": "pre23",
+    "0x00000100": "installer",
+    "0x00000200": "verifier",
+    "0x00000400": "preinstalled",
+    "0x00000800": "setup",
+    "0x00001000": "instant",
+    "0x00002000": "runtime only",
+    "0x00004000": "oem",
+    "0x00008000": "vendor privileged",
+    "0x00010000": "system text classifier",
+    "0x00020000": "wellbeing",
+    "0x00040000": "documenter",
+    "0x00080000": "configurator",
+    "0x00100000": "incident report approver",
+    "0x00200000": "app predictor",
+    "0x00400000": "module",
+    "0x00800000": "companion",
+    "0x01000000": "retail demo",
+    "0x02000000": "recents",
+    "0x04000000": "role",
+    "0x08000000": "known signer"
+}
 
 def parse_lxml_dom(tree):
     handler = SAX2DOM()
     lxml.sax.saxify(tree, handler)
     return handler.document
 
 
@@ -85,15 +131,15 @@
 
 class APKV2SignedData:
     """
     This class holds all data associated with an APK V3 SigningBlock signed data.
     source : https://source.android.com/security/apksigning/v2.html
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         self._bytes = None
         self.digests = None
         self.certificates =  None
         self.additional_attributes = None
 
     def __str__(self):
 
@@ -121,15 +167,15 @@
 
 class APKV3SignedData(APKV2SignedData):
     """
     This class holds all data associated with an APK V3 SigningBlock signed data.
     source : https://source.android.com/security/apksigning/v3.html
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self.minSDK = None
         self.maxSDK = None
 
     def __str__(self):
 
         base_str = super().__str__()
@@ -148,15 +194,15 @@
 
 class APKV2Signer:
     """
     This class holds all data associated with an APK V2 SigningBlock signer.
     source : https://source.android.com/security/apksigning/v2.html
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         self._bytes = None
         self.signed_data = None
         self.signatures = None
         self.public_key = None
 
     def __str__(self):
         return "\n".join([
@@ -168,15 +214,15 @@
 
 class APKV3Signer(APKV2Signer):
     """
     This class holds all data associated with an APK V3 SigningBlock signer.
     source : https://source.android.com/security/apksigning/v3.html
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self.minSDK = None
         self.maxSDK = None
 
     def __str__(self):
 
         base_str = super().__str__()
@@ -212,15 +258,15 @@
         0x0201 : "ECDSA with SHA2-256 digest",
         0x0202 : "ECDSA with SHA2-512 digest",
         0x0301 : "DSA with SHA2-256 digest",
     }
 
     __no_magic = False
 
-    def __init__(self, filename, raw=False, magic_file=None, skip_analysis=False, testzip=False):
+    def __init__(self, filename:str, raw:bool=False, magic_file:Union[str,None]=None, skip_analysis:bool=False, testzip:bool=False) -> None:
         """
         This class can access to all elements in an APK file
 
         example::
 
             APK("myfile.apk")
             APK(read("myfile.apk"), raw=True)
@@ -424,34 +470,34 @@
             maxSdkVersion = int(self.get_value_from_tag(item, "maxSdkVersion"))
         except ValueError:
             logger.warning(str(maxSdkVersion) + ' is not a valid value for <uses-permission> maxSdkVersion')
         except TypeError:
             pass
         return maxSdkVersion
 
-    def is_valid_APK(self):
+    def is_valid_APK(self) -> bool:
         """
         Return true if the APK is valid, false otherwise.
         An APK is seen as valid, if the AndroidManifest.xml could be successful parsed.
         This does not mean that the APK has a valid signature nor that the APK
         can be installed on an Android system.
 
         :rtype: boolean
         """
         return self.valid_apk
 
-    def get_filename(self):
+    def get_filename(self) -> str:
         """
         Return the filename of the APK
 
         :rtype: :class:`str`
         """
         return self.filename
 
-    def get_app_name(self):
+    def get_app_name(self, locale=None) -> str:
         """
         Return the appname of the APK
 
         This name is read from the AndroidManifest.xml
         using the application android:label.
         If no label exists, the android:label of the main activity is used.
 
@@ -496,22 +542,23 @@
                     return app_name
                 else:
                     # TODO should look this up, might be in the resources
                     logger.warning("Resource ID with Package name '{}' encountered! Will not resolve".format(package))
                     return app_name
 
             try:
+                config = ARSCResTableConfig(None, locale=locale) if locale else ARSCResTableConfig.default_config()
                 app_name = res_parser.get_resolved_res_configs(
                     res_id,
-                    ARSCResTableConfig.default_config())[0][1]
+                    config)[0][1]
             except Exception as e:
                 logger.warning("Exception selecting app name: %s" % e)
         return app_name
 
-    def get_app_icon(self, max_dpi=65536):
+    def get_app_icon(self, max_dpi:int=65536) -> Union[str,None]:
         """
         Return the first icon file name, which density is not greater than max_dpi,
         unless exact icon resolution is set in the manifest, in which case
         return the exact file.
 
         This information is read from the AndroidManifest.xml
 
@@ -591,53 +638,53 @@
                         app_icon = file_name
                         current_dpi = dpi
             except Exception as e:
                 logger.warning("Exception selecting app icon: %s" % e)
 
         return app_icon
 
-    def get_package(self):
+    def get_package(self) -> str:
         """
         Return the name of the package
 
         This information is read from the AndroidManifest.xml
 
         :rtype: :class:`str`
         """
         return self.package
 
-    def get_androidversion_code(self):
+    def get_androidversion_code(self) -> str:
         """
         Return the android version code
 
         This information is read from the AndroidManifest.xml
 
         :rtype: :class:`str`
         """
         return self.androidversion["Code"]
 
-    def get_androidversion_name(self):
+    def get_androidversion_name(self) -> str:
         """
         Return the android version name
 
         This information is read from the AndroidManifest.xml
 
         :rtype: :class:`str`
         """
         return self.androidversion["Name"]
 
-    def get_files(self):
+    def get_files(self) -> list[str]:
         """
         Return the file names inside the APK.
 
         :rtype: a list of :class:`str`
         """
         return self.zip.namelist()
 
-    def _get_file_magic_name(self, buffer):
+    def _get_file_magic_name(self, buffer: bytes) -> str:
         """
         Return the filetype guessed for a buffer
         :param buffer: bytes
         :returns: str of filetype
         """
         default = "Unknown"
 
@@ -681,23 +728,23 @@
 
         if not ftype:
             return default
         else:
             return self._patch_magic(buffer, ftype)
 
     @property
-    def files(self):
+    def files(self) -> dict[str, str]:
         """
         Returns a dictionary of filenames and detected magic type
 
         :returns: dictionary of files and their mime type
         """
         return self.get_files_types()
 
-    def get_files_types(self):
+    def get_files_types(self) -> dict[str,str]:
         """
         Return the files inside the APK with their associated types (by using python-magic)
 
         At the same time, the CRC32 are calculated for the files.
 
         :rtype: a dictionnary
         """
@@ -737,97 +784,97 @@
             if self.files_crc32[filename] != self.zip.infolist()[filename].crc32_of_uncompressed_data:
                 logger.error("File '{}' has different CRC32 after unpacking! "
                           "Declared: {:08x}, Calculated: {:08x}".format(filename,
                                                                         self.zip.infolist()[filename].crc32_of_uncompressed_data,
                                                                         self.files_crc32[filename]))
         return buffer
 
-    def get_files_crc32(self):
+    def get_files_crc32(self) -> dict[str, int]:
         """
         Calculates and returns a dictionary of filenames and CRC32
 
         :returns: dict of filename: CRC32
         """
         if self.files_crc32 == {}:
             for i in self.get_files():
                 self._get_crc32(i)
 
         return self.files_crc32
 
-    def get_files_information(self):
+    def get_files_information(self) -> Iterator[tuple[str, str, int]]:
         """
         Return the files inside the APK with their associated types and crc32
 
         :rtype: str, str, int
         """
         for k in self.get_files():
             yield k, self.get_files_types()[k], self.get_files_crc32()[k]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         """
         Return raw bytes of the APK
 
         :rtype: bytes
         """
 
         if self.__raw:
             return self.__raw
         else:
             with open(self.filename, 'rb') as f:
                 self.__raw = bytearray(f.read())
             return self.__raw
 
-    def get_file(self, filename):
+    def get_file(self, filename:str) -> bytes:
         """
         Return the raw data of the specified filename
         inside the APK
 
         :rtype: bytes
         """
         try:
             return self.zip.read(filename)
         except KeyError:
             raise FileNotPresent(filename)
 
-    def get_dex(self):
+    def get_dex(self) -> bytes:
         """
         Return the raw data of the classes dex file
 
         This will give you the data of the file called `classes.dex`
         inside the APK. If the APK has multiple DEX files, you need to use :func:`~APK.get_all_dex`.
 
         :rtype: bytes
         """
         try:
             return self.get_file("classes.dex")
         except FileNotPresent:
             # TODO is this a good idea to return an empty string?
             return b""
 
-    def get_dex_names(self):
+    def get_dex_names(self) -> list[str]:
         """
         Return the names of all DEX files found in the APK.
         This method only accounts for "offical" dex files, i.e. all files
         in the root directory of the APK named classes.dex or classes[0-9]+.dex
 
         :rtype: a list of str
         """
         dexre = re.compile(r"^classes(\d*).dex$")
         return filter(lambda x: dexre.match(x), self.get_files())
 
-    def get_all_dex(self):
+    def get_all_dex(self) -> Iterator[bytes]:
         """
         Return the raw data of all classes dex files
 
         :rtype: a generator of bytes
         """
         for dex_name in self.get_dex_names():
             yield self.get_file(dex_name)
 
-    def is_multidex(self):
+    def is_multidex(self) -> bool:
         """
         Test if the APK has multiple DEX files
 
         :returns: True if multiple dex found, otherwise False
         """
         dexre = re.compile(r"^classes(\d+)?.dex$")
         return len([instance for instance in self.get_files() if dexre.search(instance)]) > 1
@@ -850,16 +897,16 @@
                 value = self.package + value
             elif v_dot == -1:
                 # Not a single dot
                 value = self.package + "." + value
         return value
 
     def get_all_attribute_value(
-        self, tag_name, attribute, format_value=True, **attribute_filter
-    ):
+        self, tag_name: str, attribute: str, format_value:bool=True, **attribute_filter
+    ) -> Iterator[str]:
         """
         Yields all the attribute values in xml files which match with the tag name and the specific attribute
 
         :param str tag_name: specify the tag name
         :param str attribute: specify the attribute
         :param bool format_value: specify if the value needs to be formatted with packagename
         """
@@ -869,30 +916,30 @@
             if value is not None:
                 if format_value:
                     yield self._format_value(value)
                 else:
                     yield value
 
     def get_attribute_value(
-        self, tag_name, attribute, format_value=False, **attribute_filter
-    ):
+        self, tag_name:str, attribute:str, format_value:bool=False, **attribute_filter
+    ) -> str:
         """
         Return the attribute value in xml files which matches the tag name and the specific attribute
 
         :param str tag_name: specify the tag name
         :param str attribute: specify the attribute
         :param bool format_value: specify if the value needs to be formatted with packagename
         """
 
         for value in self.get_all_attribute_value(
                 tag_name, attribute, format_value, **attribute_filter):
             if value is not None:
                 return value
 
-    def get_value_from_tag(self, tag, attribute):
+    def get_value_from_tag(self, tag: Element, attribute: str) -> Union[str,None]:
         """
         Return the value of the android prefixed attribute in a specific tag.
 
         This function will always try to get the attribute with a android: prefix first,
         and will try to return the attribute without the prefix, if the attribute could not be found.
         This is useful for some broken AndroidManifest.xml, where no android namespace is set,
         but could also indicate malicious activity (i.e. wrongly repackaged files).
@@ -928,31 +975,31 @@
 
             if value:
                 # If value is still None, the attribute could not be found, thus is not present
                 logger.warning("Failed to get the attribute '{}' on tag '{}' with namespace. "
                             "But found the same attribute without namespace!".format(attribute, tag.tag))
         return value
 
-    def find_tags(self, tag_name, **attribute_filter):
+    def find_tags(self, tag_name: str, **attribute_filter) -> list[str]:
         """
         Return a list of all the matched tags in all available xml
 
         :param str tag: specify the tag name
         """
         all_tags = [
             self.find_tags_from_xml(
                 i, tag_name, **attribute_filter
             )
             for i in self.xml
         ]
         return [tag for tag_list in all_tags for tag in tag_list]
 
     def find_tags_from_xml(
-        self, xml_name, tag_name, **attribute_filter
-    ):
+        self, xml_name: str, tag_name: str, **attribute_filter
+    ) -> list[str]:
         """
         Return a list of all the matched tags in a specific xml
         w
         :param str xml_name: specify from which xml to pick the tag from
         :param str tag_name: specify the tag name
         """
         xml = self.xml[xml_name]
@@ -967,15 +1014,15 @@
         tags = xml.findall(".//" + tag_name)
         return [
             tag for tag in tags if self.is_tag_matched(
                 tag, **attribute_filter
             )
         ]
 
-    def is_tag_matched(self, tag, **attribute_filter):
+    def is_tag_matched(self, tag: str, **attribute_filter) -> bool:
         r"""
         Return true if the attributes matches in attribute filter.
 
         An attribute filter is a dictionary containing: {attribute_name: value}.
         This function will return True if and only if all attributes have the same value.
         This function allows to set the dictionary via kwargs, thus you can filter like this:
 
@@ -994,15 +1041,15 @@
             return True
         for attr, value in attribute_filter.items():
             _value = self.get_value_from_tag(tag, attr)
             if _value != value:
                 return False
         return True
 
-    def get_main_activities(self):
+    def get_main_activities(self) -> set[str]:
         """
         Return names of the main activities
 
         These values are read from the AndroidManifest.xml
 
         :rtype: a set of str
         """
@@ -1038,15 +1085,15 @@
                         if activity is not None:
                             y.add(item.get(self._ns("name")))
                         else:
                             logger.warning('Launcher activity without name')
 
         return x.intersection(y)
 
-    def get_main_activity(self):
+    def get_main_activity(self) -> Union[str,None]:
         """
         Return the name of the main activity
 
         This value is read from the AndroidManifest.xml
 
         :rtype: str
         """
@@ -1057,26 +1104,26 @@
             main_activities = {self._format_value(ma) for ma in activities}
             # sorted is necessary
             # 9fc7d3e8225f6b377f9181a92c551814317b77e1aa0df4c6d508d24b18f0f633
             good_main_activities = sorted(
                 main_activities.intersection(self.get_activities()))
             if good_main_activities:
                 return good_main_activities[0]
-            return main_activities[0]
+            return sorted(main_activities)[0]
         return None
 
-    def get_activities(self):
+    def get_activities(self) -> list[str]:
         """
         Return the android:name attribute of all activities
 
         :rtype: a list of str
         """
         return list(self.get_all_attribute_value("activity", "name"))
 
-    def get_activity_aliases(self):
+    def get_activity_aliases(self) -> list[dict[str,str]]:
         """
         Return the android:name and android:targetActivity attribute of all activity aliases.
 
         :rtype: a list of dict
         """
         ali = []
         for alias in self.find_tags('activity-alias'):
@@ -1087,39 +1134,39 @@
                 if not value:
                     continue
                 activity_alias[attribute] = self._format_value(value)
             if activity_alias:
                 ali.append(activity_alias)
         return ali
 
-    def get_services(self):
+    def get_services(self) -> list[str]:
         """
         Return the android:name attribute of all services
 
         :rtype: a list of str
         """
         return list(self.get_all_attribute_value("service", "name"))
 
-    def get_receivers(self):
+    def get_receivers(self) -> list[str]:
         """
         Return the android:name attribute of all receivers
 
         :rtype: a list of string
         """
         return list(self.get_all_attribute_value("receiver", "name"))
 
-    def get_providers(self):
+    def get_providers(self) -> list[str]:
         """
         Return the android:name attribute of all providers
 
         :rtype: a list of string
         """
         return list(self.get_all_attribute_value("provider", "name"))
 
-    def get_res_value(self, name):
+    def get_res_value(self, name:str) -> str:
         """
         Return the literal value with a resource id
         :rtype: str
         """
 
         res_parser = self.get_android_resources()
         if not res_parser:
@@ -1132,15 +1179,15 @@
                 ARSCResTableConfig.default_config())[0][1]
         except Exception as e:
             logger.warning("Exception get resolved resource id: %s" % e)
             return name
 
         return value
 
-    def get_intent_filters(self, itemtype, name):
+    def get_intent_filters(self, itemtype:str, name:str) -> dict[str,list[str]]:
         """
         Find intent filters for a given item and name.
 
         Intent filter are attached to activities, services or receivers.
         You can search for the intent filters of such items and get a dictionary of all
         attached actions and intent categories.
 
@@ -1183,15 +1230,15 @@
 
         for element in list(d.keys()):
             if not d[element]:
                 del d[element]
 
         return d
 
-    def get_permissions(self):
+    def get_permissions(self) -> list[str]:
         """
         Return permissions names declared in the AndroidManifest.xml.
 
         It is possible that permissions are returned multiple times,
         as this function does not filter the permissions, i.e. it shows you
         exactly what was defined in the AndroidManifest.xml.
 
@@ -1200,15 +1247,15 @@
         of implied permissions.
 
         :returns: A list of permissions
         :rtype: list
         """
         return self.permissions
 
-    def get_uses_implied_permission_list(self):
+    def get_uses_implied_permission_list(self) -> list[str]:
         """
             Return all permissions implied by the target SDK or other permissions.
 
             :rtype: list of string
         """
         target_sdk_version = self.get_effective_target_sdk_version()
 
@@ -1270,119 +1317,123 @@
             else:
                 filled_permissions[permission] = [
                     self._update_permission_protection_level(
                             protection_level, target_sdk),
                     label, description]
         return filled_permissions
 
-    def get_details_permissions(self):
+    def get_details_permissions(self) -> dict[str, list[str]]:
         """
         Return permissions with details.
 
         THis can only return details about the permission, if the permission is
         defined in the AOSP.
 
         :rtype: dict of {permission: [protectionLevel, label, description]}
         """
         l = {}
 
         for i in self.permissions:
             if i in self.permission_module:
                 x = self.permission_module[i]
                 l[i] = [x["protectionLevel"], x["label"], x["description"]]
-            else:
-                # FIXME: the permission might be signature, if it is defined by the app itself!
-                l[i] = ["normal", "Unknown permission from android reference",
+            elif i in self.declared_permissions:
+                protectionLevel_hex = self.declared_permissions[i]["protectionLevel"]
+                protectionLevel = protection_flags_to_attributes[protectionLevel_hex]
+                l[i] = [protectionLevel, "Unknown permission from android reference",
                         "Unknown permission from android reference"]
+            else:
+                # Is there a valid case not belonging to the above two?
+                logger.error(f"Unknown permission {i}")
         return self._fill_deprecated_permissions(l)
 
-    def get_requested_aosp_permissions(self):
+    def get_requested_aosp_permissions(self) -> list[str]:
         """
         Returns requested permissions declared within AOSP project.
 
         This includes several other permissions as well, which are in the platform apps.
 
         :rtype: list of str
         """
         aosp_permissions = []
         all_permissions = self.get_permissions()
         for perm in all_permissions:
             if perm in list(self.permission_module.keys()):
                 aosp_permissions.append(perm)
         return aosp_permissions
 
-    def get_requested_aosp_permissions_details(self):
+    def get_requested_aosp_permissions_details(self) -> dict[str, list[str]]:
         """
         Returns requested aosp permissions with details.
 
         :rtype: dictionary
         """
         l = {}
         for i in self.permissions:
             try:
                 l[i] = self.permission_module[i]
             except KeyError:
                 # if we have not found permission do nothing
                 continue
         return l
 
-    def get_requested_third_party_permissions(self):
+    def get_requested_third_party_permissions(self) -> list[str]:
         """
         Returns list of requested permissions not declared within AOSP project.
 
         :rtype: list of strings
         """
         third_party_permissions = []
         all_permissions = self.get_permissions()
         for perm in all_permissions:
             if perm not in list(self.permission_module.keys()):
                 third_party_permissions.append(perm)
         return third_party_permissions
 
-    def get_declared_permissions(self):
+    def get_declared_permissions(self) -> list[str]:
         """
         Returns list of the declared permissions.
 
         :rtype: list of strings
         """
         return list(self.declared_permissions.keys())
 
-    def get_declared_permissions_details(self):
+    def get_declared_permissions_details(self) -> dict[str, list[str]]:
         """
         Returns declared permissions with the details.
 
         :rtype: dict
         """
         return self.declared_permissions
 
-    def get_max_sdk_version(self):
+    def get_max_sdk_version(self) -> str:
         """
             Return the android:maxSdkVersion attribute
 
             :rtype: string
         """
         return self.get_attribute_value("uses-sdk", "maxSdkVersion")
 
-    def get_min_sdk_version(self):
+    def get_min_sdk_version(self) -> str:
         """
             Return the android:minSdkVersion attribute
 
             :rtype: string
         """
         return self.get_attribute_value("uses-sdk", "minSdkVersion")
 
-    def get_target_sdk_version(self):
+    def get_target_sdk_version(self) -> str:
         """
             Return the android:targetSdkVersion attribute
 
             :rtype: string
         """
         return self.get_attribute_value("uses-sdk", "targetSdkVersion")
 
-    def get_effective_target_sdk_version(self):
+    def get_effective_target_sdk_version(self) -> int:
         """
             Return the effective targetSdkVersion, always returns int > 0.
 
             If the targetSdkVersion is not set, it defaults to 1.  This is
             set based on defaults as defined in:
             https://developer.android.com/guide/topics/manifest/uses-sdk-element.html
 
@@ -1392,89 +1443,93 @@
         if not target_sdk_version:
             target_sdk_version = self.get_min_sdk_version()
         try:
             return int(target_sdk_version)
         except (ValueError, TypeError):
             return 1
 
-    def get_libraries(self):
+    def get_libraries(self) -> list[str]:
         """
             Return the android:name attributes for libraries
 
             :rtype: list
         """
         return list(self.get_all_attribute_value("uses-library", "name"))
 
-    def get_features(self):
+    def get_features(self) -> list[str]:
         """
         Return a list of all android:names found for the tag uses-feature
         in the AndroidManifest.xml
 
         :returns: list
         """
         return list(self.get_all_attribute_value("uses-feature", "name"))
 
-    def is_wearable(self):
+    def is_wearable(self) -> bool:
         """
         Checks if this application is build for wearables by
         checking if it uses the feature 'android.hardware.type.watch'
         See: https://developer.android.com/training/wearables/apps/creating.html for more information.
 
         Not every app is setting this feature (not even the example Google provides),
         so it might be wise to not 100% rely on this feature.
 
         :returns: True if wearable, False otherwise
         """
         return 'android.hardware.type.watch' in self.get_features()
 
-    def is_leanback(self):
+    def is_leanback(self) -> bool:
         """
         Checks if this application is build for TV (Leanback support)
         by checkin if it uses the feature 'android.software.leanback'
 
         :returns: True if leanback feature is used, false otherwise
         """
         return 'android.software.leanback' in self.get_features()
 
-    def is_androidtv(self):
+    def is_androidtv(self) -> bool:
         """
         Checks if this application does not require a touchscreen,
         as this is the rule to get into the TV section of the Play Store
         See: https://developer.android.com/training/tv/start/start.html for more information.
 
         :returns: True if 'android.hardware.touchscreen' is not required, False otherwise
         """
         return self.get_attribute_value('uses-feature', 'name', required="false", name="android.hardware.touchscreen") == "android.hardware.touchscreen"
 
-    def get_certificate_der(self, filename):
+    def get_certificate_der(self, filename:str) -> bytes:
         """
         Return the DER coded X.509 certificate from the signature file.
 
         :param filename: Signature filename in APK
         :returns: DER coded X.509 certificate as binary
         """
         pkcs7message = self.get_file(filename)
 
         pkcs7obj = cms.ContentInfo.load(pkcs7message)
+        # TODO: should be returning the matching cert here!
+        # https://github.com/androguard/androguard/pull/1038
+        if len(pkcs7obj['content']['certificates']) > 1:
+            logger.warning(f"Multiple certificates found. Returning the first one!")
         cert = pkcs7obj['content']['certificates'][0].chosen.dump()
         return cert
 
-    def get_certificate(self, filename):
+    def get_certificate(self, filename:str) -> x509.Certificate: 
         """
         Return a X.509 certificate object by giving the name in the apk file
 
         :param filename: filename of the signature file in the APK
         :returns: a :class:`Certificate` certificate
         """
         cert = self.get_certificate_der(filename)
         certificate = x509.Certificate.load(cert)
 
         return certificate
 
-    def new_zip(self, filename, deleted_files=None, new_files={}):
+    def new_zip(self, filename:str, deleted_files:Union[str,None]=None, new_files:dict={}) -> None:
         """
             Create a new zip file
 
             :param filename: the output filename of the zip
             :param deleted_files: a regex pattern to remove specific file
             :param new_files: a dictionnary of new files
 
@@ -1507,96 +1562,96 @@
             # Block three: deleted_files is None, new_files is empty.
             # Just write out the default zip
             else:
                 buffer = self.zip.read(item)
                 zout.writestr(item, buffer)
         zout.close()
 
-    def get_android_manifest_axml(self):
+    def get_android_manifest_axml(self) -> Union[AXMLPrinter,None]:
         """
             Return the :class:`AXMLPrinter` object which corresponds to the AndroidManifest.xml file
 
-            :rtype: :class:`~androguard.core.bytecodes.axml.AXMLPrinter`
+            :rtype: :class:`~androguard.core.axml.AXMLPrinter`
         """
         try:
             return self.axml["AndroidManifest.xml"]
         except KeyError:
             return None
 
-    def get_android_manifest_xml(self):
+    def get_android_manifest_xml(self) -> Union[lxml.etree.Element, None]:
         """
         Return the parsed xml object which corresponds to the AndroidManifest.xml file
 
         :rtype: :class:`~lxml.etree.Element`
         """
         try:
             return self.xml["AndroidManifest.xml"]
         except KeyError:
             return None
 
-    def get_android_resources(self):
+    def get_android_resources(self) -> Union[ARSCParser,None]:
         """
-        Return the :class:`~androguard.core.bytecodes.axml.ARSCParser` object which corresponds to the resources.arsc file
+        Return the :class:`~androguard.core.axml.ARSCParser` object which corresponds to the resources.arsc file
 
-        :rtype: :class:`~androguard.core.bytecodes.axml.ARSCParser`
+        :rtype: :class:`~androguard.core.axml.ARSCParser`
         """
         try:
             return self.arsc["resources.arsc"]
         except KeyError:
             if "resources.arsc" not in self.zip.namelist():
                 # There is a rare case, that no resource file is supplied.
                 # Maybe it was added manually, thus we check here
                 return None
             self.arsc["resources.arsc"] = ARSCParser(self.zip.read("resources.arsc"))
             return self.arsc["resources.arsc"]
 
-    def is_signed(self):
+    def is_signed(self) -> bool:
         """
         Returns true if any of v1, v2, or v3 signatures were found.
         """
         return self.is_signed_v1() or self.is_signed_v2() or self.is_signed_v3()
 
-    def is_signed_v1(self):
+    def is_signed_v1(self) -> bool:
         """
         Returns true if a v1 / JAR signature was found.
 
         Returning `True` does not mean that the file is properly signed!
         It just says that there is a signature file which needs to be validated.
         """
         return self.get_signature_name() is not None
 
-    def is_signed_v2(self):
+    def is_signed_v2(self) -> bool:
         """
         Returns true of a v2 / APK signature was found.
 
         Returning `True` does not mean that the file is properly signed!
         It just says that there is a signature file which needs to be validated.
         """
         if self._is_signed_v2 is None:
             self.parse_v2_v3_signature()
 
         return self._is_signed_v2
 
-    def is_signed_v3(self):
+    def is_signed_v3(self) -> bool:
         """
         Returns true of a v3 / APK signature was found.
 
         Returning `True` does not mean that the file is properly signed!
         It just says that there is a signature file which needs to be validated.
         """
         if self._is_signed_v3 is None:
             self.parse_v2_v3_signature()
 
         return self._is_signed_v3
 
-    def read_uint32_le(self, io_stream):
+    def read_uint32_le(self, io_stream) -> int:
         value, = unpack('<I', io_stream.read(4))
         return value
 
-    def parse_signatures_or_digests(self, digest_bytes):
+    def parse_signatures_or_digests(self, digest_bytes) -> list[tuple[int, bytes]]:
         """ Parse digests """
 
         if not len(digest_bytes):
             return []
 
         digests = []
         block = io.BytesIO(digest_bytes)
@@ -1608,15 +1663,15 @@
             digest_len = self.read_uint32_le(block)
             digest = block.read(digest_len)
 
             digests.append((algorithm_id, digest))
 
         return digests
 
-    def parse_v2_v3_signature(self):
+    def parse_v2_v3_signature(self) -> None:
         # Need to find an v2 Block in the APK.
         # The Google Docs gives you the following rule:
         # * go to the end of the ZIP File
         # * search for the End of Central directory
         # * then jump to the beginning of the central directory
         # * Read now the magic of the signing block
         # * before the magic there is the size_of_block, so we can jump to
@@ -1680,25 +1735,30 @@
         if size_of_block_start != size_of_block:
             raise BrokenAPKError("Sizes at beginning and and does not match!")
 
         # Store all blocks
         while f.tell() < end_offset - 24:
             size, key = unpack('<QI', f.read(12))
             value = f.read(size - 4)
-            self._v2_blocks[key] = value
+            if key in self._v2_blocks:
+                # TODO: Store the duplicate V2 Signature blocks and offer a way to show them
+                # https://github.com/androguard/androguard/issues/1030
+                logger.warning("Duplicate block ID in APK Signing Block: {}".format(key))
+            else:
+                self._v2_blocks[key] = value
 
         # Test if a signature is found
         if self._APK_SIG_KEY_V2_SIGNATURE in self._v2_blocks:
             self._is_signed_v2 = True
 
         if self._APK_SIG_KEY_V3_SIGNATURE in self._v2_blocks:
             self._is_signed_v3 = True
 
 
-    def parse_v3_signing_block(self):
+    def parse_v3_signing_block(self) -> None:
         """
         Parse the V2 signing block and extract all features
         """
 
         self._v3_signing_data = []
 
         # calling is_signed_v3 should also load the signature, if any
@@ -1789,15 +1849,15 @@
             signer.signatures = sigs
             signer.public_key = publickey
             signer.minSDK = signer_min_sdk
             signer.maxSDK = signer_max_sdk
 
             self._v3_signing_data.append(signer)
 
-    def parse_v2_signing_block(self):
+    def parse_v2_signing_block(self) -> None:
         """
         Parse the V2 signing block and extract all features
         """
 
         self._v2_signing_data = []
 
         # calling is_signed_v2 should also load the signature
@@ -1871,145 +1931,145 @@
             signer._bytes = view[off_signer:off_signer+size_signer]
             signer.signed_data = signed_data_object
             signer.signatures = sigs
             signer.public_key = publickey
 
             self._v2_signing_data.append(signer)
 
-    def get_public_keys_der_v3(self):
+    def get_public_keys_der_v3(self) -> list[bytes]:
         """
         Return a list of DER coded X.509 public keys from the v3 signature block
         """
 
         if self._v3_signing_data == None:
             self.parse_v3_signing_block()
 
         public_keys = []
 
         for signer in self._v3_signing_data:
             public_keys.append(signer.public_key)
 
         return public_keys
 
-    def get_public_keys_der_v2(self):
+    def get_public_keys_der_v2(self) -> list[bytes]:
         """
         Return a list of DER coded X.509 public keys from the v3 signature block
         """
 
         if self._v2_signing_data == None:
             self.parse_v2_signing_block()
 
         public_keys = []
 
         for signer in self._v2_signing_data:
             public_keys.append(signer.public_key)
 
         return public_keys
 
-    def get_certificates_der_v3(self):
+    def get_certificates_der_v3(self) -> list[bytes]:
         """
         Return a list of DER coded X.509 certificates from the v3 signature block
         """
 
         if self._v3_signing_data == None:
             self.parse_v3_signing_block()
 
         certs = []
         for signed_data in [signer.signed_data for signer in self._v3_signing_data]:
             for cert in signed_data.certificates:
                 certs.append(cert)
 
         return certs
 
-    def get_certificates_der_v2(self):
+    def get_certificates_der_v2(self) -> list[bytes]:
         """
         Return a list of DER coded X.509 certificates from the v3 signature block
         """
 
         if self._v2_signing_data == None:
             self.parse_v2_signing_block()
 
         certs = []
         for signed_data in [signer.signed_data for signer in self._v2_signing_data]:
             for cert in signed_data.certificates:
                 certs.append(cert)
 
         return certs
 
-    def get_public_keys_v3(self):
+    def get_public_keys_v3(self) -> list[keys.PublicKeyInfo]:
         """
         Return a list of :class:`asn1crypto.keys.PublicKeyInfo` which are found
         in the v3 signing block.
         """
         return [ keys.PublicKeyInfo.load(pkey) for pkey in self.get_public_keys_der_v3()]
 
-    def get_public_keys_v2(self):
+    def get_public_keys_v2(self) -> list[keys.PublicKeyInfo]:
         """
         Return a list of :class:`asn1crypto.keys.PublicKeyInfo` which are found
         in the v2 signing block.
         """
         return [ keys.PublicKeyInfo.load(pkey) for pkey in self.get_public_keys_der_v2()]
 
-    def get_certificates_v3(self):
+    def get_certificates_v3(self) -> list[x509.Certificate]:
         """
         Return a list of :class:`asn1crypto.x509.Certificate` which are found
         in the v3 signing block.
         Note that we simply extract all certificates regardless of the signer.
         Therefore this is just a list of all certificates found in all signers.
         """
         return [ x509.Certificate.load(cert) for cert in self.get_certificates_der_v3()]
 
-    def get_certificates_v2(self):
+    def get_certificates_v2(self) -> list[x509.Certificate]:
         """
         Return a list of :class:`asn1crypto.x509.Certificate` which are found
         in the v2 signing block.
         Note that we simply extract all certificates regardless of the signer.
         Therefore this is just a list of all certificates found in all signers.
         """
         return [ x509.Certificate.load(cert) for cert in self.get_certificates_der_v2()]
 
-    def get_certificates_v1(self):
+    def get_certificates_v1(self) -> list[x509.Certificate]:
         """
         Return a list of :class:`asn1crypto.x509.Certificate` which are found
         in the META-INF folder (v1 signing).
         Note that we simply extract all certificates regardless of the signer.
         Therefore this is just a list of all certificates found in all signers.
         """
         certs = []
         for x in self.get_signature_names():
             certs.append(x509.Certificate.load(self.get_certificate_der(x)))
 
         return certs
 
-    def get_certificates(self):
+    def get_certificates(self) -> list[x509.Certificate]:
         """
         Return a list of unique :class:`asn1crypto.x509.Certificate` which are found
         in v1, v2 and v3 signing
         Note that we simply extract all certificates regardless of the signer.
         Therefore this is just a list of all certificates found in all signers.
         """
         fps = []
         certs = []
         for x in self.get_certificates_v1() + self.get_certificates_v2() + self.get_certificates_v3():
             if x.sha256 not in fps:
                 fps.append(x.sha256)
                 certs.append(x)
         return certs
 
-    def get_signature_name(self):
+    def get_signature_name(self) -> Union[str,None]:
         """
             Return the name of the first signature file found.
         """
         if self.get_signature_names():
             return self.get_signature_names()[0]
         else:
             # Unsigned APK
             return None
 
-    def get_signature_names(self):
+    def get_signature_names(self) -> list[str]:
         """
         Return a list of the signature file names (v1 Signature / JAR
         Signature)
 
         :rtype: List of filenames matching a Signature
         """
         signature_expr = re.compile(r"^(META-INF/)(.*)(\.RSA|\.EC|\.DSA)$")
@@ -2020,27 +2080,27 @@
                 if "{}.SF".format(i.rsplit(".", 1)[0]) in self.get_files():
                     signatures.append(i)
                 else:
                     logger.warning("v1 signature file {} missing .SF file - Partial signature!".format(i))
 
         return signatures
 
-    def get_signature(self):
+    def get_signature(self) -> Union[str,None]:
         """
         Return the data of the first signature file found (v1 Signature / JAR
         Signature)
 
         :rtype: First signature name or None if not signed
         """
         if self.get_signatures():
             return self.get_signatures()[0]
         else:
             return None
 
-    def get_signatures(self):
+    def get_signatures(self) -> list[bytes]:
         """
         Return a list of the data of the signature files.
         Only v1 / JAR Signing.
 
         :rtype: list of bytes
         """
         signature_expr = re.compile(r"^(META-INF/)(.*)(\.RSA|\.EC|\.DSA)$")
@@ -2048,15 +2108,15 @@
 
         for i in self.get_files():
             if signature_expr.search(i):
                 signature_datas.append(self.get_file(i))
 
         return signature_datas
 
-    def show(self):
+    def show(self) -> None:
         self.get_files_types()
 
         print("FILES: ")
         for i in self.get_files():
             try:
                 print("\t", i, self._files[i], "%x" % self.files_crc32[i])
             except KeyError:
@@ -2101,15 +2161,15 @@
 
         if self.is_signed_v2():
             print("CERTIFICATES v2:")
             for c in self.get_certificates_v2():
                 show_Certificate(c)
 
 
-def show_Certificate(cert, short=False):
+def show_Certificate(cert, short:bool=False) -> None:
     """
         Print Fingerprints, Issuer and Subject of an X509 Certificate.
 
         :param cert: X509 Certificate to print
         :param short: Print in shortform for DN (Default: False)
 
         :type cert: :class:`asn1crypto.x509.Certificate`
@@ -2117,15 +2177,15 @@
     """
     print("SHA1 Fingerprint: {}".format(cert.sha1_fingerprint))
     print("SHA256 Fingerprint: {}".format(cert.sha256_fingerprint))
     print("Issuer: {}".format(get_certificate_name_string(cert.issuer.native, short=short)))
     print("Subject: {}".format(get_certificate_name_string(cert.subject.native, short=short)))
 
 
-def ensure_final_value(packageName, arsc, value):
+def ensure_final_value(packageName:str, arsc:ARSCParser, value:str) -> str:
     """Ensure incoming value is always the value, not the resid
 
     androguard will sometimes return the Android "resId" aka
     Resource ID instead of the actual value.  This checks whether
     the value is actually a resId, then performs the Android
     Resource lookup as needed.
 
@@ -2140,15 +2200,15 @@
                 returnValue = arsc.get_string(packageName, res_id)[1]
             except (ValueError, TypeError):
                 pass
         return returnValue
     return ''
 
 
-def get_apkid(apkfile):
+def get_apkid(apkfile: str) -> tuple[str,str,str]:
     """Read (appid, versionCode, versionName) from an APK
 
     This first tries to do quick binary XML parsing to just get the
     values that are needed.  It will fallback to full androguard
     parsing, which is slow, if it can't find the versionName value or
     versionName is set to a Android String Resource (e.g. an integer
     hex value that starts with @).
```

### Comparing `androguard-4.1.1/androguard/core/axml/__init__.py` & `androguard-4.1.2/androguard/core/axml/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-from androguard.core.resources import public
-from .types import *
+# Allows type hinting of types not-yet-declared
+# in Python >= 3.7
+# see https://peps.python.org/pep-0563/
+from __future__ import annotations
 
-from struct import pack, unpack
-from xml.sax.saxutils import escape
-import collections
+import binascii
 from collections import defaultdict
+import collections
+import io
+import re
+from struct import pack, unpack
+from typing import BinaryIO, Union
+
+from androguard.core.resources import public
+from .types import *
 
-from lxml import etree
 from loguru import logger
-import re
-import binascii
-import io
+from lxml import etree
+from xml.sax.saxutils import escape
 
 # Constants for ARSC Files
 # see http://aospxref.com/android-13.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#233
 RES_NULL_TYPE = 0x0000
 RES_STRING_POOL_TYPE = 0x0001
 RES_TABLE_TYPE = 0x0002
 RES_XML_TYPE = 0x0003
@@ -81,29 +87,29 @@
 
 
 class ResParserError(Exception):
     """Exception for the parsers"""
     pass
 
 
-def complexToFloat(xcomplex):
+def complexToFloat(xcomplex) -> float:
     """
     Convert a complex unit into float
     """
     return float(xcomplex & 0xFFFFFF00) * RADIX_MULTS[(xcomplex >> 4) & 3]
 
 
 class StringBlock:
     """
     StringBlock is a CHUNK inside an AXML File: `ResStringPool_header`
     It contains all strings, which are used by referecing to ID's
 
     See http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#436
     """
-    def __init__(self, buff, header):
+    def __init__(self, buff:BinaryIO, header:ARSCHeader) -> None:
         """
         :param buff: buffer which holds the string block
         :param header: a instance of :class:`~ARSCHeader`
         """
         self._cache = {}
         self.header = header
         # We already read the header (which was chunk_type and chunk_size
@@ -187,15 +193,15 @@
     def __iter__(self):
         """
         Iterable over all strings
         """
         for i in range(self.stringCount):
             yield self.getString(i)
 
-    def getString(self, idx):
+    def getString(self, idx: int) -> str:
         """
         Return the string at the index in the string table
 
         :param idx: index in the string table
         :return: str
         """
         if idx in self._cache:
@@ -209,24 +215,24 @@
         if self.m_isUTF8:
             self._cache[idx] = self._decode8(offset)
         else:
             self._cache[idx] = self._decode16(offset)
 
         return self._cache[idx]
 
-    def getStyle(self, idx):
+    def getStyle(self, idx:int) -> int:
         """
         Return the style associated with the index
 
         :param idx: index of the style
         :return:
         """
         return self.m_styles[idx]
 
-    def _decode8(self, offset):
+    def _decode8(self, offset:int) -> str:
         """
         Decode an UTF-8 String at the given offset
 
         :param offset: offset of the string inside the data
         :return: str
         """
         # UTF-8 Strings contain two lengths, as they might differ:
@@ -234,43 +240,58 @@
         str_len, skip = self._decode_length(offset, 1)
         offset += skip
 
         # 2) the utf-8 string length
         encoded_bytes, skip = self._decode_length(offset, 1)
         offset += skip
 
+        # Two checks should happen here:
+        # a) offset + encoded_bytes surpassing the string_pool length and
+        # b) non-null terminated strings which should be rejected
+        # platform/frameworks/base/libs/androidfw/ResourceTypes.cpp#789
+        if len(self.m_charbuff) < (offset + encoded_bytes):
+            logger.warning(f"String size: {offset + encoded_bytes} is exceeding string pool size. Returning empty string.")
+            return ""
         data = self.m_charbuff[offset: offset + encoded_bytes]
 
         if self.m_charbuff[offset + encoded_bytes] != 0:
             raise ResParserError("UTF-8 String is not null terminated! At offset={}".format(offset))
 
         return self._decode_bytes(data, 'utf-8', str_len)
 
-    def _decode16(self, offset):
+    def _decode16(self, offset:int) -> str:
         """
         Decode an UTF-16 String at the given offset
 
         :param offset: offset of the string inside the data
         :return: str
         """
         str_len, skip = self._decode_length(offset, 2)
         offset += skip
 
         # The len is the string len in utf-16 units
         encoded_bytes = str_len * 2
 
+        # Two checks should happen here:
+        # a) offset + encoded_bytes surpassing the string_pool length and
+        # b) non-null terminated strings which should be rejected
+        # platform/frameworks/base/libs/androidfw/ResourceTypes.cpp#789
+        if len(self.m_charbuff) < (offset + encoded_bytes):
+            logger.warning(f"String size: {offset + encoded_bytes} is exceeding string pool size. Returning empty string.")
+            return ""
+
         data = self.m_charbuff[offset: offset + encoded_bytes]
 
         if self.m_charbuff[offset + encoded_bytes:offset + encoded_bytes + 2] != b"\x00\x00":
             raise ResParserError("UTF-16 String is not null terminated! At offset={}".format(offset))
 
         return self._decode_bytes(data, 'utf-16', str_len)
 
     @staticmethod
-    def _decode_bytes(data, encoding, str_len):
+    def _decode_bytes(data:bytes, encoding:str, str_len:int) -> str:
         """
         Generic decoding with length check.
         The string is decoded from bytes with the given encoding, then the length
         of the string is checked.
         The string is decoded using the "replace" method.
 
         :param data: bytes
@@ -279,15 +300,15 @@
         :return: str
         """
         string = data.decode(encoding, 'replace')
         if len(string) != str_len:
             logger.warning("invalid decoded string length")
         return string
 
-    def _decode_length(self, offset, sizeof_char):
+    def _decode_length(self, offset:int, sizeof_char:int) -> tuple[int,int]:
         """
         Generic Length Decoding at offset of string
 
         The method works for both 8 and 16 bit Strings.
         Length checks are enforced:
         * 8 bit strings: maximum of 0x7FFF bytes (See
         http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/ResourceTypes.cpp#692)
@@ -316,15 +337,15 @@
         if sizeof_char == 1:
             assert length <= 0x7FFF, "length of UTF-8 string is too large! At offset={}".format(offset)
         else:
             assert length <= 0x7FFFFFFF, "length of UTF-16 string is too large!  At offset={}".format(offset)
 
         return length, size
 
-    def show(self):
+    def show(self) -> None:
         """
         Print some information on stdout about the string table
         """
         print("StringBlock(stringsCount=0x%x, "
               "stringsOffset=0x%x, "
               "stylesCount=0x%x, "
               "stylesOffset=0x%x, "
@@ -367,23 +388,24 @@
     Note that not all chunk types are yielded from the iterator! Some chunks are processed in
     the AXMLParser only.
     The parser will set `is_valid()` to False if it parses something not valid.
     Messages what is wrong are logged.
 
     See http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#563
     """
-    def __init__(self, raw_buff):
+    def __init__(self, raw_buff:bytes) -> None:
         logger.debug("AXMLParser")
 
         self._reset()
 
         self._valid = True
         self.axml_tampered = False
         self.buff = io.BufferedReader(io.BytesIO(raw_buff))
         self.buff_size = self.buff.raw.getbuffer().nbytes
+        self.packerwarning = False
 
         # Minimum is a single ARSCHeader, which would be a strange edge case...
         if self.buff_size < 8:
             logger.error("Filesize is too small to be a valid AXML file! Filesize: {}".format(self.buff_size))
             self._valid = False
             return
 
@@ -453,15 +475,15 @@
 
         # Stores resource ID mappings, if any
         self.m_resourceIDs = []
 
         # Store a list of prefix/uri mappings encountered
         self.namespaces = []
 
-    def is_valid(self):
+    def is_valid(self) -> bool:
         """
         Get the state of the AXMLPrinter.
         if an error happend somewhere in the process of parsing the file,
         this flag is set to False.
         """
         logger.debug(self._valid)
         return self._valid
@@ -666,52 +688,52 @@
                 break
 
             # Still here? Looks like we read an unknown XML header, try to skip it...
             logger.warning("Unknown XML Chunk: 0x{:04x}, skipping {} bytes.".format(h.type, h.size))
             self.buff.seek(h.end)
 
     @property
-    def name(self):
+    def name(self) -> str:
         """
         Return the String assosciated with the tag name
         """
         if self.m_name == -1 or (self.m_event != START_TAG and self.m_event != END_TAG):
             return ''
 
         return self.sb[self.m_name]
 
     @property
-    def comment(self):
+    def comment(self) -> Union[str,None]:
         """
         Return the comment at the current position or None if no comment is given
 
         This works only for Tags, as the comments of Namespaces are silently dropped.
         Currently, there is no way of retrieving comments of namespaces.
         """
         if self.m_comment_index == 0xFFFFFFFF:
             return None
 
         return self.sb[self.m_comment_index]
 
     @property
-    def namespace(self):
+    def namespace(self) -> str:
         """
         Return the Namespace URI (if any) as a String for the current tag
         """
         if self.m_name == -1 or (self.m_event != START_TAG and self.m_event != END_TAG):
             return ''
 
         # No Namespace
         if self.m_namespaceUri == 0xFFFFFFFF:
             return ''
 
         return self.sb[self.m_namespaceUri]
 
     @property
-    def nsmap(self):
+    def nsmap(self) -> dict[str,str]:
         """
         Returns the current namespace mapping as a dictionary
 
         there are several problems with the map and we try to guess a few
         things here:
 
         1) a URI can be mapped by many prefixes, so it is to decide which one to take
@@ -724,43 +746,43 @@
         # solve 3) by using a set
         for k, v in set(self.namespaces):
             s_prefix = self.sb[k]
             s_uri = self.sb[v]
             # Solve 2) & 4) by not including
             if s_uri != "" and s_prefix != "":
                 # solve 1) by using the last one in the list
-                NSMAP[s_prefix] = s_uri
+                NSMAP[s_prefix] = s_uri.strip()
 
         return NSMAP
 
     @property
-    def text(self):
+    def text(self) -> str:
         """
         Return the String assosicated with the current text
         """
         if self.m_name == -1 or self.m_event != TEXT:
             return ''
 
         return self.sb[self.m_name]
 
-    def getName(self):
+    def getName(self) -> str:
         """
         Legacy only!
         use :py:attr:`~androguard.core.bytecodes.AXMLParser.name` instead
         """
         return self.name
 
-    def getText(self):
+    def getText(self) -> str:
         """
         Legacy only!
         use :py:attr:`~androguard.core.bytecodes.AXMLParser.text` instead
         """
         return self.text
 
-    def getPrefix(self):
+    def getPrefix(self) -> str:
         """
         Legacy only!
         use :py:attr:`~androguard.core.bytecodes.AXMLParser.namespace` instead
         """
         return self.namespace
 
     def _get_attribute_offset(self, index):
@@ -772,81 +794,85 @@
 
         offset = index * ATTRIBUTE_LENGTH
         if offset >= len(self.m_attributes):
             logger.warning("Invalid attribute index")
 
         return offset
 
-    def getAttributeCount(self):
+    def getAttributeCount(self) -> int:
         """
         Return the number of Attributes for a Tag
         or -1 if not in a tag
         """
         if self.m_event != START_TAG:
             return -1
 
         return self.m_attribute_count
 
-    def getAttributeUri(self, index):
+    def getAttributeUri(self, index:int):
         """
         Returns the numeric ID for the namespace URI of an attribute
         """
         logger.debug(index)
 
         offset = self._get_attribute_offset(index)
         uri = self.m_attributes[offset + ATTRIBUTE_IX_NAMESPACE_URI]
 
         return uri
 
-    def getAttributeNamespace(self, index):
+    def getAttributeNamespace(self, index:int):
         """
         Return the Namespace URI (if any) for the attribute
         """
         logger.debug(index)
 
         uri = self.getAttributeUri(index)
 
         # No Namespace
         if uri == 0xFFFFFFFF:
             return ''
 
         return self.sb[uri]
 
-    def getAttributeName(self, index):
+    def getAttributeName(self, index:int):
         """
         Returns the String which represents the attribute name
         """
         logger.debug(index)
         offset = self._get_attribute_offset(index)
         name = self.m_attributes[offset + ATTRIBUTE_IX_NAME]
 
         res = self.sb[name]
         # If the result is a (null) string, we need to look it up.
-        if not res or res == ":":
+        if name <= len(self.m_resourceIDs):
             attr = self.m_resourceIDs[name]
             if attr in public.SYSTEM_RESOURCES['attributes']['inverse']:
-                res = 'android:' + public.SYSTEM_RESOURCES['attributes']['inverse'][attr]
-            else:
-                # Attach the HEX Number, so for multiple missing attributes we do not run
-                # into problems.
-                res = 'android:UNKNOWN_SYSTEM_ATTRIBUTE_{:08x}'.format(attr)
+                res = public.SYSTEM_RESOURCES['attributes']['inverse'][attr].replace("_",
+                                                                               ":")
+                if res != self.sb[name]:
+                    self.packerwarning = True
+
+        if not res or res == ":":
+            # Attach the HEX Number, so for multiple missing attributes we do not run
+            # into problems.
+            res = 'android:UNKNOWN_SYSTEM_ATTRIBUTE_{:08x}'.format(attr)
         return res
 
-    def getAttributeValueType(self, index):
+    def getAttributeValueType(self, index:int):
         """
         Return the type of the attribute at the given index
 
         :param index: index of the attribute
         """
         logger.debug(index)
 
         offset = self._get_attribute_offset(index)
         return self.m_attributes[offset + ATTRIBUTE_IX_VALUE_TYPE]
 
-    def getAttributeValueData(self, index):
+    def getAttributeValueData(self, index:int):
         """
         Return the data of the attribute at the given index
 
         :param index: index of the attribute
         """
         logger.debug(index)
 
@@ -868,15 +894,15 @@
         valueType = self.m_attributes[offset + ATTRIBUTE_IX_VALUE_TYPE]
         if valueType == TYPE_STRING:
             valueString = self.m_attributes[offset + ATTRIBUTE_IX_VALUE_STRING]
             return self.sb[valueString]
         return ''
 
 
-def format_value(_type, _data, lookup_string=lambda ix: "<string>"):
+def format_value(_type: int, _data: int, lookup_string=lambda ix: "<string>") -> str:
     """
     Format a value based on type and data.
     By default, no strings are looked up and "<string>" is returned.
     You need to define `lookup_string` in order to actually lookup strings from
     the string table.
 
     :param _type: The numeric type of the value
@@ -932,15 +958,15 @@
     converted into XML.
 
     A Reference Implementation can be found at http://androidxref.com/9.0.0_r3/xref/frameworks/base/tools/aapt/XMLNode.cpp
     """
     __charrange = None
     __replacement = None
 
-    def __init__(self, raw_buff):
+    def __init__(self, raw_buff: bytes)->bytes:
         logger.debug("AXMLPrinter")
 
         self.axml = AXMLParser(raw_buff)
 
         self.root = None
         self.packerwarning = False
         cur = []
@@ -999,60 +1025,60 @@
                 cur[-1].text = self.axml.text
             if _type == END_DOCUMENT:
                 # Check if all namespace mappings are closed
                 if len(self.axml.namespaces) > 0:
                     logger.warning("Not all namespace mappings were closed! Malformed AXML?")
                 break
 
-    def get_buff(self):
+    def get_buff(self) -> bytes:
         """
         Returns the raw XML file without prettification applied.
 
         :returns: bytes, encoded as UTF-8
         """
         return self.get_xml(pretty=False)
 
-    def get_xml(self, pretty=True):
+    def get_xml(self, pretty:bool=True) -> bytes:
         """
         Get the XML as an UTF-8 string
 
         :returns: bytes encoded as UTF-8
         """
         return etree.tostring(self.root, encoding="utf-8", pretty_print=pretty)
 
-    def get_xml_obj(self):
+    def get_xml_obj(self) -> etree.Element:
         """
         Get the XML as an ElementTree object
 
         :returns: :class:`lxml.etree.Element`
         """
         return self.root
 
-    def is_valid(self):
+    def is_valid(self) -> bool:
         """
         Return the state of the AXMLParser.
         If this flag is set to False, the parsing has failed, thus
         the resulting XML will not work or will even be empty.
         """
         return self.axml.is_valid()
 
-    def is_packed(self):
+    def is_packed(self) -> bool:
         """
         Returns True if the AXML is likely to be packed
 
         Packers do some weird stuff and we try to detect it.
         Sometimes the files are not packed but simply broken or compiled with
         some broken version of a tool.
         Some file corruption might also be appear to be a packed file.
 
         :returns: True if packer detected, False otherwise
         """
-        return self.packerwarning
+        return self.packerwarning or self.axml.packerwarning
 
-    def _get_attribute_value(self, index):
+    def _get_attribute_value(self, index: int):
         """
         Wrapper function for format_value to resolve the actual value of an attribute in a tag
         :param index: index of the current attribute
         :return: formatted value
         """
         _type = self.axml.getAttributeValueType(index)
         _data = self.axml.getAttributeValueData(index)
@@ -1348,15 +1374,15 @@
 
     The most outer chunk in the ARSC file is a chunk of type RES_TABLE_TYPE.
     Inside this chunk is a StringPool and at least one package.
 
     Each package is a chunk of type RES_TABLE_PACKAGE_TYPE.
     It contains again many more chunks.
     """
-    def __init__(self, raw_buff):
+    def __init__(self, raw_buff:bytes) -> None:
         """
         :param bytes raw_buff: the raw bytes of the file
         """
         self.buff = io.BufferedReader(io.BytesIO(raw_buff))
         self.buff_size = self.buff.raw.getbuffer().nbytes
 
         if self.buff_size < 8 or self.buff_size > 0xFFFFFFFF:
@@ -1577,92 +1603,92 @@
                                     c_value["dimen"].append(
                                         self.get_resource_dimen(ate))
 
                                 nb_i += 1
                         nb += 3 + nb_i - 1  # -1 to account for the nb+=1 on the next line
                 nb += 1
 
-    def get_resource_string(self, ate):
+    def get_resource_string(self, ate:ARSCResTableEntry) -> list:
         return [ate.get_value(), ate.get_key_data()]
 
-    def get_resource_id(self, ate):
+    def get_resource_id(self, ate:ARSCResTableEntry) -> list[str]:
         x = [ate.get_value()]
         if ate.key.get_data() == 0:
             x.append("false")
         elif ate.key.get_data() == 1:
             x.append("true")
         return x
 
-    def get_resource_bool(self, ate):
+    def get_resource_bool(self, ate:ARSCResTableEntry) -> list[str]:
         x = [ate.get_value()]
         if ate.key.get_data() == 0:
             x.append("false")
         elif ate.key.get_data() == -1:
             x.append("true")
         return x
 
-    def get_resource_integer(self, ate):
+    def get_resource_integer(self, ate:ARSCResTableEntry) -> list:
         return [ate.get_value(), ate.key.get_data()]
 
-    def get_resource_color(self, ate):
+    def get_resource_color(self, ate:ARSCResTableEntry) -> list:
         entry_data = ate.key.get_data()
         return [
             ate.get_value(),
             "#{:02x}{:02x}{:02x}{:02x}".format(
                 ((entry_data >> 24) & 0xFF),
                 ((entry_data >> 16) & 0xFF),
                 ((entry_data >> 8) & 0xFF),
                 (entry_data & 0xFF))
         ]
 
-    def get_resource_dimen(self, ate):
+    def get_resource_dimen(self, ate:ARSCResTableEntry) -> list:
         try:
             return [
                 ate.get_value(), "{}{}".format(
                     complexToFloat(ate.key.get_data()),
                     DIMENSION_UNITS[ate.key.get_data() & COMPLEX_UNIT_MASK])
             ]
         except IndexError:
             logger.debug("Out of range dimension unit index for {}: {}".format(
                 complexToFloat(ate.key.get_data()),
                 ate.key.get_data() & COMPLEX_UNIT_MASK))
             return [ate.get_value(), ate.key.get_data()]
 
     # FIXME
-    def get_resource_style(self, ate):
+    def get_resource_style(self, ate:ARSCResTableEntry) -> list:
         return ["", ""]
 
-    def get_packages_names(self):
+    def get_packages_names(self) -> list[str]:
         """
         Retrieve a list of all package names, which are available
         in the given resources.arsc.
         """
         return list(self.packages.keys())
 
-    def get_locales(self, package_name):
+    def get_locales(self, package_name:str) -> list[str]:
         """
         Retrieve a list of all available locales in a given packagename.
 
         :param package_name: the package name to get locales of
         """
         self._analyse()
         return list(self.values[package_name].keys())
 
-    def get_types(self, package_name, locale='\x00\x00'):
+    def get_types(self, package_name:str, locale:str='\x00\x00') -> list[str]:
         """
         Retrieve a list of all types which are available in the given
         package and locale.
 
         :param package_name: the package name to get types of
         :param locale: the locale to get types of (default: '\x00\x00')
         """
         self._analyse()
         return list(self.values[package_name][locale].keys())
 
-    def get_public_resources(self, package_name, locale='\x00\x00'):
+    def get_public_resources(self, package_name:str, locale:str='\x00\x00') -> bytes:
         """
         Get the XML (as string) of all resources of type 'public'.
 
         The public resources table contains the IDs for each item.
 
         :param package_name: the package name to get the resources for
         :param locale: the locale to get the resources for (default: '\x00\x00')
@@ -1680,15 +1706,15 @@
         except KeyError:
             pass
 
         buff += '</resources>\n'
 
         return buff.encode('utf-8')
 
-    def get_string_resources(self, package_name, locale='\x00\x00'):
+    def get_string_resources(self, package_name:str, locale:str='\x00\x00') -> bytes:
         """
         Get the XML (as string) of all resources of type 'string'.
 
         Read more about string resources:
         https://developer.android.com/guide/topics/resources/string-resource.html
 
         :param package_name: the package name to get the resources for
@@ -1709,15 +1735,15 @@
         except KeyError:
             pass
 
         buff += '</resources>\n'
 
         return buff.encode('utf-8')
 
-    def get_strings_resources(self):
+    def get_strings_resources(self) -> bytes:
         """
         Get the XML (as string) of all resources of type 'string'.
         This is a combined variant, which has all locales and all package names
         stored.
         """
         self._analyse()
 
@@ -1742,15 +1768,15 @@
 
             buff += "</package>\n"
 
         buff += "</packages>\n"
 
         return buff.encode('utf-8')
 
-    def get_id_resources(self, package_name, locale='\x00\x00'):
+    def get_id_resources(self, package_name:str, locale:str='\x00\x00') -> bytes:
         """
         Get the XML (as string) of all resources of type 'id'.
 
         Read more about ID resources:
         https://developer.android.com/guide/topics/resources/more-resources.html#Id
 
         :param package_name: the package name to get the resources for
@@ -1771,15 +1797,15 @@
         except KeyError:
             pass
 
         buff += '</resources>\n'
 
         return buff.encode('utf-8')
 
-    def get_bool_resources(self, package_name, locale='\x00\x00'):
+    def get_bool_resources(self, package_name:str, locale:str='\x00\x00') -> bytes:
         """
         Get the XML (as string) of all resources of type 'bool'.
 
         Read more about bool resources:
         https://developer.android.com/guide/topics/resources/more-resources.html#Bool
 
         :param package_name: the package name to get the resources for
@@ -1796,15 +1822,15 @@
         except KeyError:
             pass
 
         buff += '</resources>\n'
 
         return buff.encode('utf-8')
 
-    def get_integer_resources(self, package_name, locale='\x00\x00'):
+    def get_integer_resources(self, package_name:str, locale:str='\x00\x00') -> bytes:
         """
         Get the XML (as string) of all resources of type 'integer'.
 
         Read more about integer resources:
         https://developer.android.com/guide/topics/resources/more-resources.html#Integer
 
         :param package_name: the package name to get the resources for
@@ -1821,15 +1847,15 @@
         except KeyError:
             pass
 
         buff += '</resources>\n'
 
         return buff.encode('utf-8')
 
-    def get_color_resources(self, package_name, locale='\x00\x00'):
+    def get_color_resources(self, package_name:str, locale:str='\x00\x00') -> bytes:
         """
         Get the XML (as string) of all resources of type 'color'.
 
         Read more about color resources:
         https://developer.android.com/guide/topics/resources/more-resources.html#Color
 
         :param package_name: the package name to get the resources for
@@ -1846,15 +1872,15 @@
         except KeyError:
             pass
 
         buff += '</resources>\n'
 
         return buff.encode('utf-8')
 
-    def get_dimen_resources(self, package_name, locale='\x00\x00'):
+    def get_dimen_resources(self, package_name:str, locale:str='\x00\x00') -> bytes:
         """
         Get the XML (as string) of all resources of type 'dimen'.
 
         Read more about Dimension resources:
         https://developer.android.com/guide/topics/resources/more-resources.html#Dimension
 
         :param package_name: the package name to get the resources for
@@ -1871,15 +1897,15 @@
         except KeyError:
             pass
 
         buff += '</resources>\n'
 
         return buff.encode('utf-8')
 
-    def get_id(self, package_name, rid, locale='\x00\x00'):
+    def get_id(self, package_name:str, rid:int, locale:str='\x00\x00') -> tuple:
         """
         Returns the tuple (resource_type, resource_name, resource_id)
         for the given resource_id.
 
         :param package_name: package name to query
         :param rid: the resource_id
         :param locale: specific locale
@@ -1896,23 +1922,23 @@
         return None, None, None
 
     class ResourceResolver:
         """
         Resolves resources by ID and configuration.
         This resolver deals with complex resources as well as with references.
         """
-        def __init__(self, android_resources, config=None):
+        def __init__(self, android_resources:ARSCParser, config:Union[ARSCResTableConfig,None]=None) -> None:
             """
             :param ARSCParser android_resources: A resource parser
             :param ARSCResTableConfig config: The desired configuration or None to resolve all.
             """
             self.resources = android_resources
             self.wanted_config = config
 
-        def resolve(self, res_id):
+        def resolve(self, res_id: int) -> list[tuple[ARSCResTableConfig, str]]:
             """
             the given ID into the Resource and returns a list of matching resources.
 
             :param int res_id: numerical ID of the resource
             :return: a list of tuples of (ARSCResTableConfig, str)
             """
             result = []
@@ -1923,15 +1949,15 @@
             # First: Get all candidates
             configs = self.resources.get_res_configs(res_id, config)
 
             for config, ate in configs:
                 # deconstruct them and check if more candidates are generated
                 self.put_ate_value(result, ate, config)
 
-        def put_ate_value(self, result, ate, config):
+        def put_ate_value(self, result: list, ate:ARSCResTableEntry, config:ARSCResTableConfig) -> None:
             """
             Put a ResTableEntry into the list of results
             :param list result: results array
             :param ARSCResTableEntry ate:
             :param ARSCResTableConfig config:
             :return:
             """
@@ -1939,15 +1965,15 @@
                 complex_array = []
                 result.append((config, complex_array))
                 for _, item in ate.item.items:
                     self.put_item_value(complex_array, item, config, ate, complex_=True)
             else:
                 self.put_item_value(result, ate.key, config, ate, complex_=False)
 
-        def put_item_value(self, result, item, config, parent, complex_):
+        def put_item_value(self, result:list, item:ARSCResStringPoolRef, config:ARSCResTableConfig, parent:ARSCResTableEntry, complex_:bool)->None:
             """
             Put the tuple (ARSCResTableConfig, resolved string) into the result set
 
             :param list result: the result set
             :param ARSCResStringPoolRef item:
             :param ARSCResTableConfig config:
             :param ARSCResTableEntry parent: the originating entry
@@ -1966,15 +1992,15 @@
                     self._resolve_into_result(result, item.get_data(), self.wanted_config)
             else:
                 if complex_:
                     result.append(item.format_value())
                 else:
                     result.append((config, item.format_value()))
 
-    def get_resolved_res_configs(self, rid, config=None):
+    def get_resolved_res_configs(self, rid:int, config:Union[ARSCTableResConfig, None]=None) -> list[tuple[ARSCResTableConfig, str]]:
         """
         Return a list of resolved resource IDs with their corresponding configuration.
         It has a similar return type as :meth:`get_res_configs` but also handles complex entries
         and references.
         Also instead of returning :class:`ARSCResTableEntry` in the tuple, the actual values are resolved.
 
         This is the preferred way of resolving resource IDs to their resources.
@@ -1982,15 +2008,15 @@
         :param int rid: the numerical ID of the resource
         :param ARSCTableResConfig config: the desired configuration or None to retrieve all
         :return: A list of tuples of (ARSCResTableConfig, str)
         """
         resolver = ARSCParser.ResourceResolver(self, config)
         return resolver.resolve(rid)
 
-    def get_resolved_strings(self):
+    def get_resolved_strings(self) -> list[str]:
         self._analyse()
         if self._resolved_strings:
             return self._resolved_strings
 
         r = {}
         for package_name in self.get_packages_names():
             r[package_name] = {}
@@ -2017,15 +2043,15 @@
                             r[package_name][v_locale][k[i[0]]] = i[1]
                 except KeyError:
                     pass
 
         self._resolved_strings = r
         return r
 
-    def get_res_configs(self, rid, config=None, fallback=True):
+    def get_res_configs(self, rid:int, config:Union[ARSCResTableConfig,None]=None, fallback:bool=True) -> list[ARSCResTableConfig]:
         """
         Return the resources found with the ID `rid` and select
         the right one based on the configuration, or return all if no configuration was set.
 
         But we try to be generous here and at least try to resolve something:
         This method uses a fallback to return at least one resource (the first one in the list)
         if more than one items are found and the default config is used and no default entry could be found.
@@ -2035,15 +2061,15 @@
         In practise an app might just be designed to run on a single locale and thus only has those locales set.
 
         You can disable this fallback behaviour, to just return exactly the given result.
 
         :param rid: resource id as int
         :param config: a config to resolve from, or None to get all results
         :param fallback: Enable the fallback for resolving default configuration (default: True)
-        :return: a list of ARSCResTableConfig: ARSCResTableEntry
+        :return: a list of ARSCResTableConfig:
         """
         self._analyse()
 
         if not rid:
             raise ValueError("'rid' should be set")
         if not isinstance(rid, int):
             raise ValueError("'rid' must be an int")
@@ -2060,15 +2086,15 @@
                 logger.warning("No default resource config could be found for the given rid '0x{:08x}', using fallback!".format(rid))
                 return [list(self.resource_values[rid].items())[0]]
             else:
                 return []
         else:
             return list(res_options.items())
 
-    def get_string(self, package_name, name, locale='\x00\x00'):
+    def get_string(self, package_name:str, name:str, locale:str='\x00\x00') -> Union[str,None]:
         self._analyse()
 
         try:
             for i in self.values[package_name][locale]["string"]:
                 if i[0] == name:
                     return i
         except KeyError:
@@ -2093,15 +2119,15 @@
             if res_type.get_package_name() == package_name and (
                             type_name is None or res_type.get_type() == type_name):
                 result[res_type.get_type()].extend(configs)
 
         return result
 
     @staticmethod
-    def parse_id(name):
+    def parse_id(name:str) -> tuple[str,str]:
         """
         Resolves an id from a binary XML file in the form "@[package:]DEADBEEF"
         and returns a tuple of package name and resource id.
         If no package name was given, i.e. the ID has the form "@DEADBEEF",
         the package name is set to None.
 
         Raises a ValueError if the id is malformed.
@@ -2126,15 +2152,15 @@
             raise ValueError("Numerical ID is not 8 characters long: '{}'".format(res_id))
 
         try:
             return int(res_id, 16), package
         except ValueError:
             raise ValueError("ID is not a hex ID: '{}'".format(res_id))
 
-    def get_resource_xml_name(self, r_id, package=None):
+    def get_resource_xml_name(self, r_id:int, package:Union[str,None]=None) -> str:
         """
         Returns the XML name for a resource, including the package name if package is None.
         A full name might look like `@com.example:string/foobar`
         Otherwise the name is only looked up in the specified package and is returned without
         the package name.
         The same example from about without the package name will read as `@string/foobar`.
 
@@ -2164,33 +2190,33 @@
             if not package:
                 return None
             else:
                 return "@{}:{}/{}".format(package, resource, name)
 
 
 class PackageContext:
-    def __init__(self, current_package, stringpool_main, mTableStrings, mKeyStrings):
+    def __init__(self, current_package: ARSCResTablePackage, stringpool_main: StringBlock, mTableStrings: StringBlock, mKeyStrings: StringBlock) -> None:
         """
         :param ARSCResTablePackage current_package:
         :param StringBlock stringpool_main:
         :param StringBlock mTableStrings:
         :param StringBlock mKeyStrings:
         """
         self.stringpool_main = stringpool_main
         self.mTableStrings = mTableStrings
         self.mKeyStrings = mKeyStrings
         self.current_package = current_package
 
-    def get_mResId(self):
+    def get_mResId(self) -> int:
         return self.current_package.mResId
 
-    def set_mResId(self, mResId):
+    def set_mResId(self, mResId: int) -> None:
         self.current_package.mResId = mResId
 
-    def get_package_name(self):
+    def get_package_name(self) -> str:
         return self.current_package.get_name()
 
     def __repr__(self):
         return "<PackageContext {}, {}, {}, {}>".format(self.current_package,
                                                         self.stringpool_main,
                                                         self.mTableStrings,
                                                         self.mKeyStrings)
@@ -2212,17 +2238,17 @@
     See http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#196
     :raises: ResParserError
     """
 
     # This is the minimal size such a header must have. There might be other header data too!
     SIZE = 2 + 2 + 4
 
-    def __init__(self, buff, expected_type=None, possible_types=None):
+    def __init__(self, buff: BinaryIO, expected_type:Union[int,None]=None, possible_types:Union[set[int], None]=None) -> None:
         """
-        :param androguard.core.bytecode.BuffHandle buff: the buffer set to the position where the header starts.
+        :param buff: the buffer set to the position where the header starts.
         :param int expected_type: the type of the header which is expected.
         """
         self.start = buff.tell()
         # Make sure we do not read over the buffer:
         if buff.raw.getbuffer().nbytes < self.start + self.SIZE:
             raise ResParserError("Can not read over the buffer size! Offset={}".format(self.start))
 
@@ -2259,42 +2285,42 @@
         if self._size < self._header_size:
             raise ResParserError(
                 "declared chunk size ({}) is smaller than header size ({})! Offset={}".format(self._size,
                                                                                               self._header_size,
                                                                                               self.start))
 
     @property
-    def type(self):
+    def type(self) -> int:
         """
         Type identifier for this chunk
         """
         return self._type
 
     @property
-    def header_size(self):
+    def header_size(self) -> int:
         """
         Size of the chunk header (in bytes).  Adding this value to
         the address of the chunk allows you to find its associated data
         (if any).
         """
         return self._header_size
 
     @property
-    def size(self):
+    def size(self) -> int:
         """
         Total size of this chunk (in bytes).  This is the chunkSize plus
         the size of any data associated with the chunk.  Adding this value
         to the chunk allows you to completely skip its contents (including
         any child chunks).  If this value is the same as chunkSize, there is
         no data associated with the chunk.
         """
         return self._size
 
     @property
-    def end(self):
+    def end(self) -> int:
         """
         Get the absolute offset inside the file, where the chunk ends.
         This is equal to `ARSCHeader.start + ARSCHeader.size`.
         """
         return self.start + self.size
 
     def __repr__(self):
@@ -2306,36 +2332,36 @@
 
 class ARSCResTablePackage:
     """
     A `ResTable_package`
 
     See http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#861
     """
-    def __init__(self, buff, header):
+    def __init__(self, buff: BinaryIO, header:ARSCHeader) -> None:
         self.header = header
         self.start = buff.tell()
         self.id = unpack('<I', buff.read(4))[0]
         self.name = buff.read(256)
         self.typeStrings = unpack('<I', buff.read(4))[0]
         self.lastPublicType = unpack('<I', buff.read(4))[0]
         self.keyStrings = unpack('<I', buff.read(4))[0]
         self.lastPublicKey = unpack('<I', buff.read(4))[0]
         self.mResId = self.id << 24
 
-    def get_name(self):
+    def get_name(self) -> None:
         name = self.name.decode("utf-16", 'replace')
         name = name[:name.find("\x00")]
         return name
 
 
 class ARSCResTypeSpec:
     """
     See http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#1327
     """
-    def __init__(self, buff, parent=None):
+    def __init__(self, buff: BinaryIO, parent:Union[PackageContext, None]=None) -> None:
         self.start = buff.tell()
         self.parent = parent
         self.id = unpack('<B', buff.read(1))[0]
         self.res0 = unpack('<B', buff.read(1))[0]
         self.res1 = unpack('<H', buff.read(2))[0]
         # TODO: https://github.com/androguard/androguard/issues/1014 | Properly account for the cases where res0/1 are not zero
         try:
@@ -2354,15 +2380,15 @@
 class ARSCResType:
     """
     This is a `ResTable_type` without it's `ResChunk_header`.
     It contains a `ResTable_config`
 
     See http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#1364
     """
-    def __init__(self, buff, parent=None):
+    def __init__(self, buff: BinaryIO, parent:Union[PackageContext,None]=None) -> None:
         self.start = buff.tell()
         self.parent = parent
 
         self.id = unpack('<B', buff.read(1))[0]
         # TODO there is now FLAG_SPARSE: http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#1401
         self.flags, = unpack('<B', buff.read(1))
         self.reserved = unpack('<H', buff.read(2))[0]
@@ -2374,18 +2400,18 @@
         self.mResId = (0xff000000 & self.parent.get_mResId()) | self.id << 16
         self.parent.set_mResId(self.mResId)
 
         self.config = ARSCResTableConfig(buff)
 
         logger.debug("Parsed {}".format(self))
 
-    def get_type(self):
+    def get_type(self) -> str:
         return self.parent.mTableStrings.getString(self.id - 1)
 
-    def get_package_name(self):
+    def get_package_name(self) -> str:
         return self.parent.get_package_name()
 
     def __repr__(self):
         return "<ARSCResType(start=0x%x, id=0x%x, flags=0x%x, entryCount=%d, entriesStart=0x%x, mResId=0x%x, %s)>" % (
             self.start,
             self.id,
             self.flags,
@@ -2407,15 +2433,15 @@
     """
     @classmethod
     def default_config(cls):
         if not hasattr(cls, 'DEFAULT'):
             cls.DEFAULT = ARSCResTableConfig(None)
         return cls.DEFAULT
 
-    def __init__(self, buff=None, **kwargs):
+    def __init__(self, buff:Union[BinaryIO, None]=None, **kwargs) -> None:
         if buff is not None:
             self.start = buff.tell()
 
             # uint32_t
             self.size = unpack('<I', buff.read(4))[0]
 
             # union: uint16_t mcc, uint16_t mnc
@@ -2429,30 +2455,42 @@
 
             # struct of:
             # uint8_t orientation
             # uint8_t touchscreen
             # uint16_t density
             self.screenType = unpack('<I', buff.read(4))[0]
 
-            # struct of
-            # uint8_t keyboard
-            # uint8_t navigation
-            # uint8_t inputFlags
-            # uint8_t inputPad0
-            self.input = unpack('<I', buff.read(4))[0]
-
-            # struct of
-            # uint16_t screenWidth
-            # uint16_t screenHeight
-            self.screenSize = unpack('<I', buff.read(4))[0]
-
-            # struct of
-            # uint16_t sdkVersion
-            # uint16_t minorVersion  which should be always 0, as the meaning is not defined
-            self.version = unpack('<I', buff.read(4))[0]
+            if self.size >= 20:
+                # struct of
+                # uint8_t keyboard
+                # uint8_t navigation
+                # uint8_t inputFlags
+                # uint8_t inputPad0
+                self.input = unpack('<I', buff.read(4))[0]
+            else:
+                logger.debug("This file does not have input flags! size={}".format(self.size))
+                self.input = 0
+
+            if self.size >= 24:
+                # struct of
+                # uint16_t screenWidth
+                # uint16_t screenHeight
+                self.screenSize = unpack('<I', buff.read(4))[0]
+            else:
+                logger.debug("This file does not have screenSize! size={}".format(self.size))
+                self.screenSize = 0
+
+            if self.size >= 28:
+                # struct of
+                # uint16_t sdkVersion
+                # uint16_t minorVersion  which should be always 0, as the meaning is not defined
+                self.version = unpack('<I', buff.read(4))[0]
+            else:
+                logger.debug("This file does not have version! size={}".format(self.size))
+                self.version = 0
 
             # The next three fields seems to be optional
             if self.size >= 32:
                 # struct of
                 # uint8_t screenLayout
                 # uint8_t uiMode
                 # uint16_t smallestScreenWidthDp
@@ -2494,15 +2532,20 @@
         else:
             self.start = 0
             self.size = 0
             self.imsi = \
                 ((kwargs.pop('mcc', 0) & 0xffff) << 0) + \
                 ((kwargs.pop('mnc', 0) & 0xffff) << 16)
 
-            self.locale = 0
+            temp_locale = kwargs.pop('locale', 0)
+            if isinstance(temp_locale, str):
+                self.set_language_and_region(temp_locale)
+            else:
+                self.locale = temp_locale
+
             for char_ix, char in kwargs.pop('locale', "")[0:4]:
                 self.locale += (ord(char) << (char_ix * 8))
 
             self.screenType = \
                 ((kwargs.pop('orientation', 0) & 0xff) << 0) + \
                 ((kwargs.pop('touchscreen', 0) & 0xff) << 8) + \
                 ((kwargs.pop('density', 0) & 0xffff) << 16)
@@ -2547,34 +2590,54 @@
         else:
             if char_in[0]:
                 char_out += chr(char_in[0])
             if char_in[1]:
                 char_out += chr(char_in[1])
         return char_out
 
-    def get_language_and_region(self):
+    def _pack_language_or_region(self, char_in: str) -> list[int]:
+        char_out = [0x00, 0x00]
+        if len(char_in) != 2:
+            return char_out
+        char_out[0] = ord(char_in[0])
+        char_out[1] = ord(char_in[1])
+        return char_out
+
+    def set_language_and_region(self, language_region):
+        try:
+            language, region = language_region.split("-r")
+        except ValueError:
+            language, region = language_region, None
+        language_bytes = self._pack_language_or_region(language)
+        if region:
+            region_bytes = self._pack_language_or_region(region)
+        else:
+            region_bytes = [0x00, 0x00]
+        self.locale = language_bytes[0] | (language_bytes[1] << 8) | (region_bytes[0] << 16) | (region_bytes[1] << 24)
+
+    def get_language_and_region(self) -> str:
         """
         Returns the combined language+region string or \x00\x00 for the default locale
         :return:
         """
         if self.locale != 0:
             _language = self._unpack_language_or_region([self.locale & 0xff, (self.locale & 0xff00) >> 8, ], ord('a'))
             _region = self._unpack_language_or_region([(self.locale & 0xff0000) >> 16, (self.locale & 0xff000000) >> 24, ], ord('0'))
             return (_language + "-r" + _region) if _region else _language
         return "\x00\x00"
 
-    def get_config_name_friendly(self):
+    def get_config_name_friendly(self) -> str:
         """
         Here for legacy reasons.
 
         use :meth:`~get_qualifier` instead.
         """
         return self.get_qualifier()
 
-    def get_qualifier(self):
+    def get_qualifier(self) -> str:
         """
         Return resource name qualifier for the current configuration.
         for example
         * `ldpi-v4`
         * `hdpi-v4`
 
         All possible qualifiers are listed in table 2 of https://developer.android.com/guide/topics/resources/providing-resources
@@ -2787,27 +2850,27 @@
             minorVersion = (self.version & 0xffff0000) >> 16
             res.append("v%d" % sdkVersion)
             if minorVersion != 0:
                 res.append(".%d" % minorVersion)
 
         return "-".join(res)
 
-    def get_language(self):
+    def get_language(self) -> str:
         x = self.locale & 0x0000ffff
         return chr(x & 0x00ff) + chr((x & 0xff00) >> 8)
 
-    def get_country(self):
+    def get_country(self) -> str:
         x = (self.locale & 0xffff0000) >> 16
         return chr(x & 0x00ff) + chr((x & 0xff00) >> 8)
 
-    def get_density(self):
+    def get_density(self) -> str:
         x = ((self.screenType >> 16) & 0xffff)
         return x
 
-    def is_default(self):
+    def is_default(self) -> bool:
         """
         Test if this is a default resource, which matches all
 
         This is indicated that all fields are zero.
         :return: True if default, False otherwise
         """
         return all(map(lambda x: x == 0, self._get_tuple()))
@@ -2850,15 +2913,15 @@
     FLAG_PUBLIC = 2
 
     # If set, this is a weak resource and may be overriden by strong
     # resources of the same name/type. This is only useful during
     # linking with other resource tables.
     FLAG_WEAK = 4
 
-    def __init__(self, buff, mResId, parent=None):
+    def __init__(self, buff:BinaryIO, mResId:int, parent:Union[PackageContext, None]=None) -> None:
         self.start = buff.tell()
         self.mResId = mResId
         self.parent = parent
 
         self.size = unpack('<H', buff.read(2))[0]
         self.flags = unpack('<H', buff.read(2))[0]
         # This is a ResStringPool_ref
@@ -2869,30 +2932,30 @@
         else:
             # If FLAG_COMPLEX is not set, a Res_value structure will follow
             self.key = ARSCResStringPoolRef(buff, self.parent)
 
         if self.is_weak():
             logger.debug("Parsed {}".format(self))
 
-    def get_index(self):
+    def get_index(self) -> int:
         return self.index
 
-    def get_value(self):
+    def get_value(self) -> str:
         return self.parent.mKeyStrings.getString(self.index)
 
-    def get_key_data(self):
+    def get_key_data(self) -> str:
         return self.key.get_data_value()
 
-    def is_public(self):
+    def is_public(self) -> bool:
         return (self.flags & self.FLAG_PUBLIC) != 0
 
-    def is_complex(self):
+    def is_complex(self) -> bool:
         return (self.flags & self.FLAG_COMPLEX) != 0
 
-    def is_weak(self):
+    def is_weak(self) -> bool:
         return (self.flags & self.FLAG_WEAK) != 0
 
     def __repr__(self):
         return "<ARSCResTableEntry idx='0x{:08x}' mResId='0x{:08x}' size='{}' flags='0x{:02x}' index='0x{:x}' holding={}>".format(
             self.start,
             self.mResId,
             self.size,
@@ -2907,15 +2970,15 @@
 
     It contains a set of {name: value} mappings, which are of type `ResTable_map`.
     A `ResTable_map` contains two items: `ResTable_ref` and `Res_value`.
 
     See http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#1485 for `ResTable_map_entry`
     and http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#1498 for `ResTable_map`
     """
-    def __init__(self, buff, parent=None):
+    def __init__(self, buff:BinaryIO, parent:Union[PackageContext,None]=None) -> None:
         self.start = buff.tell()
         self.parent = parent
 
         self.id_parent = unpack('<I', buff.read(4))[0]
         self.count = unpack('<I', buff.read(4))[0]
 
         self.items = []
@@ -2932,66 +2995,66 @@
 class ARSCResStringPoolRef:
     """
     This is actually a `Res_value`
     It holds information about the stored resource value
 
     See: http://androidxref.com/9.0.0_r3/xref/frameworks/base/libs/androidfw/include/androidfw/ResourceTypes.h#262
     """
-    def __init__(self, buff, parent=None):
+    def __init__(self, buff:BinaryIO, parent:Union[PackageContext, None]=None) -> None:
         self.start = buff.tell()
         self.parent = parent
 
         self.size, = unpack("<H", buff.read(2))
         self.res0, = unpack("<B", buff.read(1))
         try:
             if self.res0 != 0:
                 logger.warning("res0 must be always zero!")
             self.data_type = unpack('<B', buff.read(1))[0]
             # data is interpreted according to data_type
             self.data = unpack('<I', buff.read(4))[0]
         except Exception as e:
             logger.error(e)
 
-    def get_data_value(self):
+    def get_data_value(self) -> str:
         return self.parent.stringpool_main.getString(self.data)
 
-    def get_data(self):
+    def get_data(self) -> int:
         return self.data
 
-    def get_data_type(self):
+    def get_data_type(self) -> bytes:
         return self.data_type
 
-    def get_data_type_string(self):
+    def get_data_type_string(self) -> str:
         return TYPE_TABLE[self.data_type]
 
-    def format_value(self):
+    def format_value(self) -> str:
         """
         Return the formatted (interpreted) data according to `data_type`.
         """
         return format_value(
             self.data_type,
             self.data,
             self.parent.stringpool_main.getString
         )
 
-    def is_reference(self):
+    def is_reference(self) -> bool:
         """
         Returns True if the Res_value is actually a reference to another resource
         """
         return self.data_type == TYPE_REFERENCE
 
     def __repr__(self):
         return "<ARSCResStringPoolRef idx='0x{:08x}' size='{}' type='{}' data='0x{:08x}'>".format(
             self.start,
             self.size,
             TYPE_TABLE.get(self.data_type, "0x%x" % self.data_type),
             self.data)
 
 
-def get_arsc_info(arscobj):
+def get_arsc_info(arscobj:ARSCParser) -> str:
     """
     Return a string containing all resources packages ordered by packagename, locale and type.
 
     :param arscobj: :class:`~ARSCParser`
     :return: a string
     """
     buff = ""
```

### Comparing `androguard-4.1.1/androguard/core/axml/types.py` & `androguard-4.1.2/androguard/core/axml/types.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/bytecode.py` & `androguard-4.1.2/androguard/core/bytecode.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,27 @@
+# Allows type hinting of types not-yet-declared
+# in Python >= 3.7
+# see https://peps.python.org/pep-0563/
+from __future__ import annotations
+
 import hashlib
-from xml.sax.saxutils import escape
+import json
 from struct import pack
 import textwrap
-import json
-from loguru import logger
+from typing import TYPE_CHECKING, Union
+
 
 from androguard.core.androconf import CONF, color_range
 from androguard.core.dex.dex_types import Kind, Operand
+if TYPE_CHECKING:
+    from androguard.core.analysis import DEXBasicBlock, MethodAnalysis
+    from androguard.core.dex import DEX
 
+from loguru import logger
+from xml.sax.saxutils import escape
 
 def _PrintBanner():
     print_fct = CONF["PRINT_FCT"]
     print_fct("*" * 75 + "\n")
 
 
 def _PrintSubBanner(title=None):
@@ -102,15 +112,15 @@
                 yield "{}{}{}".format(colors["type"], operand[2], colors["normal"])
             else:
                 yield "{}".format(repr(operands[2]))
         else:
             yield "{}".format(repr(operands[1]))
 
 
-def PrettyShow(basic_blocks, notes={}):
+def PrettyShow(basic_blocks: list[DEXBasicBlock], notes:list=[]) -> None:
     idx = 0
 
     offset_color = CONF["COLORS"]["OFFSET"]
     offset_addr_color = CONF["COLORS"]["OFFSET_ADDR"]
     instruction_name_color = CONF["COLORS"]["INSTRUCTION_NAME"]
     branch_false_color = CONF["COLORS"]["BRANCH_FALSE"]
     branch_true_color = CONF["COLORS"]["BRANCH_TRUE"]
@@ -122,14 +132,16 @@
 
     colors = CONF["COLORS"]["OUTPUT"]
 
     for nb, i in enumerate(basic_blocks):
         print_fct("{}{}{} : \n".format(bb_color, i.get_name(), normal_color))
         instructions = list(i.get_instructions())
         for ins in instructions:
+
+            # TODO: this seems wrong, notes is a list[str], but maybe it used to be a dict?
             if nb in notes:
                 for note in notes[nb]:
                     _PrintNote(note, 1)
 
             print_fct("\t%s%-3d%s(%s%08x%s) " %
                       (offset_color, nb, normal_color, offset_addr_color, idx,
                        normal_color))
@@ -181,15 +193,15 @@
 
 def _get_operand_html(operand, registers_colors, colors):
     """
     Return a HTML representation of the operand.
     The HTML should be compatible with pydot/graphviz to be used
     inside a node label.
 
-    This is solely used in :func:`~androguard.core.bytecodes.method2dot`
+    This is solely used in :func:`~androguard.core.bytecode.method2dot`
 
     :param operand: tuple containing the operand type and operands
     :param dict register_colors: key: register number, value: register color
     :param dict colors: dictionary containing the register colors
     :returns: HTML code of the operands
     """
     if operand[0] == Operand.REGISTER:
@@ -218,15 +230,15 @@
             return '<FONT color="{}">{}</FONT>'.format(colors["type"], escape(operand[2]))
 
         return escape(str(operand[2]))
 
     return escape(str(operand[1]))
 
 
-def method2dot(mx, colors=None):
+def method2dot(mx: MethodAnalysis, colors:Union[dict[str,str],None]=None) -> str:
     """
     Export analysis method to dot format.
 
     A control flow graph is created by using the concept of BasicBlocks.
     Each BasicBlock is a sequence of opcode without any jumps or branch.
 
     :param mx: :class:`~androguard.core.analysis.analysis.MethodAnalysis`
@@ -390,15 +402,19 @@
             for register, rtype in method_information["params"]:
                 method_label += "\\nparam v%d = %s" % (register, rtype)
         method_label += "\\nreturn = %s" % (method_information["return"])
 
     return {'name': method_label, 'nodes': blocks_html, 'edges': edges_html}
 
 
-def method2format(output, _format="png", mx=None, raw=None):
+def method2format(
+    output:str,
+    _format:str="png",
+    mx:Union[MethodAnalysis,None]=None,
+    raw:Union[str,None]=None):
     """
     Export method structure as a graph to a specific file format using dot from the graphviz package.
     The result is written to the file specified via :code:`output`.
 
     There are two possibilites to give input for this method:
 
     1) use :code:`raw` argument and pass a dictionary containing the keys
@@ -412,15 +428,15 @@
     is handled by pydot.
 
     :param str output: output filename
     :param str _format: format type (png, jpg ...). Can use all formats which are understood by pydot.
     :param androguard.core.analysis.analysis.MethodAnalysis mx: specify the MethodAnalysis object
     :param dict raw: use directly a dot raw buffer if None
     """
-    # pydot is optional!
+    # pydot is optional, it's only needed for png, jpg formats
     import pydot
 
     if raw:
         data = raw
     else:
         data = method2dot(mx)
 
@@ -461,19 +477,22 @@
     else:
         d = pydot.graph_from_dot_data(buff)
         if len(d) > 1:
             # Not sure what to do in this case?!
             logger.warning("The graph generated for '{}' has too many subgraphs! "
                        "Only plotting the first one.".format(output))
         for g in d:
-            getattr(g, "write_" + _format.lower())(output)
-            break
-
+            try:
+                getattr(g, "write_" + _format.lower())(output)
+                break
+            except FileNotFoundError:
+                logger.error("Could not write graph image, ensure graphviz is installed!")
+                raise
 
-def method2png(output, mx, raw=False):
+def method2png(output:str, mx:MethodAnalysis, raw:Union[str,None]=None) -> None:
     """
     Export method to a png file format
 
     :param output: output filename
     :type output: string
     :param mx: specify the MethodAnalysis object
     :type mx: :class:`MethodAnalysis` object
@@ -483,15 +502,15 @@
     buff = raw
     if not raw:
         buff = method2dot(mx)
 
     method2format(output, "png", mx, buff)
 
 
-def method2jpg(output, mx, raw=False):
+def method2jpg(output:str, mx:MethodAnalysis, raw:Union[str,None]=None) -> None:
     """
     Export method to a jpg file format
 
     :param output: output filename
     :type output: string
     :param mx: specify the MethodAnalysis object
     :type mx: :class:`MethodAnalysis` object
@@ -501,20 +520,20 @@
     buff = raw
     if not raw:
         buff = method2dot(mx)
 
     method2format(output, "jpg", mx, buff)
 
 
-def vm2json(vm):
+def vm2json(vm:DEX) -> str:
     """
     Get a JSON representation of a DEX file
 
-    :param vm: :class:`~androguard.core.bytecodes.dvm.DEX`
-    :return:
+    :param vm: :class:`~androguard.core.dex.DEX`
+    :return: str
     """
     d = {"name": "root", "children": []}
 
     for _class in vm.get_classes():
         c_class = {"name": _class.get_name(), "children": []}
 
         for method in _class.get_methods():
@@ -524,39 +543,39 @@
 
         d["children"].append(c_class)
 
     return json.dumps(d)
 
 
 class TmpBlock:
-    def __init__(self, name):
+    def __init__(self, name:str) -> None:
         self.name = name
 
-    def get_name(self):
+    def get_name(self) -> str:
         return self.name
 
 
-def method2json(mx, directed_graph=False):
+def method2json(mx: MethodAnalysis, directed_graph:bool=False) -> str:
     """
     Create directed or undirected graph in the json format.
 
     :param mx: :class:`~androguard.core.analysis.analysis.MethodAnalysis`
     :param directed_graph: True if a directed graph should be created (default: False)
-    :return:
+    :return: str
     """
     if directed_graph:
         return method2json_direct(mx)
     return method2json_undirect(mx)
 
 
-def method2json_undirect(mx):
+def method2json_undirect(mx: MethodAnalysis) -> str:
     """
 
     :param mx: :class:`~androguard.core.analysis.analysis.MethodAnalysis`
-    :return:
+    :return: str
     """
     d = {}
     reports = []
     d["reports"] = reports
 
     for DVMBasicMethodBlock in mx.basic_blocks.gets():
         cblock = {"BasicBlockId": DVMBasicMethodBlock.get_name(),
@@ -576,15 +595,15 @@
             cblock["Edge"].append(DVMBasicMethodBlockChild[-1].get_name())
 
         reports.append(cblock)
 
     return json.dumps(d)
 
 
-def method2json_direct(mx):
+def method2json_direct(mx: MethodAnalysis) -> str:
     """
 
     :param mx: :class:`~androguard.core.analysis.analysis.MethodAnalysis`
     :return:
     """
     d = {}
     reports = []
@@ -670,15 +689,15 @@
         reports.append(cblock)
 
     reports.extend(l)
 
     return json.dumps(d)
 
 
-def object_to_bytes(obj):
+def object_to_bytes(obj:Union[str,bool,int,bytearray]) -> bytearray:
     """
     Convert a object to a bytearray or call get_raw() of the object
     if no useful type was found.
     """
     if isinstance(obj, str):
         return bytearray(obj, "UTF-8")
     if isinstance(obj, bool):
@@ -689,30 +708,30 @@
         return bytearray()
     if isinstance(obj, bytearray):
         return obj
 
     return obj.get_raw()
 
 
-def FormatClassToJava(i):
+def FormatClassToJava(i:str) -> str:
     """
     Transform a java class name into the typed variant found in DEX files.
 
     example::
 
         >>> FormatClassToJava('java.lang.Object')
         'Ljava/lang/Object;'
 
     :param i: the input class name
     :rtype: str
     """
     return "L" + i.replace(".", "/") + ";"
 
 
-def FormatClassToPython(i):
+def FormatClassToPython(i:str) -> str:
     """
     Transform a typed class name into a form which can be used as a python
     attribute
 
     example::
 
         >>> FormatClassToPython('Lfoo/bar/foo/Barfoo$InnerClass;')
@@ -724,15 +743,15 @@
     i = i[:-1]
     i = i.replace("/", "_")
     i = i.replace("$", "_")
 
     return i
 
 
-def get_package_class_name(name):
+def get_package_class_name(name:str)->tuple[str, str]:
     """
     Return package and class name in a java variant from a typed variant name.
 
     If no package could be found, the package is an empty string.
 
     If the name is an array type, the array is discarded.
 
@@ -766,15 +785,15 @@
 
     package, clsname = name.rsplit('/', 1)
     package = package.replace('/', '.')
 
     return package, clsname
 
 
-def FormatNameToPython(i):
+def FormatNameToPython(i:str) -> str:
     """
     Transform a (method) name into a form which can be used as a python
     attribute
 
     example::
 
         >>> FormatNameToPython('<clinit>')
@@ -787,15 +806,15 @@
     i = i.replace("<", "")
     i = i.replace(">", "")
     i = i.replace("$", "_")
 
     return i
 
 
-def FormatDescriptorToPython(i):
+def FormatDescriptorToPython(i:str) -> str:
     """
     Format a descriptor into a form which can be used as a python attribute
 
     example::
 
         >>> FormatDescriptorToPython('(Ljava/lang/Long; Ljava/lang/Long; Z Z)V')
         'Ljava_lang_LongLjava_lang_LongZZV
```

### Comparing `androguard-4.1.1/androguard/core/dex/__init__.py` & `androguard-4.1.2/androguard/core/dex/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 
-from androguard.core import bytecode, apk
-from androguard.core.androconf import CONF
-from androguard.util import read_at
+# Allows type hinting of types not-yet-declared
+# in Python >= 3.7
+# see https://peps.python.org/pep-0563/
+from __future__ import annotations
 
-import sys
+import binascii
+from enum import IntEnum
+import hashlib
 import io
 import re
 import struct
-import binascii
-import time
 from struct import pack, unpack, calcsize
-import logging
-import warnings
+import sys
+import time
+from typing import Union, IO, BinaryIO, Iterator
+from typing import TYPE_CHECKING
 import zlib
-import hashlib
-from enum import IntEnum
-from loguru import logger
 
+if TYPE_CHECKING:
+    from androguard.core.analysis.analysis import Analysis, MethodAnalysis
+    from androguard.decompiler.decompiler import DecompilerDAD
+    from androguard.decompiler.node import Node
 
+from androguard.core import bytecode, apk
+from androguard.core.androconf import CONF
+from androguard.util import read_at
 from androguard.core import mutf8
 from .dex_types import (
         TypeMapItem,
         ACCESS_FLAGS,
         TYPE_DESCRIPTOR,
         Kind,
         Operand,
         )
 
+from loguru import logger
 
 # TODO: have some more generic magic...
 DEX_FILE_MAGIC_35 = b'dex\n035\x00'
 DEX_FILE_MAGIC_36 = b'dex\n036\x00'
 DEX_FILE_MAGIC_37 = b'dex\n037\x00'
 DEX_FILE_MAGIC_38 = b'dex\n038\x00'
 DEX_FILE_MAGIC_39 = b'dex\n039\x00'
@@ -94,15 +102,15 @@
 DBG_LINE_RANGE = 15
 
 
 class InvalidInstruction(Exception):
     pass
 
 
-def read_null_terminated_string(f):
+def read_null_terminated_string(f: IO) -> bytearray:
     """
     Read a null terminated string from a file-like object.
     :param f: file-like object
     :rtype: bytearray
     """
     x = []
     while True:
@@ -114,15 +122,15 @@
             f.seek(idx - len(s[1]))
             break
         else:
             x.append(z)
     return b''.join(x)
 
 
-def get_access_flags_string(value):
+def get_access_flags_string(value: int) -> str:
     """
     Transform an access flag field to the corresponding string
 
     :param value: the value of the access flags
     :type value: int
 
     :rtype: string
@@ -131,15 +139,15 @@
     for k, v in ACCESS_FLAGS.items():
         if (k & value) == k:
             flags.append(v)
 
     return " ".join(flags)
 
 
-def get_type(atype, size=None):
+def get_type(atype:str, size:Union[int,None]=None) -> str:
     """
     Retrieve the type of a descriptor (e.g : I)
     """
     if atype.startswith('java.lang'):
         atype = atype.replace('java.lang.', '')
     res = TYPE_DESCRIPTOR.get(atype.lstrip('java.lang'))
     if res is None:
@@ -172,26 +180,26 @@
 
 BREAK_DVM_OPCODES = ["invoke.", "move.", ".put", "if."]
 
 BRANCH_DEX_OPCODES = ["throw", "throw.", "if.", "goto", "goto.", "return",
                       "return.", "packed-switch$", "sparse-switch$"]
 
 
-def clean_name_instruction(instruction):
+def clean_name_instruction(instruction: Instruction) -> str:
     """USED IN ELSIM"""
     op_value = instruction.get_op_value()
 
     # goto range
     if 0x28 <= op_value <= 0x2a:
         return "goto"
 
     return instruction.get_name()
 
 
-def static_operand_instruction(instruction):
+def static_operand_instruction(instruction: Instruction) -> str:
     """USED IN ELSIM"""
     buff = ""
 
     if isinstance(instruction, Instruction):
         # get instructions without registers
         for val in instruction.get_literals():
             buff += "%s" % val
@@ -199,23 +207,23 @@
     op_value = instruction.get_op_value()
     if op_value == 0x1a or op_value == 0x1b:
         buff += instruction.get_string()
 
     return buff
 
 
-def get_sbyte(cm, buff):
+def get_sbyte(cm: ClassManager, buff: BinaryIO) -> int:
     return cm.packer["b"].unpack(buff.read(1))[0]
 
 
-def get_byte(cm, buff):
+def get_byte(cm: ClassManager, buff: BinaryIO) -> int:
     return cm.packer["B"].unpack(buff.read(1))[0]
 
 
-def readuleb128(cm, buff):
+def readuleb128(cm: ClassManager, buff: BinaryIO) -> int:
     """
     Read an unsigned LEB128 at the current position of the buffer
 
     :param buff: a file like object
     :return: decoded unsigned LEB128
     """
     result = get_byte(cm, buff)
@@ -233,26 +241,26 @@
                     if cur > 0x0f:
                         logger.warning("possible error while decoding number")
                     result |= cur << 28
 
     return result
 
 
-def readuleb128p1(cm, buff):
+def readuleb128p1(cm: ClassManager, buff: BinaryIO) -> int:
     """
     Read an unsigned LEB128p1 at the current position of the buffer.
     This format is the same as uLEB128 but has the ability to store the value -1.
 
     :param buff: a file like object
     :return: decoded uLEB128p1
     """
     return readuleb128(cm, buff) - 1
 
 
-def readsleb128(cm, buff):
+def readsleb128(cm: ClassManager, buff: BinaryIO) -> int:
     """
     Read a signed LEB128 at the current position of the buffer.
 
     :param buff: a file like object
     :return: decoded sLEB128
     """
     result = 0
@@ -270,15 +278,15 @@
                 result = (0x7fffffff & result) - 0x80000000
             result = result >> bit_left
             break
 
     return result
 
 
-def writeuleb128(cm, value):
+def writeuleb128(cm: ClassManager, value: int) -> bytearray:
     """
     Convert an integer value to the corresponding unsigned LEB128.
 
     Raises a value error, if the given value is negative.
 
     :param value: non-negative integer
     :return: bytes
@@ -295,15 +303,15 @@
         value = remaining
         remaining >>= 7
 
     buff += cm.packer["B"].pack(value & 0x7f)
     return buff
 
 
-def writesleb128(cm, value):
+def writesleb128(cm: ClassManager, value: int) -> bytearray:
     """
     Convert an integer value to the corresponding signed LEB128
 
     :param value: integer value
     :return: bytes
     """
     remaining = value >> 7
@@ -324,15 +332,15 @@
         buff += cm.packer["B"].pack((value & 0x7f) | tmp)
         value = remaining
         remaining >>= 7
 
     return buff
 
 
-def determineNext(i, cur_idx, m):
+def determineNext(i: Instruction, cur_idx: int, m: EncodedMethod) -> list:
     """
     Determine the next offsets inside the bytecode of an :class:`EncodedMethod`.
     The offsets are calculated in number of bytes from the start of the method.
     Note, that offsets inside the bytecode are denoted in 16bit units but this method returns actual bytes!
 
     Offsets inside the opcode are counted from the beginning of the opcode.
 
@@ -392,15 +400,15 @@
             logger.warning("Could not determine payload of switch command at offset {} inside {}! "
                         "Possibly broken bytecode?".format(cur_idx, m))
 
         return x
     return []
 
 
-def determineException(vm, m):
+def determineException(vm: DEX, m:EncodedMethod) ->  list[list]:
     """
     Returns try-catch handler inside the method.
 
     :param vm: a :class:`~DEX`
     :param m: a :class:`~EncodedMethod`
     :return:
     """
@@ -431,20 +439,22 @@
 
     exceptions = []
     # print m.get_name(), h_off
     for i in h_off:
         for value in h_off[i]:
             try_value = value[0]
 
+            # start,end
             z = [try_value.get_start_addr() * 2,
                  (try_value.get_start_addr() * 2) +
                  (try_value.get_insn_count() * 2) - 1]
 
             handler_catch = value[1]
 
+            # exceptions
             for handler in handler_catch.get_handlers():
                 z.append([vm.get_cm_type(handler.get_type_idx()),
                           handler.get_addr() * 2])
 
             if handler_catch.get_size() <= 0:
                 z.append(["Ljava/lang/Throwable;",
                           handler_catch.get_catch_all_addr() * 2])
@@ -463,15 +473,15 @@
     corruption.
     :param buff: a string which represents a Buff object of the header_item
     :type io.BufferedReader buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, size, buff, cm):
+    def __init__(self, size, buff: BinaryIO, cm:ClassManager) -> None:
         logger.debug("HeaderItem")
 
         self.CM = cm
 
         self.offset = buff.tell()
 
         if self.offset != 0:
@@ -543,15 +553,15 @@
         self.type_off_obj = None
         self.proto_off_obj = None
         self.field_off_obj = None
         self.method_off_obj = None
         self.class_off_obj = None
         self.data_off_obj = None
 
-    def get_obj(self):
+    def get_obj(self) -> bytes:
         if self.map_off_obj is None:
             self.map_off_obj = self.CM.get_item_by_offset(self.map_off)
 
         if self.string_off_obj is None:
             self.string_off_obj = self.CM.get_item_by_offset(self.string_ids_off)
 
         if self.type_off_obj is None:
@@ -618,21 +628,21 @@
                pack("<I", self.method_ids_size) + \
                pack("<I", self.method_ids_off) + \
                pack("<I", self.class_defs_size) + \
                pack("<I", self.class_defs_off) + \
                pack("<I", self.data_size) + \
                pack("<I", self.data_off)
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.get_obj()
 
-    def get_length(self):
+    def get_length(self) -> int:
         return 112
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Header Item")
         bytecode._PrintDefault("magic=%s, checksum=%s, signature=%s\n" %
                                (self.magic, self.checksum,
                                    binascii.hexlify(self.signature).decode("ASCII")))
         bytecode._PrintDefault("file_size=%x, header_size=%x, endian_tag=%x\n" %
                                (self.file_size, self.header_size,
                                 self.endian_tag))
@@ -671,103 +681,103 @@
             self.type_ids_size, self.type_ids_off,
             self.proto_ids_size, self.proto_ids_off,
             self.field_ids_size, self.field_ids_off,
             self.method_ids_size, self.method_ids_off,
             self.class_defs_size, self.class_defs_off,
             self.data_size, self.data_off)
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
 
 class AnnotationOffItem:
     """
     This class can parse an annotation_off_item of a dex file
 
     :param buff: a string which represents a Buff object of the annotation_off_item
-    :type buff: Buff object
+    :type buff: BinaryIO bytes object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm: ClassManager) -> None:
         self.CM = cm
         self.annotation_off, = cm.packer["I"].unpack(buff.read(4))
 
-    def get_annotation_off(self):
+    def get_annotation_off(self) -> int:
         return self.annotation_off
 
     def show(self):
         bytecode._PrintSubBanner("Annotation Off Item")
         bytecode._PrintDefault("annotation_off=0x%x\n" % self.annotation_off)
 
-    def get_obj(self):
+    def get_obj(self) -> bytes:
         if self.annotation_off != 0:
             self.annotation_off = self.CM.get_obj_by_offset(
                 self.annotation_off).get_off()
 
         return self.CM.packer["I"].pack(self.annotation_off)
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.get_obj()
 
-    def get_length(self):
+    def get_length(self) -> int:
         return len(self.get_obj())
 
-    def get_annotation_item(self):
+    def get_annotation_item(self) -> list[AnnotationItem]:
         return self.CM.get_annotation_item(self.get_annotation_off())
 
 
 class AnnotationSetItem:
     """
     This class can parse an annotation_set_item of a dex file
 
     :param buff: a string which represents a Buff object of the annotation_set_item
     :type io.BufferedReader buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
         self.offset = buff.tell()
 
         self.size, = cm.packer["I"].unpack(buff.read(4))
         self.annotation_off_item = [AnnotationOffItem(buff, cm) for _ in range(self.size)]
 
-    def get_annotation_off_item(self):
+    def get_annotation_off_item(self) -> list[AnnotationOffItem]:
         """
         Return the offset from the start of the file to an annotation
 
         :rtype: a list of :class:`AnnotationOffItem`
         """
         return self.annotation_off_item
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Annotation Set Item")
         for i in self.annotation_off_item:
             i.show()
 
-    def get_obj(self):
+    def get_obj(self) -> bytes:
         return self.CM.packer["I"].pack(self.size)
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.get_obj() + b''.join(i.get_raw()
                                          for i in self.annotation_off_item)
 
-    def get_length(self):
+    def get_length(self) -> int:
         length = len(self.get_obj())
 
         for i in self.annotation_off_item:
             length += i.get_length()
 
         return length
 
@@ -778,273 +788,273 @@
 
     :param buff: a string which represents a Buff object of the annotation_set_ref_item
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
         self.annotations_off, = cm.packer["I"].unpack(buff.read(4))
 
-    def get_annotations_off(self):
+    def get_annotations_off(self) -> int:
         """
         Return the offset from the start of the file to the referenced annotation set or
         0 if there are no annotations for this element.
 
         :rtype: int
         """
         return self.annotations_off
 
-    def show(self):
+    def show(self) -> str:
         bytecode._PrintSubBanner("Annotation Set Ref Item")
         bytecode._PrintDefault("annotation_off=0x%x\n" % self.annotations_off)
 
-    def get_obj(self):
+    def get_obj(self) -> bytes:
         if self.annotations_off != 0:
             self.annotations_off = self.CM.get_obj_by_offset(
                 self.annotations_off).get_off()
 
         return self.CM.packer["I"].pack(self.annotations_off)
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.get_obj()
 
 
 class AnnotationSetRefList:
     """
     This class can parse an annotation_set_ref_list_item of a dex file
 
     :param buff: a string which represents a Buff object of the annotation_set_ref_list_item
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.offset = buff.tell()
 
         self.CM = cm
         self.size, = cm.packer["I"].unpack(buff.read(4))
 
         self.list = [AnnotationSetRefItem(buff, cm) for _ in range(self.size)]
 
-    def get_list(self):
+    def get_list(self) -> list[AnnotationSetRefItem]:
         """
-        Return elements of the list
+        Return list of AnnotationSetRefItem
 
-        :rtype: :class:`AnnotationSetRefItem`
+        :rtype: list
         """
         return self.list
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Annotation Set Ref List Item")
         for i in self.list:
             i.show()
 
-    def get_obj(self):
+    def get_obj(self) -> list[AnnotationSetRefItem]:
         return [i for i in self.list]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.CM.packer["I"].pack(self.size) + b''.join(i.get_raw() for i in self.list)
 
-    def get_length(self):
+    def get_length(self) -> int:
         return len(self.get_raw())
 
 
 class FieldAnnotation:
     """
     This class can parse a field_annotation of a dex file
 
     :param buff: a string which represents a Buff object of the field_annotation
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.offset = buff.tell()
 
         self.CM = cm
         self.field_idx, self.annotations_off = cm.packer["2I"].unpack(buff.read(8))
 
-    def get_field_idx(self):
+    def get_field_idx(self) -> int:
         """
         Return the index into the field_ids list for the identity of the field being annotated
 
         :rtype: int
         """
         return self.field_idx
 
-    def get_annotations_off(self):
+    def get_annotations_off(self) -> int:
         """
         Return the offset from the start of the file to the list of annotations for the field
 
         :rtype: int
         """
         return self.annotations_off
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Field Annotation")
         bytecode._PrintDefault("field_idx=0x%x annotations_off=0x%x\n" %
                                (self.field_idx, self.annotations_off))
 
-    def get_obj(self):
+    def get_obj(self) -> bytes:
         if self.annotations_off != 0:
             self.annotations_off = self.CM.get_obj_by_offset(
                 self.annotations_off).get_off()
 
         return self.CM.packer["2I"].pack(self.field_idx, self.annotations_off)
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.get_obj()
 
-    def get_length(self):
+    def get_length(self) -> int:
         return len(self.get_raw())
 
 
 class MethodAnnotation:
     """
     This class can parse a method_annotation of a dex file
 
     :param buff: a string which represents a Buff object of the method_annotation
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.offset = buff.tell()
 
         self.CM = cm
         self.method_idx, \
         self.annotations_off = cm.packer["2I"].unpack(buff.read(8))
 
-    def get_method_idx(self):
+    def get_method_idx(self) -> int:
         """
         Return the index into the method_ids list for the identity of the method being annotated
 
         :rtype: int
         """
         return self.method_idx
 
-    def get_annotations_off(self):
+    def get_annotations_off(self) -> int:
         """
         Return the offset from the start of the file to the list of annotations for the method
 
         :rtype: int
         """
         return self.annotations_off
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Method Annotation")
         bytecode._PrintDefault("method_idx=0x%x annotations_off=0x%x\n" %
                                (self.method_idx, self.annotations_off))
 
-    def get_obj(self):
+    def get_obj(self) -> bytes:
         if self.annotations_off != 0:
             self.annotations_off = self.CM.get_obj_by_offset(
                 self.annotations_off).get_off()
 
         return self.CM.packer["2I"].pack(self.method_idx, self.annotations_off)
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.get_obj()
 
-    def get_length(self):
+    def get_length(self) -> int:
         return len(self.get_raw())
 
 
 class ParameterAnnotation:
     """
     This class can parse a parameter_annotation of a dex file
 
     :param buff: a string which represents a Buff object of the parameter_annotation
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.offset = buff.tell()
 
         self.CM = cm
         self.method_idx, \
         self.annotations_off = cm.packer["2I"].unpack(buff.read(8))
 
-    def get_method_idx(self):
+    def get_method_idx(self) -> int:
         """
         Return the index into the method_ids list for the identity of the method whose parameters are being annotated
 
         :rtype: int
         """
         return self.method_idx
 
-    def get_annotations_off(self):
+    def get_annotations_off(self) -> int:
         """
         Return the offset from the start of the file to the list of annotations for the method parameters
 
         :rtype: int
         """
         return self.annotations_off
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Parameter Annotation")
         bytecode._PrintDefault("method_idx=0x%x annotations_off=0x%x\n" %
                                (self.method_idx, self.annotations_off))
 
-    def get_obj(self):
+    def get_obj(self) -> bytes:
         if self.annotations_off != 0:
             self.annotations_off = self.CM.get_obj_by_offset(
                 self.annotations_off).get_off()
 
         return self.CM.packer["2I"].pack(self.method_idx, self.annotations_off)
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.get_obj()
 
-    def get_length(self):
+    def get_length(self) -> int:
         return len(self.get_raw())
 
 
 class AnnotationsDirectoryItem:
     """
     This class can parse an annotations_directory_item of a dex file
 
     :param buff: a string which represents a Buff object of the annotations_directory_item
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
 
         self.offset = buff.tell()
 
         self.class_annotations_off, \
         self.annotated_fields_size, \
         self.annotated_methods_size, \
@@ -1052,81 +1062,81 @@
 
         self.field_annotations = [FieldAnnotation(buff, cm) for i in range(0, self.annotated_fields_size)]
 
         self.method_annotations = [MethodAnnotation(buff, cm) for i in range(0, self.annotated_methods_size)]
 
         self.parameter_annotations = [ParameterAnnotation(buff, cm) for i in range(0, self.annotated_parameters_size)]
 
-    def get_class_annotations_off(self):
+    def get_class_annotations_off(self) -> int:
         """
         Return the offset from the start of the file to the annotations made directly on the class,
         or 0 if the class has no direct annotations
 
         :rtype: int
         """
         return self.class_annotations_off
 
-    def get_annotation_set_item(self):
+    def get_annotation_set_item(self) -> list[AnnotationSetItem]:
         return self.CM.get_annotation_set_item(self.class_annotations_off)
 
-    def get_annotated_fields_size(self):
+    def get_annotated_fields_size(self) -> int:
         """
         Return the count of fields annotated by this item
 
         :rtype: int
         """
         return self.annotated_fields_size
 
-    def get_annotated_methods_size(self):
+    def get_annotated_methods_size(self) -> int:
         """
         Return the count of methods annotated by this item
 
         :rtype: int
         """
         return self.annotated_methods_size
 
-    def get_annotated_parameters_size(self):
+    def get_annotated_parameters_size(self) -> int:
         """
         Return the count of method parameter lists annotated by this item
 
         :rtype: int
         """
         return self.annotated_parameters_size
 
-    def get_field_annotations(self):
+    def get_field_annotations(self) -> list[FieldAnnotation]:
         """
         Return the list of associated field annotations
 
         :rtype: a list of :class:`FieldAnnotation`
         """
         return self.field_annotations
 
-    def get_method_annotations(self):
+    def get_method_annotations(self) -> list[MethodAnnotation]:
         """
         Return the list of associated method annotations
 
         :rtype: a list of :class:`MethodAnnotation`
         """
         return self.method_annotations
 
-    def get_parameter_annotations(self):
+    def get_parameter_annotations(self) -> list[ParameterAnnotation]:
         """
         Return the list of associated method parameter annotations
 
         :rtype: a list of :class:`ParameterAnnotation`
         """
         return self.parameter_annotations
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Annotations Directory Item")
         bytecode._PrintDefault(
             "class_annotations_off=0x%x annotated_fields_size=%d annotated_methods_size=%d annotated_parameters_size=%d\n"
             % (self.class_annotations_off, self.annotated_fields_size,
                self.annotated_methods_size, self.annotated_parameters_size))
 
         for i in self.field_annotations:
@@ -1134,31 +1144,31 @@
 
         for i in self.method_annotations:
             i.show()
 
         for i in self.parameter_annotations:
             i.show()
 
-    def get_obj(self):
+    def get_obj(self) -> bytes:
         if self.class_annotations_off != 0:
             self.class_annotations_off = self.CM.get_obj_by_offset(
                 self.class_annotations_off).get_off()
 
         return self.CM.packer["4I"].pack(self.class_annotations_off,
                     self.annotated_fields_size,
                     self.annotated_methods_size,
                     self.annotated_parameters_size)
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.get_obj() + \
                b''.join(i.get_raw() for i in self.field_annotations) + \
                b''.join(i.get_raw() for i in self.method_annotations) + \
                b''.join(i.get_raw() for i in self.parameter_annotations)
 
-    def get_length(self):
+    def get_length(self) -> int:
         length = len(self.get_obj())
         for i in self.field_annotations:
             length += i.get_length()
 
         for i in self.method_annotations:
             length += i.get_length()
 
@@ -1188,15 +1198,15 @@
         GREYLIST_MAX_R = 6
 
     class DomapiApiFlag(IntEnum):
         NONE = 0
         CORE_PLATFORM_API = 1
         TEST_API = 2
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
 
         self.offset = buff.tell()
 
         self.section_size, = cm.packer["I"].unpack(buff.read(4))
 
         # Find the end of the offsets array (first non-zero offset entry is the start of `flags`)
@@ -1232,15 +1242,15 @@
         :param idx: The index to return the flags of (index of the class)
         :type idx: int
 
         :rtype: Tuple[RestrictionApiFlag, DomainApiFlag]
         """
         return self.flags[idx]
 
-    def set_off(self, off):
+    def set_off(self, off:int):
         self.offset = off
 
     def get_off(self):
         return self.offset
 
     def show(self):
         bytecode._PrintSubBanner("HiddenApi Class Data Item")
@@ -1277,15 +1287,15 @@
 
     :param buff: a string which represents a Buff object of the type_item
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
         self.type_idx, = cm.packer["H"].unpack(buff.read(2))
 
     def get_type_idx(self):
         """
         Return the index into the type_ids list
 
@@ -1321,15 +1331,15 @@
 
     :param buff: a string which represents a Buff object of the type_list
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
         self.offset = buff.tell()
         self.size, = cm.packer["I"].unpack(buff.read(4))
 
         self.list = [TypeItem(buff, cm) for _ in range(self.size)]
 
         self.pad = b""
@@ -1374,15 +1384,15 @@
         """
         Return the list of TypeItem
 
         :rtype: a list of :class:`TypeItem` objects
         """
         return self.list
 
-    def set_off(self, off):
+    def set_off(self, off:int):
         self.offset = off
 
     def get_off(self):
         return self.offset + self.len_pad
 
     def show(self):
         bytecode._PrintSubBanner("Type List")
@@ -1441,15 +1451,15 @@
                 buff += writeuleb128(self.CM, i[0])
             elif i[1] == "s":
                 buff += writesleb128(self.CM, i[0])
         return buff
 
 
 class DebugInfoItem:
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
 
         self.offset = buff.tell()
 
         self.line_start = readuleb128(cm, buff)
         self.parameters_size = readuleb128(cm, buff)
 
@@ -1537,24 +1547,24 @@
         #                      b''.join(i.get_raw() for i in self.bytecodes))]
 
     def get_off(self):
         return self.offset
 
 
 class DebugInfoItemEmpty:
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
 
         self.offset = buff.tell()
         self.__buff = buff
         self.__raw = ""
 
         self.reload()
 
-    def set_off(self, off):
+    def set_off(self, off:int):
         self.offset = off
 
     def get_off(self):
         return self.offset
 
     def reload(self):
         offset = self.offset
@@ -1585,15 +1595,15 @@
 
     :param buff: a string which represents a Buff object of the encoded_array
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
         self.offset = buff.tell()
 
         self.size = readuleb128(cm, buff)
 
         self.values = [EncodedValue(buff, cm) for _ in range(self.size)]
 
@@ -1620,15 +1630,15 @@
 
         for i in self.values:
             i.show()
 
     def get_obj(self):
         return writeuleb128(self.CM, self.size)
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.get_obj() + b''.join(i.get_raw() for i in self.values)
 
     def get_length(self):
         length = len(self.get_obj())
         for i in self.values:
             length += i.get_length()
 
@@ -1641,15 +1651,15 @@
 
     :param buff: a string which represents a Buff object of the encoded_value
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
 
         self.val = get_byte(cm, buff)
         self.value_arg = self.val >> 5
         self.value_type = self.val & 0x1f
 
         self.raw_value = None
@@ -1745,15 +1755,15 @@
 
     :param buff: a string which represents a Buff object of the annotation_element
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
         self.offset = buff.tell()
 
         self.name_idx = readuleb128(cm, buff)
         self.value = EncodedValue(buff, cm)
 
     def get_name_idx(self):
@@ -1793,15 +1803,15 @@
 
     :param buff: a string which represents a Buff object of the encoded_annotation
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
         self.offset = buff.tell()
 
         self.type_idx = readuleb128(cm, buff)
         self.size = readuleb128(cm, buff)
 
         self.elements = [AnnotationElement(buff, cm) for _ in range(self.size)]
@@ -1855,105 +1865,105 @@
 
 
 class AnnotationItem:
     """
     This class can parse an annotation_item of a dex file
 
     :param buff: a string which represents a Buff object of the annotation_item
-    :type buff: Buff object
+    :type buff: BinaryIO bytes object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
 
         self.offset = buff.tell()
 
         self.visibility = get_byte(cm, buff)
         self.annotation = EncodedAnnotation(buff, cm)
 
-    def get_visibility(self):
+    def get_visibility(self) -> int:
         """
         Return the intended visibility of this annotation
 
         :rtype: int
         """
         return self.visibility
 
-    def get_annotation(self):
+    def get_annotation(self) -> EncodedAnnotation:
         """
         Return the encoded annotation contents
 
         :rtype: a :class:`EncodedAnnotation` object
         """
         return self.annotation
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Annotation Item")
         bytecode._PrintDefault("visibility=%d\n" % self.visibility)
         self.annotation.show()
 
-    def get_obj(self):
+    def get_obj(self) -> list[EncodedAnnotation]:
         return [self.annotation]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.CM.packer["B"].pack(self.visibility) + self.annotation.get_raw()
 
-    def get_length(self):
+    def get_length(self) -> int:
         return len(self.get_raw())
 
 
 class EncodedArrayItem:
     """
     This class can parse an encoded_array_item of a dex file
 
     :param buff: a string which represents a Buff object of the encoded_array_item
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm: ClassManager) -> None:
         self.CM = cm
 
         self.offset = buff.tell()
         self.value = EncodedArray(buff, cm)
 
-    def get_value(self):
+    def get_value(self) -> EncodedArray:
         """
         Return the bytes representing the encoded array value
 
         :rtype: a :class:`EncodedArray` object
         """
         return self.value
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Encoded Array Item")
         self.value.show()
 
-    def get_obj(self):
+    def get_obj(self) -> list[EncodedArray]:
         return [self.value]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.value.get_raw()
 
-    def get_length(self):
+    def get_length(self) -> int:
         return self.value.get_length()
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
 
 class StringDataItem:
     """
     This class can parse a string_data_item of a dex file
 
@@ -1972,78 +1982,78 @@
     string and can handle encoding yourself.
     Or you use :meth:`get_unicode` to return a decoded UTF-16 string, which
     might cause problems during printing or saving.
     If you want a representation of the string, which should be printable in
     python you ca use :meth:`get` which escapes invalid characters.
 
     :param buff: a string which represents a Buff object of the string_data_item
-    :type buff: io.io.BufferedReader
+    :type buff: BinaryIO.io.BufferedReader
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm: ClassManager) -> None:
         self.CM = cm
 
         self.offset = buff.tell()
 
         # Content of string_data_item
         self.utf16_size = readuleb128(cm, buff)
         self.data = read_null_terminated_string(buff)
 
-    def get_utf16_size(self):
+    def get_utf16_size(self) -> int:
         """
         Return the size of this string, in UTF-16 code units
 
         :rtype:int
         """
         return self.utf16_size
 
-    def get_data(self):
+    def get_data(self) -> str:
         """
         Return a series of MUTF-8 code units (a.k.a. octets, a.k.a. bytes) followed by a byte of value 0
 
         :rtype: string
         """
         return self.data + b"\x00"
 
-    def set_off(self, off):
+    def set_off(self, off: int) -> None:
         self.offset = off
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def get(self):
+    def get(self) -> str:
         """
         Returns a str object
         """
         try:
             return mutf8.decode(self.data)
         except UnicodeDecodeError:
             logger.error("Impossible to decode {}".format(self.data))
             return "ANDROGUARD[INVALID_STRING] {}".format(self.data)
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("String Data Item")
         bytecode._PrintDefault("utf16_size=%d data=%s\n" %
                                (self.utf16_size, repr(self.get())))
 
-    def get_obj(self):
+    def get_obj(self) -> list:
         return []
 
-    def get_raw(self):
+    def get_raw(self) ->  bytes:
         """
         Returns the raw string including the ULEB128 coded length
         and null byte string terminator
 
         :return: bytes
         """
         return writeuleb128(self.CM, self.utf16_size) + self.data + b"\x00"
 
-    def get_length(self):
+    def get_length(self) -> int:
         """
         Get the length of the raw string including the ULEB128 coded
         length and the null byte terminator
 
         :return: int
         """
         return len(writeuleb128(self.CM, self.utf16_size)) + len(self.data) + 1
@@ -2055,149 +2065,149 @@
 
     :param buff: a string which represents a Buff object of the string_id_item
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm: ClassManager):
         self.CM = cm
         self.offset = buff.tell()
 
         self.string_data_off, = cm.packer["I"].unpack(buff.read(4))
 
-    def get_string_data_off(self):
+    def get_string_data_off(self) -> int:
         """
         Return the offset from the start of the file to the string data for this item
 
         :rtype: int
         """
         return self.string_data_off
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("String Id Item")
         bytecode._PrintDefault("string_data_off=%x\n" % self.string_data_off)
 
-    def get_obj(self):
+    def get_obj(self) -> bytes:
         if self.string_data_off != 0:
             self.string_data_off = self.CM.get_string_by_offset(
                 self.string_data_off).get_off()
 
         return self.CM.packer["I"].pack(self.string_data_off)
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.get_obj()
 
-    def get_length(self):
+    def get_length(self) -> int:
         return len(self.get_obj())
 
 
 class TypeIdItem:
     """
     This class can parse a type_id_item of a dex file
 
     :param buff: a string which represents a Buff object of the type_id_item
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm: ClassManager):
         self.CM = cm
         self.offset = buff.tell()
 
         self.descriptor_idx, = cm.packer["I"].unpack(buff.read(4))
         self.descriptor_idx_value = self.CM.get_string(self.descriptor_idx)
 
-    def get_descriptor_idx(self):
+    def get_descriptor_idx(self) -> int:
         """
         Return the index into the string_ids list for the descriptor string of this type
 
         :rtype: int
         """
         return self.descriptor_idx
 
-    def get_descriptor_idx_value(self):
+    def get_descriptor_idx_value(self) -> str:
         """
         Return the string associated to the descriptor
 
         :rtype: string
         """
         return self.descriptor_idx_value
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Type Id Item")
         bytecode._PrintDefault("descriptor_idx=%d descriptor_idx_value=%s\n" %
                                (self.descriptor_idx, self.descriptor_idx_value))
 
-    def get_obj(self):
+    def get_obj(self) -> bytes:
         return self.CM.packer["I"].pack(self.descriptor_idx)
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.get_obj()
 
-    def get_length(self):
+    def get_length(self) -> int:
         return len(self.get_obj())
 
 
 class TypeHIdItem:
     """
     This class can parse a list of type_id_item of a dex file
 
     :param buff: a string which represents a Buff object of the list of type_id_item
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, size, buff, cm):
+    def __init__(self, size: int, buff: BinaryIO, cm: ClassManager) -> None:
         self.CM = cm
 
         self.offset = buff.tell()
 
         self.type = [TypeIdItem(buff, cm) for i in range(0,size)]
 
-    def get_type(self):
+    def get_type(self) -> list[TypeIdItem]:
         """
         Return the list of type_id_item
 
         :rtype: a list of :class:`TypeIdItem` objects
         """
         return self.type
 
-    def get(self, idx):
+    def get(self, idx: int) -> int:
         try:
             return self.type[idx].get_descriptor_idx()
         except IndexError:
             return -1
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Type List Item")
         for i in self.type:
             i.show()
 
-    def get_obj(self):
+    def get_obj(self) -> list[TypeIdItem]:
         return [i for i in self.type]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return b''.join(i.get_raw() for i in self.type)
 
-    def get_length(self):
+    def get_length(self) -> int:
         length = 0
         for i in self.type:
             length += i.get_length()
         return length
 
 
 class ProtoIdItem:
@@ -2206,149 +2216,148 @@
 
     :param buff: a string which represents a Buff object of the proto_id_item
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm: ClassManager):
         self.CM = cm
         self.offset = buff.tell()
 
         self.shorty_idx, \
         self.return_type_idx, \
         self.parameters_off = cm.packer["3I"].unpack(buff.read(12))
 
         self.shorty_idx_value = self.CM.get_string(self.shorty_idx)
         self.return_type_idx_value = self.CM.get_type(self.return_type_idx)
         self.parameters_off_value = None
 
-    def get_shorty_idx(self):
+    def get_shorty_idx(self) -> int:
         """
         Return the index into the string_ids list for the short-form descriptor string of this prototype
 
         :rtype: int
         """
         return self.shorty_idx
 
-    def get_return_type_idx(self):
+    def get_return_type_idx(self) -> int:
         """
         Return the index into the type_ids list for the return type of this prototype
 
         :rtype: int
         """
         return self.return_type_idx
 
-    def get_parameters_off(self):
+    def get_parameters_off(self) -> int:
         """
         Return the offset from the start of the file to the list of parameter types for this prototype, or 0 if this prototype has no parameters
 
         :rtype: int
         """
         return self.parameters_off
 
-    def get_shorty_idx_value(self):
+    def get_shorty_idx_value(self) -> str:
         """
         Return the string associated to the shorty_idx
 
         :rtype: string
         """
         if self.shorty_idx_value is None:
             self.shorty_idx_value = self.CM.get_string(self.shorty_idx)
         return self.shorty_idx_value
 
-    def get_return_type_idx_value(self):
+    def get_return_type_idx_value(self) -> str:
         """
         Return the string associated to the return_type_idx
 
         :rtype: string
         """
         if self.return_type_idx_value is None:
             self.return_type_idx_value = self.CM.get_type(self.return_type_idx)
-
         return self.return_type_idx_value
 
-    def get_parameters_off_value(self):
+    def get_parameters_off_value(self) -> str:
         """
         Return the string associated to the parameters_off
 
         :rtype: str
         """
         if self.parameters_off_value is None:
             params = self.CM.get_type_list(self.parameters_off)
             self.parameters_off_value = '(' + ' '.join(params) + ')'
         return self.parameters_off_value
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Proto Item")
         bytecode._PrintDefault(
             "shorty_idx=%d return_type_idx=%d parameters_off=%d\n" %
             (self.shorty_idx, self.return_type_idx, self.parameters_off))
         bytecode._PrintDefault(
             "shorty_idx_value=%s return_type_idx_value=%s parameters_off_value=%s\n"
             % (self.shorty_idx_value, self.return_type_idx_value,
                self.parameters_off_value))
 
-    def get_obj(self):
+    def get_obj(self) -> bytes:
         if self.parameters_off != 0:
             self.parameters_off = self.CM.get_obj_by_offset(
                 self.parameters_off).get_off()
 
         return self.CM.packer["3I"].pack(self.shorty_idx,
                     self.return_type_idx,
                     self.parameters_off)
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.get_obj()
 
-    def get_length(self):
+    def get_length(self) -> int:
         return len(self.get_obj())
 
 
 class ProtoHIdItem:
     """
     This class can parse a list of proto_id_item of a dex file
 
     :param buff: a string which represents a Buff object of the list of proto_id_item
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, size, buff, cm):
+    def __init__(self, size:int, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
 
         self.offset = buff.tell()
 
         self.proto = [ProtoIdItem(buff, cm) for i in range(0, size)]
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def get(self, idx):
+    def get(self, idx:int) -> ProtoIdItem:
         try:
             return self.proto[idx]
         except IndexError:
             return ProtoIdItemInvalid()
 
-    def show(self):
+    def show(self) ->  None:
         bytecode._PrintSubBanner("Proto List Item")
         for i in self.proto:
             i.show()
 
-    def get_obj(self):
+    def get_obj(self) ->  list[ProtoIdItem]:
         return [i for i in self.proto]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return b''.join(i.get_raw() for i in self.proto)
 
-    def get_length(self):
+    def get_length(self) -> int:
         length = 0
         for i in self.proto:
             length += i.get_length()
         return length
 
 
 class FieldIdItem:
@@ -2357,164 +2366,160 @@
 
     :param buff: a string which represents a Buff object of the field_id_item
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm: ClassManager):
         self.CM = cm
         self.offset = buff.tell()
 
         self.class_idx, \
         self.type_idx, \
         self.name_idx = cm.packer["2HI"].unpack(buff.read(8))
 
         self.reload()
 
-    def reload(self):
+    def reload(self) -> None:
         self.class_idx_value = self.CM.get_type(self.class_idx)
         self.type_idx_value = self.CM.get_type(self.type_idx)
         self.name_idx_value = self.CM.get_string(self.name_idx)
 
-    def get_class_idx(self):
+    def get_class_idx(self) -> int:
         """
         Return the index into the type_ids list for the definer of this field
 
         :rtype: int
         """
         return self.class_idx
 
-    def get_type_idx(self):
+    def get_type_idx(self) -> int:
         """
         Return the index into the type_ids list for the type of this field
 
         :rtype: int
         """
         return self.type_idx
 
-    def get_name_idx(self):
+    def get_name_idx(self) -> int:
         """
         Return the index into the string_ids list for the name of this field
 
         :rtype: int
         """
         return self.name_idx
 
-    def get_class_name(self):
+    def get_class_name(self) -> str:
         """
         Return the class name of the field
 
         :rtype: string
         """
         if self.class_idx_value is None:
             self.class_idx_value = self.CM.get_type(self.class_idx)
-
         return self.class_idx_value
 
-    def get_type(self):
+    def get_type(self) -> str:
         """
         Return the type of the field
 
         :rtype: string
         """
         if self.type_idx_value is None:
             self.type_idx_value = self.CM.get_type(self.type_idx)
-
         return self.type_idx_value
 
-    def get_descriptor(self):
+    def get_descriptor(self) -> str:
         """
         Return the descriptor of the field
 
         :rtype: string
         """
         if self.type_idx_value is None:
             self.type_idx_value = self.CM.get_type(self.type_idx)
-
         return self.type_idx_value
 
-    def get_name(self):
+    def get_name(self) -> str:
         """
         Return the name of the field
 
         :rtype: string
         """
         if self.name_idx_value is None:
             self.name_idx_value = self.CM.get_string(self.name_idx)
-
         return self.name_idx_value
 
-    def get_list(self):
+    def get_list(self) -> list[str]:
         return [self.get_class_name(), self.get_type(), self.get_name()]
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Field Id Item")
         bytecode._PrintDefault("class_idx=%d type_idx=%d name_idx=%d\n" %
                                (self.class_idx, self.type_idx, self.name_idx))
         bytecode._PrintDefault(
             "class_idx_value=%s type_idx_value=%s name_idx_value=%s\n" %
             (self.class_idx_value, self.type_idx_value, self.name_idx_value))
 
-    def get_obj(self):
+    def get_obj(self) -> bytes:
         return self.CM.packer["2HI"].pack(self.class_idx,
                     self.type_idx,
                     self.name_idx)
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.get_obj()
 
-    def get_length(self):
+    def get_length(self) -> int:
         return len(self.get_obj())
 
 
 class FieldHIdItem:
     """
     This class can parse a list of field_id_item of a dex file
 
     :param buff: a string which represents a Buff object of the list of field_id_item
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, size, buff, cm):
+    def __init__(self, size:int, buff: BinaryIO, cm:ClassManager) -> None:
         self.offset = buff.tell()
 
         self.field_id_items = [FieldIdItem(buff, cm) for i in range(0, size)]
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def gets(self):
+    def gets(self) -> list[FieldIdItem]:
         return self.field_id_items
 
-    def get(self, idx):
+    def get(self, idx:int) -> Union[FieldIdItem,FieldIdItemInvalid]:
         try:
             return self.field_id_items[idx]
         except IndexError:
             return FieldIdItemInvalid()
 
-    def show(self):
+    def show(self) -> None:
         nb = 0
         for i in self.field_id_items:
             print(nb, end=' ')
             i.show()
             nb = nb + 1
 
-    def get_obj(self):
+    def get_obj(self) -> list[FieldIdItem]:
         return [i for i in self.field_id_items]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return b''.join(i.get_raw() for i in self.field_id_items)
 
-    def get_length(self):
+    def get_length(self) -> int:
         length = 0
         for i in self.field_id_items:
             length += i.get_length()
         return length
 
 
 class MethodIdItem:
@@ -2523,254 +2528,253 @@
 
     :param buff: a string which represents a Buff object of the method_id_item
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
         self.offset = buff.tell()
 
         self.class_idx, \
         self.proto_idx, \
         self.name_idx = cm.packer["2HI"].unpack(buff.read(8))
 
         self.reload()
 
-    def reload(self):
+    def reload(self) -> None:
         self.class_idx_value = self.CM.get_type(self.class_idx)
         self.proto_idx_value = self.CM.get_proto(self.proto_idx)
         self.name_idx_value = self.CM.get_string(self.name_idx)
 
-    def get_class_idx(self):
+    def get_class_idx(self) -> int:
         """
         Return the index into the type_ids list for the definer of this method
 
         :rtype: int
         """
         return self.class_idx
 
-    def get_proto_idx(self):
+    def get_proto_idx(self) -> int:
         """
         Return the index into the proto_ids list for the prototype of this method
 
         :rtype: int
         """
         return self.proto_idx
 
-    def get_name_idx(self):
+    def get_name_idx(self) -> int:
         """
         Return the index into the string_ids list for the name of this method
 
         :rtype: int
         """
         return self.name_idx
 
-    def get_class_name(self):
+    def get_class_name(self) -> str:
         """
         Return the class name of the method
 
         :rtype: string
         """
         if self.class_idx_value is None:
             self.class_idx_value = self.CM.get_type(self.class_idx)
 
         return self.class_idx_value
 
-    def get_proto(self):
+    def get_proto(self) -> str:
         """
         Return the prototype of the method
 
         :rtype: string
         """
         if self.proto_idx_value is None:
             self.proto_idx_value = self.CM.get_proto(self.proto_idx)
 
         return self.proto_idx_value
 
-    def get_descriptor(self):
+    def get_descriptor(self) -> str:
         """
         Return the descriptor
 
         :rtype: string
         """
         proto = self.get_proto()
         return proto[0] + proto[1]
 
-    def get_real_descriptor(self):
+    def get_real_descriptor(self) -> str:
         """
         Return the real descriptor (i.e. without extra spaces)
 
         :rtype: string
         """
         proto = self.get_proto()
         return proto[0].replace(' ', '') + proto[1]
 
-    def get_name(self):
+    def get_name(self) -> str:
         """
         Return the name of the method
 
         :rtype: string
         """
         if self.name_idx_value is None:
             self.name_idx_value = self.CM.get_string(self.name_idx)
-
         return self.name_idx_value
 
-    def get_list(self):
+    def get_list(self) -> list[str]:
         return [self.get_class_name(), self.get_name(), self.get_proto()]
 
-    def get_triple(self):
+    def get_triple(self) -> tuple[str,str,str]:
         return self.get_class_name()[1:-1], self.get_name(
         ), self.get_real_descriptor()
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Method Id Item")
         bytecode._PrintDefault("class_idx=%d proto_idx=%d name_idx=%d\n" %
                                (self.class_idx, self.proto_idx, self.name_idx))
         bytecode._PrintDefault(
             "class_idx_value=%s proto_idx_value=%s name_idx_value=%s\n" %
             (self.class_idx_value, self.proto_idx_value, self.name_idx_value))
 
-    def get_obj(self):
+    def get_obj(self) -> bytes:
         return self.CM.packer["2HI"].pack(self.class_idx,
                     self.proto_idx,
                     self.name_idx)
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.get_obj()
 
-    def get_length(self):
+    def get_length(self) -> int:
         return len(self.get_obj())
 
 
 class MethodHIdItem:
     """
     This class can parse a list of method_id_item of a dex file
 
     :param buff: a string which represents a Buff object of the list of method_id_item
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, size, buff, cm):
+    def __init__(self, size:int, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
 
         self.offset = buff.tell()
 
         self.method_id_items = [MethodIdItem(buff, cm) for i in range(0, size)]
 
-    def set_off(self, off):
+    def set_off(self, off: int):
         self.offset = off
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def gets(self):
+    def gets(self) -> list[MethodIdItem]:
         return self.method_id_items
 
-    def get(self, idx):
+    def get(self, idx) -> Union[MethodIdItem,MethodIdItemInvalid]:
         try:
             return self.method_id_items[idx]
         except IndexError:
             return MethodIdItemInvalid()
 
-    def reload(self):
+    def reload(self) -> None:
         for i in self.method_id_items:
             i.reload()
 
-    def show(self):
+    def show(self) -> None:
         print("METHOD_ID_ITEM")
         nb = 0
         for i in self.method_id_items:
             print(nb, end=' ')
             i.show()
             nb = nb + 1
 
-    def get_obj(self):
+    def get_obj(self) -> list[MethodIdItem]:
         return [i for i in self.method_id_items]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return b''.join(i.get_raw() for i in self.method_id_items)
 
-    def get_length(self):
+    def get_length(self) -> int:
         length = 0
         for i in self.method_id_items:
             length += i.get_length()
         return length
 
 
 class ProtoIdItemInvalid:
-    def get_params(self):
+    def get_params(self) -> str:
         return "AG:IPI:invalid_params;"
 
-    def get_shorty(self):
+    def get_shorty(self) -> str:
         return "(AG:IPI:invalid_shorty)"
 
-    def get_return_type(self):
+    def get_return_type(self) -> str:
         return "(AG:IPI:invalid_return_type)"
 
-    def show(self):
+    def show(self) -> None:
         print("AG:IPI:invalid_proto_item", self.get_shorty(
         ), self.get_return_type(), self.get_params())
 
 
 class FieldIdItemInvalid:
-    def get_class_name(self):
+    def get_class_name(self) -> str:
         return "AG:IFI:invalid_class_name;"
 
-    def get_type(self):
+    def get_type(self) -> str:
         return "(AG:IFI:invalid_type)"
 
-    def get_descriptor(self):
+    def get_descriptor(self) -> str:
         return "(AG:IFI:invalid_descriptor)"
 
-    def get_name(self):
+    def get_name(self) -> str:
         return "AG:IFI:invalid_name"
 
-    def get_list(self):
+    def get_list(self) -> list[str]:
         return [self.get_class_name(), self.get_type(), self.get_name()]
 
-    def show(self):
+    def show(self) -> None:
         print("AG:IFI:invalid_field_item")
 
 
 class MethodIdItemInvalid:
-    def get_class_name(self):
+    def get_class_name(self) -> str:
         return "AG:IMI:invalid_class_name;"
 
-    def get_descriptor(self):
+    def get_descriptor(self) -> str:
         return "(AG:IMI:invalid_descriptor)"
 
-    def get_proto(self):
+    def get_proto(self) -> str:
         return "()AG:IMI:invalid_proto"
 
-    def get_name(self):
+    def get_name(self) -> str:
         return "AG:IMI:invalid_name"
 
-    def get_list(self):
+    def get_list(self) -> list[str]:
         return [self.get_class_name(), self.get_name(), self.get_proto()]
 
-    def show(self):
+    def show(self) -> None:
         print("AG:IMI:invalid_method_item")
 
 
 class EncodedField:
     """
     This class can parse an encoded_field of a dex file
 
     :param buff: a string which represents a Buff object of the encoded field
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
         self.offset = buff.tell()
 
         self.field_idx_diff = readuleb128(cm, buff)
         self.access_flags = readuleb128(cm, buff)
 
         self.field_idx = 0
@@ -2779,104 +2783,104 @@
         self.proto = None
         self.class_name = None
 
         self.init_value = None
         self.access_flags_string = None
         self.loaded = False
 
-    def load(self):
+    def load(self) -> None:
         if self.loaded:
             return
         self.reload()
         self.loaded = True
 
-    def reload(self):
+    def reload(self) -> None:
         name = self.CM.get_field(self.field_idx)
         self.class_name = name[0]
         self.name = name[2]
         self.proto = name[1]
 
-    def set_init_value(self, value):
+    def set_init_value(self, value: EncodedValue) -> None:
         """
         Setup the init value object of the field
 
         :param value: the init value
         :type value: :class:`EncodedValue`
         """
         self.init_value = value
 
-    def get_init_value(self):
+    def get_init_value(self) -> EncodedValue:
         """
         Return the init value object of the field
 
         :rtype: :class:`EncodedValue`
         """
         return self.init_value
 
-    def adjust_idx(self, val):
+    def adjust_idx(self, val: int) -> None:
         self.field_idx = self.field_idx_diff + val
 
-    def get_field_idx_diff(self):
+    def get_field_idx_diff(self) -> int:
         """
         Return the index into the field_ids list for the identity of this field (includes the name and descriptor),
         represented as a difference from the index of previous element in the list
 
         :rtype: int
         """
         return self.field_idx_diff
 
-    def get_field_idx(self):
+    def get_field_idx(self) -> int:
         """
         Return the real index of the method
 
         :rtype: int
         """
         return self.field_idx
 
-    def get_access_flags(self):
+    def get_access_flags(self) -> int:
         """
         Return the access flags of the field
 
         :rtype: int
         """
         return self.access_flags
 
-    def get_class_name(self):
+    def get_class_name(self) -> str:
         """
         Return the class name of the field
 
         :rtype: string
         """
         if not self.loaded:
             self.load()
         return self.class_name
 
-    def get_descriptor(self):
+    def get_descriptor(self) -> str:
         """
         Return the descriptor of the field
 
         The descriptor of a field is the type of the field.
 
         :rtype: string
         """
         if not self.loaded:
             self.load()
         return self.proto
 
-    def get_name(self):
+    def get_name(self) -> str:
         """
         Return the name of the field
 
         :rtype: string
         """
         if not self.loaded:
             self.load()
         return self.name
 
-    def get_access_flags_string(self):
+    def get_access_flags_string(self) -> str:
         """
         Return the access flags string of the field
 
         :rtype: string
         """
         if self.access_flags_string is None:
             if self.get_access_flags() == 0:
@@ -2888,29 +2892,29 @@
             self.access_flags_string = get_access_flags_string(self.get_access_flags())
 
             # Fallback for unknown strings
             if self.access_flags_string == "":
                 self.access_flags_string = "0x{:06x}".format(self.get_access_flags())
         return self.access_flags_string
 
-    def set_name(self, value):
+    def set_name(self, value: str) -> None:
         self.CM.set_hook_field_name(self, value)
         self.reload()
 
-    def get_obj(self):
+    def get_obj(self) -> list:
         return []
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return writeuleb128(self.CM, self.field_idx_diff) + writeuleb128(self.CM, 
             self.access_flags)
 
-    def get_size(self):
+    def get_size(self) -> bytes:
         return len(self.get_raw())
 
-    def show(self):
+    def show(self) -> None:
         """
         Display the information (with a pretty print) about the field
         """
         bytecode._PrintSubBanner("Field Information")
         bytecode._PrintDefault("{}->{} {} [access_flags={}]\n".format(
             self.get_class_name(), self.get_name(), self.get_descriptor(),
             self.get_access_flags_string()))
@@ -2932,15 +2936,15 @@
 
     :param buff: a string which represents a Buff object of the encoded_method
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
         self.offset = buff.tell()
 
         self.method_idx_diff = readuleb128(cm, buff)  #: method index diff in the corresponding section
         self.access_flags = readuleb128(cm, buff)  #: access flags of the method
         self.code_off = readuleb128(cm, buff)  #: offset of the code section
 
@@ -2953,61 +2957,61 @@
         self.code = None
 
         self.access_flags_string = None
 
         self.notes = []
         self.loaded = False
 
-    def adjust_idx(self, val):
+    def adjust_idx(self, val: int) -> None:
         self.method_idx = self.method_idx_diff + val
 
-    def get_method_idx(self):
+    def get_method_idx(self) -> int:
         """
         Return the real index of the method
 
         :rtype: int
         """
         return self.method_idx
 
-    def get_method_idx_diff(self):
+    def get_method_idx_diff(self) -> int:
         """
         Return index into the method_ids list for the identity of this method (includes the name and descriptor),
         represented as a difference from the index of previous element in the lis
 
         :rtype: int
         """
         return self.method_idx_diff
 
-    def get_access_flags(self):
+    def get_access_flags(self) -> int:
         """
         Return the access flags of the method
 
         :rtype: int
         """
         return self.access_flags
 
-    def get_code_off(self):
+    def get_code_off(self) -> int:
         """
         Return the offset from the start of the file to the code structure for this method,
         or 0 if this method is either abstract or native
 
         :rtype: int
         """
         return self.code_off
 
-    def get_address(self):
+    def get_address(self) -> int:
         """
         Return the offset from the start of the file to the code structure for this method,
         or 0 if this method is either abstract or native
 
         :rtype: int
         """
         return self.code_off + 0x10
 
-    def get_access_flags_string(self):
+    def get_access_flags_string(self) -> str:
         """
         Return the access flags string of the method
 
         A description of all access flags can be found here:
         https://source.android.com/devices/tech/dalvik/dex-format#access-flags
 
         :rtype: string
@@ -3015,21 +3019,21 @@
         if self.access_flags_string is None:
             self.access_flags_string = get_access_flags_string(self.get_access_flags())
 
             if self.access_flags_string == "" and self.get_access_flags() != 0x0:
                 self.access_flags_string = "0x%x" % self.get_access_flags()
         return self.access_flags_string
 
-    def load(self):
+    def load(self) -> None:
         if self.loaded:
             return
         self.reload()
         self.loaded = True
 
-    def reload(self):
+    def reload(self) -> None:
         v = self.CM.get_method(self.method_idx)
         # TODO this can probably be more elegant:
         # get_method returns an array with the already resolved types.
         # But for example to count the number of parameters, we need to split the string now.
         # This is quite tedious and could be avoided if we would return the type IDs
         # instead and resolve them here.
         if v and len(v) >= 3:
@@ -3039,29 +3043,29 @@
         else:
             self.class_name = 'CLASS_NAME_ERROR'
             self.name = 'NAME_ERROR'
             self.proto = 'PROTO_ERROR'
 
         self.code = self.CM.get_code(self.code_off)
 
-    def get_locals(self):
+    def get_locals(self) -> int:
         """
         Get the number of local registers used by the method
 
         This number is equal to the number of registers minus the number of parameters minus 1.
 
         :return: number of local registers
         :rtype: int
         """
         ret = self.proto.split(')')
         params = ret[0][1:].split()
 
         return self.code.get_registers_size() - len(params) - 1
 
-    def get_information(self):
+    def get_information(self) -> dict[str, Union[str,tuple[int,int],list]]:
         """
         Get brief information about the method's register use,
         parameters and return type.
 
         The resulting dictionary has the form:
 
         .. code-block:: none
@@ -3099,15 +3103,15 @@
                     info["params"].append((i, get_type(params[j])))
                     j += 1
             else:
                 info["registers"] = (0, nb - 1)
 
         return info
 
-    def each_params_by_register(self, nb, proto):
+    def each_params_by_register(self, nb: int, proto: str) -> None:
         """
         From the Dalvik Bytecode documentation:
 
         > The N arguments to a method land in the last N registers
         > of the method's invocation frame, in order.
         > Wide arguments consume two registers.
         > Instance methods are passed a this reference as their first argument.
@@ -3136,38 +3140,38 @@
 
     def __str__(self):
         return "{}->{}{} [access_flags={}] @ 0x{:x}".format(
             self.get_class_name(), self.get_name(), self.get_descriptor(),
             self.get_access_flags_string(), self.get_code_off())
 
     @property
-    def full_name(self):
+    def full_name(self) -> str:
         """Return class_name + name + descriptor, separated by spaces (no access flags"""
         return ' '.join([self.class_name, self.name, self.get_descriptor()])
 
     @property
-    def descriptor(self):
+    def descriptor(self) -> str:
         """Get the descriptor of the method"""
         return self.get_descriptor()
 
-    def get_short_string(self):
+    def get_short_string(self) -> str:
         """
         Return a shorter formatted String which encodes this method.
         The returned name has the form:
         <classname> <methodname> ([arguments ...])<returntype>
 
         * All Class names are condensed to the actual name (no package).
         * Access flags are not returned.
         * <init> and <clinit> are NOT replaced by the classname!
 
         This name might not be unique!
 
         :return: str
         """
-        def _fmt_classname(cls):
+        def _fmt_classname(cls) -> str:
             arr = ""
             # Test for arrays
             while cls.startswith("["):
                 arr += "["
                 cls = cls[1:]
 
             # is a object type
@@ -3181,24 +3185,24 @@
         clsname = _fmt_classname(str(self.get_class_name()))
 
         param, ret = str(self.get_descriptor())[1:].split(")")
         params = map(_fmt_classname, param.split(" "))
         desc = "({}){}".format(''.join(params), _fmt_classname(ret))
         return "{cls} {meth} {desc}".format(cls=clsname, meth=self.get_name(), desc=desc)
 
-    def show_info(self):
+    def show_info(self) -> None:
         """
         Display the basic information about the method
         """
         bytecode._PrintSubBanner("Method Information")
         bytecode._PrintDefault("{}->{}{} [access_flags={}]\n".format(
             self.get_class_name(), self.get_name(), self.get_descriptor(),
             self.get_access_flags_string()))
 
-    def show(self):
+    def show(self) -> None:
         """
         Display the information (with a pretty print) about the method
         """
         self.show_info()
         self.show_notes()
 
         if self.CM.get_analysis():
@@ -3206,73 +3210,73 @@
         else:
             if self.code:
                 self.each_params_by_register(self.code.get_registers_size(), self.get_descriptor())
                 self.code.show()
 
 
 
-    def show_notes(self):
+    def show_notes(self) -> None:
         """
         Display the notes about the method
         """
         if self.notes:
             bytecode._PrintSubBanner("Notes")
             for i in self.notes:
                 bytecode._PrintNote(i)
             bytecode._PrintSubBanner()
 
-    def source(self):
+    def source(self) -> str:
         """
         Return the source code of this method
 
         :rtype: string
         """
         self.CM.decompiler_ob.display_source(self)
 
-    def get_source(self):
+    def get_source(self) -> str:
         return self.CM.decompiler_ob.get_source_method(self)
 
-    def get_length(self):
+    def get_length(self) -> int:
         """
         Return the length of the associated code of the method
 
         :rtype: int
         """
         if self.code is not None:
             return self.code.get_length()
         return 0
 
-    def get_code(self):
+    def get_code(self) -> Union[DalvikCode,None]:
         """
         Return the code object associated to the method
 
 
         :rtype: :class:`DalvikCode` object or None if no Code
         """
         if not self.loaded:
             self.load()
         return self.code
 
-    def is_cached_instructions(self):
+    def is_cached_instructions(self) -> bool:
         if self.code is None:
             return False
 
         return self.code.get_bc().is_cached_instructions()
 
-    def get_instructions(self):
+    def get_instructions(self) -> Iterator[Instruction]:
         """
         Get the instructions
 
         :rtype: a generator of each :class:`Instruction` (or a cached list of instructions if you have setup instructions)
         """
         if self.get_code() is None:
             return []
         return self.get_code().get_bc().get_instructions()
 
-    def get_instructions_idx(self):
+    def get_instructions_idx(self) -> Iterator[tuple[int,Instruction]]:
         """
         Iterate over all instructions of the method, but also return the current index.
         This is the same as using :meth:`get_instructions` and adding the instruction length
         to a variable each time.
 
         :return:
         :rtype: Iterator[(int, Instruction)]
@@ -3280,51 +3284,51 @@
         if self.get_code() is None:
             return []
         idx = 0
         for ins in self.get_code().get_bc().get_instructions():
             yield idx, ins
             idx += ins.get_length()
 
-    def set_instructions(self, instructions):
+    def set_instructions(self, instructions: list[Instruction]) -> None:
         """
         Set the instructions
 
         :param instructions: the list of instructions
         :type instructions: a list of :class:`Instruction`
         """
         if self.code is None:
             return []
         return self.code.get_bc().set_instructions(instructions)
 
-    def get_instruction(self, idx, off=None):
+    def get_instruction(self, idx, off:Union[int,None]=None) -> Iterator[Instruction]:
         """
         Get a particular instruction by using (default) the index of the address if specified
 
         :param idx: index of the instruction (the position in the list of the instruction)
         :type idx: int
         :param off: address of the instruction
         :type off: int
 
         :rtype: an :class:`Instruction` object
         """
         if self.get_code() is not None:
             return self.get_code().get_bc().get_instruction(idx, off)
         return None
 
-    def get_debug(self):
+    def get_debug(self) -> DebugInfoItem:
         """
         Return the debug object associated to this method
 
         :rtype: :class:`DebugInfoItem`
         """
         if self.get_code() is None:
             return None
         return self.get_code().get_debug()
 
-    def get_descriptor(self):
+    def get_descriptor(self) -> str:
         """
         Return the descriptor of the method
         A method descriptor will have the form (A A A ...)R
         Where A are the arguments to the method and R is the return type.
         Basic types will have the short form, i.e. I for integer, V for void
         and class types will be named like a classname, e.g. Ljava/lang/String;.
 
@@ -3342,52 +3346,52 @@
 
         :rtype: string
         """
         if not self.loaded:
             self.load()
         return self.proto
 
-    def get_class_name(self):
+    def get_class_name(self) -> str:
         """
         Return the class name of the method
 
         :rtype: string
         """
         if not self.loaded:
             self.load()
         return self.class_name
 
-    def get_name(self):
+    def get_name(self) -> str:
         """
         Return the name of the method
 
         :rtype: string
         """
         if not self.loaded:
             self.load()
         return self.name
 
-    def get_triple(self):
+    def get_triple(self) -> tuple[str,str,str]:
         return self.CM.get_method_ref(self.method_idx).get_triple()
 
-    def add_inote(self, msg, idx, off=None):
+    def add_inote(self, msg:str, idx:int, off:Union[int,None]=None) -> None:
         """
         Add a message to a specific instruction by using (default) the index of the address if specified
 
         :param msg: the message
         :type msg: string
         :param idx: index of the instruction (the position in the list of the instruction)
         :type idx: int
         :param off: address of the instruction
         :type off: int
         """
         if self.code is not None:
             self.code.add_inote(msg, idx, off)
 
-    def add_note(self, msg):
+    def add_note(self, msg:str) -> None:
         """
         Add a message to this method
 
         :param msg: the message
         :type msg: string
         """
         self.notes.append(msg)
@@ -3423,15 +3427,15 @@
 
     :param buff: a string which represents a Buff object of the class_data_item
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
 
         self.offset = buff.tell()
 
         self.static_fields_size = readuleb128(cm, buff)
         self.instance_fields_size = readuleb128(cm, buff)
         self.direct_methods_size = readuleb128(cm, buff)
@@ -3532,15 +3536,15 @@
         Return static and instance fields
 
         :rtype: a list of :class:`EncodedField` objects
         """
         return [x for x in self.static_fields] + [x
                                                   for x in self.instance_fields]
 
-    def set_off(self, off):
+    def set_off(self, off:int):
         self.offset = off
 
     def set_static_fields(self, value):
         if value is not None:
             values = value.get_values()
             if len(values) <= len(self.static_fields):
                 for i in range(0, len(values)):
@@ -3629,15 +3633,15 @@
 
     :param buff: a string which represents a Buff object of the class_def_item
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
         self.offset = buff.tell()
 
         self.class_idx, \
         self.access_flags, \
         self.superclass_idx, \
         self.interfaces_off, \
@@ -3653,15 +3657,15 @@
 
         self.name = None
         self.sname = None
         self.access_flags_string = None
 
         self.reload()
 
-    def reload(self):
+    def reload(self) -> None:
         self.name = self.CM.get_type(self.class_idx)
         self.sname = self.CM.get_type(self.superclass_idx)
         self.interfaces = self.CM.get_type_list(self.interfaces_off)
 
         if self.class_data_off != 0:
             self.class_data_item = self.CM.get_class_data_item(self.class_data_off)
 
@@ -3676,205 +3680,205 @@
 
     def __str__(self):
         return "{}->{}".format(self.get_superclassname(), self.get_name())
 
     def __repr__(self):
         return "<dvm.ClassDefItem {}>".format(self.__str__())
 
-    def get_methods(self):
+    def get_methods(self) -> list[EncodedMethod]:
         """
         Return all EncodedMethods of this class
 
         :rtype: a list of :class:`EncodedMethod` objects
         """
         if self.class_data_item is not None:
             return self.class_data_item.get_methods()
         return []
 
-    def get_fields(self):
+    def get_fields(self) -> list[EncodedField]:
         """
         Return all EncodedFields of this class
 
         :rtype: a list of :class:`EncodedField` objects
         """
         if self.class_data_item is not None:
             return self.class_data_item.get_fields()
         return []
 
-    def _get_annotation_type_ids(self):
+    def _get_annotation_type_ids(self) -> list[EncodedAnnotation]:
         """
         Get the EncodedAnnotations from this class
 
-        :rtype: Iterator[EncodedAnnotation]
+        :rtype: list[EncodedAnnotation]
         """
         if self.annotations_directory_item is None:
             return []
         annotation_set_item = self.annotations_directory_item.get_annotation_set_item()
         if annotation_set_item is None:
             return []
         
         annotation_off_item = annotation_set_item.get_annotation_off_item()
 
         if annotation_off_item is None:
             return []
         
         return [annotation.get_annotation_item().annotation for annotation in annotation_off_item]
 
-    def get_annotations(self):
+    def get_annotations(self) -> list[str]:
         """
         Returns the class names of the annotations of this class.
 
         For example, if the class is marked as :code:`@Deprecated`, this will return
         :code:`['Ljava/lang/Deprecated;']`.
 
-        :rtype: Iterator[str]
+        :rtype: list[str]
         """
         return [self.CM.get_type(x.get_type_idx()) for x in self._get_annotation_type_ids()]
 
-    def get_class_idx(self):
+    def get_class_idx(self) -> int:
         """
         Return the index into the type_ids list for this class
 
         :rtype: int
         """
         return self.class_idx
 
-    def get_access_flags(self):
+    def get_access_flags(self) -> int:
         """
         Return the access flags for the class (public, final, etc.)
 
         :rtype: int
         """
         return self.access_flags
 
-    def get_superclass_idx(self):
+    def get_superclass_idx(self) -> int:
         """
         Return the index into the type_ids list for the superclass
 
         :rtype: int
         """
         return self.superclass_idx
 
-    def get_interfaces_off(self):
+    def get_interfaces_off(self) -> int:
         """
         Return the offset from the start of the file to the list of interfaces, or 0 if there are none
 
         :rtype: int
         """
         return self.interfaces_off
 
-    def get_source_file_idx(self):
+    def get_source_file_idx(self) -> int:
         """
         Return the index into the string_ids list for the name of the file containing the original
         source for (at least most of) this class, or the special value NO_INDEX to represent a lack of this information
 
         :rtype: int
         """
         return self.source_file_idx
 
-    def get_annotations_off(self):
+    def get_annotations_off(self) -> int:
         """
         Return the offset from the start of the file to the annotations structure for this class,
         or 0 if there are no annotations on this class.
 
         :rtype: int
         """
         return self.annotations_off
 
-    def get_class_data_off(self):
+    def get_class_data_off(self) -> int:
         """
         Return the offset from the start of the file to the associated class data for this item,
         or 0 if there is no class data for this class
 
         :rtype: int
         """
         return self.class_data_off
 
-    def get_static_values_off(self):
+    def get_static_values_off(self) -> int:
         """
         Return the offset from the start of the file to the list of initial values for static fields,
         or 0 if there are none (and all static fields are to be initialized with 0 or null)
 
         :rtype: int
         """
         return self.static_values_off
 
-    def get_class_data(self):
+    def get_class_data(self) -> ClassDataItem:
         """
         Return the associated class_data_item
 
         :rtype: a :class:`ClassDataItem` object
         """
         return self.class_data_item
 
-    def get_name(self):
+    def get_name(self) -> str:
         """
         Return the name of this class
 
         :rtype: str
         """
         return self.name
 
-    def get_superclassname(self):
+    def get_superclassname(self) -> str:
         """
         Return the name of the super class
 
         :rtype: str
         """
         return self.sname
 
-    def get_interfaces(self):
+    def get_interfaces(self) -> list[str]:
         """
         Return the names of the interfaces
 
         :rtype: List[str]
         """
         return self.interfaces
 
-    def get_access_flags_string(self):
+    def get_access_flags_string(self) -> str:
         """
         Return the access flags string of the class
 
         :rtype: str
         """
         if self.access_flags_string is None:
             self.access_flags_string = get_access_flags_string(
                 self.get_access_flags())
 
             if self.access_flags_string == "":
                 self.access_flags_string = "0x%x" % self.get_access_flags()
         return self.access_flags_string
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Class Def Item")
         bytecode._PrintDefault(
             "name=%s, sname=%s, interfaces=%s, access_flags=%s\n" %
             (self.name, self.sname, self.interfaces,
              self.get_access_flags_string()))
         bytecode._PrintDefault(
             "class_idx=%d, superclass_idx=%d, interfaces_off=%x, source_file_idx=%d, annotations_off=%x, class_data_off=%x, static_values_off=%x\n"
             % (self.class_idx, self.superclass_idx, self.interfaces_off,
                self.source_file_idx, self.annotations_off, self.class_data_off,
                self.static_values_off))
 
         for method in self.get_methods():
             method.show()
 
-    def source(self):
+    def source(self) -> None:
         """
-        Return the source code of the entire class
+        Print the source code of the entire class
 
         :rtype: string
         """
         self.CM.decompiler_ob.display_all(self)
 
-    def get_source(self):
+    def get_source(self) -> str:
         return self.CM.decompiler_ob.get_source_class(self)
 
-    def get_source_ext(self):
+    def get_source_ext(self) -> list[tuple[str, list]]:
         return self.CM.decompiler_ob.get_source_class_ext(self)
 
     def get_ast(self):
         return self.CM.decompiler_ob.get_ast_class(self)
 
     def set_name(self, value):
         self.CM.set_hook_class_name(self, value)
@@ -3918,66 +3922,65 @@
 
     :param buff: a string which represents a Buff object of the list of class_def_item
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, size, buff, cm):
+    def __init__(self, size:int, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
 
         self.offset = buff.tell()
 
         self.class_def = []
 
         for i in range(0, size):
             idx = buff.tell()
 
             class_def = ClassDefItem(buff, cm)
             self.class_def.append(class_def)
 
             buff.seek(idx + calcsize("8I"))
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def get_class_idx(self, idx):
+    def get_class_idx(self, idx: int) -> ClassDefItem:
         for i in self.class_def:
             if i.get_class_idx() == idx:
                 return i
         return None
 
-    def get_method(self, name_class, name_method):
+    def get_method(self, name_class: str, name_method: str) -> list[EncodedMethod]:
         l = []
 
         for i in self.class_def:
             if i.get_name() == name_class:
                 for j in i.get_methods():
                     if j.get_name() == name_method:
                         l.append(j)
-
         return l
 
-    def get_names(self):
+    def get_names(self) -> list[str]:
         return [x.get_name() for x in self.class_def]
 
-    def show(self):
+    def show(self) -> None:
         for i in self.class_def:
             i.show()
 
-    def get_obj(self):
+    def get_obj(self) -> list[ClassDefItem]:
         return [i for i in self.class_def]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return b''.join(i.get_raw() for i in self.class_def)
 
-    def get_length(self):
+    def get_length(self) -> int:
         length = 0
         for i in self.class_def:
             length += i.get_length()
         return length
 
 
 class EncodedTypeAddrPair:
@@ -3986,129 +3989,129 @@
 
     :param buff: a string which represents a Buff object of the encoded_type_addr_pair
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: BinaryIO) -> None:
         self.CM = cm
         self.type_idx = readuleb128(cm, buff)
         self.addr = readuleb128(cm, buff)
 
-    def get_type_idx(self):
+    def get_type_idx(self) -> int:
         """
         Return the index into the type_ids list for the type of the exception to catch
 
         :rtype: int
         """
         return self.type_idx
 
-    def get_addr(self):
+    def get_addr(self) -> int:
         """
         Return the bytecode address of the associated exception handler
 
         :rtype: int
         """
         return self.addr
 
-    def get_obj(self):
+    def get_obj(self) -> list:
         return []
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Encoded Type Addr Pair")
         bytecode._PrintDefault("type_idx=%d addr=%x\n" %
                                (self.type_idx, self.addr))
 
-    def get_raw(self):
+    def get_raw(self) -> bytearray:
         return writeuleb128(self.CM, self.type_idx) + writeuleb128(self.CM, self.addr)
 
-    def get_length(self):
+    def get_length(self) -> int:
         return len(self.get_raw())
 
 
 class EncodedCatchHandler:
     """
     This class can parse an encoded_catch_handler of a dex file
 
     :param buff: a string which represents a Buff object of the encoded_catch_handler
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
         self.offset = buff.tell()
 
         self.size = readsleb128(cm, buff)
 
         self.handlers = []
 
         for i in range(0, abs(self.size)):
             self.handlers.append(EncodedTypeAddrPair(cm, buff))
 
         if self.size <= 0:
             self.catch_all_addr = readuleb128(cm, buff)
 
-    def get_size(self):
+    def get_size(self) -> int:
         """
         Return the number of catch types in this list
 
         :rtype: int
         """
         return self.size
 
-    def get_handlers(self):
+    def get_handlers(self) -> list[EncodedTypeAddrPair]:
         """
         Return the stream of abs(size) encoded items, one for each caught type, in the order that the types should be tested.
 
         :rtype: a list of :class:`EncodedTypeAddrPair` objects
         """
         return self.handlers
 
-    def get_catch_all_addr(self):
+    def get_catch_all_addr(self) -> int:
         """
         Return the bytecode address of the catch-all handler. This element is only present if size is non-positive.
 
         :rtype: int
         """
         return self.catch_all_addr
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Encoded Catch Handler")
         bytecode._PrintDefault("size=%d\n" % self.size)
 
         for i in self.handlers:
             i.show()
 
         if self.size <= 0:
             bytecode._PrintDefault("catch_all_addr=%x\n" % self.catch_all_addr)
 
-    def get_raw(self):
+    def get_raw(self) -> bytearray:
         """
         :rtype: bytearray
         """
         buff = bytearray()
         buff += writesleb128(self.CM, self.size)
         for i in self.handlers:
             buff += i.get_raw()
 
         if self.size <= 0:
             buff += writeuleb128(self.CM, self.catch_all_addr)
 
         return buff
 
-    def get_length(self):
+    def get_length(self) -> int:
         length = len(writesleb128(self.CM, self.size))
 
         for i in self.handlers:
             length += i.get_length()
 
         if self.size <= 0:
             length += len(writeuleb128(self.CM, self.catch_all_addr))
@@ -4122,72 +4125,72 @@
 
     :param buff: a string which represents a Buff object of the encoded_catch_handler_list
     :type buff: Buff object
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
         self.offset = buff.tell()
 
         self.size = readuleb128(cm, buff)
         self.list = [EncodedCatchHandler(buff, cm) for _ in range(self.size)]
 
-    def get_size(self):
+    def get_size(self) -> int:
         """
         Return the size of this list, in entries
 
         :rtype: int
         """
         return self.size
 
-    def get_list(self):
+    def get_list(self) -> list[EncodedCatchHandler]:
         """
         Return the actual list of handler lists, represented directly (not as offsets), and concatenated sequentially
 
         :rtype: a list of :class:`EncodedCatchHandler` objects
         """
         return self.list
 
-    def show(self):
+    def show(self) -> None:
         bytecode._PrintSubBanner("Encoded Catch Handler List")
         bytecode._PrintDefault("size=%d\n" % self.size)
 
         for i in self.list:
             i.show()
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def get_obj(self):
+    def get_obj(self) -> bytearray:
         return writeuleb128(self.CM, self.size)
 
-    def get_raw(self):
+    def get_raw(self) -> bytearray:
         """
         :rtype: bytearray
         """
         buff = bytearray()
         buff += self.get_obj()
         for i in self.list:
             buff += i.get_raw()
         return buff
 
-    def get_length(self):
+    def get_length(self) -> int:
         length = len(self.get_obj())
 
         for i in self.list:
             length += i.get_length()
         return length
 
 
-def get_kind(cm, kind, value):
+def get_kind(cm:ClassManager, kind: int, value: int) -> str:
     """
     Return the value of the 'kind' argument
 
     :param cm: a ClassManager object
     :type cm: :class:`ClassManager`
     :param kind: the type of the 'kind' argument
     :type kind: int
@@ -4267,97 +4270,97 @@
     For the sign-extension, nothing is really done here, as it only affects the bit represenation
     in the virtual machine. As androguard parses the values and uses python types internally,
     we are not bound to specific size.
     """
     length = 0
     OP = 0
 
-    def get_kind(self):
+    def get_kind(self) -> int:
         """
         Return the 'kind' argument of the instruction
 
         This is the type of the argument, i.e. in which kind of table you have
         to look up the argument in the ClassManager
 
         :rtype: int
         """
         if self.OP >= 0xf2ff:
             return DALVIK_OPCODES_OPTIMIZED[self.OP][1][1]
         return DALVIK_OPCODES_FORMAT[self.OP][1][1]
 
-    def get_name(self):
+    def get_name(self) -> str:
         """
         Return the mnemonic of the instruction
 
         :rtype: string
         """
         if self.OP >= 0xf2ff:
             return DALVIK_OPCODES_OPTIMIZED[self.OP][1][0]
         return DALVIK_OPCODES_FORMAT[self.OP][1][0]
 
-    def get_op_value(self):
+    def get_op_value(self) -> int:
         """
         Return the numerical value of the opcode
 
         :rtype: int
         """
         return self.OP
 
-    def get_literals(self):
+    def get_literals(self) -> list:
         """
         Return the associated literals
 
         :rtype: list of int
         """
         return []
 
-    def show(self, idx):
+    def show(self, idx: int) -> None:
         """
         Print the instruction
 
         No Line ending is printed.
         """
         print(self.get_name() + " " + self.get_output(idx), end=' ')
 
-    def show_buff(self, idx):
+    def show_buff(self, idx:int) -> str:
         """
         Return the display of the instruction
 
         :rtype: string
         """
         return self.get_output(idx)
 
-    def get_translated_kind(self):
+    def get_translated_kind(self) -> str:
         """
         Return the translated value of the 'kind' argument
 
         :rtype: string
         """
         return get_kind(self.cm, self.get_kind(), self.get_ref_kind())
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         """
         Return an additional output of the instruction
 
         :rtype: string
         """
         return ""
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list:
         """
         Return all operands
 
         This will return a list of tuples, containing the Enum :class:`Operand`
         at the first position and the objects afterwards.
 
         :rtype: List[Tuple(Operand, object, ...)]
         """
         return []
 
-    def get_length(self):
+    def get_length(self) -> int:
         """
         Return the length of the instruction in bytes
 
         :rtype: int
         """
         return self.length
 
@@ -4373,15 +4376,15 @@
         """
         Return the value of the 'kind' argument
 
         :rtype: value
         """
         raise Exception("not implemented")
 
-    def get_hex(self):
+    def get_hex(self) -> str:
         """
         Returns a HEX String, separated by spaces every byte
 
         The hex string contains the raw bytes of the instruction,
         including the opcode and all arguments.
 
         :rtype: str
@@ -4389,30 +4392,30 @@
         s = binascii.hexlify(self.get_raw()).decode('ascii')
         return " ".join(s[i:i + 2] for i in range(0, len(s), 2))
 
     def __str__(self):
         return "{} {}".format(self.get_name(), self.get_output())
 
     # FIXME Better name
-    def disasm(self):
+    def disasm(self) -> str:
         """Some small line for disassembly view"""
         s = binascii.hexlify(self.get_raw()).decode('ascii')
         byteview = " ".join(s[i:i + 4] for i in range(0, len(s), 4))
         return '{:24s}  {:24s} {}'.format(byteview, self.get_name(), self.get_output())
 
 
 class FillArrayData:
     """
     This class can parse a FillArrayData instruction
 
     :param buff: a Buff object which represents a buffer where the instruction is stored
     """
 
     # FIXME: why is this not a subclass of Instruction?
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: BinaryIO) -> None:
         self.OP = 0x0
         self.notes = []
         self.CM = cm
 
         self.format_general_size = calcsize("2HI")
         self.ident, \
         self.element_width, \
@@ -4420,48 +4423,48 @@
 
         buf_len = self.size * self.element_width
         if buf_len % 2:
             buf_len += 1
 
         self.data = buff[self.format_general_size:self.format_general_size + buf_len]
 
-    def add_note(self, msg):
+    def add_note(self, msg: str) -> None:
         """
         Add a note to this instruction
 
         :param msg: the message
-        :type msg: objects (string)
+        :type msg: string
         """
         self.notes.append(msg)
 
-    def get_notes(self):
+    def get_notes(self) -> list[str]:
         """
         Get all notes from this instruction
 
-        :rtype: a list of objects
+        :rtype: a list of string notes
         """
         return self.notes
 
-    def get_op_value(self):
+    def get_op_value(self) -> int:
         """
         Get the value of the opcode
 
         :rtype: int
         """
         return self.ident
 
-    def get_data(self):
+    def get_data(self) -> bytes:
         """
         Return the data of this instruction (the payload)
 
         :rtype: bytes
         """
         return self.data
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         """
         Return an additional output of the instruction
 
         :rtype: string
         """
         buff = ""
 
@@ -4469,83 +4472,83 @@
 
         buff += repr(data) + " | "
         for i in range(0, len(data)):
             buff += "\\x{:02x}".format(data[i])
 
         return buff
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx: int=-1) -> tuple[Operand, str]:
         # FIXME: not sure of binascii is the right choise here,
         # but before it was repr(), which lead to weird outputs of bytearrays
         if isinstance(self.get_data(), bytearray):
             return [(Operand.RAW, binascii.hexlify(self.get_data()).decode('ascii'))]
         else:
             return [(Operand.RAW, repr(self.get_data()))]
 
-    def get_formatted_operands(self):
+    def get_formatted_operands(self) -> None:
         return None
 
-    def get_name(self):
+    def get_name(self) -> str:
         """
         Return the name of the instruction
 
         :rtype: string
         """
         return "fill-array-data-payload"
 
-    def show_buff(self, pos):
+    def show_buff(self, pos:int) -> str:
         """
         Return the display of the instruction
 
         :rtype: string
         """
         buff = self.get_name() + " "
 
         for i in range(0, len(self.data)):
             buff += "\\x%02x" % self.data[i]
         return buff
 
-    def show(self, pos):
+    def show(self, pos) -> None:
         """
         Print the instruction
         """
         print(self.show_buff(pos), end=' ')
 
-    def get_length(self):
+    def get_length(self) -> int:
         """
         Return the length of the instruction
 
         :rtype: int
         """
         return ((self.size * self.element_width + 1) // 2 + 4) * 2
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.CM.packer["2HI"].pack(self.ident, self.element_width, self.size) + self.data
 
-    def get_hex(self):
+    def get_hex(self) -> str:
         """
         Returns a HEX String, separated by spaces every byte
         """
         s = binascii.hexlify(self.get_raw()).decode("ascii")
         return " ".join(s[i:i + 2] for i in range(0, len(s), 2))
 
-    def disasm(self):
+    def disasm(self) -> str:
         # FIXME:
         return self.show_buff(None)
 
 
 class SparseSwitch:
     """
     This class can parse a SparseSwitch instruction
 
     :param buff: a Buff object which represents a buffer where the instruction is stored
     """
 
     # FIXME: why is this not a subclass of Instruction?
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         self.OP = 0x0
         self.notes = []
         self.CM = cm
 
         self.format_general_size = calcsize("2H")
         self.ident, \
         self.size = cm.packer["2H"].unpack(buff[0:4])
@@ -4558,130 +4561,130 @@
             self.keys.append(cm.packer["l"].unpack(buff[idx:idx + 4])[0])
             idx += 4
 
         for i in range(0, self.size):
             self.targets.append(cm.packer["l"].unpack(buff[idx:idx + 4])[0])
             idx += 4
 
-    def add_note(self, msg):
+    def add_note(self, msg:str) -> None:
         """
         Add a note to this instruction
 
         :param msg: the message
-        :type msg: objects (string)
+        :type msg: string
         """
         self.notes.append(msg)
 
-    def get_notes(self):
+    def get_notes(self) -> list[str]:
         """
         Get all notes from this instruction
 
         :rtype: a list of objects
         """
         return self.notes
 
-    def get_op_value(self):
+    def get_op_value(self) -> int:
         """
         Get the value of the opcode
 
         :rtype: int
         """
         return self.ident
 
-    def get_keys(self):
+    def get_keys(self) -> list[int]:
         """
         Return the keys of the instruction
 
-        :rtype: a list of long
+        :rtype: a list of long (integer)
         """
         return self.keys
 
-    def get_values(self):
+    def get_values(self) -> list[int]:
         return self.get_keys()
 
-    def get_targets(self):
+    def get_targets(self) -> list[int]:
         """
         Return the targets (address) of the instruction
 
-        :rtype: a list of long
+        :rtype: a list of long (integer)
         """
         return self.targets
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         """
         Return an additional output of the instruction
 
         :rtype: string
         """
         return " ".join("%x" % i for i in self.keys)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> str:
         """
         Return an additional output of the instruction
 
         :rtype: string
         """
         return []
 
-    def get_formatted_operands(self):
+    def get_formatted_operands(self) -> None:
         return None
 
-    def get_name(self):
+    def get_name(self) -> str:
         """
         Return the name of the instruction
 
         :rtype: string
         """
         return "sparse-switch-payload"
 
-    def show_buff(self, pos):
+    def show_buff(self, pos:int) -> str:
         """
         Return the display of the instruction
 
         :rtype: string
         """
         buff = self.get_name() + " "
         for i in range(0, len(self.keys)):
             buff += "{:x}:{:x} ".format(self.keys[i], self.targets[i])
 
         return buff
 
-    def show(self, pos):
+    def show(self, pos) -> None:
         """
         Print the instruction
         """
         print(self.show_buff(pos), end=' ')
 
-    def get_length(self):
+    def get_length(self) -> int:
         return self.format_general_size + (self.size * calcsize('<L')) * 2
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.CM.packer["2H"].pack(self.ident, self.size) + b''.join(self.CM.packer["l"].pack(i) for i in self.keys) + b''.join(self.CM.packer["l"].pack(i) for i in self.targets)
 
-    def get_hex(self):
+    def get_hex(self) -> str:
         """
         Returns a HEX String, separated by spaces every byte
         """
         s = binascii.hexlify(self.get_raw()).decode('ascii')
         return " ".join(s[i:i + 2] for i in range(0, len(s), 2))
 
-    def disasm(self):
+    def disasm(self) -> str:
         # FIXME:
         return self.show_buff(None)
 
 
 class PackedSwitch:
     """
     This class can parse a PackedSwitch instruction
 
     :param buff: a Buff object which represents a buffer where the instruction is stored
     """
 
     # FIXME: why is this not a subclass of Instruction?
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         self.OP = 0x0
         self.notes = []
         self.CM = cm
 
         self.format_general_size = calcsize("2HI")
 
         self.ident, \
@@ -4696,146 +4699,146 @@
         if (max_size * 4) > len(buff):
             max_size = len(buff) - idx - 8
 
         for i in range(0, max_size):
             self.targets.append(cm.packer["l"].unpack(buff[idx:idx + 4])[0])
             idx += 4
 
-    def add_note(self, msg):
+    def add_note(self, msg: str) -> None:
         """
         Add a note to this instruction
 
         :param msg: the message
-        :type msg: objects (string)
+        :type msg: string
         """
         self.notes.append(msg)
 
-    def get_notes(self):
+    def get_notes(self) -> list[str]:
         """
         Get all notes from this instruction
 
         :rtype: a list of objects
         """
         return self.notes
 
-    def get_op_value(self):
+    def get_op_value(self) -> int:
         """
         Get the value of the opcode
 
         :rtype: int
         """
         return self.ident
 
-    def get_keys(self):
+    def get_keys(self) -> list[int]:
         """
         Return the keys of the instruction
 
-        :rtype: a list of long
+        :rtype: a list of long (integer)
         """
         return [(self.first_key + i) for i in range(0, len(self.targets))]
 
-    def get_values(self):
+    def get_values(self) -> list[int]:
         return self.get_keys()
 
-    def get_targets(self):
+    def get_targets(self) -> list[int]:
         """
         Return the targets (address) of the instruction
 
-        :rtype: a list of long
+        :rtype: a list of long (integer)
         """
         return self.targets
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         """
       Return an additional output of the instruction
 
         :rtype: string
 
         """
         return " ".join("%x" % (self.first_key + i)
                         for i in range(0, len(self.targets)))
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list:
         """
         Return an additional output of the instruction
 
-        :rtype: string
+        :rtype: list
         """
         return []
 
-    def get_formatted_operands(self):
+    def get_formatted_operands(self) -> None:
         return None
 
-    def get_name(self):
+    def get_name(self) -> str:
         """
         Return the name of the instruction
 
         :rtype: string
         """
         return "packed-switch-payload"
 
-    def show_buff(self, pos):
+    def show_buff(self, pos:int) -> str:
         """
         Return the display of the instruction
 
         :rtype: string
         """
         buff = self.get_name() + " "
         buff += "%x:" % self.first_key
 
         for i in self.targets:
             buff += " %x" % i
 
         return buff
 
-    def show(self, pos):
+    def show(self, pos: int) -> None:
         """
         Print the instruction
         """
         print(self.show_buff(pos), end=' ')
 
-    def get_length(self):
+    def get_length(self) -> int:
         return self.format_general_size + (self.size * calcsize('<L'))
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.CM.packer["2Hi"].pack(self.ident, self.size, self.first_key) + b''.join(self.CM.packer["l"].pack(i) for i in self.targets)
 
-    def get_hex(self):
+    def get_hex(self) -> bytes:
         """
         Returns a HEX String, separated by spaces every byte
         """
         s = binascii.hexlify(self.get_raw()).decode('ascii')
         return " ".join(s[i:i + 2] for i in range(0, len(s), 2))
 
-    def disasm(self):
+    def disasm(self) -> str:
         # FIXME:
         return self.show_buff(None)
 
 
 class Instruction35c(Instruction):
     """
     This class represents all instructions which have the 35c format
     """
     length = 6
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         i16a, self.BBBB, i16b = cm.packer["3H"].unpack(buff[:self.length])
         self.OP = i16a & 0xff
         self.G = (i16a >> 8) & 0xf
         self.A = (i16a >> 12) & 0xf
 
         self.C = i16b & 0xf
         self.D = (i16b >> 4) & 0xf
         self.E = (i16b >> 8) & 0xf
         self.F = (i16b >> 12) & 0xf
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         kind = get_kind(self.cm, self.get_kind(), self.BBBB)
 
         if self.A == 0:
             return "%s" % kind
         elif self.A == 1:
             return "v%d, %s" % (self.C, kind)
         elif self.A == 2:
@@ -4847,15 +4850,15 @@
                                                kind)
         elif self.A == 5:
             return "v%d, v%d, v%d, v%d, v%d, %s" % (self.C, self.D, self.E,
                                                     self.F, self.G, kind)
 
         return ''
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple]:
         l = []
         kind = get_kind(self.cm, self.get_kind(), self.BBBB)
 
         if self.A == 0:
             l.append((self.get_kind() + Operand.KIND, self.BBBB, kind))
         elif self.A == 1:
             l.extend([(Operand.REGISTER, self.C), (self.get_kind(
@@ -4875,48 +4878,48 @@
             l.extend([(Operand.REGISTER, self.C), (Operand.REGISTER, self.D), (
                 Operand.REGISTER, self.E), (Operand.REGISTER, self.F), (
                           Operand.REGISTER, self.G), (self.get_kind() + Operand.KIND,
                                                       self.BBBB, kind)])
 
         return l
 
-    def get_ref_kind(self):
+    def get_ref_kind(self) -> int:
         return self.BBBB
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["3H"].pack((self.A << 12) | (self.G << 8) | self.OP, self.BBBB,
                     (self.F << 12) | (self.E << 8) | (self.D << 4) | self.C)
 
 
 class Instruction10x(Instruction):
     """
     This class represents all instructions which have the 10x format
     """
 
     length = 2
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, padding = cm.packer["BB"].unpack(buff[:self.length])
         if padding != 0:
             raise InvalidInstruction('High byte of opcode with format 10x must be zero!')
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["H"].pack(self.OP)
 
 
 class Instruction21h(Instruction):
     """
     This class represents all instructions which have the 21h format
     """
     length = 4
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm:ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, self.AA, self.__BBBB = cm.packer["BBh"].unpack(buff[:self.length])
 
         if self.OP == 0x15:
             # OP 0x15: int16_t -> int32_t
@@ -4924,702 +4927,702 @@
         elif self.OP == 0x19:
             # OP 0x19: int16_t -> int64_t
             self.BBBB = self.__BBBB << 48
         else:
             # Unknown opcode?
             self.BBBB = self.__BBBB
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         return "v{}, {}".format(self.AA, self.BBBB)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.REGISTER, self.AA), (Operand.LITERAL, self.BBBB)]
 
-    def get_literals(self):
+    def get_literals(self) -> list[int]:
         return [self.BBBB]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["Hh"].pack((self.AA << 8) | self.OP, self.__BBBB)
 
 
 class Instruction11n(Instruction):
     """
     This class represents all instructions which have the 11n format
     """
     length = 2
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, i8 = cm.packer["Bb"].unpack(buff[:self.length])
         self.A = i8 & 0xf
         # Sign extension not required
         self.B = i8 >> 4
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         return "v{}, {}".format(self.A, self.B)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.REGISTER, self.A), (Operand.LITERAL, self.B)]
 
-    def get_literals(self):
+    def get_literals(self) -> list[int]:
         return [self.B]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["h"].pack((self.B << 12) | (self.A << 8) | self.OP)
 
 
 class Instruction21c(Instruction):
     """
     This class represents all instructions which have the 21c format
     """
 
     length = 4
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
         self.OP, self.AA, self.BBBB = cm.packer["BBH"].unpack(buff[:self.length])
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         kind = get_kind(self.cm, self.get_kind(), self.BBBB)
         if self.get_kind() == Kind.STRING:
             kind = '"{}"'.format(kind)
         return "v{}, {}".format(self.AA, kind)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int, int]]:
         kind = get_kind(self.cm, self.get_kind(), self.BBBB)
         return [(Operand.REGISTER, self.AA),
                 (self.get_kind() + Operand.KIND, self.BBBB, kind)]
 
-    def get_ref_kind(self):
+    def get_ref_kind(self) -> int:
         return self.BBBB
 
-    def get_string(self):
+    def get_string(self) -> str:
         return get_kind(self.cm, self.get_kind(), self.BBBB)
 
-    def get_raw_string(self):
+    def get_raw_string(self) -> str:
         return get_kind(self.cm, Kind.RAW_STRING, self.BBBB)
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["2H"].pack((self.AA << 8) | self.OP, self.BBBB)
 
 
 class Instruction21s(Instruction):
     """
     This class represents all instructions which have the 21s format
     """
 
     length = 4
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> bytes:
         super().__init__()
         self.cm = cm
 
         # BBBB is a signed int (16bit)
         self.OP, self.AA, self.BBBB = self.cm.packer["BBh"].unpack(buff[:self.length])
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         return "v{}, {}".format(self.AA, self.BBBB)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.REGISTER, self.AA), (Operand.LITERAL, self.BBBB)]
 
-    def get_literals(self):
+    def get_literals(self) -> list[int]:
         return [self.BBBB]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["BBh"].pack(self.OP, self.AA, self.BBBB)
 
 
 class Instruction22c(Instruction):
     """
     This class represents all instructions which have the 22c format
     """
 
     length = 4
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         i16, self.CCCC = cm.packer["2H"].unpack(buff[:self.length])
         self.OP = i16 & 0xff
         self.A = (i16 >> 8) & 0xf
         self.B = (i16 >> 12) & 0xf
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1):
         kind = get_kind(self.cm, self.get_kind(), self.CCCC)
         return "v{}, v{}, {}".format(self.A, self.B, kind)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         kind = get_kind(self.cm, self.get_kind(), self.CCCC)
         return [(Operand.REGISTER, self.A), (Operand.REGISTER, self.B),
                 (self.get_kind() + Operand.KIND, self.CCCC, kind)]
 
-    def get_ref_kind(self):
+    def get_ref_kind(self) -> int:
         return self.CCCC
 
-    def get_raw(self):
+    def get_raw(self) -> int:
         return self.cm.packer["2H"].pack((self.B << 12) | (self.A << 8) | self.OP, self.CCCC)
 
 
 class Instruction22cs(Instruction):
     """
     This class represents all instructions which have the 22cs format
     """
 
     length = 4
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> str:
         super().__init__()
         self.cm = cm
 
         i16, self.CCCC = cm.packer["2H"].unpack(buff[:self.length])
         self.OP = i16 & 0xff
         self.A = (i16 >> 8) & 0xf
         self.B = (i16 >> 12) & 0xf
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         kind = get_kind(self.cm, self.get_kind(), self.CCCC)
         return "v{}, v{}, {}".format(self.A, self.B, kind)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         kind = get_kind(self.cm, self.get_kind(), self.CCCC)
         return [(Operand.REGISTER, self.A), (Operand.REGISTER, self.B),
                 (self.get_kind() + Operand.KIND, self.CCCC, kind)]
 
-    def get_ref_kind(self):
+    def get_ref_kind(self) -> int:
         return self.CCCC
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["2H"].pack((self.B << 12) | (self.A << 8) | self.OP, self.CCCC)
 
 
 class Instruction31t(Instruction):
     """
     This class represents all instructions which have the 31t format
     """
     length = 6
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, self.AA, self.BBBBBBBB = cm.packer["BBi"].unpack(buff[:self.length])
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         return "v{}, {:+08x}h".format(self.AA, self.BBBBBBBB)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.REGISTER, self.AA), (Operand.OFFSET, self.BBBBBBBB)]
 
-    def get_ref_off(self):
+    def get_ref_off(self) -> int:
         return self.BBBBBBBB
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["Hi"].pack((self.AA << 8) | self.OP, self.BBBBBBBB)
 
 
 class Instruction31c(Instruction):
     """
     This class represents all instructions which have the 31c format
     """
 
     length = 6
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
         self.OP, self.AA, self.BBBBBBBB = cm.packer["BBi"].unpack(buff[:self.length])
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         kind = get_kind(self.cm, self.get_kind(), self.BBBBBBBB)
         return "v{}, {}".format(self.AA, kind)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         kind = get_kind(self.cm, self.get_kind(), self.BBBBBBBB)
         return [(Operand.REGISTER, self.AA),
                 (self.get_kind() + Operand.KIND, self.BBBBBBBB, kind)]
 
-    def get_ref_kind(self):
+    def get_ref_kind(self) -> int:
         return self.BBBBBBBB
 
-    def get_string(self):
+    def get_string(self) -> str:
         """
         Return the string associated to the 'kind' argument
 
         :rtype: string
         """
         return get_kind(self.cm, self.get_kind(), self.BBBBBBBB)
 
-    def get_raw_string(self):
+    def get_raw_string(self) -> str:
         return get_kind(self.cm, Kind.RAW_STRING, self.BBBBBBBB)
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["HI"].pack((self.AA << 8) | self.OP, self.BBBBBBBB)
 
 
 class Instruction12x(Instruction):
     """
     This class represents all instructions which have the 12x format
     """
 
     length = 2
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         i16, = cm.packer["h"].unpack(buff[:self.length])
         self.OP = i16 & 0xff
         self.A = (i16 >> 8) & 0xf
         self.B = (i16 >> 12) & 0xf
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         return "v{}, v{}".format(self.A, self.B)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.REGISTER, self.A), (Operand.REGISTER, self.B)]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["H"].pack((self.B << 12) | (self.A << 8) | self.OP)
 
 
 class Instruction11x(Instruction):
     """
     This class represents all instructions which have the 11x format
     """
 
     length = 2
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, self.AA = cm.packer["BB"].unpack(buff[:self.length])
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         return "v{}".format(self.AA)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.REGISTER, self.AA)]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["H"].pack((self.AA << 8) | self.OP)
 
 
 class Instruction51l(Instruction):
     """
     This class represents all instructions which have the 51l format
     """
 
     length = 10
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         # arbitrary double-width (64-bit) constant
         self.OP, self.AA, self.BBBBBBBBBBBBBBBB = cm.packer["BBq"].unpack(buff[:self.length])
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         return "v{}, {}".format(self.AA, self.BBBBBBBBBBBBBBBB)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.REGISTER, self.AA), (Operand.LITERAL, self.BBBBBBBBBBBBBBBB)]
 
-    def get_literals(self):
+    def get_literals(self) -> list[int]:
         return [self.BBBBBBBBBBBBBBBB]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["BBq"].pack(self.OP, self.AA, self.BBBBBBBBBBBBBBBB)
 
 
 class Instruction31i(Instruction):
     """
     This class represents all instructions which have the 31i format
     """
     length = 6
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, self.AA, self.BBBBBBBB = cm.packer["BBi"].unpack(buff[:self.length])
 
         # 0x14 // const vAA, #+BBBBBBBB: arbitrary 32-bit constant
         # 0x17 // const-wide/32 vAA, #+BBBBBBBB: signed int (32 bits)
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         #FIXME: on const-wide/32: it is actually a register pair vAA:vAA+1!
         return "v{}, {}".format(self.AA, self.BBBBBBBB)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.REGISTER, self.AA), (Operand.LITERAL, self.BBBBBBBB)]
 
-    def get_literals(self):
+    def get_literals(self) -> list[int]:
         return [self.BBBBBBBB]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["BBi"].pack(self.OP, self.AA, self.BBBBBBBB)
 
 
 class Instruction22x(Instruction):
     """
     This class represents all instructions which have the 22x format
     """
 
     length = 4
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, self.AA, self.BBBB = cm.packer["BBH"].unpack(buff[:self.length])
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         return "v{}, v{}".format(self.AA, self.BBBB)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.REGISTER, self.AA), (Operand.REGISTER, self.BBBB)]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["2H"].pack((self.AA << 8) | self.OP, self.BBBB)
 
 
 class Instruction23x(Instruction):
     """
     This class represents all instructions which have the 23x format
     """
 
     length = 4
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, self.AA, self.BB, self.CC = cm.packer["BBBB"].unpack(buff[:self.length])
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         return "v{}, v{}, v{}".format(self.AA, self.BB, self.CC)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.REGISTER, self.AA),
                 (Operand.REGISTER, self.BB),
                 (Operand.REGISTER, self.CC)]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["2H"].pack((self.AA << 8) | self.OP, (self.CC << 8) | self.BB)
 
 
 class Instruction20t(Instruction):
     """
     This class represents all instructions which have the 20t format
     """
 
     length = 4
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, padding, self.AAAA = cm.packer["BBh"].unpack(buff[:self.length])
         if padding != 0:
             raise InvalidInstruction('High byte of opcode with format 20t must be zero!')
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         # Offset is in 16bit units
         return "{:+04x}h".format(self.AAAA)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.OFFSET, self.AAAA)]
 
-    def get_ref_off(self):
+    def get_ref_off(self) -> int:
         return self.AAAA
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["Hh"].pack(self.OP, self.AAAA)
 
 
 class Instruction21t(Instruction):
     """
     This class represents all instructions which have the 21t format
     """
     length = 4
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, self.AA, self.BBBB = cm.packer["BBh"].unpack(buff[:self.length])
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         return "v{}, {:+04x}h".format(self.AA, self.BBBB)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.REGISTER, self.AA), (Operand.OFFSET, self.BBBB)]
 
-    def get_ref_off(self):
+    def get_ref_off(self) -> int:
         return self.BBBB
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["Hh"].pack((self.AA << 8) | self.OP, self.BBBB)
 
 
 class Instruction10t(Instruction):
     """
     This class represents all instructions which have the 10t format
     """
 
     length = 2
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, self.AA = cm.packer["Bb"].unpack(buff[:self.length])
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         # Offset is given in 16bit units
         return "{:+02x}h".format(self.AA)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.OFFSET, self.AA)]
 
-    def get_ref_off(self):
+    def get_ref_off(self) -> int:
         return self.AA
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["Bb"].pack(self.OP, self.AA)
 
 
 class Instruction22t(Instruction):
     """
     This class represents all instructions which have the 22t format
     """
 
     length = 4
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         i16, self.CCCC = cm.packer["Hh"].unpack(buff[:self.length])
         self.OP = i16 & 0xff
         self.A = (i16 >> 8) & 0xf
         self.B = (i16 >> 12) & 0xf
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         return "v{}, v{}, {:+04x}h".format(self.A, self.B, self.CCCC)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.REGISTER, self.A), (Operand.REGISTER, self.B),
                 (Operand.OFFSET, self.CCCC)]
 
-    def get_ref_off(self):
+    def get_ref_off(self) -> int:
         return self.CCCC
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["Hh"].pack((self.B << 12) | (self.A << 8) | self.OP, self.CCCC)
 
 
 class Instruction22s(Instruction):
     """
     This class represents all instructions which have the 22s format
     """
 
     length = 4
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         i16, self.CCCC = cm.packer["Hh"].unpack(buff[:self.length])
         self.OP = i16 & 0xff
         self.A = (i16 >> 8) & 0xf
         self.B = (i16 >> 12) & 0xf
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         return "v{}, v{}, {}".format(self.A, self.B, self.CCCC)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.REGISTER, self.A), (Operand.REGISTER, self.B),
                 (Operand.LITERAL, self.CCCC)]
 
-    def get_literals(self):
+    def get_literals(self) -> list[int]:
         return [self.CCCC]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["Hh"].pack((self.B << 12) | (self.A << 8) | self.OP, self.CCCC)
 
 
 class Instruction22b(Instruction):
     """
     This class represents all instructions which have the 22b format
     """
 
     length = 4
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, self.AA, self.BB, self.CC = cm.packer["BBBb"].unpack(buff[:self.length])
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         return "v{}, v{}, {}".format(self.AA, self.BB, self.CC)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.REGISTER, self.AA), (Operand.REGISTER, self.BB),
                 (Operand.LITERAL, self.CC)]
 
-    def get_literals(self):
+    def get_literals(self) -> list[int]:
         return [self.CC]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["Hh"].pack((self.AA << 8) | self.OP, (self.CC << 8) | self.BB)
 
 
 class Instruction30t(Instruction):
     """
     This class represents all instructions which have the 30t format
     """
 
     length = 6
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, padding, self.AAAAAAAA = cm.packer["BBi"].unpack(buff[:self.length])
         if padding != 0:
             raise InvalidInstruction('High byte of opcode with format 30t must be zero!')
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         return "{:+08x}h".format(self.AAAAAAAA)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.OFFSET, self.AAAAAAAA)]
 
-    def get_ref_off(self):
+    def get_ref_off(self) -> int:
         return self.AAAAAAAA
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["Hi"].pack(self.OP, self.AAAAAAAA)
 
 
 class Instruction3rc(Instruction):
     """
     This class represents all instructions which have the 3rc format
     """
 
     length = 6
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, self.AA, self.BBBB, self.CCCC = cm.packer["BBHH"].unpack(buff[:self.length])
 
         self.NNNN = self.CCCC + self.AA - 1
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         kind = get_kind(self.cm, self.get_kind(), self.BBBB)
 
         if self.CCCC == self.NNNN:
             return "v{}, {}".format(self.CCCC, kind)
         else:
             return "v{} ... v{}, {}".format(self.CCCC, self.NNNN, kind)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         kind = get_kind(self.cm, self.get_kind(), self.BBBB)
 
         return [(Operand.REGISTER, i) for i in range(self.CCCC, self.NNNN + 1)] + \
                [(self.get_kind() + Operand.KIND, self.BBBB, kind)]
 
-    def get_ref_kind(self):
+    def get_ref_kind(self) -> int:
         return self.BBBB
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["3H"].pack((self.AA << 8) | self.OP, self.BBBB, self.CCCC)
 
 
 class Instruction32x(Instruction):
     """
     This class represents all instructions which have the 32x format
     """
 
     length = 6
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, padding, self.AAAA, self.BBBB = cm.packer["BBHH"].unpack(buff[:self.length])
         if padding != 0:
             raise InvalidInstruction('High byte of opcode with format 32x must be zero!')
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         return "v{}, v{}".format(self.AAAA, self.BBBB)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.REGISTER, self.AAAA), (Operand.REGISTER, self.BBBB)]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["3H"].pack(self.OP, self.AAAA, self.BBBB)
 
 
 class Instruction20bc(Instruction):
     """
     This class represents all instructions which have the 20bc format
     """
 
     length = 4
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, self.AA, self.BBBB = cm.packer["BBH"].unpack(buff[:self.length])
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         return "{}, {}".format(self.AA, self.BBBB)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         return [(Operand.LITERAL, self.AA), (Operand.LITERAL, self.BBBB)]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["2H"].pack((self.AA << 8) | self.OP, self.BBBB)
 
 
 class Instruction35mi(Instruction):
     """
     This class represents all instructions which have the 35mi format
     """
 
     length = 6
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         i16a, \
         self.BBBB, \
         i16b = cm.packer["3H"].unpack(buff[:self.length])
         self.OP = i16a & 0xff
         self.G = (i16a >> 8) & 0xf
         self.A = (i16a >> 12) & 0xf
         self.C = i16b & 0xf
         self.D = (i16b >> 4) & 0xf
         self.E = (i16b >> 8) & 0xf
         self.F = (i16b >> 12) & 0xf
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         kind = get_kind(self.cm, self.get_kind(), self.BBBB)
 
         if self.A == 1:
             return "v%d, %s" % (self.C, kind)
         elif self.A == 2:
             return "v%d, v%d, %s" % (self.C, self.D, kind)
         elif self.A == 3:
@@ -5627,15 +5630,15 @@
         elif self.A == 4:
             return "v%d, v%d, v%d, v%d, %s" % (self.C, self.D, self.E, self.F,
                                                 kind)
         elif self.A == 5:
             return "v%d, v%d, v%d, v%d, v%d, %s" % (self.C, self.D, self.E,
                                                      self.F, self.G, kind)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         l = []
         kind = get_kind(self.cm, self.get_kind(), self.BBBB)
 
         if self.A == 1:
             l.extend([(Operand.REGISTER, self.C), (self.get_kind(
             ) + Operand.KIND, self.BBBB, kind)])
         elif self.A == 2:
@@ -5653,45 +5656,45 @@
             l.extend([(Operand.REGISTER, self.C), (Operand.REGISTER, self.D), (
                 Operand.REGISTER, self.E), (Operand.REGISTER, self.F), (
                           Operand.REGISTER, self.G), (self.get_kind() + Operand.KIND,
                                                       self.BBBB, kind)])
 
         return l
 
-    def get_ref_kind(self):
+    def get_ref_kind(self) -> int:
         return self.BBBB
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["3H"].pack((self.A << 12) | (self.G << 8) | self.OP, self.BBBB,
                     (self.F << 12) | (self.E << 8) | (self.D << 4) | self.C)
 
 
 class Instruction35ms(Instruction):
     """
     This class represents all instructions which have the 35ms format
     """
 
     length = 6
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         i16a, \
         self.BBBB, \
         i16b = cm.packer["3H"].unpack(buff[:self.length])
         self.OP = i16a & 0xff
         self.G = (i16a >> 8) & 0xf
         self.A = (i16a >> 12) & 0xf
         self.C = i16b & 0xf
         self.D = (i16b >> 4) & 0xf
         self.E = (i16b >> 8) & 0xf
         self.F = (i16b >> 12) & 0xf
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         kind = get_kind(self.cm, self.get_kind(), self.BBBB)
 
         if self.A == 1:
             return "v%d, %s" % (self.C, kind)
         elif self.A == 2:
             return "v%d, v%d, %s" % (self.C, self.D, kind)
         elif self.A == 3:
@@ -5699,15 +5702,15 @@
         elif self.A == 4:
             return "v%d, v%d, v%d, v%d, %s" % (self.C, self.D, self.E, self.F,
                                                kind)
         elif self.A == 5:
             return "v%d, v%d, v%d, v%d, v%d, %s" % (self.C, self.D, self.E,
                                                     self.F, self.G, kind)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         l = []
         kind = get_kind(self.cm, self.get_kind(), self.BBBB)
 
         if self.A == 1:
             l.extend([(Operand.REGISTER, self.C), (self.get_kind(
             ) + Operand.KIND, self.BBBB, kind)])
         elif self.A == 2:
@@ -5725,270 +5728,270 @@
             l.extend([(Operand.REGISTER, self.C), (Operand.REGISTER, self.D), (
                 Operand.REGISTER, self.E), (Operand.REGISTER, self.F), (
                           Operand.REGISTER, self.G), (self.get_kind() + Operand.KIND,
                                                       self.BBBB, kind)])
 
         return l
 
-    def get_ref_kind(self):
+    def get_ref_kind(self) -> int:
         return self.BBBB
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["3H"].pack((self.A << 12) | (self.G << 8) | self.OP, self.BBBB,
                                          (self.F << 12) | (self.E << 8) | (self.D << 4) | self.C)
 
 
 class Instruction3rmi(Instruction):
     """
     This class represents all instructions which have the 3rmi format
 
     Note, this instruction is similar to 3rc but holds an inline
     """
 
     length = 6
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, self.AA, self.BBBB, self.CCCC = cm.packer["BBHH"].unpack(buff[:self.length])
 
         self.NNNN = self.CCCC + self.AA - 1
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         kind = get_kind(self.cm, self.get_kind(), self.BBBB)
 
         if self.CCCC == self.NNNN:
             return "v{}, {}".format(self.CCCC, kind)
         else:
             return "v{} ... v{}, {}".format(self.CCCC, self.NNNN, kind)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         kind = get_kind(self.cm, self.get_kind(), self.BBBB)
 
         if self.CCCC == self.NNNN:
             return [(Operand.REGISTER, self.CCCC),
                     (self.get_kind() + Operand.KIND, self.BBBB, kind)]
         else:
             l = []
             for i in range(self.CCCC, self.NNNN):
                 l.append((Operand.REGISTER, i))
 
             l.append((self.get_kind() + Operand.KIND, self.BBBB, kind))
             return l
 
-    def get_ref_kind(self):
+    def get_ref_kind(self) -> int:
         return self.BBBB
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["3H"].pack((self.AA << 8) | self.OP, self.BBBB, self.CCCC)
 
 
 class Instruction3rms(Instruction):
     """
     This class represents all instructions which have the 3rms format
 
     Note, this instruction is similar to 3rc but holds a vtaboff
     """
 
     length = 6
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, self.AA, self.BBBB, self.CCCC = cm.packer["BBHH"].unpack(buff[:self.length])
 
         self.NNNN = self.CCCC + self.AA - 1
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         kind = get_kind(self.cm, self.get_kind(), self.BBBB)
 
         if self.CCCC == self.NNNN:
             return "v{}, {}".format(self.CCCC, kind)
         else:
             return "v{} ... v{}, {}".format(self.CCCC, self.NNNN, kind)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         kind = get_kind(self.cm, self.get_kind(), self.BBBB)
 
         if self.CCCC == self.NNNN:
             return [(Operand.REGISTER, self.CCCC),
                     (self.get_kind() + Operand.KIND, self.BBBB, kind)]
         else:
             l = []
             for i in range(self.CCCC, self.NNNN):
                 l.append((Operand.REGISTER, i))
 
             l.append((self.get_kind() + Operand.KIND, self.BBBB, kind))
             return l
 
-    def get_ref_kind(self):
+    def get_ref_kind(self) -> int:
         return self.BBBB
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["3H"].pack((self.AA << 8) | self.OP, self.BBBB, self.CCCC)
 
 
 class Instruction41c(Instruction):
     """
     This class represents all instructions which have the 41c format
 
     This instruction is only used in ODEX
     """
 
     length = 8
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, \
         self.BBBBBBBB, \
         self.AAAA = cm.packer["HIH"].unpack(buff[:self.length])
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         kind = get_kind(self.cm, self.get_kind(), self.BBBBBBBB)
         return "v{}, {}".format(self.AAAA, kind)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         kind = get_kind(self.cm, self.get_kind(), self.BBBBBBBB)
         return [(Operand.REGISTER, self.AAAA),
                 (self.get_kind() + Operand.KIND, self.BBBBBBBB, kind)]
 
-    def get_ref_kind(self):
+    def get_ref_kind(self) -> int:
         return self.BBBBBBBB
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["HIH"].pack(self.OP, self.BBBBBBBB, self.AAAA)
 
 
 class Instruction40sc(Instruction):
     """
     This class represents all instructions which have the 40sc format
 
     This instruction is only used in ODEX
     """
 
     length = 8
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, \
         self.BBBBBBBB, \
         self.AAAA = cm.packer["HIH"].unpack(buff[:self.length])
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         kind = get_kind(self.cm, self.get_kind(), self.BBBBBBBB)
         return "{}, {}".format(self.AAAA, kind)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         kind = get_kind(self.cm, self.get_kind(), self.BBBBBBBB)
         return [(Operand.LITERAL, self.AAAA),
                 (self.get_kind() + Operand.KIND, self.BBBBBBBB, kind)]
 
-    def get_ref_kind(self):
+    def get_ref_kind(self) -> int:
         return self.BBBBBBBB
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["HIH"].pack(self.OP, self.BBBBBBBB, self.AAAA)
 
 
 class Instruction52c(Instruction):
     """
     This class represents all instructions which have the 52c format
 
     This instruction is only used in ODEX
     """
 
     length = 10
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         # FIXME: Not in the documentation!
         # Using 16bit for opcode, but its ODEX, so...
         self.OP, \
         self.CCCCCCCC, \
         self.AAAA, \
         self.BBBB = cm.packer["HI2H"].unpack(buff[:self.length])
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         kind = get_kind(self.cm, self.get_kind(), self.CCCCCCCC)
         return "v{}, v{}, {}".format(self.AAAA, self.BBBB, kind)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         kind = get_kind(self.cm, self.get_kind(), self.CCCCCCCC)
         return [(Operand.LITERAL, self.AAAA), (Operand.LITERAL, self.BBBB),
                 (self.get_kind() + Operand.KIND, self.CCCCCCCC, kind)]
 
-    def get_ref_kind(self):
+    def get_ref_kind(self) -> int:
         return self.CCCCCCCC
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["HI2H"].pack(self.OP, self.CCCCCCCC, self.AAAA, self.BBBB)
 
 
 class Instruction5rc(Instruction):
     """
     This class represents all instructions which have the 5rc format
 
     This instruction is only used in ODEX
     """
 
     length = 10
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, \
         self.BBBBBBBB, \
         self.AAAA, \
         self.CCCC = cm.packer["HI2H"].unpack(buff[:self.length])
 
         self.NNNN = self.CCCC + self.AAAA - 1
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         kind = get_kind(self.cm, self.get_kind(), self.BBBBBBBB)
 
         if self.CCCC == self.NNNN:
             return "v{}, {}".format(self.CCCC, kind)
         else:
             return "v{} ... v{}, {}".format(self.CCCC, self.NNNN, kind)
 
-    def get_operands(self, idx=-1):
+    def get_operands(self, idx:int=-1) -> list[tuple[Operand, int]]:
         kind = get_kind(self.cm, self.get_kind(), self.BBBBBBBB)
 
         if self.CCCC == self.NNNN:
             return [(Operand.REGISTER, self.CCCC),
                     (self.get_kind() + Operand.KIND, self.BBBBBBBB, kind)]
         else:
             l = []
             for i in range(self.CCCC, self.NNNN):
                 l.append((Operand.REGISTER, i))
 
             l.append((self.get_kind() + Operand.KIND, self.BBBBBBBB, kind))
             return l
 
-    def get_ref_kind(self):
+    def get_ref_kind(self) -> int:
         return self.BBBBBBBB
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["HI2H"].pack(self.OP, self.BBBBBBBB, self.AAAA, self.CCCC)
 
 
 class Instruction45cc(Instruction):
     length = 8
 
     # FIXME!!!
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         # Note: the documentation says A|G|op|BBBB ... but we need to parse op|A|G because of LE
         self.OP, reg1, self.BBBB, reg2, self.HHHH = self.cm.packer["BBHHH"].unpack(buff[:self.get_length()])
         # TODO need to check if registers are correct
         self.A = (reg1 & 0xF0) >> 4
@@ -5998,23 +6001,23 @@
 
         self.D = (reg2 & 0xF0) >> 4
         self.C = (reg2 & 0x0F)
 
         self.F = (reg2 & 0xF000) >> 12
         self.E = (reg2 & 0x0F00) >> 8
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer["BBHHH"].pack(
                     self.OP,
                     self.A << 4 | self.G,
                     self.BBBB,
                     self.F << 12 | self.E << 8 | self.D << 4 | self.C,
                     self.HHHH)
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         # FIXME get_kind of BBBB (method) and HHHH (proto)
         if self.A == 1:
             return 'v{}, {}, {}'.format(self.C, self.BBBB, self.HHHH)
         if self.A == 2:
             return 'v{}, v{}, {}, {}'.format(self.C, self.D, self.BBBB, self.HHHH)
         if self.A == 3:
             return 'v{}, v{}, v{}, {}, {}'.format(self.C, self.D, self.E, self.BBBB, self.HHHH)
@@ -6030,38 +6033,38 @@
         pass
 
 
 class Instruction4rcc(Instruction):
     length = 8
 
     # FIXME!!!
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         super().__init__()
         self.cm = cm
 
         self.OP, self.AA, self.BBBB, self.CCCC, self.HHHH = self.cm.packer['BBHHH'].unpack(buff[:self.get_length()])
         self.NNNN = self.AA + self.CCCC - 1
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.cm.packer['BBHHH'].pack(self.OP, self.AA, self.BBBB, self.CCCC, self.HHHH)
 
-    def get_output(self, idx=-1):
+    def get_output(self, idx:int=-1) -> str:
         # FIXME get_kind of BBBB (meth) and HHHH (proto)
         return 'v{} .. v{} {} {}'.format(self.CCCC, self.NNNN, self.BBBB, self.HHHH)
 
     def get_operands(self):
         # FIXME
         pass
 
 
 class Instruction00x(Instruction):
     """A class for unused instructions, has zero length and raises an error on initialization"""
     length = 0
 
-    def __init__(self, cm, buff):
+    def __init__(self, cm: ClassManager, buff: bytes) -> None:
         raise InvalidInstruction("Instruction with opcode '0x{:02x}' is unused! This looks like invalid bytecode.".format(buff[0]))
 
 
 DALVIK_OPCODES_FORMAT = {
     # From the Dalvik documentation:
     #
     # > Most format IDs consist of three characters, two digits followed by a letter.
@@ -6392,15 +6395,15 @@
     0xfcff: [Instruction41c, ["sput-volatile/jumbo", Kind.FIELD]],
     0xfdff: [Instruction41c, ["sput-wide-volatile/jumbo", Kind.FIELD]],
     0xfeff: [Instruction41c, ["sput-object-volatile/jumbo", Kind.FIELD]],
     0xffff: [Instruction40sc, ["throw-verification-error/jumbo", Kind.VARIES]],
 }
 
 
-def get_instruction(cm, op_value, buff):
+def get_instruction(cm: ClassManager, op_value: int, buff: bytearray) -> Instruction:
     """
     Return the :class:`Instruction` for the given opcode
 
     :param ClassManager cm: ClassManager to propagate to Instruction
     :param int op_value: integer value of the instruction
     :param bytearray buff: Bytecode starting with the instruction
     :return: the parsed Instruction
@@ -6409,37 +6412,37 @@
     try:
         return DALVIK_OPCODES_FORMAT[op_value][0](cm, buff)
     except struct.error:
         # FIXME: there are other possible errors too...
         raise InvalidInstruction("Invalid Instruction for '0x{:02x}': {}".format(op_value, repr(buff)))
 
 
-def get_optimized_instruction(cm, op_value, buff):
+def get_optimized_instruction(cm: ClassManager, op_value: int, buff: bytearray) -> Instruction:
     try:
         return DALVIK_OPCODES_OPTIMIZED[op_value][0](cm, buff)
     except struct.error:
         # FIXME: there are other possible errors too...
         raise InvalidInstruction("Invalid Instruction for '0x{:04x}': {}".format(op_value, repr(buff)))
 
 
-def get_instruction_payload(op_value, cm, buff):
+def get_instruction_payload(op_value: int, cm: ClassManager, buff: bytearray) -> Union[PackedSwitch,SparseSwitch,FillArrayData]:
     try:
         return DALVIK_OPCODES_PAYLOAD[op_value][0](cm, buff)
     except struct.error:
         # FIXME: there are other possible errors too...
         raise InvalidInstruction("Invalid Instruction for '0x{:04x}': {}".format(op_value, repr(buff)))
 
 
 class LinearSweepAlgorithm:
     """
     This class is used to disassemble a method. The algorithm used by this class is linear sweep.
     """
 
     @staticmethod
-    def get_instructions(cm, size, insn, idx):
+    def get_instructions(cm: ClassManager, size: int, insn: bytearray, idx: int) -> Iterator[Instruction]:
         """
         Yields all instructions for the given bytecode sequence.
         If unknown/corrupt/unused instructions are encountered,
         the loop will stop and an error is written to the logger.
 
         That means that the bytecode read might be corrupt
         or was crafted in this way, to break parsers.
@@ -6494,84 +6497,84 @@
     :param class_manager: the ClassManager
     :type class_manager: :class:`ClassManager` object
     :param offset: the offset of the buffer
     :type offset: int
     :param size: the total size of the buffer
     :type size: int
     :param buff: a raw buffer where are the instructions
-    :type buff: string
+    :type buff: bytes
     """
 
-    def __init__(self, class_manager, offset, size, buff):
+    def __init__(self, class_manager: ClassManager, offset: int, size: int, buff: bytes) -> None:
         self.CM = class_manager
         self.insn = buff
         self.offset = offset
         self.size = size
 
         self.notes = {}
         self.cached_instructions = None
 
         self.idx = 0
 
-    def get_insn(self):
+    def get_insn(self) -> bytes:
         """
         Get the insn buffer
 
         :rtype: bytes
         """
         return self.insn
 
-    def set_insn(self, insn):
+    def set_insn(self, insn: bytes) -> None:
         """
         Set a new raw buffer to disassemble
 
         :param insn: the buffer
         :type insn: bytes
         """
         self.insn = insn
         self.size = len(self.insn)
 
-    def seek(self, idx):
+    def seek(self, idx: int) -> None:
         """
         Set the start address of the buffer
 
         :param idx: the index
         :type idx: int
         """
         self.idx = idx
 
-    def is_cached_instructions(self):
+    def is_cached_instructions(self) -> bool:
         if self.cached_instructions is not None:
             return True
         return False
 
-    def set_instructions(self, instructions):
+    def set_instructions(self, instructions:list[Instruction]) -> None:
         """
         Set the instructions
 
         :param instructions: the list of instructions
         :type instructions: a list of :class:`Instruction`
         """
         self.cached_instructions = instructions
 
-    def get_instructions(self):
+    def get_instructions(self) -> Iterator[Instruction]:
         """
         Get the instructions
 
         :rtype: a generator of each :class:`Instruction` (or a cached list of instructions if you have setup instructions)
         """
         # it is possible to a cache for instructions (avoid a new disasm)
         if self.cached_instructions is None:
             ins = LinearSweepAlgorithm.get_instructions(self.CM, self.size, self.insn, self.idx)
             self.cached_instructions = list(ins)
 
         for i in self.cached_instructions:
             yield i
 
-    def add_inote(self, msg, idx, off=None):
+    def add_inote(self, msg: str, idx: int, off:Union[int,None]=None) -> None:
         """
         Add a message to a specific instruction by using (default) the index of the address if specified
 
         :param msg: the message
         :type msg: string
         :param idx: index of the instruction (the position in the list of the instruction)
         :type idx: int
@@ -6582,15 +6585,15 @@
             idx = self.off_to_pos(off)
 
         if idx not in self.notes:
             self.notes[idx] = []
 
         self.notes[idx].append(msg)
 
-    def get_instruction(self, idx, off=None):
+    def get_instruction(self, idx: int, off:Union[int,None]=None) -> Instruction:
         """
         Get a particular instruction by using (default) the index of the address if specified
 
         :param idx: index of the instruction (the position in the list of the instruction)
         :type idx: int
         :param off: address of the instruction
         :type off: int
@@ -6599,15 +6602,15 @@
         """
         if off is not None:
             idx = self.off_to_pos(off)
         if self.cached_instructions is None:
             self.get_instructions()
         return self.cached_instructions[idx]
 
-    def off_to_pos(self, off):
+    def off_to_pos(self, off:int) -> int:
         """
         Get the position of an instruction by using the address
 
         :param off: address of the instruction
         :type off: int
 
         :rtype: int
@@ -6617,15 +6620,15 @@
         for i in self.get_instructions():
             if idx == off:
                 return nb
             nb += 1
             idx += i.get_length()
         return -1
 
-    def get_ins_off(self, off):
+    def get_ins_off(self, off:int) -> Instruction:
         """
         Get a particular instruction by using the address
 
         :param off: address of the instruction
         :type off: int
 
         :rtype: an :class:`Instruction` object
@@ -6633,112 +6636,112 @@
         idx = 0
         for i in self.get_instructions():
             if idx == off:
                 return i
             idx += i.get_length()
         return None
 
-    def show(self):
+    def show(self) -> None:
         """
         Display (with a pretty print) this object
         """
         off = 0
         for n, i in enumerate(self.get_instructions()):
             print("{:8d} (0x{:08x}) {:04x} {:30} {}".format(n, off, i.get_op_value(), i.get_name(), i.get_output(self.idx)))
             off += i.get_length()
 
-    def get_raw(self):
+    def get_raw(self) -> bytearray:
         """
         Return the raw buffer of this object
 
         :rtype: bytearray
         """
         buff = bytearray()
         for i in self.get_instructions():
             buff += i.get_raw()
         return buff
 
-    def get_length(self):
+    def get_length(self) -> int:
         """
         Return the length of this object
 
         :rtype: int
         """
         return len(self.get_raw())
 
 
 class TryItem:
     """
     This class represents the try_item format
 
     :param buff: a raw buffer where are the try_item format
-    :type buff: io.BufferedReader
+    :type buff: BinaryIO.BufferedReader
     :param cm: the ClassManager
     :type cm: ClassManager
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.offset = buff.tell()
 
         self.CM = cm
 
         self.start_addr, \
         self.insn_count, \
         self.handler_off = cm.packer["I2H"].unpack(buff.read(8))
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def get_start_addr(self):
+    def get_start_addr(self) -> int:
         """
         Get the start address of the block of code covered by this entry. The address is a count of 16-bit code units to the start of the first covered instruction.
 
         :rtype: int
         """
         return self.start_addr
 
-    def get_insn_count(self):
+    def get_insn_count(self) -> int:
         """
         Get the number of 16-bit code units covered by this entry
 
         :rtype: int
         """
         return self.insn_count
 
-    def get_handler_off(self):
+    def get_handler_off(self) -> int:
         """
         Get the offset in bytes from the start of the associated :class:`EncodedCatchHandlerList` to the :class:`EncodedCatchHandler` for this entry.
 
         :rtype: int
         """
         return self.handler_off
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.CM.packer["I2H"].pack(self.start_addr,
                     self.insn_count,
                     self.handler_off)
 
-    def get_length(self):
+    def get_length(self) -> int:
         return len(self.get_raw())
 
 
 class DalvikCode:
     """
     This class represents the instructions of a method
 
     :param buff: a raw buffer where are the instructions
-    :type buff: io.BufferedReader
+    :type buff: BinaryIO.BufferedReader
     :param cm: the ClassManager
     :type cm: :class:`ClassManager` object
     """
 
-    def __init__(self, buff, cm):
+    def __init__(self, buff: BinaryIO, cm:ClassManager) -> None:
         self.CM = cm
         self.offset = buff.tell()
 
         self.registers_size, \
         self.ins_size, \
         self.outs_size, \
         self.tries_size, \
@@ -6756,122 +6759,122 @@
         self.handlers = None
         if self.tries_size > 0:
             for i in range(0, self.tries_size):
                 self.tries.append(TryItem(buff, self.CM))
 
             self.handlers = EncodedCatchHandlerList(buff, self.CM)
 
-    def get_registers_size(self):
+    def get_registers_size(self) -> int:
         """
         Get the number of registers used by this code
 
         :rtype: int
         """
         return self.registers_size
 
-    def get_ins_size(self):
+    def get_ins_size(self) -> int:
         """
         Get the number of words of incoming arguments to the method that this code is for
 
         :rtype: int
         """
         return self.ins_size
 
-    def get_outs_size(self):
+    def get_outs_size(self) -> int:
         """
         Get the number of words of outgoing argument space required by this code for method invocation
 
         :rtype: int
         """
         return self.outs_size
 
-    def get_tries_size(self):
+    def get_tries_size(self) -> int:
         """
         Get the number of :class:`TryItem` for this instance
 
         :rtype: int
         """
         return self.tries_size
 
-    def get_debug_info_off(self):
+    def get_debug_info_off(self) -> int:
         """
         Get the offset from the start of the file to the debug info (line numbers + local variable info) sequence for this code, or 0 if there simply is no information
 
         :rtype: int
         """
         return self.debug_info_off
 
-    def get_insns_size(self):
+    def get_insns_size(self) -> int:
         """
         Get the size of the instructions list, in 16-bit code units
 
         :rtype: int
         """
         return self.insns_size
 
-    def get_handlers(self):
+    def get_handlers(self) -> EncodedCatchHandlerList:
         """
         Get the bytes representing a list of lists of catch types and associated handler addresses.
 
         :rtype: :class:`EncodedCatchHandlerList`
         """
         return self.handlers
 
-    def get_tries(self):
+    def get_tries(self) -> list[TryItem]:
         """
         Get the array indicating where in the code exceptions are caught and how to handle them
 
         :rtype: a list of :class:`TryItem` objects
         """
         return self.tries
 
-    def get_debug(self):
+    def get_debug(self) -> DebugInfoItem:
         """
         Return the associated debug object
 
         :rtype: :class:`DebugInfoItem`
         """
         return self.CM.get_debug_off(self.debug_info_off)
 
-    def get_bc(self):
+    def get_bc(self) -> DCode:
         """
         Return the associated code object
 
         :rtype: :class:`DCode`
         """
         return self.code
 
-    def seek(self, idx):
+    def seek(self, idx: int) -> None:
         self.code.seek(idx)
 
-    def get_length(self):
+    def get_length(self) -> int:
         return self.insns_size
 
-    def _begin_show(self):
+    def _begin_show(self) -> None:
         logger.debug("registers_size: %d" % self.registers_size)
         logger.debug("ins_size: %d" % self.ins_size)
         logger.debug("outs_size: %d" % self.outs_size)
         logger.debug("tries_size: %d" % self.tries_size)
         logger.debug("debug_info_off: %d" % self.debug_info_off)
         logger.debug("insns_size: %d" % self.insns_size)
 
         bytecode._PrintBanner()
 
-    def show(self):
+    def show(self) -> None:
         self._begin_show()
         self.code.show()
         self._end_show()
 
-    def _end_show(self):
+    def _end_show(self) -> None:
         bytecode._PrintBanner()
 
-    def get_obj(self):
+    def get_obj(self) -> tuple[DCode, list[TryItem], EncodedCatchHandlerList]:
         return [self.code, self.tries, self.handlers]
 
-    def get_raw(self):
+    def get_raw(self) -> bytearray:
         """
         Get the reconstructed code as bytearray
 
         :rtype: bytearray
         """
         code_raw = self.code.get_raw()
         self.insns_size = (len(code_raw) // 2) + (len(code_raw) % 2)
@@ -6890,44 +6893,44 @@
 
             for i in self.tries:
                 buff += i.get_raw()
             buff += self.handlers.get_raw()
 
         return buff
 
-    def add_inote(self, msg, idx, off=None):
+    def add_inote(self, msg: str, idx: int, off:int=None) -> None:
         """
         Add a message to a specific instruction by using (default) the index of the address if specified
 
         :param msg: the message
         :type msg: string
         :param idx: index of the instruction (the position in the list of the instruction)
         :type idx: int
         :param off: address of the instruction
         :type off: int
         """
         if self.code:
             return self.code.add_inote(msg, idx, off)
 
-    def get_instruction(self, idx, off=None):
+    def get_instruction(self, idx:int, off:Union[int,None]=None) -> Instruction:
         if self.code:
             return self.code.get_instruction(idx, off)
 
-    def get_size(self):
+    def get_size(self) -> int:
         return len(self.get_raw())
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
 
 class CodeItem:
-    def __init__(self, size, buff, cm):
+    def __init__(self, size:int, buff:bytes, cm:ClassManager) -> None:
         self.CM = cm
 
         self.offset = buff.tell()
 
         self.code = []
         self.__code_off = {}
 
@@ -6939,52 +6942,52 @@
             if off % 4 != 0:
                 buff.seek(off + (4 - (off % 4)))
 
             x = DalvikCode(buff, cm)
             self.code.append(x)
             self.__code_off[x.get_off()] = x
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def get_code(self, off):
+    def get_code(self, off:int) -> DalvikCode:
         try:
             return self.__code_off[off]
         except KeyError:
             return None
 
-    def show(self):
+    def show(self) -> None:
         # FIXME workaround for showing the MAP_ITEMS
         # if m_a is none, we use get_raw.
         # Otherwise the real code is printed...
         bytecode._PrintDefault("CODE_ITEM\n")
         bytecode._PrintDefault(binascii.hexlify(self.get_raw()).decode("ASCII"))
         bytecode._PrintDefault("\n")
 
-    def get_obj(self):
+    def get_obj(self) -> list[DalvikCode]:
         return [i for i in self.code]
 
-    def get_raw(self):
+    def get_raw(self) -> bytearray:
         buff = bytearray()
         for c in self.code:
             buff += c.get_raw()
         return buff
 
-    def get_length(self):
+    def get_length(self) -> int:
         length = 0
         for i in self.code:
             length += i.get_size()
         return length
 
 
 class MapItem:
-    def __init__(self, buff, cm):
+    def __init__(self, buff:bytes, cm:ClassManager) -> None:
         """
         Implementation of a map_item, which occours in a map_list
 
         https://source.android.com/devices/tech/dalvik/dex-format#map-item
         """
         self.CM = cm
         self.buff = buff
@@ -6994,33 +6997,33 @@
         self.type = TypeMapItem(cm.packer["H"].unpack(buff.read(2))[0])
         self.unused, \
         self.size, \
         self.offset = cm.packer["H2I"].unpack(buff.read(10))
 
         self.item = None
 
-    def get_off(self):
+    def get_off(self) -> int:
         """Gets the offset of the map item itself inside the DEX file"""
         return self.off
 
-    def get_offset(self):
+    def get_offset(self) -> int:
         """Gets the offset of the item of the map item"""
         return self.offset
 
-    def get_type(self):
+    def get_type(self) -> TypeMapItem:
         return self.type
 
-    def get_size(self):
+    def get_size(self) -> int:
         """
         Returns the number of items found at the location indicated by
         :meth:`get_offset`.
         """
         return self.size
 
-    def parse(self):
+    def parse(self) -> None:
         logger.debug("Starting parsing map_item '{}'".format(self.type.name))
         started_at = time.time()
 
         # Not all items are aligned in the same way. Most are aligned by four bytes,
         # but there are a few which are not!
         # Hence, we need to check the alignment for each item.
 
@@ -7128,63 +7131,63 @@
                         "size: {size} is unknown. "
                         "Is this a newer DEX format?".format(type=self.type, off=buff.tell(), size=self.size))
 
         diff = time.time() - started_at
         minutes, seconds = diff // 60, diff % 60
         logger.debug("End of parsing map_item '{}'. Required time {:.0f}:{:07.4f}".format(self.type.name, minutes, seconds))
 
-    def show(self):
+    def show(self) -> None:
         bytecode._Print("\tMAP_TYPE_ITEM", self.type.name)
 
         if self.item is not None:
             if isinstance(self.item, list):
                 for i in self.item:
                     i.show()
             else:
                 self.item.show()
 
-    def get_obj(self):
+    def get_obj(self) -> object:
         """
         Return the associated item itself.
         Might return None, if :meth:`parse` was not called yet.
 
         This method is the same as :meth:`get_item`.
         """
         return self.item
 
     # alias
     get_item = get_obj
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         # FIXME why is it necessary to get the offset here agin? We have this
         # stored?!
         if isinstance(self.item, list):
             self.offset = self.item[0].get_off()
         else:
             self.offset = self.item.get_off()
 
         return self.CM.packer["2H2I"].pack(self.type,
                     self.unused,
                     self.size,
                     self.offset)
 
-    def get_length(self):
+    def get_length(self) -> int:
         return calcsize("HHII")
 
-    def set_item(self, item):
+    def set_item(self, item: object) -> None:
         self.item = item
 
 
 class ClassManager:
     """
     This class is used to access to all elements (strings, type, proto ...) of the dex format
     based on their offset or index.
     """
 
-    def __init__(self, vm):
+    def __init__(self, vm: DEX) -> None:
         """
         :param DEX vm: the VM to create a ClassManager for
         """
         self.vm = vm
         self.buff = vm
 
         self.analysis_dex = None
@@ -7215,53 +7218,53 @@
     def packer(self):
         return self.__packer
 
     @packer.setter
     def packer(self, p):
         self.__packer = p
 
-    def get_ascii_string(self, s):
+    def get_ascii_string(self, s: str) -> str:
         # TODO Remove method
         try:
             return s.decode("ascii")
         except UnicodeDecodeError:
             d = ""
             for i in s:
                 if i < 128:
                     d += i
                 else:
                     d += "%x" % i
             return d
 
-    def get_odex_format(self):
+    def get_odex_format(self) -> bool:
         """Returns True if the underlying VM is ODEX"""
         return self.odex_format
 
-    def get_obj_by_offset(self, offset):
+    def get_obj_by_offset(self, offset: int) -> object:
         """
         Returnes a object from as given offset inside the DEX file
         """
         return self.__obj_offset[offset]
 
-    def get_item_by_offset(self, offset):
+    def get_item_by_offset(self, offset: int) -> object:
         return self.__item_offset[offset]
 
-    def get_string_by_offset(self, offset):
+    def get_string_by_offset(self, offset: int) -> object:
         return self.__strings_off[offset]
 
-    def set_decompiler(self, decompiler):
+    def set_decompiler(self, decompiler: DecompilerDAD) -> None:
         self.decompiler_ob = decompiler
 
-    def set_analysis(self, analysis_dex):
+    def set_analysis(self, analysis_dex: Analysis) -> None:
         self.analysis_dex = analysis_dex
 
-    def get_analysis(self):
+    def get_analysis(self) -> Analysis:
         return self.analysis_dex
 
-    def add_type_item(self, type_item, c_item, item):
+    def add_type_item(self, type_item: TypeMapItem, c_item: MapItem, item: object) -> None:
         self.__manage_item[type_item] = item
 
         self.__obj_offset[c_item.get_off()] = c_item
         self.__item_offset[c_item.get_offset()] = item
 
         if item is None:
             pass
@@ -7277,71 +7280,70 @@
                 elif type_item == TypeMapItem.TYPE_LIST:
                     self.__typelists_off[goff] = i
                 elif type_item == TypeMapItem.CLASS_DATA_ITEM:
                     self.__classdata_off[goff] = i
         else:
             self.__manage_item_off.append(c_item.get_offset())
 
-    def get_code(self, idx):
+    def get_code(self, idx: int) -> Union[DalvikCode,None]:
         try:
             return self.__manage_item[TypeMapItem.CODE_ITEM].get_code(idx)
         except KeyError:
             return None
 
-    def get_class_data_item(self, off):
+    def get_class_data_item(self, off:int) -> ClassDataItem :
         i = self.__classdata_off.get(off)
         if i is None:
             logger.warning("unknown class data item @ 0x%x" % off)
-
         return i
 
-    def get_encoded_array_item(self, off):
+    def get_encoded_array_item(self, off:int) -> EncodedArrayItem:
         for i in self.__manage_item[TypeMapItem.ENCODED_ARRAY_ITEM]:
             if i.get_off() == off:
                 return i
 
-    def get_annotations_directory_item(self, off):
+    def get_annotations_directory_item(self, off:int) -> AnnotationsDirectoryItem:
         for i in self.__manage_item[TypeMapItem.ANNOTATIONS_DIRECTORY_ITEM]:
             if i.get_off() == off:
                 return i
 
-    def get_annotation_set_item(self, off):
+    def get_annotation_set_item(self, off:int) -> AnnotationSetItem:
         for i in self.__manage_item[TypeMapItem.ANNOTATION_SET_ITEM]:
             if i.get_off() == off:
                 return i
 
-    def get_annotation_off_item(self, off):
+    def get_annotation_off_item(self, off:int) -> AnnotationOffItem:
         for i in self.__manage_item[TypeMapItem.ANNOTATION_OFF_ITEM]:
             if i.get_off() == off:
                 return i
 
-    def get_annotation_item(self, off):
+    def get_annotation_item(self, off:int) -> AnnotationItem:
         for i in self.__manage_item[TypeMapItem.ANNOTATION_ITEM]:
             if i.get_off() == off:
                 return i
 
-    def get_hiddenapi_class_data_item(self, off):
+    def get_hiddenapi_class_data_item(self, off:int) -> HiddenApiClassDataItem:
         for i in self.__manage_item[TypeMapItem.HIDDENAPI_CLASS_DATA_ITEM]:
             if i.get_off() == off:
                 return i
 
-    def get_string(self, idx):
+    def get_string(self, idx: int) -> str:
         """
         Return a string from the string table at index `idx`
 
         If string is hooked, the hooked string is returned.
 
         :param int idx: index in the string section
         """
         if idx in self.hook_strings:
             return self.hook_strings[idx]
 
         return self.get_raw_string(idx)
 
-    def get_raw_string(self, idx):
+    def get_raw_string(self, idx: int) -> str:
         """
         Return the (unprocessed) string from the string table at index `idx`.
 
         :param int idx: the index in the string section
         """
         try:
             off = self.__manage_item[TypeMapItem.STRING_ID_ITEM][idx].get_string_data_off()
@@ -7351,70 +7353,71 @@
 
         try:
             return self.__strings_off[off].get()
         except KeyError:
             logger.warning("unknown string item @ 0x%x(%d)" % (off, idx))
             return "AG:IS: invalid string"
 
-    def get_type_list(self, off):
+    def get_type_list(self, off:int) -> list[str]:
         if off == 0:
             return []
 
         i = self.__typelists_off[off]
         return [type_.get_string() for type_ in i.get_list()]
 
-    def get_type(self, idx):
+    def get_type(self, idx: int) -> str:
         """
         Return the resolved type name based on the index
 
         This returns the string associated with the type.
 
         :param int idx:
         :return: the type name
         :rtype: str
         """
         _type = self.get_type_ref(idx)
         if _type == -1:
             return "AG:ITI: invalid type"
         return self.get_string(_type)
 
-    def get_type_ref(self, idx):
+    def get_type_ref(self, idx: int) -> TypeIdItem:
         """
         Returns the string reference ID for a given type ID.
 
         This method is similar to :meth:`get_type` but does not resolve
         the string but returns the ID into the string section.
 
         If the type IDX is not found, -1 is returned.
         """
         return self.__manage_item[TypeMapItem.TYPE_ID_ITEM].get(idx)
 
-    def get_proto(self, idx):
+    def get_proto(self, idx: int) -> list:
         proto = self.__cached_proto.get(idx)
         if not proto:
             proto = self.__manage_item[TypeMapItem.PROTO_ID_ITEM].get(idx)
             self.__cached_proto[idx] = proto
 
         return [proto.get_parameters_off_value(),
                 proto.get_return_type_idx_value()]
 
-    def get_field(self, idx):
+    def get_field(self, idx: int) -> list[str]:
         field = self.get_field_ref(idx)
-        return [field.get_class_name(), field.get_type(), field.get_name()]
-
-    def get_field_ref(self, idx):
+        # return [field.get_class_name(), field.get_type(), field.get_name()]
+        return field.get_list()
+    
+    def get_field_ref(self, idx: int) -> FieldIdItem:
         return self.__manage_item[TypeMapItem.FIELD_ID_ITEM].get(idx)
 
-    def get_method(self, idx):
+    def get_method(self, idx: int) -> list[str]:
         return self.get_method_ref(idx).get_list()
 
-    def get_method_ref(self, idx):
+    def get_method_ref(self, idx: int) -> MethodIdItem:
         return self.__manage_item[TypeMapItem.METHOD_ID_ITEM].get(idx)
 
-    def set_hook_class_name(self, class_def, value):
+    def set_hook_class_name(self, class_def: ClassDefItem, value: str) -> None:
         python_export = True
         _type = self.__manage_item[TypeMapItem.TYPE_ID_ITEM].get(
             class_def.get_class_idx())
         self.set_hook_string(_type, value)
 
         try:
             self.vm._delete_python_export_class(class_def)
@@ -7431,15 +7434,15 @@
 
         for i in class_def.get_fields():
             i.reload()
 
         if python_export:
             self.vm._create_python_export_class(class_def)
 
-    def set_hook_method_name(self, encoded_method, value):
+    def set_hook_method_name(self, encoded_method: EncodedMethod, value: str) -> None:
         python_export = True
 
         method = self.__manage_item[TypeMapItem.METHOD_ID_ITEM].get(
             encoded_method.get_method_idx())
         self.set_hook_string(method.get_name_idx(), value)
 
         class_def = self.__manage_item[TypeMapItem.CLASS_DEF_ITEM].get_class_idx(
@@ -7480,15 +7483,15 @@
                 setattr(class_def.M, name, encoded_method)
                 logger.debug("new name in python: created: %s." % name)
             else:
                 logger.debug("skipping creating new name in python")
 
         method.reload()
 
-    def set_hook_field_name(self, encoded_field, value):
+    def set_hook_field_name(self, encoded_field: EncodedField, value: str) -> None:
         python_export = True
 
         field = self.__manage_item[TypeMapItem.FIELD_ID_ITEM].get(
             encoded_field.get_field_idx())
         self.set_hook_string(field.get_name_idx(), value)
 
         class_def = self.__manage_item[TypeMapItem.CLASS_DEF_ITEM].get_class_idx(
@@ -7507,37 +7510,36 @@
 
             if python_export:
                 name = bytecode.FormatNameToPython(value)
                 setattr(class_def.F, name, encoded_field)
 
         field.reload()
 
-    def set_hook_string(self, idx, value):
+    def set_hook_string(self, idx: int, value: str) -> None:
         self.hook_strings[idx] = value
 
-    def get_next_offset_item(self, idx):
+    def get_next_offset_item(self, idx: int) -> int:
         for i in self.__manage_item_off:
             if i > idx:
                 return i
         return idx
 
-    def get_debug_off(self, off):
+    def get_debug_off(self, off:int) -> DebugInfoItem:
         self.buff.seek(off)
-
         return DebugInfoItem(self.buff, self)
 
 
 class MapList:
     """
     This class can parse the "map_list" of the dex format
 
     https://source.android.com/devices/tech/dalvik/dex-format#map-list
     """
 
-    def __init__(self, cm, off, buff):
+    def __init__(self, cm: ClassManager, off: int, buff: BinaryIO) -> None:
         self.CM = cm
 
         buff.seek(off)
 
         self.offset = off
 
         self.size, = cm.packer["I"].unpack(buff.read(4))
@@ -7560,62 +7562,62 @@
             c_item = mi.get_item()
             if c_item is None:
                 mi.set_item(self)
                 c_item = mi.get_item()
 
             self.CM.add_type_item(mi.get_type(), mi, c_item)
 
-    def get_off(self):
+    def get_off(self) -> int:
         return self.offset
 
-    def set_off(self, off):
+    def set_off(self, off:int) -> None:
         self.offset = off
 
-    def get_item_type(self, ttype):
+    def get_item_type(self, ttype: TypeMapItem) -> object:
         """
         Get a particular item type
 
         :param ttype: a :class:`~TypeMapItem` enum which represents the desired type
 
         :rtype: None or the item object
         """
         for i in self.map_item:
             if i.get_type() == ttype:
                 return i.get_item()
         return None
 
-    def show(self):
+    def show(self) -> None:
         """
         Print with a pretty display the MapList object
         """
         bytecode._Print("MAP_LIST SIZE", self.size)
         for i in self.map_item:
             if i.item != self:
                 # FIXME this does not work for CodeItems!
                 # as we do not have the method analysis here...
                 i.show()
 
-    def get_obj(self):
+    def get_obj(self) -> list[object]:
         return [x.get_obj() for x in self.map_item]
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         return self.CM.packer["I"].pack(self.size) + b''.join(x.get_raw() for x in self.map_item)
 
-    def get_class_manager(self):
+    def get_class_manager(self) -> ClassManager:
         return self.CM
 
-    def get_length(self):
+    def get_length(self) -> int:
         return len(self.get_raw())
 
 
 class DalvikPacker:
     """
     Generic Packer class to unpack bytes based on different endianness
     """
-    def __init__(self, endian_tag):
+    def __init__(self, endian_tag: int) -> None:
         if endian_tag == 0x78563412:
             logger.error("DEX file with byte swapped endian tag is not supported!")
             raise NotImplementedError("Byte swapped endian tag encountered!")
         elif endian_tag == 0x12345678:
             self.endian_tag = '<'
         else:
             raise ValueError("This is not a DEX file! Wrong endian tag: '0x{:08x}'".format(endian_tag))
@@ -7638,23 +7640,23 @@
 
 class DEX:
     """
     This class can parse a classes.dex file of an Android application (APK).
 
     :param buff: a string which represents the classes.dex file
     :param decompiler: associate a decompiler object to display the java source code
-    :type buff: bytes
+    :type buff: BinaryIO
     :type decompiler: object
 
     example::
 
         d = DEX( read("classes.dex") )
     """
 
-    def __init__(self, buff, decompiler=None, config=None, using_api=None):
+    def __init__(self, buff, decompiler:Union[DecompilerDAD,None]=None, config=None, using_api:Union[int,None]=None) -> None:
         logger.debug("DEX {} {} {}".format(decompiler, config, using_api))
 
         # to allow to pass apk object ==> we do not need to pass additionally target version
         if isinstance(buff, apk.APK):
             self.api_version = buff.get_target_sdk_version()
             buff = buff.get_dex()  # getting dex from APK file
         elif using_api:
@@ -7671,15 +7673,15 @@
 
         self._preload(buff)
         self._load(buff)
 
     def _preload(self, buff):
         pass
 
-    def _load(self, buff):
+    def _load(self, buff) -> None:
         self.header = HeaderItem(0, self.raw, self.CM)
 
         if self.header.map_off == 0:
             # TODO check if the header specifies items but does not have a map
             logger.warning("no map list! This DEX file is probably empty.")
         else:
             self.map_list = MapList(self.CM, self.header.map_off, self.raw)
@@ -7690,129 +7692,129 @@
             self.codes = self.map_list.get_item_type(TypeMapItem.CODE_ITEM)
             self.strings = self.map_list.get_item_type(TypeMapItem.STRING_DATA_ITEM)
             self.debug = self.map_list.get_item_type(TypeMapItem.DEBUG_INFO_ITEM)
             self.hidden_api = self.map_list.get_item_type(TypeMapItem.HIDDENAPI_CLASS_DATA_ITEM)
 
         self._flush()
 
-    def _flush(self):
+    def _flush(self) -> None:
         """
         Flush all caches
         Might be used after classes, methods or fields are added.
         """
         self.classes_names = None
         self.__cache_methods = None
         self.__cached_methods_idx = None
         self.__cache_fields = None
 
         # cache methods and fields as well, otherwise the decompiler is quite slow
         self.__cache_all_methods = None
         self.__cache_all_fields = None
 
     @property
-    def version(self):
+    def version(self) -> int:
         """
         Returns the version number of the DEX Format
         """
         return self.header.dex_version
 
-    def get_api_version(self):
+    def get_api_version(self) -> int:
         """
         This method returns api version that should be used for loading api
         specific resources.
 
-        :rtype: int
+        :rtype: string
         """
         return self.api_version
 
-    def get_classes_def_item(self):
+    def get_classes_def_item(self) -> ClassHDefItem:
         """
         This function returns the class def item
 
         :rtype: :class:`ClassHDefItem` object
         """
         return self.classes
 
-    def get_methods_id_item(self):
+    def get_methods_id_item(self) -> MethodHIdItem:
         """
         This function returns the method id item
 
         :rtype: :class:`MethodHIdItem` object
         """
         return self.methods
 
-    def get_fields_id_item(self):
+    def get_fields_id_item(self) -> FieldHIdItem:
         """
         This function returns the field id item
 
         :rtype: :class:`FieldHIdItem` object
         """
         return self.fields
 
-    def get_codes_item(self):
+    def get_codes_item(self) -> CodeItem:
         """
         This function returns the code item
 
         :rtype: :class:`CodeItem` object
         """
         return self.codes
 
-    def get_string_data_item(self):
+    def get_string_data_item(self) -> StringDataItem:
         """
         This function returns the string data item
 
         :rtype: :class:`StringDataItem` object
         """
         return self.strings
 
-    def get_debug_info_item(self):
+    # TODO: this returns DebugInfoItemEmpty, as DebugInfoItem never gets set as a MapItem
+    def get_debug_info_item(self) -> DebugInfoItemEmpty:
         """
         This function returns the debug info item
-
-        :rtype: :class:`DebugInfoItem` object
+        :rtype: :class:`DebugInfoItemEmpty` object
         """
         return self.debug
 
-    def get_header_item(self):
+    def get_header_item(self) -> HeaderItem:
         """
         This function returns the header item
 
         :rtype: :class:`HeaderItem` object
         """
         return self.header
 
-    def get_hidden_api(self):
+    def get_hidden_api(self) -> HiddenApiClassDataItem:
         """
         This function returns the hidden api item (from Android 10)
 
         :rtype: :class:`HiddenApiClassDataItem` object
         """
         return self.hidden_api
 
-    def get_class_manager(self):
+    def get_class_manager(self) -> ClassManager:
         """
         This function returns a ClassManager object which allow you to get
         access to all index references (strings, methods, fields, ....)
 
         :rtype: :class:`ClassManager` object
         """
         return self.CM
 
-    def show(self):
+    def show(self) -> None:
         """
         Show the all information in the object
         """
         self.map_list.show()
 
-    def save(self):
+    def save(self) -> bytes:
         """
         Return the dex (with the modifications) into raw format (fix checksums)
         (beta: do not use !)
 
-        :rtype: string
+        :rtype: bytes
         """
         l = []
         h = {}
         s = {}
         h_r = {}
 
         idx = 0
@@ -7882,114 +7884,114 @@
                 buff += b"\x00"
             last_idx = idx + s[idx]
 
         logger.debug("GLOBAL SIZE %d" % len(buff))
 
         return self.fix_checksums(buff)
 
-    def fix_checksums(self, buff):
+    def fix_checksums(self, buff: bytes) -> bytes:
         """
           Fix a dex format buffer by setting all checksums
 
-          :rtype: string
+          :rtype: bytes
         """
 
         signature = hashlib.sha1(buff[32:]).digest()
 
         buff = buff[:12] + signature + buff[32:]
         checksum = zlib.adler32(buff[12:])
         buff = buff[:8] + self.CM.packer["I"].pack(checksum) + buff[12:]
 
         logger.debug("NEW SIGNATURE %s" % repr(signature))
         logger.debug("NEW CHECKSUM %x" % checksum)
 
         return buff
 
-    def get_cm_field(self, idx):
+    def get_cm_field(self, idx: int) -> list[str]:
         """
         Get a specific field by using an index
 
         :param idx: index of the field
         :type idx: int
         """
         return self.CM.get_field(idx)
 
-    def get_cm_method(self, idx):
+    def get_cm_method(self, idx: int) -> list[str]:
         """
         Get a specific method by using an index
 
         :param idx: index of the method
         :type idx: int
         """
         return self.CM.get_method(idx)
 
-    def get_cm_string(self, idx):
+    def get_cm_string(self, idx: int) -> str:
         """
         Get a specific string by using an index
 
         :param idx: index of the string
         :type idx: int
         """
         return self.CM.get_raw_string(idx)
 
-    def get_cm_type(self, idx):
+    def get_cm_type(self, idx: int) -> str:
         """
         Get a specific type by using an index
 
         :param idx: index of the type
         :type idx: int
         """
         return self.CM.get_type(idx)
 
-    def get_classes_names(self, update=False):
+    def get_classes_names(self, update:bool=False) -> list[str]:
         """
         Return the names of classes
 
         :param update: True indicates to recompute the list.
                        Maybe needed after using a MyClass.set_name().
         :rtype: a list of string
         """
         if self.classes_names is None or update:
             self.classes_names = [i.get_name() for i in self.get_classes()]
         return self.classes_names
 
-    def get_classes(self):
+    def get_classes(self) -> list[ClassDefItem]:
         """
         Return all classes
 
         :rtype: a list of :class:`ClassDefItem` objects
         """
         if self.classes:
             return self.classes.class_def
         else:
             # There is a rare case that the DEX has no classes
             return []
 
-    def get_len_classes(self):
+    def get_len_classes(self) -> int:
         """
         Return the number of classes
 
         :rtype: int
         """
         return len(self.get_classes())
 
-    def get_class(self, name):
+    def get_class(self, name: str) -> Union[ClassDefItem, None]:
         """
         Return a specific class
 
         :param name: the name of the class
 
         :rtype: a :class:`ClassDefItem` object
         """
         for i in self.get_classes():
             if i.get_name() == name:
                 return i
         return None
 
-    def get_field(self, name):
+    def get_field(self, name: str) -> list[FieldIdItem]:
         """get field id item by name
 
         :param name: the name of the field (a python regexp)
         :type name: str
         :return: the list of matching :class:`FieldIdItem` objects
         :rtype: list
         """
@@ -7997,34 +7999,34 @@
         prog = re.compile(name)
         l = []
         for i in self.get_fields():
             if prog.match(i.name):
                 l.append(i)
         return l
 
-    def get_fields(self):
+    def get_fields(self) -> list[FieldIdItem]:
         """
         Return a list of field items
 
         :rtype: a list of :class:`FieldIdItem` objects
         """
         try:
             return self.fields.gets()
         except AttributeError:
             return []
 
-    def get_len_fields(self):
+    def get_len_fields(self) -> int:
         """
         Return the number of fields
 
         :rtype: int
         """
         return len(self.get_fields())
 
-    def get_encoded_field(self, name):
+    def get_encoded_field(self, name:str) -> list[EncodedField]:
         """
         Return a list all fields which corresponds to the regexp
 
         :param name: the name of the field (a python regexp)
 
         :rtype: a list with all :class:`EncodedField` objects
         """
@@ -8032,116 +8034,116 @@
         prog = re.compile(name)
         l = []
         for i in self.get_encoded_fields():
             if prog.match(i.get_name()):
                 l.append(i)
         return l
 
-    def get_encoded_fields(self):
+    def get_encoded_fields(self) -> list[EncodedField]:
         """
         Return all field objects
 
         :rtype: a list of :class:`EncodedField` objects
         """
         if self.__cache_all_fields is None:
             self.__cache_all_fields = []
             for i in self.get_classes():
                 for j in i.get_fields():
                     self.__cache_all_fields.append(j)
         return self.__cache_all_fields
 
-    def get_len_encoded_fields(self):
+    def get_len_encoded_fields(self) -> int:
         return len(self.get_encoded_fields())
 
-    def get_field(self, name):
+    def get_field(self, name: str) -> list[FieldIdItem]:
         """get field id item by name
 
         :param name: the name of the field (a python regexp)
         :type name: str
         :return: the list of matching :class:`FieldIdItem` objects
         :rtype: list
         """
         prog = re.compile(name)
         l = []
         for i in self.get_fields():
             if prog.match(i.name):
                 l.append(i)
         return l
 
-    def get_method(self, name):
+    def get_method(self, name: str) -> list[MethodIdItem]:
         """get method id item by name
 
         :param name: the name of the field (a python regexp)
         :type name: str
         :return: the list of matching :class:`MethodIdItem` objects
         :rtype: list
         """
         prog = re.compile(name)
         l = []
         for i in self.get_methods():
             if prog.match(i.name):
                 l.append(i)
         return l
 
-    def get_methods(self):
+    def get_methods(self) -> list[MethodIdItem]:
         """
         Return a list of method items
 
         :rtype: a list of :class:`MethodIdItem` objects
         """
         try:
             return self.methods.gets()
         except AttributeError:
             return []
 
-    def get_len_methods(self):
+    def get_len_methods(self) -> int:
         """
         Return the number of methods
 
         :rtype: int
         """
         return len(self.get_methods())
 
-    def get_encoded_method(self, name):
+    def get_encoded_method(self, name:str) -> list[EncodedMethod]:
         """
         Return a list all encoded methods whose name corresponds to the regexp
 
         :param name: the name of the method (a python regexp)
 
         :rtype: a list with all :class:`EncodedMethod` objects
         """
         prog = re.compile(name)
         l = []
         for i in self.get_encoded_methods():
             if prog.match(i.name):
                 l.append(i)
         return l
 
-    def get_encoded_methods(self):
+    def get_encoded_methods(self) -> list[EncodedMethod]:
         """
         Return all encoded method objects
 
         :rtype: a list of :class:`EncodedMethod` objects
         """
         if self.__cache_all_methods is None:
             self.__cache_all_methods = []
             for i in self.get_classes():
                 for j in i.get_methods():
                     self.__cache_all_methods.append(j)
         return self.__cache_all_methods
 
-    def get_len_encoded_methods(self):
+    def get_len_encoded_methods(self) -> int:
         """
         Return the number of encoded methods
 
         :rtype: int
         """
         return len(self.get_encoded_methods())
 
-    def get_encoded_method_by_idx(self, idx):
+    def get_encoded_method_by_idx(self, idx: int) -> Union[EncodedMethod,None]:
         """
         Return a specific encoded method by using an index
         :param idx: the index of the method
         :type idx: int
 
         :rtype: None or an :class:`EncodedMethod` object
         """
@@ -8152,15 +8154,15 @@
                     self.__cached_methods_idx[j.get_method_idx()] = j
 
         try:
             return self.__cached_methods_idx[idx]
         except KeyError:
             return None
 
-    def get_encoded_method_descriptor(self, class_name, method_name, descriptor):
+    def get_encoded_method_descriptor(self, class_name: str, method_name: str, descriptor: str) -> Union[EncodedMethod,None]:
         """
         Return the specific encoded method given a class name, method name, and descriptor
 
         :param class_name: the class name of the method
         :type class_name: string
         :param method_name: the name of the method
         :type method_name: string
@@ -8176,15 +8178,15 @@
             for i in self.get_classes():
                 for j in i.get_methods():
                     self.__cache_methods[j.get_class_name() + j.get_name() +
                                          j.get_descriptor()] = j
 
         return self.__cache_methods.get(key)
 
-    def get_encoded_methods_class_method(self, class_name, method_name):
+    def get_encoded_methods_class_method(self, class_name: str, method_name: str) -> Union[EncodedMethod,None]:
         """
         Return the specific encoded methods of the class
 
         :param class_name: the class name of the method
         :type class_name: string
         :param method_name: the name of the method
         :type method_name: string
@@ -8192,45 +8194,45 @@
         :rtype: None or a :class:`EncodedMethod` object
         """
         for i in self.get_encoded_methods():
             if i.get_name() == method_name and i.get_class_name() == class_name:
                 return i
         return None
 
-    def get_encoded_methods_class(self, class_name):
+    def get_encoded_methods_class(self, class_name: str) -> list[EncodedMethod]:
         """
         Return all encoded methods of a specific class by class name
 
         :param class_name: the class name
         :type class_name: string
 
         :rtype: a list with :class:`EncodedMethod` objects
         """
         l = []
         for i in self.get_encoded_methods():
             if class_name == i.get_class_name():
                 l.append(i)
         return l
 
-    def get_encoded_fields_class(self, class_name):
+    def get_encoded_fields_class(self, class_name: str) -> list[EncodedField]:
         """
         Return all encoded fields of a specific class by class name
 
         :param class_name: the class name
         :type class_name: string
 
         :rtype: a list with :class:`EncodedField` objects
         """
         l = []
         for i in self.get_encoded_fields():
             if class_name == i.get_class_name():
                 l.append(i)
         return l
 
-    def get_encoded_field_descriptor(self, class_name, field_name, descriptor):
+    def get_encoded_field_descriptor(self, class_name: str, field_name: str, descriptor: str) -> EncodedField:
         """
         Return the specific encoded field given a class name, field name, and descriptor
 
         :param class_name: the class name of the field
         :type class_name: string
         :param field_name: the name of the field
         :type field_name: string
@@ -8247,87 +8249,87 @@
             for i in self.get_classes():
                 for j in i.get_fields():
                     self.__cache_fields[j.get_class_name() + j.get_name() +
                                         j.get_descriptor()] = j
 
         return self.__cache_fields.get(key)
 
-    def get_strings(self):
+    def get_strings(self) -> list[str]:
         """
         Return all strings
 
         The strings will have escaped surrogates, if only a single high or low surrogate is found.
         Complete surrogates are put together into the representing 32bit character.
 
         :rtype: a list with all strings used in the format (types, names ...)
         """
         return [i.get() for i in self.strings]
 
-    def get_len_strings(self):
+    def get_len_strings(self) -> int:
         """
         Return the number of strings
 
         :rtype: int
         """
         return len(self.get_strings())
 
-    def get_regex_strings(self, regular_expressions):
+    def get_regex_strings(self, regular_expressions: str) -> Union[list[str],None]:
         """
         Return all target strings matched the regex
 
-        :param regular_expressions: the python regex
+        :param regular_expressions: the python regex string
         :type regular_expressions: string
 
         :rtype: a list of strings matching the regex expression
         """
         str_list = []
         if regular_expressions.count is None:
             return None
         for i in self.get_strings():
             if re.match(regular_expressions, i):
                 str_list.append(i)
         return str_list
 
-    def get_format_type(self):
+    def get_format_type(self) -> str:
         """
         Return the type
 
         :rtype: a string
         """
         return "DEX"
 
-    def create_python_export(self):
+    def create_python_export(self) -> None:
         """
         Export classes/methods/fields' names in the python namespace
         """
         logger.debug("Exporting Python objects")
         setattr(self, "C", ExportObject())
 
         for _class in self.get_classes():
             self._create_python_export_class(_class)
 
-    def _delete_python_export_class(self, _class):
+    def _delete_python_export_class(self, _class: ClassDefItem) -> None:
         self._create_python_export_class(_class, True)
 
-    def _create_python_export_class(self, _class, delete=False):
+    def _create_python_export_class(self, _class: ClassDefItem, delete:bool=False) -> None:
         if _class is not None:
             ### Class
             name = str(bytecode.FormatClassToPython(_class.get_name()))
             if delete:
                 delattr(self.C, name)
                 return
             else:
                 setattr(self.C, name, _class)
                 setattr(_class, "M", ExportObject())
                 setattr(_class, "F", ExportObject())
 
             self._create_python_export_methods(_class, delete)
             self._create_python_export_fields(_class, delete)
 
-    def _create_python_export_methods(self, _class, delete):
+    def _create_python_export_methods(self, _class: ClassDefItem, delete) -> None:
         m = {}
         for method in _class.get_methods():
             if method.get_name() not in m:
                 m[method.get_name()] = []
             m[method.get_name()].append(method)
             setattr(method, "XF", ExportObject())
             setattr(method, "XT", ExportObject())
@@ -8340,15 +8342,15 @@
             else:
                 for j in m[i]:
                     name = (
                         str(bytecode.FormatNameToPython(j.get_name())) + "_" +
                         str(bytecode.FormatDescriptorToPython(j.get_descriptor())))
                     setattr(_class.M, name, j)
 
-    def _create_python_export_fields(self, _class, delete):
+    def _create_python_export_fields(self, _class: ClassDefItem, delete) -> None:
         f = {}
         for field in _class.get_fields():
             if field.get_name() not in f:
                 f[field.get_name()] = []
             f[field.get_name()].append(field)
             setattr(field, "XR", ExportObject())
             setattr(field, "XW", ExportObject())
@@ -8361,41 +8363,41 @@
             else:
                 for j in f[i]:
                     name = str(bytecode.FormatNameToPython(j.get_name(
                     ))) + "_" + str(bytecode.FormatDescriptorToPython(
                         j.get_descriptor()))
                     setattr(_class.F, name, j)
 
-    def set_decompiler(self, decompiler):
+    def set_decompiler(self, decompiler: DecompilerDAD) -> None:
         self.CM.set_decompiler(decompiler)
 
-    def set_analysis(self, analysis_dex):
+    def set_analysis(self, analysis_dex: Analysis) -> None:
         self.CM.set_analysis(analysis_dex)
 
-    def disassemble(self, offset, size):
+    def disassemble(self, offset: int, size: int) -> Iterator[Instruction]:
         """
         Disassembles a given offset in the DEX file
 
         :param offset: offset to disassemble in the file (from the beginning of the file)
         :type offset: int
         :param size:
         :type size:
         """
         for i in DCode(
                 self.CM, offset, size,
                 read_at(self.raw, offset, size)).get_instructions():
             yield i
 
-    def _get_class_hierarchy(self):
+    def _get_class_hierarchy(self) -> Node:
         """
         Constructs a tree out of all the classes.
         The classes are added to this tree by their superclass.
 
         :return:
-        :rtype: androguard.core.bytecode.Node
+        :rtype: androguard.decompiler.Node
         """
         # Contains the class names as well as their running number
         ids = dict()
         present = dict()
         r_ids = dict()
         to_add = dict()
         els = []
@@ -8434,15 +8436,15 @@
 
             if not parentId in treeMap:
                 treeMap[parentId] = bytecode.Node(0, '')
             treeMap[parentId].children.append(treeMap[nodeId])
 
         return Root
 
-    def list_classes_hierarchy(self):
+    def list_classes_hierarchy(self) -> dict[str, list[dict[str, list]]]:
         """
         Get a tree structure of the classes.
         The parent is always the superclass.
 
         You can use pprint.pprint to print the
         dictionary in a pretty way.
 
@@ -8471,32 +8473,32 @@
 class OdexHeaderItem:
     """
     This class can parse the odex header
 
     :param buff: a Buff object string which represents the odex dependencies
     """
 
-    def __init__(self, buff):
+    def __init__(self, buff: BinaryIO) -> None:
         buff.seek(8)
 
         self.dex_offset = unpack("=I", buff.read(4))[0]
         self.dex_length = unpack("=I", buff.read(4))[0]
         self.deps_offset = unpack("=I", buff.read(4))[0]
         self.deps_length = unpack("=I", buff.read(4))[0]
         self.aux_offset = unpack("=I", buff.read(4))[0]
         self.aux_length = unpack("=I", buff.read(4))[0]
         self.flags = unpack("=I", buff.read(4))[0]
         self.padding = unpack("=I", buff.read(4))[0]
 
-    def show(self):
+    def show(self) -> None:
         print("dex_offset:{:x} dex_length:{:x} deps_offset:{:x} deps_length:{:x} aux_offset:{:x} aux_length:{:x} flags:{:x}".format(
             self.dex_offset, self.dex_length, self.deps_offset,
             self.deps_length, self.aux_offset, self.aux_length, self.flags))
 
-    def get_raw(self):
+    def get_raw(self)  -> bytes:
         return pack("=I", self.dex_offset) + \
                pack("=I", self.dex_length) + \
                pack("=I", self.deps_offset) + \
                pack("=I", self.deps_length) + \
                pack("=I", self.aux_offset) + \
                pack("=I", self.aux_length) + \
                pack("=I", self.flags) + \
@@ -8506,37 +8508,37 @@
 class OdexDependencies:
     """
     This class can parse the odex dependencies
 
     :param buff: a Buff object string which represents the odex dependencies
     """
 
-    def __init__(self, buff):
+    def __init__(self, buff: BinaryIO) -> None:
         self.modification_time = unpack("=I", buff.read(4))[0]
         self.crc = unpack("=I", buff.read(4))[0]
         self.dalvik_build = unpack("=I", buff.read(4))[0]
         self.dependency_count = unpack("=I", buff.read(4))[0]
         self.dependencies = []
         self.dependency_checksums = []
 
         for i in range(0, self.dependency_count):
             string_length = unpack("=I", buff.read(4))[0]
             name_dependency = buff.read(string_length)
             self.dependencies.append(name_dependency)
             self.dependency_checksums.append(buff.read(20))
 
-    def get_dependencies(self):
+    def get_dependencies(self) -> list[str]:
         """
             Return the list of dependencies
 
             :rtype: a list of strings
         """
         return self.dependencies
 
-    def get_raw(self):
+    def get_raw(self) -> bytes:
         dependencies = b""
 
         for idx, value in enumerate(self.dependencies):
             dependencies += pack("=I", len(value)) + \
                             pack("=%ds" % len(value), value) + \
                             pack("=20s", self.dependency_checksums[idx])
 
@@ -8547,24 +8549,24 @@
                dependencies
 
 
 class ODEX(DEX):
     """
         This class can parse an odex file
 
-        :param buff: a string which represents the odex file
+        :param buff: byteswhich represents the odex file
         :param decompiler: associate a decompiler object to display the java source code
-        :type buff: string
+        :type buff: bytes
         :type decompiler: object
 
         :Example:
           ODEX( read("classes.odex") )
     """
 
-    def _preload(self, buff):
+    def _preload(self, buff: BinaryIO):
         self.orig_buff = buff
         self.magic = buff[:8]
         if self.magic in (ODEX_FILE_MAGIC_35, ODEX_FILE_MAGIC_36, ODEX_FILE_MAGIC_37):
             self.odex_header = OdexHeaderItem(self)
 
             self.seek(self.odex_header.deps_offset)
             self.dependencies = OdexDependencies(self)
@@ -8572,43 +8574,43 @@
             self.padding = buff[self.odex_header.deps_offset +
                                 self.odex_header.deps_length:]
 
             self.seek(self.odex_header.dex_offset)
             self.set_buff(self.read(self.odex_header.dex_length))
             self.seek(0)
 
-    def save(self):
+    def save(self) -> bytes:
         """
           Do not use !
         """
         dex_raw = super().save()
         return self.magic + self.odex_header.get_raw(
         ) + dex_raw + self.dependencies.get_raw() + self.padding
 
-    def get_buff(self):
+    def get_buff(self) -> bytes:
         return self.magic + self.odex_header.get_raw() + super().get_buff() + self.dependencies.get_raw() + self.padding
 
-    def get_dependencies(self):
+    def get_dependencies(self) -> OdexDependencies:
         """
             Return the odex dependencies object
 
             :rtype: an OdexDependencies object
         """
         return self.dependencies
 
-    def get_format_type(self):
+    def get_format_type(self) -> str:
         """
             Return the type
 
             :rtype: a string
         """
         return "ODEX"
 
 
-def get_params_info(nb, proto):
+def get_params_info(nb: int, proto: str) -> str:
     i_buffer = "# Parameters:\n"
 
     ret = proto.split(')')
     params = ret[0][1:].split()
     if params:
         i_buffer += "# - local registers: v%d...v%d\n" % (0,
                                                           nb - len(params) - 1)
@@ -8620,20 +8622,20 @@
         i_buffer += "# local registers: v%d...v%d\n" % (0, nb - 1)
 
     i_buffer += "#\n# - return:%s\n\n" % get_type(ret[1])
 
     return i_buffer
 
 
-def get_bytecodes_method(dex_object, ana_object, method):
-    mx = ana_object.get_method(method)
+def get_bytecodes_method(dex_object, analysis_object: Analysis, method: EncodedMethod) -> str:
+    mx = analysis_object.get_method(method)
     return get_bytecodes_methodx(method, mx)
 
 
-def get_bytecodes_methodx(method, mx):
+def get_bytecodes_methodx(method: EncodedMethod, mx: MethodAnalysis) -> str:
     basic_blocks = mx.basic_blocks.gets()
     i_buffer = ""
 
     idx = 0
     nb = 0
 
     i_buffer += "# {}->{}{} [access_flags={}]\n#\n".format(
```

### Comparing `androguard-4.1.1/androguard/core/dex/dex_types.py` & `androguard-4.1.2/androguard/core/dex/dex_types.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/resources/public.json` & `androguard-4.1.2/androguard/core/resources/public.json`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/resources/public.py` & `androguard-4.1.2/androguard/core/resources/public.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/core/resources/public.xml` & `androguard-4.1.2/androguard/core/resources/public.xml`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/decompiler/basic_blocks.py` & `androguard-4.1.2/androguard/decompiler/basic_blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,51 +12,52 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS-IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections import defaultdict
+
 from androguard.decompiler.opcode_ins import INSTRUCTION_SET
 from androguard.decompiler.instruction import MoveExceptionExpression
 from androguard.decompiler.node import Node
 from androguard.decompiler.util import get_type
 
 from loguru import logger
 
 
 class BasicBlock(Node):
-    def __init__(self, name, block_ins):
+    def __init__(self, name: str, block_ins: list) -> None:
         super().__init__(name)
         self.ins = block_ins
         self.ins_range = None
         self.loc_ins = None
         self.var_to_declare = set()
         self.catch_type = None
 
-    def get_ins(self):
+    def get_ins(self) -> list:
         return self.ins
 
-    def get_loc_with_ins(self):
+    def get_loc_with_ins(self) -> list:
         if self.loc_ins is None:
             self.loc_ins = list(zip(range(*self.ins_range), self.ins))
         return self.loc_ins
 
-    def remove_ins(self, loc, ins):
+    def remove_ins(self, loc, ins) -> None:
         self.ins.remove(ins)
         self.loc_ins.remove((loc, ins))
 
-    def add_ins(self, new_ins_list):
+    def add_ins(self, new_ins_list: list) -> None:
         for new_ins in new_ins_list:
             self.ins.append(new_ins)
 
     def add_variable_declaration(self, variable):
         self.var_to_declare.add(variable)
 
-    def number_ins(self, num):
+    def number_ins(self, num: int) -> int:
         last_ins_num = num + len(self.ins)
         self.ins_range = [num, last_ins_num]
         self.loc_ins = None
         return last_ins_num
 
     def set_catch_type(self, _type):
         self.catch_type = _type
```

### Comparing `androguard-4.1.1/androguard/decompiler/control_flow.py` & `androguard-4.1.2/androguard/decompiler/control_flow.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/decompiler/dast.py` & `androguard-4.1.2/androguard/decompiler/dast.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from androguard.decompiler import basic_blocks, instruction, opcode_ins
 from androguard.core.dex.dex_types import TYPE_DESCRIPTOR
 
 from loguru import logger
 
 
-def array_access(arr, ind):
+def array_access(arr, ind) -> list:
     return ['ArrayAccess', [arr, ind]]
 
 
 def array_creation(tn, params, dim):
     return ['ArrayCreation', [tn] + params, dim]
 
 
@@ -64,15 +64,15 @@
     return ['MethodInvocation', [base] + params, triple, name, True]
 
 
 def parenthesis(expr):
     return ['Parenthesis', [expr]]
 
 
-def typen(baset, dim):
+def typen(baset: str, dim: int) -> list:
     return ['TypeName', (baset, dim)]
 
 
 def unary_prefix(op, left):
     return ['Unary', [left], op, False]
 
 
@@ -137,15 +137,15 @@
 # Add a statement to the end of a statement block
 def _append(sb, stmt):
     assert (sb[0] == 'BlockStatement')
     if stmt is not None:
         sb[2].append(stmt)
 
 
-def parse_descriptor(desc):
+def parse_descriptor(desc: str) -> list:
     dim = 0
     while desc and desc[0] == '[':
         desc = desc[1:]
         dim += 1
 
     if desc in TYPE_DESCRIPTOR:
         return typen('.' + TYPE_DESCRIPTOR[desc], dim)
```

### Comparing `androguard-4.1.1/androguard/decompiler/dataflow.py` & `androguard-4.1.2/androguard/decompiler/dataflow.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/decompiler/decompile.py` & `androguard-4.1.2/androguard/decompiler/decompile.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS-IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# Allows type hinting of types not-yet-declared
+# in Python >= 3.7
+# see https://peps.python.org/pep-0563/
+from __future__ import annotations
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from androguard.core.analysis.analysis import Analysis, MethodAnalysis
+    from androguard.core.dex import EncodedField
+
 import struct
 import sys
 from collections import defaultdict
 
 from loguru import logger
 
 import androguard.core.androconf as androconf
@@ -44,15 +53,15 @@
 from androguard.decompiler.instruction import Param, ThisParam
 from androguard.decompiler.writer import Writer
 from androguard.util import readFile
 
 logger.add(sys.stderr, format="{time} {level} {message}", filter="dad", level="INFO")
 
 # No seperate DvField class currently
-def get_field_ast(field):
+def get_field_ast(field: EncodedField) -> dict:
     triple = field.get_class_name()[1:-1], field.get_name(), field.get_descriptor()
 
     expr = None
     if field.init_value:
         val = field.init_value.value
         expr = dummy(str(val))
 
@@ -69,19 +78,19 @@
         'expr': expr,
     }
 
 
 class DvMethod:
     """
     This is a wrapper around :class:`~androguard.core.analysis.analysis.MethodAnalysis` and
-    :class:`~androguard.core.bytecodes.dvm.EncodedMethod` inside the decompiler.
+    :class:`~androguard.core.dex.EncodedMethod` inside the decompiler.
 
     :param androguard.core.analysis.analysis.MethodAnalysis methanalysis:
     """
-    def __init__(self, methanalysis):
+    def __init__(self, methanalysis: MethodAnalysis) -> None:
         method = methanalysis.get_method()
         self.method = method
         self.start_block = next(methanalysis.get_basic_blocks().get(), None)
         self.cls_name = method.get_class_name()
         self.name = method.get_name()
         self.lparams = []
         self.var_to_name = defaultdict()
@@ -115,15 +124,15 @@
                 num_param += util.get_type_size(ptype)
 
         if not __debug__:
             from androguard.core import bytecode
             # TODO: use tempfile to create a correct tempfile (cross platform compatible)
             bytecode.method2png('/tmp/dad/graphs/{}#{}.png'.format(self.cls_name.split('/')[-1][:-1], self.name), methanalysis)
 
-    def process(self, doAST=False):
+    def process(self, doAST:bool=False) -> None:
         """
         Processes the method and decompile the code.
 
         There are two modes of operation:
 
         1) Normal Decompilation to Java Code
         2) Decompilation into an abstract syntax tree (AST)
@@ -189,15 +198,15 @@
 
         if doAST:
             self.ast = JSONWriter(graph, self).get_ast()
         else:
             self.writer = Writer(graph, self)
             self.writer.write_method()
 
-    def get_ast(self):
+    def get_ast(self) -> dict:
         """
         Returns the AST, if previously was generated by calling :meth:`process` with argument :code:`doAST=True`.
 
         The AST is a :class:`dict` with the following keys:
 
         * triple
         * flags
@@ -208,43 +217,43 @@
 
         The actual AST for the method is in the :code:`body`.
 
         :return: dict
         """
         return self.ast
 
-    def show_source(self):
+    def show_source(self) -> None:
         print(self.get_source())
 
-    def get_source(self):
+    def get_source(self) -> str:
         if self.writer:
             return str(self.writer)
         return ''
 
-    def get_source_ext(self):
+    def get_source_ext(self) -> list[tuple]:
         if self.writer:
             return self.writer.str_ext()
         return []
 
     def __repr__(self):
         # return 'Method %s' % self.name
         return '<class DvMethod(object): %s>' % self.name
 
 
 class DvClass:
     """
     This is a wrapper for :class:`~androguard.core.bytecodes.dvm.ClassDefItem` inside the decompiler.
 
-    At first, :py:attr:`methods` contains a list of :class:`~androguard.core.bytecodes.dvm.EncodedMethods`,
+    At first, :py:attr:`methods` contains a list of :class:`~androguard.core.dex.EncodedMethod`,
     which are successively replaced by :class:`DvMethod` in the process of decompilation.
 
-    :param androguard.core.bytecodes.dvm.ClassDefItem dvclass: the class item
+    :param androguard.core.dex.ClassDefItem dvclass: the class item
     :param androguard.core.analysis.analysis.Analysis vma: an Analysis object
     """
-    def __init__(self, dvclass, vma):
+    def __init__(self, dvclass: dex.ClassDefItem, vma: analysis.Analysis) -> None:
         name = dvclass.get_name()
         if name.find('/') > 0:
             pckg, name = name.rsplit('/', 1)
         else:
             pckg, name = '', name
         self.package = pckg[1:].replace('/', '.')
         self.name = name[:-1]
@@ -273,34 +282,34 @@
 
         logger.debug('Class : %s', self.name)
         logger.debug('Methods added :')
         for meth in self.methods:
             logger.debug('%s (%s, %s)', meth.get_method_idx(), self.name, meth.name)
         logger.debug('')
 
-    def get_methods(self):
+    def get_methods(self) -> list[dex.EncodedMethod]:
         return self.methods
 
-    def process_method(self, num, doAST=False):
+    def process_method(self, num: int, doAST:bool=False) -> None:
         method = self.methods[num]
         if not isinstance(method, DvMethod):
             self.methods[num] = DvMethod(self.vma.get_method(method))
             self.methods[num].process(doAST=doAST)
         else:
             method.process(doAST=doAST)
 
-    def process(self, doAST=False):
+    def process(self, doAST:bool=False) -> None:
         for i in range(len(self.methods)):
             try:
                 self.process_method(i, doAST=doAST)
             except Exception as e:
                 # FIXME: too broad exception?
                 logger.warning('Error decompiling method %s: %s', self.methods[i], e)
 
-    def get_ast(self):
+    def get_ast(self) -> dict:
         fields = [get_field_ast(f) for f in self.fields]
         methods = []
         for m in self.methods:
             if isinstance(m, DvMethod) and m.ast:
                 methods.append(m.get_ast())
         isInterface = 'interface' in self.access
         return {
@@ -310,15 +319,15 @@
             'flags': self.access,
             'isInterface': isInterface,
             'interfaces': list(map(parse_descriptor, self.interfaces)),
             'fields': fields,
             'methods': methods,
         }
 
-    def get_source(self):
+    def get_source(self) -> str:
         source = []
         if not self.inner and self.package:
             source.append('package %s;\n' % self.package)
 
         superclass, prototype = self.superclass, self.prototype
         if superclass is not None and superclass != 'Ljava/lang/Object;':
             superclass = superclass[1:-1].replace('/', '.')
@@ -358,15 +367,15 @@
         for method in self.methods:
             if isinstance(method, DvMethod):
                 source.append(method.get_source())
 
         source.append('}\n')
         return ''.join(source)
 
-    def get_source_ext(self):
+    def get_source_ext(self) -> list[tuple[str, list]]:
         source = []
         if not self.inner and self.package:
             source.append(
                 ('PACKAGE', [('PACKAGE_START', 'package '), (
                     'NAME_PACKAGE', '%s' % self.package), ('PACKAGE_END', ';\n')
                              ]))
         list_proto = [('PROTOTYPE_ACCESS', '%s class ' % ' '.join(self.access)),
@@ -430,33 +439,33 @@
 
         for method in self.methods:
             if isinstance(method, DvMethod):
                 source.append(("METHOD", method.get_source_ext()))
         source.append(("CLASS_END", [('CLASS_END', '}\n')]))
         return source
 
-    def show_source(self):
+    def show_source(self) -> None:
         print(self.get_source())
 
     def __repr__(self):
         return '<Class(%s)>' % self.name
 
 
 class DvMachine:
     """
     Wrapper class for a Dalvik Object, like a DEX or ODEX file.
 
     The wrapper allows to take a Dalvik file and get a list of Classes out of it.
     The :class:`~androguard.decompiler.decompile.DvMachine` can take either an APK file directly,
     where all DEX files from the multidex are used, or a single DEX or ODEX file as an argument.
 
-    At first, :py:attr:`classes` contains only :class:`~androguard.core.bytecodes.dvm.ClassDefItem` as values.
+    At first, :py:attr:`classes` contains only :class:`~androguard.core.dex.ClassDefItem` as values.
     Then these objects are replaced by :class:`DvClass` items successively.
     """
-    def __init__(self, name):
+    def __init__(self, name: str) -> None:
         """
 
         :param name: filename to load
         """
         self.vma = analysis.Analysis()
 
         # Proper detection which supports multidex inside APK
@@ -471,78 +480,78 @@
         else:
             raise ValueError("Format not recognised for filename '%s'" % name)
 
         self.classes = {dvclass.orig_class.get_name(): dvclass.orig_class for dvclass in self.vma.get_classes()}
         # TODO why not?
         # util.merge_inner(self.classes)
 
-    def get_classes(self):
+    def get_classes(self) -> list[str]:
         """
         Return a list of classnames contained in this machine.
         The format of each name is Lxxx;
 
         :return: list of class names
         """
         return list(self.classes.keys())
 
-    def get_class(self, class_name):
+    def get_class(self, class_name: str) -> DvClass:
         """
         Return the :class:`DvClass` with the given name
 
         The name is partially matched against the known class names and the first result is returned.
         For example, the input `foobar` will match on Lfoobar/bla/foo;
 
         :param str class_name:
         :return: the class matching on the name
-        :rtype: DvClass
+        :rtype: :class:`DvClass`
         """
         for name, klass in self.classes.items():
             # TODO why use the name partially?
             if class_name in name:
                 if isinstance(klass, DvClass):
                     return klass
                 dvclass = self.classes[name] = DvClass(klass, self.vma)
                 return dvclass
 
-    def process(self):
+    def process(self) -> None:
         """
         Process all classes inside the machine.
 
         This calls :meth:`~androgaurd.decompiler.decompile.DvClass.process` on each :class:`DvClass`.
         """
         for name, klass in self.classes.items():
             logger.debug('Processing class: %s', name)
             if isinstance(klass, DvClass):
                 klass.process()
             else:
                 dvclass = self.classes[name] = DvClass(klass, self.vma)
                 dvclass.process()
 
-    def show_source(self):
+    def show_source(self) -> None:
         """
         Calls `show_source` on all classes inside the machine.
         This prints the source to stdout.
 
         This calls :meth:`~androgaurd.decompiler.decompile.DvClass.show_source` on each :class:`DvClass`.
         """
         for klass in self.classes.values():
             klass.show_source()
 
-    def process_and_show(self):
+    def process_and_show(self) -> None:
         """
         Run :meth:`process` and :meth:`show_source` after each other.
         """
         for name, klass in sorted(self.classes.items()):
             logger.debug('Processing class: %s', name)
             if not isinstance(klass, DvClass):
                 klass = DvClass(klass, self.vma)
             klass.process()
             klass.show_source()
 
-    def get_ast(self):
+    def get_ast(self) -> dict:
         """
         Processes each class with AST enabled and returns a dictionary with all single ASTs
         Classnames as keys.
 
         :return: an dictionary for all classes
         :rtype: dict
         """
```

### Comparing `androguard-4.1.1/androguard/decompiler/decompiler.py` & `androguard-4.1.2/androguard/decompiler/decompiler.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,78 +11,88 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS-IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# Allows type hinting of types not-yet-declared
+# in Python >= 3.7
+# see https://peps.python.org/pep-0563/
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from androguard.core.analysis.analysis import Analysis, MethodAnalysis
+    from androguard.core.dex import DEX, ClassDefItem
+
 from androguard.decompiler import decompile
 
 from pygments import highlight
 from pygments.lexers import get_lexer_by_name
 from pygments.formatters import TerminalFormatter
 from pygments.token import Token
 
 from loguru import logger
 
 
 class DecompilerDAD:
-    def __init__(self, vm, vmx):
+    def __init__(self, vm: DEX, vmx: Analysis) -> None:
         """
         Decompiler wrapper for DAD: **D**AD is **A** **D**ecompiler
         DAD is the androguard internal decompiler.
 
         This Method does not use the :class:`~androguard.decompiler.decompile.DvMachine` but
         creates :class:`~androguard.decompiler.decompile.DvClass` and
         :class:`~androguard.decompiler.decompile.DvMethod` on demand.
 
-        :param androguard.core.bytecodes.dvm.DEX vm: `DEX` object
+        :param androguard.core.bytecodes.DEX vm: `DEX` object
         :param androguard.core.analysis.analysis.Analysis vmx: `Analysis` object
         """
         self.vm = vm
         self.vmx = vmx
 
-    def get_source_method(self, m):
+    def get_source_method(self, m: MethodAnalysis) -> str:
         mx = self.vmx.get_method(m)
         z = decompile.DvMethod(mx)
         z.process()
         return z.get_source()
 
-    def get_ast_method(self, m):
+    def get_ast_method(self, m: MethodAnalysis) -> dict:
         mx = self.vmx.get_method(m)
         z = decompile.DvMethod(mx)
         z.process(doAST=True)
         return z.get_ast()
 
-    def display_source(self, m):
+    def display_source(self, m: MethodAnalysis) -> None:
         result = self.get_source_method(m)
 
         lexer = get_lexer_by_name("java", stripall=True)
         formatter = TerminalFormatter()
         result = highlight(result, lexer, formatter)
         print(result)
 
-    def get_source_class(self, _class):
+    def get_source_class(self, _class: ClassDefItem) -> str:
         c = decompile.DvClass(_class, self.vmx)
         c.process()
         return c.get_source()
 
-    def get_ast_class(self, _class):
+    def get_ast_class(self, _class: ClassDefItem) -> dict:
         c = decompile.DvClass(_class, self.vmx)
         c.process(doAST=True)
         return c.get_ast()
 
-    def get_source_class_ext(self, _class):
+    def get_source_class_ext(self, _class: ClassDefItem) -> list[tuple[str, list]]:
         c = decompile.DvClass(_class, self.vmx)
         c.process()
 
         result = c.get_source_ext()
 
         return result
 
-    def display_all(self, _class):
+    def display_all(self, _class: ClassDefItem) -> None:
         result = self.get_source_class(_class)
 
         lexer = get_lexer_by_name("java", stripall=True)
         formatter = TerminalFormatter()
         result = highlight(result, lexer, formatter)
         print(result)
```

### Comparing `androguard-4.1.1/androguard/decompiler/graph.py` & `androguard-4.1.2/androguard/decompiler/graph.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/decompiler/instruction.py` & `androguard-4.1.2/androguard/decompiler/instruction.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/decompiler/node.py` & `androguard-4.1.2/androguard/decompiler/node.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/decompiler/opcode_ins.py` & `androguard-4.1.2/androguard/decompiler/opcode_ins.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/decompiler/util.py` & `androguard-4.1.2/androguard/decompiler/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS-IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+# Allows type hinting of types not-yet-declared
+# in Python >= 3.7
+# see https://peps.python.org/pep-0563/
+from __future__ import annotations
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from androguard.decompiler.graph import Graph
+
 from loguru import logger
 
 TYPE_DESCRIPTOR = {
     'V': 'void',
     'Z': 'boolean',
     'B': 'byte',
     'S': 'short',
@@ -73,27 +81,27 @@
 
 ACCESS_ORDER = [0x1, 0x4, 0x2, 0x400, 0x8, 0x10, 0x80, 0x40, 0x20, 0x100, 0x800,
                 0x200, 0x1000, 0x2000, 0x4000, 0x10000, 0x20000]
 
 TYPE_LEN = {'J': 2, 'D': 2, }
 
 
-def get_access_class(access):
+def get_access_class(access: int) -> list[str]:
     sorted_access = [i for i in ACCESS_ORDER if i & access]
     return [ACCESS_FLAGS_CLASSES.get(flag, 'unkn_%d' % flag)
             for flag in sorted_access]
 
 
-def get_access_method(access):
+def get_access_method(access: int) -> list[str]:
     sorted_access = [i for i in ACCESS_ORDER if i & access]
     return [ACCESS_FLAGS_METHODS.get(flag, 'unkn_%d' % flag)
             for flag in sorted_access]
 
 
-def get_access_field(access):
+def get_access_field(access: int) -> list[str]:
     sorted_access = [i for i in ACCESS_ORDER if i & access]
     return [ACCESS_FLAGS_FIELDS.get(flag, 'unkn_%d' % flag)
             for flag in sorted_access]
 
 
 def build_path(graph, node1, node2, path=None):
     """
@@ -161,15 +169,15 @@
 def get_type_size(param):
     """
     Return the number of register needed by the type @param
     """
     return TYPE_LEN.get(param, 1)
 
 
-def get_type(atype, size=None):
+def get_type(atype:str, size:int=None) -> str:
     """
     Retrieve the java type of a descriptor (e.g : I)
     """
     res = TYPE_DESCRIPTOR.get(atype)
     if res is None:
         if atype[0] == 'L':
             if atype.startswith('Ljava/lang'):
@@ -183,25 +191,25 @@
                 res = '{}[{}]'.format(get_type(atype[1:]), size)
         else:
             res = atype
             logger.debug('Unknown descriptor: "%s".', atype)
     return res
 
 
-def get_params_type(descriptor):
+def get_params_type(descriptor: str) -> list[str]:
     """
     Return the parameters type of a descriptor (e.g (IC)V)
     """
     params = descriptor.split(')')[0][1:].split()
     if params:
         return [param for param in params]
     return []
 
 
-def create_png(cls_name, meth_name, graph, dir_name='graphs2'):
+def create_png(cls_name: str, meth_name: str, graph: Graph, dir_name:str='graphs2') -> None:
     """
     Creates a PNG from a given :class:`~androguard.decompiler.graph.Graph`.
 
     :param str cls_name: name of the class
     :param str meth_name: name of the method
     :param androguard.decompiler.graph.Graph graph:
     :param str dir_name: output directory
```

### Comparing `androguard-4.1.1/androguard/decompiler/writer.py` & `androguard-4.1.2/androguard/decompiler/writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self.next_case = None
         self.skip = False
         self.need_break = True
 
     def __str__(self):
         return ''.join([str(i) for i in self.buffer])
 
-    def str_ext(self):
+    def str_ext(self) -> list[tuple]:
         return self.buffer2
 
     def inc_ind(self, i=1):
         self.ind += (4 * i)
 
     def dec_ind(self, i=1):
         self.ind -= (4 * i)
```

### Comparing `androguard-4.1.1/androguard/misc.py` & `androguard-4.1.2/androguard/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,51 @@
+# Allows type hinting of types not-yet-declared
+# in Python >= 3.7
+# see https://peps.python.org/pep-0563/
+from __future__ import annotations
+import hashlib
+import os
+import re
+from typing import Union
+
+from loguru import logger
+
 from androguard.session import Session
 from androguard.decompiler import decompiler
 from androguard.core import androconf
 from androguard.core import apk, dex
 from androguard.core.analysis.analysis import Analysis
 
-import hashlib
-import re
-import os
-from loguru import logger
-
-
-def get_default_session():
+def get_default_session() -> Session:
     """
     Return the default Session from the configuration
     or create a new one, if the session in the configuration is None.
 
     :rtype: androguard.session.Session
     """
     if androconf.CONF["SESSION"] is None:
         androconf.CONF["SESSION"] = Session()
     return androconf.CONF["SESSION"]
 
 
-def AnalyzeAPK(_file, session=None, raw=False):
+def AnalyzeAPK(_file: Union[str,bytes], session:Union[Session,None]=None, raw:bool=False) -> tuple[apk.APK, list[dex.DEX], Analysis]:
     """
     Analyze an android application and setup all stuff for a more quickly
     analysis!
     If session is None, no session is used at all. This is the default
     behaviour.
     If you like to continue your work later, it might be a good idea to use a
     session.
     A default session can be created by using :meth:`~get_default_session`.
 
     :param _file: the filename of the android application or a buffer which represents the application
     :type _file: string (for filename) or bytes (for raw)
     :param session: A session (default: None)
     :param raw: boolean if raw bytes are supplied instead of a filename
-    :rtype: return the :class:`~androguard.core.apk.APK`, list of :class:`~androguard.core.dvm.DEX`, and :class:`~androguard.core.analysis.analysis.Analysis` objects
+    :rtype: return the :class:`~androguard.core.apk.APK`, list of :class:`~androguard.core.dex.DEX`, and :class:`~androguard.core.analysis.analysis.Analysis` objects
     """
     logger.debug("AnalyzeAPK")
 
     if session:
         logger.debug("Using existing session {}".format(session))
         if raw:
             data = _file
@@ -67,15 +72,15 @@
             df.set_decompiler(decompiler.DecompilerDAD(df, dx))
 
         dx.create_xref()
 
         return a, d, dx
 
 
-def AnalyzeDex(filename, session=None, raw=False):
+def AnalyzeDex(filename: str, session:Session=None, raw:bool=False) -> tuple[str, dex.DEX, Analysis]:
     """
     Analyze an android dex file and setup all stuff for a more quickly analysis !
 
     :param filename: the filename of the android dex file or a buffer which represents the dex file
     :type filename: string
     :param session: A session (Default None)
     :param raw: If set, ``filename`` will be used as the odex's data (bytes). Defaults to ``False``
@@ -92,40 +97,40 @@
     else:
         with open(filename, "rb") as fd:
             data = fd.read()
 
     return session.addDEX(filename, data)
 
 
-def AnalyzeODex(filename, session=None, raw=False):
-    """
-    Analyze an android odex file and setup all stuff for a more quickly analysis !
+# def AnalyzeODex(filename: str, session:Session=None, raw:bool=False):
+#     """
+#     Analyze an android odex file and setup all stuff for a more quickly analysis !
 
-    :param filename: the filename of the android dex file or a buffer which represents the dex file
-    :type filename: string
-    :param session: The Androguard Session to add the ODex to (default: None)
-    :param raw: If set, ``filename`` will be used as the odex's data (bytes). Defaults to ``False``
+#     :param filename: the filename of the android dex file or a buffer which represents the dex file
+#     :type filename: string
+#     :param session: The Androguard Session to add the ODex to (default: None)
+#     :param raw: If set, ``filename`` will be used as the odex's data (bytes). Defaults to ``False``
 
-    :rtype: return a tuple of (sha256hash, :class:`DalvikOdexVMFormat`, :class:`Analysis`)
-    """
-    logger.debug("AnalyzeODex")
+#     :rtype: return a tuple of (sha256hash, :class:`DalvikOdexVMFormat`, :class:`Analysis`)
+#     """
+#     logger.debug("AnalyzeODex")
 
-    if not session:
-        session = get_default_session()
+#     if not session:
+#         session = get_default_session()
 
-    if raw:
-        data = filename
-    else:
-        with open(filename, "rb") as fd:
-            data = fd.read()
+#     if raw:
+#         data = filename
+#     else:
+#         with open(filename, "rb") as fd:
+#             data = fd.read()
 
-    return session.addDEY(filename, data)
+#     return session.addDEY(filename, data) # <- this function is missing
 
 
-def clean_file_name(filename, unique=True, replace="_", force_nt=False):
+def clean_file_name(filename: str, unique:bool=True, replace:str="_", force_nt:bool=False) -> str:
     """
     Return a filename version, which has no characters in it which are forbidden.
     On Windows these are for example <, /, ?, ...
 
     The intention of this function is to allow distribution of files to different OSes.
 
     :param filename: string to clean
```

### Comparing `androguard-4.1.1/androguard/pentest/__init__.py` & `androguard-4.1.2/androguard/pentest/__init__.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/internal/utils.js` & `androguard-4.1.2/androguard/pentest/internal/utils.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/binder/intercept_binder.js` & `androguard-4.1.2/androguard/pentest/modules/binder/intercept_binder.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/code_loading/dex.js` & `androguard-4.1.2/androguard/pentest/modules/code_loading/dex.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/code_loading/dyndex.js` & `androguard-4.1.2/androguard/pentest/modules/code_loading/dyndex.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/code_loading/load_class.js` & `androguard-4.1.2/androguard/pentest/modules/code_loading/load_class.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/code_loading/native.js` & `androguard-4.1.2/androguard/pentest/modules/code_loading/native.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/compression/gzip.js` & `androguard-4.1.2/androguard/pentest/modules/compression/gzip.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/encoding/base64.js` & `androguard-4.1.2/androguard/pentest/modules/encoding/base64.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/encryption/cipher.js` & `androguard-4.1.2/androguard/pentest/modules/encryption/cipher.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/file_system/shared_preferences.js` & `androguard-4.1.2/androguard/pentest/modules/file_system/shared_preferences.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/framework/flutter/disable_cert_chain_bypass_v7a.js` & `androguard-4.1.2/androguard/pentest/modules/framework/flutter/disable_cert_chain_bypass_v7a.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/framework/flutter/disable_cert_chain_bypass_v8a.js` & `androguard-4.1.2/androguard/pentest/modules/framework/flutter/disable_cert_chain_bypass_v8a.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/framework/flutter/disable_cert_chain_bypass_x86_64.js` & `androguard-4.1.2/androguard/pentest/modules/framework/flutter/disable_cert_chain_bypass_x86_64.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/helpers/antidebug/binaries.js` & `androguard-4.1.2/androguard/pentest/modules/helpers/antidebug/binaries.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/helpers/antidebug/environment.js` & `androguard-4.1.2/androguard/pentest/modules/helpers/antidebug/environment.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/helpers/antidebug/package.js` & `androguard-4.1.2/androguard/pentest/modules/helpers/antidebug/package.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/helpers/antidebug/process.js` & `androguard-4.1.2/androguard/pentest/modules/helpers/antidebug/process.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/helpers/dump/dexdump.js` & `androguard-4.1.2/androguard/pentest/modules/helpers/dump/dexdump.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/helpers/pinning/ssl.js` & `androguard-4.1.2/androguard/pentest/modules/helpers/pinning/ssl.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/http_communications/uri.js` & `androguard-4.1.2/androguard/pentest/modules/http_communications/uri.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/intents/intents.js` & `androguard-4.1.2/androguard/pentest/modules/intents/intents.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/intents/intents_creation.js` & `androguard-4.1.2/androguard/pentest/modules/intents/intents_creation.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/intents/pending_intents.js` & `androguard-4.1.2/androguard/pentest/modules/intents/pending_intents.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/ipc/ipc.js` & `androguard-4.1.2/androguard/pentest/modules/ipc/ipc.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/sockets/sockets.js` & `androguard-4.1.2/androguard/pentest/modules/sockets/sockets.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/pentest/modules/webviews/webviews.js` & `androguard-4.1.2/androguard/pentest/modules/webviews/webviews.js`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/session.py` & `androguard-4.1.2/androguard/session.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from androguard.core.analysis.analysis import Analysis
+import collections
+import hashlib
+from typing import Union, Iterator
+
+from androguard.core.analysis.analysis import Analysis, StringAnalysis
 from androguard.core import dex, apk
 from androguard.decompiler.decompiler import DecompilerDAD
 from androguard.core import androconf
 
-import hashlib
-import collections
 import dataset
-
 from loguru import logger
 
 
 class Session:
     """
     A Session is able to store in a database, basic information about APK, DEX or ODEX files.
     Additionally, it offers the possibility to store actions done when using the 'pentest' module.
@@ -18,15 +19,15 @@
     NOTE: an attempt to move from pickling to dataset was started here:
     https://github.com/androguard/androguard/commit/4dd0dc8c4b55605af863925faf16e8eb35f13e45
     but is NOT finished!
 
     >>> Should we go back to pickling or proceed further with the dataset ?<<<
     """
 
-    def __init__(self, export_ipython=False):
+    def __init__(self, export_ipython:bool=False) -> None:
         """
         Create a new Session object
 
         :param export_ipython: set to True in order to create attributes for the
         use in iPython
         """
         self._setup_objects()
@@ -40,15 +41,15 @@
         self.table_system = self.db["system"]
 
         self.session_id = len(self.table_session)
 
         self.table_session.insert(dict(id=self.session_id))
         logger.info("Creating new session [{}]".format(self.session_id))
 
-    def save(self, filename=None):
+    def save(self, filename:Union[str,None]=None) -> None:
         """
         Save the current session, see also :func:`~androguard.session.Save`.
         """
         logger.info("Saving the database")
         self.db.commit()
 
     def _setup_objects(self):
@@ -63,29 +64,29 @@
         self.analyzed_vms = collections.OrderedDict()
 
         # Dict of digest and DEX/DalvikOdexFormat
         # Actually not needed, as we have Analysis objects which store the DEX
         # files as well, but we do not remove it here for legacy reasons
         self.analyzed_dex = dict()
 
-    def reset(self):
+    def reset(self) -> None:
         """
         Reset the current session, delete all added files.
         """
         self._setup_objects()
 
-    def isOpen(self):
+    def isOpen(self) -> bool:
         """
         Test if any file was analyzed in this session
 
         :return: `True` if any file was analyzed, `False` otherwise
         """
         return len(self.analyzed_digest) > 0
 
-    def show(self):
+    def show(self) -> None:
         """
         Print information to stdout about the current session.
         Gets all APKs, all DEX files and all Analysis objects.
         """
         print("APKs in Session: {}".format(len(self.analyzed_apk)))
         for d, a in self.analyzed_apk.items():
             print("\t{}: {}".format(d, a))
@@ -102,15 +103,15 @@
         self.table_pentest.insert(
             dict(session_id=str(self.session_id), call=call, callee=callee, params=params, ret=ret))
 
     def insert_system_event(self, call, callee, information, params):
         self.table_system.insert(
             dict(session_id=str(self.session_id), call=call, callee=callee, information=information, params=params))
 
-    def addAPK(self, filename, data):
+    def addAPK(self, filename: str, data:bytes) -> tuple[str, apk.APK]:
         """
         Add an APK file to the Session and run analysis on it.
 
         :param filename: (file)name of APK file
         :param data: binary data of the APK file
         :return: a tuple of SHA256 Checksum and APK Object
         """
@@ -135,15 +136,15 @@
 
         # Postponed
         dx.create_xref()
 
         logger.info("added APK {}:{}".format(filename, digest))
         return digest, newapk
 
-    def addDEX(self, filename, data, dx=None, postpone_xref=False):
+    def addDEX(self, filename: str, data: bytes, dx:Union[Analysis,None]=None, postpone_xref:bool=False) -> tuple[str, dex.DEX, Analysis]:
         """
         Add a DEX file to the Session and run analysis.
 
         :param filename: the (file)name of the DEX file
         :param data: binary data of the dex file
         :param dx: an existing Analysis Object (optional)
         :param postpone_xref: True if no xref shall be created, and will be called manually
@@ -180,15 +181,15 @@
 
         if self.export_ipython:
             logger.debug("Exporting in ipython")
             d.create_python_export()
 
         return digest, d, dx
 
-    def addODEX(self, filename, data, dx=None):
+    def addODEX(self, filename:str, data:bytes, dx:Union[Analysis,None]=None) -> tuple[str, dex.ODEX, Analysis]:
         """
         Add an ODEX file to the session and run the analysis
         """
         digest = hashlib.sha256(data).hexdigest()
         logger.info("add ODEX:%s" % digest)
 
         self.table_information.insert(
@@ -216,15 +217,15 @@
             d.set_decompiler(DecompilerDAD(d, dx))
             d.set_vmanalysis(dx)
 
         self.analyzed_vms[digest] = dx
 
         return digest, d, dx
 
-    def add(self, filename, raw_data=None, dx=None):
+    def add(self, filename: str, raw_data:Union[bytes,None]=None, dx:Union[Analysis,None]=None) -> Union[str,None]:
         """
         Generic method to add a file to the session.
 
         This is the main method to use when adding files to a Session!
 
         If an APK file is supplied, all DEX files are analyzed too.
         For DEX and ODEX files, only this file is analyzed (what else should be
@@ -254,49 +255,49 @@
         elif ret == "DEY":
             digest, _, _ = self.addODEX(filename, raw_data, dx)
         else:
             return None
 
         return digest
 
-    def get_classes(self):
+    def get_classes(self) -> Iterator[tuple[int, str, str, list[dex.ClassDefItem]]]:
         """
         Returns all Java Classes from the DEX objects as an array of DEX files.
         """
         for idx, digest in enumerate(self.analyzed_vms):
             dx = self.analyzed_vms[digest]
             for vm in dx.vms:
                 filename = self.analyzed_digest[digest]
                 yield idx, filename, digest, vm.get_classes()
 
-    def get_analysis(self, current_class):
+    def get_analysis(self, current_class: dex.ClassDefItem) -> Analysis:
         """
         Returns the :class:`~androguard.core.analysis.analysis.Analysis` object
         which contains the `current_class`.
 
         :param current_class: The class to search for
         :type current_class: androguard.core.bytecodes.dvm.ClassDefItem
         :rtype: androguard.core.analysis.analysis.Analysis
         """
         for digest in self.analyzed_vms:
             dx = self.analyzed_vms[digest]
             if dx.is_class_present(current_class.get_name()):
                 return dx
         return None
 
-    def get_format(self, current_class):
+    def get_format(self, current_class: dex.ClassDefItem) -> dex.DEX:
         """
         Returns the :class:`~androguard.core.bytecodes.dvm.DEX` of a
         given :class:`~androguard.core.bytecodes.dvm.ClassDefItem`.
 
         :param current_class: A ClassDefItem
         """
         return current_class.CM.vm
 
-    def get_filename_by_class(self, current_class):
+    def get_filename_by_class(self, current_class: dex.ClassDefItem) -> Union[str,None]:
         """
         Returns the filename of the DEX file where the class is in.
 
         Returns the first filename this class was present.
         For example, if you analyzed an APK, this should return the filename of
         the APK and not of the DEX file.
 
@@ -304,60 +305,60 @@
         :returns: None if class was not found or the filename
         """
         for digest, dx in self.analyzed_vms.items():
             if dx.is_class_present(current_class.get_name()):
                 return self.analyzed_digest[digest]
         return None
 
-    def get_digest_by_class(self, current_class):
+    def get_digest_by_class(self, current_class: dex.ClassDefItem) -> Union[str,None]:
         """
         Return the SHA256 hash of the object containing the ClassDefItem
 
         Returns the first digest this class was present.
         For example, if you analyzed an APK, this should return the digest of
         the APK and not of the DEX file.
         """
         for digest, dx in self.analyzed_vms.items():
             if dx.is_class_present(current_class.get_name()):
                 return digest
         return None
 
-    def get_strings(self):
+    def get_strings(self) -> Iterator[tuple[str, str, dict[str,StringAnalysis]]]:
         """
         Yields all StringAnalysis for all unique Analysis objects
         """
         seen = []
         for digest, dx in self.analyzed_vms.items():
             if dx in seen:
                 continue
             seen.append(dx)
             yield digest, self.analyzed_digest[digest], dx.get_strings_analysis()
 
-    def get_nb_strings(self):
+    def get_nb_strings(self) -> int:
         """
         Return the total number of strings in all Analysis objects
         """
         nb = 0
         seen = []
         for digest, dx in self.analyzed_vms.items():
             if dx in seen:
                 continue
             seen.append(dx)
             nb += len(dx.get_strings_analysis())
         return nb
 
-    def get_all_apks(self):
+    def get_all_apks(self) -> Iterator[tuple[str, apk.APK]]:
         """
         Yields a list of tuples of SHA256 hash of the APK and APK objects
         of all analyzed APKs in the Session.
         """
         for digest, a in self.analyzed_apk.items():
             yield digest, a
 
-    def get_objects_apk(self, filename=None, digest=None):
+    def get_objects_apk(self, filename:Union[str,None]=None, digest:Union[str,None]=None) -> Iterator[tuple[apk.APK, list[dex.DEX], Analysis]]:
         """
         Returns APK, DEX and Analysis of a specified APK.
 
         You must specify either `filename` or `digest`.
         It is possible to use both, but in this case only `digest` is used.
 
         example::
@@ -387,15 +388,15 @@
                 return None, None, None
             digest = digests[0]
 
         a = self.analyzed_apk[digest][0]
         dx = self.analyzed_vms[digest]
         return a, dx.vms, dx
 
-    def get_objects_dex(self):
+    def get_objects_dex(self) -> Iterator[tuple[str, dex.DEX, Analysis]]:
         """
         Yields all dex objects inclduing their Analysis objects
 
         :returns: tuple of (sha256, DEX, Analysis)
         """
         # TODO: there is no variant like get_objects_apk
         for digest, d in self.analyzed_dex.items():
```

### Comparing `androguard-4.1.1/androguard/ui/__init__.py` & `androguard-4.1.2/androguard/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/ui/data_types.py` & `androguard-4.1.2/androguard/ui/data_types.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/ui/filter.py` & `androguard-4.1.2/androguard/ui/filter.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/ui/selection.py` & `androguard-4.1.2/androguard/ui/selection.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/ui/table.py` & `androguard-4.1.2/androguard/ui/table.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/ui/widget/details.py` & `androguard-4.1.2/androguard/ui/widget/details.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/ui/widget/filters.py` & `androguard-4.1.2/androguard/ui/widget/filters.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/ui/widget/frame.py` & `androguard-4.1.2/androguard/ui/widget/frame.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/ui/widget/help.py` & `androguard-4.1.2/androguard/ui/widget/help.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/ui/widget/toolbar.py` & `androguard-4.1.2/androguard/ui/widget/toolbar.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/ui/widget/transactions.py` & `androguard-4.1.2/androguard/ui/widget/transactions.py`

 * *Files identical despite different names*

### Comparing `androguard-4.1.1/androguard/util.py` & `androguard-4.1.2/androguard/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,72 @@
-#  External dependecies
-import asn1crypto
+
 
 import sys
-from loguru import logger
+from typing import Union, BinaryIO
 
+#  External dependecies
+# import asn1crypto
+from asn1crypto.x509 import Name
+from loguru import logger
 
 class MyFilter:
-    def __init__(self, level):
+    def __init__(self, level:int) -> None:
         self.level = level
 
     def __call__(self, record):
         levelno = logger.level(self.level).no
         return record["level"].no >= levelno
 
 
-def set_log(level):
+def set_log(level:int) -> None:
     """
     Sets the log for loguru based on the level being passed.
     The possible values are TRACE, DEBUG, INFO, SUCCESS, WARNING, ERROR, CRITICAL
     """
     logger.remove(0)
     my_filter = MyFilter(level)
     logger.add(sys.stderr, filter=my_filter, level=0)
 
 
 # Stuff that might be useful
 
-def read_at(buff, offset, size=-1):
+def read_at(buff: BinaryIO, offset:int, size:int=-1) -> bytes:
     idx = buff.tell()
     buff.seek(offset)
     d = buff.read(size)
     buff.seek(idx)
     return d
 
 
-def readFile(filename, binary=True):
+def readFile(filename: str, binary:bool=True) -> bytes:
     """
     Open and read a file
     :param filename: filename to open and read
     :param binary: True if the file should be read as binary
     :return: bytes if binary is True, str otherwise
     """
     with open(filename, 'rb' if binary else 'r') as f:
         return f.read()
 
 
-def get_certificate_name_string(name, short=False, delimiter=', '):
+def get_certificate_name_string(name:Union[dict,Name], short:bool=False, delimiter:str=', ') -> str:
     """
     Format the Name type of a X509 Certificate in a human readable form.
 
     :param name: Name object to return the DN from
     :param short: Use short form (default: False)
     :param delimiter: Delimiter string or character between two parts (default: ', ')
 
     :type name: dict or :class:`asn1crypto.x509.Name`
     :type short: boolean
     :type delimiter: str
 
     :rtype: str
     """
-    if isinstance(name, asn1crypto.x509.Name):
+    if isinstance(name, Name):#asn1crypto.x509.Name):
         name = name.native
 
     # For the shortform, we have a lookup table
     # See RFC4514 for more details
     _ = {
         'business_category': ("businessCategory", "businessCategory"),
         'serial_number': ("serialNumber", "serialNumber"),
```

### Comparing `androguard-4.1.1/pyproject.toml` & `androguard-4.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "androguard"
 description = "Androguard is a full python tool to play with Android files."
 authors = ["desnos <desnos@t0t0.fr>"]
-version = "4.1.1"
+version = "4.1.2"
 license = "Apache Licence, Version 2.0"
 readme = "README.md"
 homepage = "https://github.com/androguard/androguard"
 
 packages = [
     { include = "androguard" },
 ]
@@ -23,17 +23,16 @@
 mutf8 = "*"
 dataset = "*"
 frida = "*"
 loguru = "*"
 apkInspector = ">=1.1.7"
 matplotlib = "*"
 networkx = "*"
-PyQt5 = "*"
-PyQt5-Qt5 = {version = "^5.15,!=5.15.11,!=5.15.12"}
 pyyaml = "*"
+oscrypto = ">=1.3.0"
 
 [tool.setuptools.package_data]
 "androguard.core.api_specific_resources" = ["aosp_permissions/*.json", "api_permission_mappings/*.json"]
 "androguard.core.resources" = ["public.xml"]
 
 [tool.poetry.scripts]
 androguard = "androguard.cli.cli:entry_point"
```

### Comparing `androguard-4.1.1/PKG-INFO` & `androguard-4.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: androguard
-Version: 4.1.1
+Version: 4.1.2
 Summary: Androguard is a full python tool to play with Android files.
 Home-page: https://github.com/androguard/androguard
 License: Apache Licence, Version 2.0
 Author: desnos
 Author-email: desnos@t0t0.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: PyQt5
-Requires-Dist: PyQt5-Qt5 (>=5.15,<6.0,!=5.15.11,!=5.15.12)
 Requires-Dist: apkInspector (>=1.1.7)
 Requires-Dist: asn1crypto (>=0.24.0)
 Requires-Dist: click (>=7.0)
 Requires-Dist: colorama (>=0.4.1)
 Requires-Dist: dataset
 Requires-Dist: frida
 Requires-Dist: ipython (>=5.0.0)
 Requires-Dist: loguru
 Requires-Dist: lxml (>=4.3.0)
 Requires-Dist: matplotlib
 Requires-Dist: mutf8
 Requires-Dist: networkx
+Requires-Dist: oscrypto (>=1.3.0)
 Requires-Dist: pydot (>=1.4.1)
 Requires-Dist: pygments (>=2.3.1)
 Requires-Dist: pyyaml
 Description-Content-Type: text/markdown
 
 ![banner](https://raw.githubusercontent.com/androguard/androguard/master/assets/web/androguardwithname.jpg)
```

