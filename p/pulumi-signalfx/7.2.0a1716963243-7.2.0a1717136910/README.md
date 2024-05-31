# Comparing `tmp/pulumi_signalfx-7.2.0a1716963243.tar.gz` & `tmp/pulumi_signalfx-7.2.0a1717136910.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_signalfx-7.2.0a1716963243.tar", last modified: Wed May 29 06:22:31 2024, max compression
+gzip compressed data, was "pulumi_signalfx-7.2.0a1717136910.tar", last modified: Fri May 31 06:44:27 2024, max compression
```

## Comparing `pulumi_signalfx-7.2.0a1716963243.tar` & `pulumi_signalfx-7.2.0a1717136910.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.698932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   169197 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    18519 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/alert_muting_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.702932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/external_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    78469 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    10176 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/token_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.702932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/azure/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    51988 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/azure/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/azure/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.702932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    61667 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    32113 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/dashboard_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    20850 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/data_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    56014 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    17564 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/event_feed_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.702932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/gcp/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34395 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/gcp/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/gcp/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/get_dimension_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    40028 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/heatmap_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/jira/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31138 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/jira/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    59930 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/list_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20439 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    26019 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/view.py
--rw-r--r--   0 runner    (1001) docker     (127)    18836 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/metric_ruleset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/opsgenie/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/opsgenie/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    21592 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/org_token.py
--rw-r--r--   0 runner    (1001) docker     (127)   153891 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/pagerduty/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/pagerduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/pagerduty/get_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/pagerduty/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/servicenow/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/servicenow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26431 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/servicenow/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    39002 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/single_value_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/slack/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/slack/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    16847 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/slo.py
--rw-r--r--   0 runner    (1001) docker     (127)    30799 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/table_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    26819 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/team.py
--rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/text_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    77114 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/time_chart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/victorops/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/victorops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/victorops/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/webhook_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-29 06:22:31.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-29 06:22:31.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 06:22:31.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 06:22:31.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 06:22:31.000000 pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-29 06:22:25.000000 pulumi_signalfx-7.2.0a1716963243/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 06:22:31.706932 pulumi_signalfx-7.2.0a1716963243/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:44:27.176990 pulumi_signalfx-7.2.0a1717136910/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-31 06:44:27.176990 pulumi_signalfx-7.2.0a1717136910/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:44:27.168990 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   170372 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21389 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/alert_muting_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:44:27.172990 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/aws/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/aws/external_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78469 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/aws/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10176 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/aws/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9479 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/aws/token_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:44:27.172990 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/azure/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51988 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/azure/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/azure/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:44:27.172990 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61667 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32113 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/dashboard_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20850 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/data_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56014 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17564 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/event_feed_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:44:27.172990 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/gcp/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34395 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/gcp/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/gcp/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/get_dimension_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40028 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/heatmap_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:44:27.172990 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/jira/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31138 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/jira/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59930 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/list_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:44:27.176990 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/log/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/log/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/log/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20439 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/log/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26019 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/log/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18836 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/metric_ruleset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:44:27.176990 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12007 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/opsgenie/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21592 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/org_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154770 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:44:27.176990 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/pagerduty/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/pagerduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/pagerduty/get_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9709 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/pagerduty/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:44:27.176990 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/servicenow/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/servicenow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26431 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/servicenow/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39002 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/single_value_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:44:27.176990 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/slack/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/slack/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16847 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/slo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30799 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/table_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26819 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/text_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77114 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/time_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:44:27.176990 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/victorops/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/victorops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9572 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/victorops/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/webhook_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:44:27.176990 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-31 06:44:27.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-31 06:44:27.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 06:44:27.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 06:44:27.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 06:44:27.000000 pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-31 06:44:18.000000 pulumi_signalfx-7.2.0a1717136910/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 06:44:27.176990 pulumi_signalfx-7.2.0a1717136910/setup.cfg
```

### Comparing `pulumi_signalfx-7.2.0a1716963243/PKG-INFO` & `pulumi_signalfx-7.2.0a1717136910/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_signalfx
-Version: 7.2.0a1716963243
+Version: 7.2.0a1717136910
 Summary: A Pulumi package for creating and managing SignalFx resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
 Keywords: pulumi,signalfx
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_signalfx-7.2.0a1716963243/README.md` & `pulumi_signalfx-7.2.0a1717136910/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/__init__.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/_inputs.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
     'AlertMutingRuleFilterArgs',
+    'AlertMutingRuleRecurrenceArgs',
     'DashboardChartArgs',
     'DashboardColumnArgs',
     'DashboardEventOverlayArgs',
     'DashboardEventOverlaySourceArgs',
     'DashboardFilterArgs',
     'DashboardGridArgs',
     'DashboardGroupDashboardArgs',
@@ -114,14 +115,51 @@
 
     @property.setter
     def property(self, value: pulumi.Input[str]):
         pulumi.set(self, "property", value)
 
 
 @pulumi.input_type
+class AlertMutingRuleRecurrenceArgs:
+    def __init__(__self__, *,
+                 unit: pulumi.Input[str],
+                 value: pulumi.Input[int]):
+        """
+        :param pulumi.Input[str] unit: The unit of the period. Can be days (d) or weeks (w).
+        :param pulumi.Input[int] value: The amount of time, expressed as an integer, applicable to the unit specified.
+        """
+        pulumi.set(__self__, "unit", unit)
+        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def unit(self) -> pulumi.Input[str]:
+        """
+        The unit of the period. Can be days (d) or weeks (w).
+        """
+        return pulumi.get(self, "unit")
+
+    @unit.setter
+    def unit(self, value: pulumi.Input[str]):
+        pulumi.set(self, "unit", value)
+
+    @property
+    @pulumi.getter
+    def value(self) -> pulumi.Input[int]:
+        """
+        The amount of time, expressed as an integer, applicable to the unit specified.
+        """
+        return pulumi.get(self, "value")
+
+    @value.setter
+    def value(self, value: pulumi.Input[int]):
+        pulumi.set(self, "value", value)
+
+
+@pulumi.input_type
 class DashboardChartArgs:
     def __init__(__self__, *,
                  chart_id: pulumi.Input[str],
                  column: Optional[pulumi.Input[int]] = None,
                  height: Optional[pulumi.Input[int]] = None,
                  row: Optional[pulumi.Input[int]] = None,
                  width: Optional[pulumi.Input[int]] = None):
```

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/_utilities.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/alert_muting_rule.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/log/timeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,367 +3,462 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from . import _utilities
-from . import outputs
-from ._inputs import *
+from .. import _utilities
 
-__all__ = ['AlertMutingRuleArgs', 'AlertMutingRule']
+__all__ = ['TimelineArgs', 'Timeline']
 
 @pulumi.input_type
-class AlertMutingRuleArgs:
+class TimelineArgs:
     def __init__(__self__, *,
-                 description: pulumi.Input[str],
-                 start_time: pulumi.Input[int],
-                 detectors: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 filters: Optional[pulumi.Input[Sequence[pulumi.Input['AlertMutingRuleFilterArgs']]]] = None,
-                 stop_time: Optional[pulumi.Input[int]] = None):
-        """
-        The set of arguments for constructing a AlertMutingRule resource.
-        :param pulumi.Input[str] description: The description for this muting rule
-        :param pulumi.Input[int] start_time: Starting time of an alert muting rule as a Unit time stamp in seconds.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] detectors: A convenience attribute that associated this muting rule with specific detector IDs. Currently, only one ID is supported.
-        :param pulumi.Input[Sequence[pulumi.Input['AlertMutingRuleFilterArgs']]] filters: Filters for this rule. See [Creating muting rules from scratch](https://docs.splunk.com/Observability/alerts-detectors-notifications/mute-notifications.html#rule-from-scratch) for more information.
-        :param pulumi.Input[int] stop_time: Stop time of an alert muting rule as a Unix time stamp in seconds.
-        """
-        pulumi.set(__self__, "description", description)
-        pulumi.set(__self__, "start_time", start_time)
-        if detectors is not None:
-            pulumi.set(__self__, "detectors", detectors)
-        if filters is not None:
-            pulumi.set(__self__, "filters", filters)
-        if stop_time is not None:
-            pulumi.set(__self__, "stop_time", stop_time)
+                 program_text: pulumi.Input[str],
+                 default_connection: Optional[pulumi.Input[str]] = None,
+                 description: Optional[pulumi.Input[str]] = None,
+                 end_time: Optional[pulumi.Input[int]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 start_time: Optional[pulumi.Input[int]] = None,
+                 time_range: Optional[pulumi.Input[int]] = None):
+        """
+        The set of arguments for constructing a Timeline resource.
+        :param pulumi.Input[str] program_text: Signalflow program text for the log timeline. More info at https://dev.splunk.com/observability/docs/.
+        :param pulumi.Input[str] default_connection: The connection that the log timeline uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
+        :param pulumi.Input[str] description: Description of the log timeline.
+        :param pulumi.Input[int] end_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
+        :param pulumi.Input[str] name: Name of the log timeline.
+        :param pulumi.Input[int] start_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
+        :param pulumi.Input[int] time_range: From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
+        """
+        pulumi.set(__self__, "program_text", program_text)
+        if default_connection is not None:
+            pulumi.set(__self__, "default_connection", default_connection)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+        if end_time is not None:
+            pulumi.set(__self__, "end_time", end_time)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if start_time is not None:
+            pulumi.set(__self__, "start_time", start_time)
+        if time_range is not None:
+            pulumi.set(__self__, "time_range", time_range)
+
+    @property
+    @pulumi.getter(name="programText")
+    def program_text(self) -> pulumi.Input[str]:
+        """
+        Signalflow program text for the log timeline. More info at https://dev.splunk.com/observability/docs/.
+        """
+        return pulumi.get(self, "program_text")
+
+    @program_text.setter
+    def program_text(self, value: pulumi.Input[str]):
+        pulumi.set(self, "program_text", value)
+
+    @property
+    @pulumi.getter(name="defaultConnection")
+    def default_connection(self) -> Optional[pulumi.Input[str]]:
+        """
+        The connection that the log timeline uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
+        """
+        return pulumi.get(self, "default_connection")
+
+    @default_connection.setter
+    def default_connection(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_connection", value)
 
     @property
     @pulumi.getter
-    def description(self) -> pulumi.Input[str]:
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        The description for this muting rule
+        Description of the log timeline.
         """
         return pulumi.get(self, "description")
 
     @description.setter
-    def description(self, value: pulumi.Input[str]):
+    def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="startTime")
-    def start_time(self) -> pulumi.Input[int]:
+    @pulumi.getter(name="endTime")
+    def end_time(self) -> Optional[pulumi.Input[int]]:
         """
-        Starting time of an alert muting rule as a Unit time stamp in seconds.
+        Seconds since epoch. Used for visualization. Conflicts with `time_range`.
         """
-        return pulumi.get(self, "start_time")
+        return pulumi.get(self, "end_time")
 
-    @start_time.setter
-    def start_time(self, value: pulumi.Input[int]):
-        pulumi.set(self, "start_time", value)
+    @end_time.setter
+    def end_time(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "end_time", value)
 
     @property
     @pulumi.getter
-    def detectors(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def name(self) -> Optional[pulumi.Input[str]]:
         """
-        A convenience attribute that associated this muting rule with specific detector IDs. Currently, only one ID is supported.
+        Name of the log timeline.
         """
-        return pulumi.get(self, "detectors")
+        return pulumi.get(self, "name")
 
-    @detectors.setter
-    def detectors(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "detectors", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter
-    def filters(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['AlertMutingRuleFilterArgs']]]]:
+    @pulumi.getter(name="startTime")
+    def start_time(self) -> Optional[pulumi.Input[int]]:
         """
-        Filters for this rule. See [Creating muting rules from scratch](https://docs.splunk.com/Observability/alerts-detectors-notifications/mute-notifications.html#rule-from-scratch) for more information.
+        Seconds since epoch. Used for visualization. Conflicts with `time_range`.
         """
-        return pulumi.get(self, "filters")
+        return pulumi.get(self, "start_time")
 
-    @filters.setter
-    def filters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['AlertMutingRuleFilterArgs']]]]):
-        pulumi.set(self, "filters", value)
+    @start_time.setter
+    def start_time(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "start_time", value)
 
     @property
-    @pulumi.getter(name="stopTime")
-    def stop_time(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="timeRange")
+    def time_range(self) -> Optional[pulumi.Input[int]]:
         """
-        Stop time of an alert muting rule as a Unix time stamp in seconds.
+        From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
         """
-        return pulumi.get(self, "stop_time")
+        return pulumi.get(self, "time_range")
 
-    @stop_time.setter
-    def stop_time(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "stop_time", value)
+    @time_range.setter
+    def time_range(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "time_range", value)
 
 
 @pulumi.input_type
-class _AlertMutingRuleState:
+class _TimelineState:
     def __init__(__self__, *,
+                 default_connection: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 detectors: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 effective_start_time: Optional[pulumi.Input[int]] = None,
-                 filters: Optional[pulumi.Input[Sequence[pulumi.Input['AlertMutingRuleFilterArgs']]]] = None,
+                 end_time: Optional[pulumi.Input[int]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 program_text: Optional[pulumi.Input[str]] = None,
                  start_time: Optional[pulumi.Input[int]] = None,
-                 stop_time: Optional[pulumi.Input[int]] = None):
+                 time_range: Optional[pulumi.Input[int]] = None,
+                 url: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering AlertMutingRule resources.
-        :param pulumi.Input[str] description: The description for this muting rule
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] detectors: A convenience attribute that associated this muting rule with specific detector IDs. Currently, only one ID is supported.
-        :param pulumi.Input[Sequence[pulumi.Input['AlertMutingRuleFilterArgs']]] filters: Filters for this rule. See [Creating muting rules from scratch](https://docs.splunk.com/Observability/alerts-detectors-notifications/mute-notifications.html#rule-from-scratch) for more information.
-        :param pulumi.Input[int] start_time: Starting time of an alert muting rule as a Unit time stamp in seconds.
-        :param pulumi.Input[int] stop_time: Stop time of an alert muting rule as a Unix time stamp in seconds.
+        Input properties used for looking up and filtering Timeline resources.
+        :param pulumi.Input[str] default_connection: The connection that the log timeline uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
+        :param pulumi.Input[str] description: Description of the log timeline.
+        :param pulumi.Input[int] end_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
+        :param pulumi.Input[str] name: Name of the log timeline.
+        :param pulumi.Input[str] program_text: Signalflow program text for the log timeline. More info at https://dev.splunk.com/observability/docs/.
+        :param pulumi.Input[int] start_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
+        :param pulumi.Input[int] time_range: From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
+        :param pulumi.Input[str] url: The URL of the log timeline.
         """
+        if default_connection is not None:
+            pulumi.set(__self__, "default_connection", default_connection)
         if description is not None:
             pulumi.set(__self__, "description", description)
-        if detectors is not None:
-            pulumi.set(__self__, "detectors", detectors)
-        if effective_start_time is not None:
-            pulumi.set(__self__, "effective_start_time", effective_start_time)
-        if filters is not None:
-            pulumi.set(__self__, "filters", filters)
+        if end_time is not None:
+            pulumi.set(__self__, "end_time", end_time)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if program_text is not None:
+            pulumi.set(__self__, "program_text", program_text)
         if start_time is not None:
             pulumi.set(__self__, "start_time", start_time)
-        if stop_time is not None:
-            pulumi.set(__self__, "stop_time", stop_time)
+        if time_range is not None:
+            pulumi.set(__self__, "time_range", time_range)
+        if url is not None:
+            pulumi.set(__self__, "url", url)
+
+    @property
+    @pulumi.getter(name="defaultConnection")
+    def default_connection(self) -> Optional[pulumi.Input[str]]:
+        """
+        The connection that the log timeline uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
+        """
+        return pulumi.get(self, "default_connection")
+
+    @default_connection.setter
+    def default_connection(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "default_connection", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        The description for this muting rule
+        Description of the log timeline.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter
-    def detectors(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="endTime")
+    def end_time(self) -> Optional[pulumi.Input[int]]:
         """
-        A convenience attribute that associated this muting rule with specific detector IDs. Currently, only one ID is supported.
+        Seconds since epoch. Used for visualization. Conflicts with `time_range`.
         """
-        return pulumi.get(self, "detectors")
+        return pulumi.get(self, "end_time")
 
-    @detectors.setter
-    def detectors(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "detectors", value)
+    @end_time.setter
+    def end_time(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "end_time", value)
 
     @property
-    @pulumi.getter(name="effectiveStartTime")
-    def effective_start_time(self) -> Optional[pulumi.Input[int]]:
-        return pulumi.get(self, "effective_start_time")
+    @pulumi.getter
+    def name(self) -> Optional[pulumi.Input[str]]:
+        """
+        Name of the log timeline.
+        """
+        return pulumi.get(self, "name")
 
-    @effective_start_time.setter
-    def effective_start_time(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "effective_start_time", value)
+    @name.setter
+    def name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter
-    def filters(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['AlertMutingRuleFilterArgs']]]]:
+    @pulumi.getter(name="programText")
+    def program_text(self) -> Optional[pulumi.Input[str]]:
         """
-        Filters for this rule. See [Creating muting rules from scratch](https://docs.splunk.com/Observability/alerts-detectors-notifications/mute-notifications.html#rule-from-scratch) for more information.
+        Signalflow program text for the log timeline. More info at https://dev.splunk.com/observability/docs/.
         """
-        return pulumi.get(self, "filters")
+        return pulumi.get(self, "program_text")
 
-    @filters.setter
-    def filters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['AlertMutingRuleFilterArgs']]]]):
-        pulumi.set(self, "filters", value)
+    @program_text.setter
+    def program_text(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "program_text", value)
 
     @property
     @pulumi.getter(name="startTime")
     def start_time(self) -> Optional[pulumi.Input[int]]:
         """
-        Starting time of an alert muting rule as a Unit time stamp in seconds.
+        Seconds since epoch. Used for visualization. Conflicts with `time_range`.
         """
         return pulumi.get(self, "start_time")
 
     @start_time.setter
     def start_time(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "start_time", value)
 
     @property
-    @pulumi.getter(name="stopTime")
-    def stop_time(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="timeRange")
+    def time_range(self) -> Optional[pulumi.Input[int]]:
+        """
+        From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
+        """
+        return pulumi.get(self, "time_range")
+
+    @time_range.setter
+    def time_range(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "time_range", value)
+
+    @property
+    @pulumi.getter
+    def url(self) -> Optional[pulumi.Input[str]]:
         """
-        Stop time of an alert muting rule as a Unix time stamp in seconds.
+        The URL of the log timeline.
         """
-        return pulumi.get(self, "stop_time")
+        return pulumi.get(self, "url")
 
-    @stop_time.setter
-    def stop_time(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "stop_time", value)
+    @url.setter
+    def url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "url", value)
 
 
-class AlertMutingRule(pulumi.CustomResource):
+class Timeline(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 default_connection: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 detectors: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 filters: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AlertMutingRuleFilterArgs']]]]] = None,
+                 end_time: Optional[pulumi.Input[int]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 program_text: Optional[pulumi.Input[str]] = None,
                  start_time: Optional[pulumi.Input[int]] = None,
-                 stop_time: Optional[pulumi.Input[int]] = None,
+                 time_range: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        Provides a Splunk Observability Cloud resource for managing alert muting rules. See [Mute Notifications](https://docs.splunk.com/Observability/alerts-detectors-notifications/mute-notifications.html) for more information.
-
-        Splunk Observability Cloud currently allows linking an alert muting rule with only one detector ID. Specifying multiple detector IDs makes the muting rule obsolete.
+        You can add logs data to your Observability Cloud dashboards without turning your logs into metrics first.
 
-        > **WARNING** Splunk Observability Cloud does not allow the start time of a **currently active** muting rule to be modified. Attempting to modify a currently active rule destroys the existing rule and creates a new rule. This might result in the emission of notifications.
+        A log timeline chart displays timeline visualization in a dashboard and shows you in detail what is happening and why.
 
         ## Example
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: The description for this muting rule
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] detectors: A convenience attribute that associated this muting rule with specific detector IDs. Currently, only one ID is supported.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AlertMutingRuleFilterArgs']]]] filters: Filters for this rule. See [Creating muting rules from scratch](https://docs.splunk.com/Observability/alerts-detectors-notifications/mute-notifications.html#rule-from-scratch) for more information.
-        :param pulumi.Input[int] start_time: Starting time of an alert muting rule as a Unit time stamp in seconds.
-        :param pulumi.Input[int] stop_time: Stop time of an alert muting rule as a Unix time stamp in seconds.
+        :param pulumi.Input[str] default_connection: The connection that the log timeline uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
+        :param pulumi.Input[str] description: Description of the log timeline.
+        :param pulumi.Input[int] end_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
+        :param pulumi.Input[str] name: Name of the log timeline.
+        :param pulumi.Input[str] program_text: Signalflow program text for the log timeline. More info at https://dev.splunk.com/observability/docs/.
+        :param pulumi.Input[int] start_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
+        :param pulumi.Input[int] time_range: From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: AlertMutingRuleArgs,
+                 args: TimelineArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Provides a Splunk Observability Cloud resource for managing alert muting rules. See [Mute Notifications](https://docs.splunk.com/Observability/alerts-detectors-notifications/mute-notifications.html) for more information.
+        You can add logs data to your Observability Cloud dashboards without turning your logs into metrics first.
 
-        Splunk Observability Cloud currently allows linking an alert muting rule with only one detector ID. Specifying multiple detector IDs makes the muting rule obsolete.
-
-        > **WARNING** Splunk Observability Cloud does not allow the start time of a **currently active** muting rule to be modified. Attempting to modify a currently active rule destroys the existing rule and creates a new rule. This might result in the emission of notifications.
+        A log timeline chart displays timeline visualization in a dashboard and shows you in detail what is happening and why.
 
         ## Example
 
         :param str resource_name: The name of the resource.
-        :param AlertMutingRuleArgs args: The arguments to use to populate this resource's properties.
+        :param TimelineArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(AlertMutingRuleArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(TimelineArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 default_connection: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 detectors: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 filters: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AlertMutingRuleFilterArgs']]]]] = None,
+                 end_time: Optional[pulumi.Input[int]] = None,
+                 name: Optional[pulumi.Input[str]] = None,
+                 program_text: Optional[pulumi.Input[str]] = None,
                  start_time: Optional[pulumi.Input[int]] = None,
-                 stop_time: Optional[pulumi.Input[int]] = None,
+                 time_range: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = AlertMutingRuleArgs.__new__(AlertMutingRuleArgs)
+            __props__ = TimelineArgs.__new__(TimelineArgs)
 
-            if description is None and not opts.urn:
-                raise TypeError("Missing required property 'description'")
+            __props__.__dict__["default_connection"] = default_connection
             __props__.__dict__["description"] = description
-            __props__.__dict__["detectors"] = detectors
-            __props__.__dict__["filters"] = filters
-            if start_time is None and not opts.urn:
-                raise TypeError("Missing required property 'start_time'")
+            __props__.__dict__["end_time"] = end_time
+            __props__.__dict__["name"] = name
+            if program_text is None and not opts.urn:
+                raise TypeError("Missing required property 'program_text'")
+            __props__.__dict__["program_text"] = program_text
             __props__.__dict__["start_time"] = start_time
-            __props__.__dict__["stop_time"] = stop_time
-            __props__.__dict__["effective_start_time"] = None
-        super(AlertMutingRule, __self__).__init__(
-            'signalfx:index/alertMutingRule:AlertMutingRule',
+            __props__.__dict__["time_range"] = time_range
+            __props__.__dict__["url"] = None
+        super(Timeline, __self__).__init__(
+            'signalfx:log/timeline:Timeline',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            default_connection: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
-            detectors: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            effective_start_time: Optional[pulumi.Input[int]] = None,
-            filters: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AlertMutingRuleFilterArgs']]]]] = None,
+            end_time: Optional[pulumi.Input[int]] = None,
+            name: Optional[pulumi.Input[str]] = None,
+            program_text: Optional[pulumi.Input[str]] = None,
             start_time: Optional[pulumi.Input[int]] = None,
-            stop_time: Optional[pulumi.Input[int]] = None) -> 'AlertMutingRule':
+            time_range: Optional[pulumi.Input[int]] = None,
+            url: Optional[pulumi.Input[str]] = None) -> 'Timeline':
         """
-        Get an existing AlertMutingRule resource's state with the given name, id, and optional extra
+        Get an existing Timeline resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: The description for this muting rule
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] detectors: A convenience attribute that associated this muting rule with specific detector IDs. Currently, only one ID is supported.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AlertMutingRuleFilterArgs']]]] filters: Filters for this rule. See [Creating muting rules from scratch](https://docs.splunk.com/Observability/alerts-detectors-notifications/mute-notifications.html#rule-from-scratch) for more information.
-        :param pulumi.Input[int] start_time: Starting time of an alert muting rule as a Unit time stamp in seconds.
-        :param pulumi.Input[int] stop_time: Stop time of an alert muting rule as a Unix time stamp in seconds.
+        :param pulumi.Input[str] default_connection: The connection that the log timeline uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
+        :param pulumi.Input[str] description: Description of the log timeline.
+        :param pulumi.Input[int] end_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
+        :param pulumi.Input[str] name: Name of the log timeline.
+        :param pulumi.Input[str] program_text: Signalflow program text for the log timeline. More info at https://dev.splunk.com/observability/docs/.
+        :param pulumi.Input[int] start_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
+        :param pulumi.Input[int] time_range: From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
+        :param pulumi.Input[str] url: The URL of the log timeline.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _AlertMutingRuleState.__new__(_AlertMutingRuleState)
+        __props__ = _TimelineState.__new__(_TimelineState)
 
+        __props__.__dict__["default_connection"] = default_connection
         __props__.__dict__["description"] = description
-        __props__.__dict__["detectors"] = detectors
-        __props__.__dict__["effective_start_time"] = effective_start_time
-        __props__.__dict__["filters"] = filters
+        __props__.__dict__["end_time"] = end_time
+        __props__.__dict__["name"] = name
+        __props__.__dict__["program_text"] = program_text
         __props__.__dict__["start_time"] = start_time
-        __props__.__dict__["stop_time"] = stop_time
-        return AlertMutingRule(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["time_range"] = time_range
+        __props__.__dict__["url"] = url
+        return Timeline(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter
-    def description(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="defaultConnection")
+    def default_connection(self) -> pulumi.Output[Optional[str]]:
         """
-        The description for this muting rule
+        The connection that the log timeline uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "default_connection")
 
     @property
     @pulumi.getter
-    def detectors(self) -> pulumi.Output[Optional[Sequence[str]]]:
+    def description(self) -> pulumi.Output[Optional[str]]:
         """
-        A convenience attribute that associated this muting rule with specific detector IDs. Currently, only one ID is supported.
+        Description of the log timeline.
         """
-        return pulumi.get(self, "detectors")
+        return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter(name="effectiveStartTime")
-    def effective_start_time(self) -> pulumi.Output[int]:
-        return pulumi.get(self, "effective_start_time")
+    @pulumi.getter(name="endTime")
+    def end_time(self) -> pulumi.Output[Optional[int]]:
+        """
+        Seconds since epoch. Used for visualization. Conflicts with `time_range`.
+        """
+        return pulumi.get(self, "end_time")
 
     @property
     @pulumi.getter
-    def filters(self) -> pulumi.Output[Optional[Sequence['outputs.AlertMutingRuleFilter']]]:
+    def name(self) -> pulumi.Output[str]:
         """
-        Filters for this rule. See [Creating muting rules from scratch](https://docs.splunk.com/Observability/alerts-detectors-notifications/mute-notifications.html#rule-from-scratch) for more information.
+        Name of the log timeline.
         """
-        return pulumi.get(self, "filters")
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="programText")
+    def program_text(self) -> pulumi.Output[str]:
+        """
+        Signalflow program text for the log timeline. More info at https://dev.splunk.com/observability/docs/.
+        """
+        return pulumi.get(self, "program_text")
 
     @property
     @pulumi.getter(name="startTime")
-    def start_time(self) -> pulumi.Output[int]:
+    def start_time(self) -> pulumi.Output[Optional[int]]:
         """
-        Starting time of an alert muting rule as a Unit time stamp in seconds.
+        Seconds since epoch. Used for visualization. Conflicts with `time_range`.
         """
         return pulumi.get(self, "start_time")
 
     @property
-    @pulumi.getter(name="stopTime")
-    def stop_time(self) -> pulumi.Output[Optional[int]]:
+    @pulumi.getter(name="timeRange")
+    def time_range(self) -> pulumi.Output[Optional[int]]:
+        """
+        From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
+        """
+        return pulumi.get(self, "time_range")
+
+    @property
+    @pulumi.getter
+    def url(self) -> pulumi.Output[str]:
         """
-        Stop time of an alert muting rule as a Unix time stamp in seconds.
+        The URL of the log timeline.
         """
-        return pulumi.get(self, "stop_time")
+        return pulumi.get(self, "url")
```

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/_inputs.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/aws/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/external_integration.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/aws/external_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/integration.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/aws/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/outputs.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/aws/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/aws/token_integration.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/aws/token_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/azure/_inputs.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/azure/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/azure/integration.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/azure/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/azure/outputs.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/azure/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/config/__init__.pyi` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/config/vars.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/dashboard.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/dashboard_group.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/dashboard_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/data_link.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/data_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/detector.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/detector.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/event_feed_chart.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/event_feed_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/gcp/_inputs.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/gcp/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/gcp/integration.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/gcp/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/gcp/outputs.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/gcp/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/get_dimension_values.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/get_dimension_values.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/heatmap_chart.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/heatmap_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/jira/integration.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/jira/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/list_chart.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/list_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/_inputs.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/log/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/outputs.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/log/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/timeline.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/log/view.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,80 +4,102 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from . import outputs
+from ._inputs import *
 
-__all__ = ['TimelineArgs', 'Timeline']
+__all__ = ['ViewArgs', 'View']
 
 @pulumi.input_type
-class TimelineArgs:
+class ViewArgs:
     def __init__(__self__, *,
                  program_text: pulumi.Input[str],
+                 columns: Optional[pulumi.Input[Sequence[pulumi.Input['ViewColumnArgs']]]] = None,
                  default_connection: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  end_time: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
+                 sort_options: Optional[pulumi.Input[Sequence[pulumi.Input['ViewSortOptionArgs']]]] = None,
                  start_time: Optional[pulumi.Input[int]] = None,
                  time_range: Optional[pulumi.Input[int]] = None):
         """
-        The set of arguments for constructing a Timeline resource.
-        :param pulumi.Input[str] program_text: Signalflow program text for the log timeline. More info at https://dev.splunk.com/observability/docs/.
-        :param pulumi.Input[str] default_connection: The connection that the log timeline uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
-        :param pulumi.Input[str] description: Description of the log timeline.
+        The set of arguments for constructing a View resource.
+        :param pulumi.Input[str] program_text: Signalflow program text for the log view. More info at https://developers.signalfx.com/docs/signalflow-overview.
+        :param pulumi.Input[Sequence[pulumi.Input['ViewColumnArgs']]] columns: The column headers to show on the log view.
+        :param pulumi.Input[str] default_connection: The connection that the log view uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
+        :param pulumi.Input[str] description: Description of the log view.
         :param pulumi.Input[int] end_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
-        :param pulumi.Input[str] name: Name of the log timeline.
+        :param pulumi.Input[str] name: Name of the log view.
+        :param pulumi.Input[Sequence[pulumi.Input['ViewSortOptionArgs']]] sort_options: The sorting options configuration to specify if the log view table needs to be sorted in a particular field.
         :param pulumi.Input[int] start_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
         :param pulumi.Input[int] time_range: From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
         """
         pulumi.set(__self__, "program_text", program_text)
+        if columns is not None:
+            pulumi.set(__self__, "columns", columns)
         if default_connection is not None:
             pulumi.set(__self__, "default_connection", default_connection)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if end_time is not None:
             pulumi.set(__self__, "end_time", end_time)
         if name is not None:
             pulumi.set(__self__, "name", name)
+        if sort_options is not None:
+            pulumi.set(__self__, "sort_options", sort_options)
         if start_time is not None:
             pulumi.set(__self__, "start_time", start_time)
         if time_range is not None:
             pulumi.set(__self__, "time_range", time_range)
 
     @property
     @pulumi.getter(name="programText")
     def program_text(self) -> pulumi.Input[str]:
         """
-        Signalflow program text for the log timeline. More info at https://dev.splunk.com/observability/docs/.
+        Signalflow program text for the log view. More info at https://developers.signalfx.com/docs/signalflow-overview.
         """
         return pulumi.get(self, "program_text")
 
     @program_text.setter
     def program_text(self, value: pulumi.Input[str]):
         pulumi.set(self, "program_text", value)
 
     @property
+    @pulumi.getter
+    def columns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ViewColumnArgs']]]]:
+        """
+        The column headers to show on the log view.
+        """
+        return pulumi.get(self, "columns")
+
+    @columns.setter
+    def columns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ViewColumnArgs']]]]):
+        pulumi.set(self, "columns", value)
+
+    @property
     @pulumi.getter(name="defaultConnection")
     def default_connection(self) -> Optional[pulumi.Input[str]]:
         """
-        The connection that the log timeline uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
+        The connection that the log view uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
         """
         return pulumi.get(self, "default_connection")
 
     @default_connection.setter
     def default_connection(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_connection", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Description of the log timeline.
+        Description of the log view.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -93,23 +115,35 @@
     def end_time(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "end_time", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the log timeline.
+        Name of the log view.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
+    @pulumi.getter(name="sortOptions")
+    def sort_options(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ViewSortOptionArgs']]]]:
+        """
+        The sorting options configuration to specify if the log view table needs to be sorted in a particular field.
+        """
+        return pulumi.get(self, "sort_options")
+
+    @sort_options.setter
+    def sort_options(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ViewSortOptionArgs']]]]):
+        pulumi.set(self, "sort_options", value)
+
+    @property
     @pulumi.getter(name="startTime")
     def start_time(self) -> Optional[pulumi.Input[int]]:
         """
         Seconds since epoch. Used for visualization. Conflicts with `time_range`.
         """
         return pulumi.get(self, "start_time")
 
@@ -127,69 +161,89 @@
 
     @time_range.setter
     def time_range(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "time_range", value)
 
 
 @pulumi.input_type
-class _TimelineState:
+class _ViewState:
     def __init__(__self__, *,
+                 columns: Optional[pulumi.Input[Sequence[pulumi.Input['ViewColumnArgs']]]] = None,
                  default_connection: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  end_time: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  program_text: Optional[pulumi.Input[str]] = None,
+                 sort_options: Optional[pulumi.Input[Sequence[pulumi.Input['ViewSortOptionArgs']]]] = None,
                  start_time: Optional[pulumi.Input[int]] = None,
                  time_range: Optional[pulumi.Input[int]] = None,
                  url: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering Timeline resources.
-        :param pulumi.Input[str] default_connection: The connection that the log timeline uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
-        :param pulumi.Input[str] description: Description of the log timeline.
+        Input properties used for looking up and filtering View resources.
+        :param pulumi.Input[Sequence[pulumi.Input['ViewColumnArgs']]] columns: The column headers to show on the log view.
+        :param pulumi.Input[str] default_connection: The connection that the log view uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
+        :param pulumi.Input[str] description: Description of the log view.
         :param pulumi.Input[int] end_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
-        :param pulumi.Input[str] name: Name of the log timeline.
-        :param pulumi.Input[str] program_text: Signalflow program text for the log timeline. More info at https://dev.splunk.com/observability/docs/.
+        :param pulumi.Input[str] name: Name of the log view.
+        :param pulumi.Input[str] program_text: Signalflow program text for the log view. More info at https://developers.signalfx.com/docs/signalflow-overview.
+        :param pulumi.Input[Sequence[pulumi.Input['ViewSortOptionArgs']]] sort_options: The sorting options configuration to specify if the log view table needs to be sorted in a particular field.
         :param pulumi.Input[int] start_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
         :param pulumi.Input[int] time_range: From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
-        :param pulumi.Input[str] url: The URL of the log timeline.
+        :param pulumi.Input[str] url: The URL of the log view.
         """
+        if columns is not None:
+            pulumi.set(__self__, "columns", columns)
         if default_connection is not None:
             pulumi.set(__self__, "default_connection", default_connection)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if end_time is not None:
             pulumi.set(__self__, "end_time", end_time)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if program_text is not None:
             pulumi.set(__self__, "program_text", program_text)
+        if sort_options is not None:
+            pulumi.set(__self__, "sort_options", sort_options)
         if start_time is not None:
             pulumi.set(__self__, "start_time", start_time)
         if time_range is not None:
             pulumi.set(__self__, "time_range", time_range)
         if url is not None:
             pulumi.set(__self__, "url", url)
 
     @property
+    @pulumi.getter
+    def columns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ViewColumnArgs']]]]:
+        """
+        The column headers to show on the log view.
+        """
+        return pulumi.get(self, "columns")
+
+    @columns.setter
+    def columns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ViewColumnArgs']]]]):
+        pulumi.set(self, "columns", value)
+
+    @property
     @pulumi.getter(name="defaultConnection")
     def default_connection(self) -> Optional[pulumi.Input[str]]:
         """
-        The connection that the log timeline uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
+        The connection that the log view uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
         """
         return pulumi.get(self, "default_connection")
 
     @default_connection.setter
     def default_connection(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_connection", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Description of the log timeline.
+        Description of the log view.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -205,35 +259,47 @@
     def end_time(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "end_time", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the log timeline.
+        Name of the log view.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="programText")
     def program_text(self) -> Optional[pulumi.Input[str]]:
         """
-        Signalflow program text for the log timeline. More info at https://dev.splunk.com/observability/docs/.
+        Signalflow program text for the log view. More info at https://developers.signalfx.com/docs/signalflow-overview.
         """
         return pulumi.get(self, "program_text")
 
     @program_text.setter
     def program_text(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "program_text", value)
 
     @property
+    @pulumi.getter(name="sortOptions")
+    def sort_options(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ViewSortOptionArgs']]]]:
+        """
+        The sorting options configuration to specify if the log view table needs to be sorted in a particular field.
+        """
+        return pulumi.get(self, "sort_options")
+
+    @sort_options.setter
+    def sort_options(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ViewSortOptionArgs']]]]):
+        pulumi.set(self, "sort_options", value)
+
+    @property
     @pulumi.getter(name="startTime")
     def start_time(self) -> Optional[pulumi.Input[int]]:
         """
         Seconds since epoch. Used for visualization. Conflicts with `time_range`.
         """
         return pulumi.get(self, "start_time")
 
@@ -253,168 +319,192 @@
     def time_range(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "time_range", value)
 
     @property
     @pulumi.getter
     def url(self) -> Optional[pulumi.Input[str]]:
         """
-        The URL of the log timeline.
+        The URL of the log view.
         """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "url", value)
 
 
-class Timeline(pulumi.CustomResource):
+class View(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 columns: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewColumnArgs']]]]] = None,
                  default_connection: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  end_time: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  program_text: Optional[pulumi.Input[str]] = None,
+                 sort_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewSortOptionArgs']]]]] = None,
                  start_time: Optional[pulumi.Input[int]] = None,
                  time_range: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         You can add logs data to your Observability Cloud dashboards without turning your logs into metrics first.
 
-        A log timeline chart displays timeline visualization in a dashboard and shows you in detail what is happening and why.
+        A log view displays log lines in a table form in a dashboard and shows you in detail what is happening and why.
 
         ## Example
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] default_connection: The connection that the log timeline uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
-        :param pulumi.Input[str] description: Description of the log timeline.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewColumnArgs']]]] columns: The column headers to show on the log view.
+        :param pulumi.Input[str] default_connection: The connection that the log view uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
+        :param pulumi.Input[str] description: Description of the log view.
         :param pulumi.Input[int] end_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
-        :param pulumi.Input[str] name: Name of the log timeline.
-        :param pulumi.Input[str] program_text: Signalflow program text for the log timeline. More info at https://dev.splunk.com/observability/docs/.
+        :param pulumi.Input[str] name: Name of the log view.
+        :param pulumi.Input[str] program_text: Signalflow program text for the log view. More info at https://developers.signalfx.com/docs/signalflow-overview.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewSortOptionArgs']]]] sort_options: The sorting options configuration to specify if the log view table needs to be sorted in a particular field.
         :param pulumi.Input[int] start_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
         :param pulumi.Input[int] time_range: From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: TimelineArgs,
+                 args: ViewArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         You can add logs data to your Observability Cloud dashboards without turning your logs into metrics first.
 
-        A log timeline chart displays timeline visualization in a dashboard and shows you in detail what is happening and why.
+        A log view displays log lines in a table form in a dashboard and shows you in detail what is happening and why.
 
         ## Example
 
         :param str resource_name: The name of the resource.
-        :param TimelineArgs args: The arguments to use to populate this resource's properties.
+        :param ViewArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(TimelineArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ViewArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 columns: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewColumnArgs']]]]] = None,
                  default_connection: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  end_time: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  program_text: Optional[pulumi.Input[str]] = None,
+                 sort_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewSortOptionArgs']]]]] = None,
                  start_time: Optional[pulumi.Input[int]] = None,
                  time_range: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = TimelineArgs.__new__(TimelineArgs)
+            __props__ = ViewArgs.__new__(ViewArgs)
 
+            __props__.__dict__["columns"] = columns
             __props__.__dict__["default_connection"] = default_connection
             __props__.__dict__["description"] = description
             __props__.__dict__["end_time"] = end_time
             __props__.__dict__["name"] = name
             if program_text is None and not opts.urn:
                 raise TypeError("Missing required property 'program_text'")
             __props__.__dict__["program_text"] = program_text
+            __props__.__dict__["sort_options"] = sort_options
             __props__.__dict__["start_time"] = start_time
             __props__.__dict__["time_range"] = time_range
             __props__.__dict__["url"] = None
-        super(Timeline, __self__).__init__(
-            'signalfx:log/timeline:Timeline',
+        alias_opts = pulumi.ResourceOptions(aliases=[pulumi.Alias(type_="signalfx:logs/view:View")])
+        opts = pulumi.ResourceOptions.merge(opts, alias_opts)
+        super(View, __self__).__init__(
+            'signalfx:log/view:View',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            columns: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewColumnArgs']]]]] = None,
             default_connection: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
             end_time: Optional[pulumi.Input[int]] = None,
             name: Optional[pulumi.Input[str]] = None,
             program_text: Optional[pulumi.Input[str]] = None,
+            sort_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewSortOptionArgs']]]]] = None,
             start_time: Optional[pulumi.Input[int]] = None,
             time_range: Optional[pulumi.Input[int]] = None,
-            url: Optional[pulumi.Input[str]] = None) -> 'Timeline':
+            url: Optional[pulumi.Input[str]] = None) -> 'View':
         """
-        Get an existing Timeline resource's state with the given name, id, and optional extra
+        Get an existing View resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] default_connection: The connection that the log timeline uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
-        :param pulumi.Input[str] description: Description of the log timeline.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewColumnArgs']]]] columns: The column headers to show on the log view.
+        :param pulumi.Input[str] default_connection: The connection that the log view uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
+        :param pulumi.Input[str] description: Description of the log view.
         :param pulumi.Input[int] end_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
-        :param pulumi.Input[str] name: Name of the log timeline.
-        :param pulumi.Input[str] program_text: Signalflow program text for the log timeline. More info at https://dev.splunk.com/observability/docs/.
+        :param pulumi.Input[str] name: Name of the log view.
+        :param pulumi.Input[str] program_text: Signalflow program text for the log view. More info at https://developers.signalfx.com/docs/signalflow-overview.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewSortOptionArgs']]]] sort_options: The sorting options configuration to specify if the log view table needs to be sorted in a particular field.
         :param pulumi.Input[int] start_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
         :param pulumi.Input[int] time_range: From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
-        :param pulumi.Input[str] url: The URL of the log timeline.
+        :param pulumi.Input[str] url: The URL of the log view.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _TimelineState.__new__(_TimelineState)
+        __props__ = _ViewState.__new__(_ViewState)
 
+        __props__.__dict__["columns"] = columns
         __props__.__dict__["default_connection"] = default_connection
         __props__.__dict__["description"] = description
         __props__.__dict__["end_time"] = end_time
         __props__.__dict__["name"] = name
         __props__.__dict__["program_text"] = program_text
+        __props__.__dict__["sort_options"] = sort_options
         __props__.__dict__["start_time"] = start_time
         __props__.__dict__["time_range"] = time_range
         __props__.__dict__["url"] = url
-        return Timeline(resource_name, opts=opts, __props__=__props__)
+        return View(resource_name, opts=opts, __props__=__props__)
+
+    @property
+    @pulumi.getter
+    def columns(self) -> pulumi.Output[Optional[Sequence['outputs.ViewColumn']]]:
+        """
+        The column headers to show on the log view.
+        """
+        return pulumi.get(self, "columns")
 
     @property
     @pulumi.getter(name="defaultConnection")
     def default_connection(self) -> pulumi.Output[Optional[str]]:
         """
-        The connection that the log timeline uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
+        The connection that the log view uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
         """
         return pulumi.get(self, "default_connection")
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
-        Description of the log timeline.
+        Description of the log view.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter(name="endTime")
     def end_time(self) -> pulumi.Output[Optional[int]]:
         """
@@ -422,27 +512,35 @@
         """
         return pulumi.get(self, "end_time")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Name of the log timeline.
+        Name of the log view.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="programText")
     def program_text(self) -> pulumi.Output[str]:
         """
-        Signalflow program text for the log timeline. More info at https://dev.splunk.com/observability/docs/.
+        Signalflow program text for the log view. More info at https://developers.signalfx.com/docs/signalflow-overview.
         """
         return pulumi.get(self, "program_text")
 
     @property
+    @pulumi.getter(name="sortOptions")
+    def sort_options(self) -> pulumi.Output[Optional[Sequence['outputs.ViewSortOption']]]:
+        """
+        The sorting options configuration to specify if the log view table needs to be sorted in a particular field.
+        """
+        return pulumi.get(self, "sort_options")
+
+    @property
     @pulumi.getter(name="startTime")
     def start_time(self) -> pulumi.Output[Optional[int]]:
         """
         Seconds since epoch. Used for visualization. Conflicts with `time_range`.
         """
         return pulumi.get(self, "start_time")
 
@@ -454,11 +552,11 @@
         """
         return pulumi.get(self, "time_range")
 
     @property
     @pulumi.getter
     def url(self) -> pulumi.Output[str]:
         """
-        The URL of the log timeline.
+        The URL of the log view.
         """
         return pulumi.get(self, "url")
```

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/log/view.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/table_chart.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,560 +3,695 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
-from .. import _utilities
+from . import _utilities
 from . import outputs
 from ._inputs import *
 
-__all__ = ['ViewArgs', 'View']
+__all__ = ['TableChartArgs', 'TableChart']
 
 @pulumi.input_type
-class ViewArgs:
+class TableChartArgs:
     def __init__(__self__, *,
                  program_text: pulumi.Input[str],
-                 columns: Optional[pulumi.Input[Sequence[pulumi.Input['ViewColumnArgs']]]] = None,
-                 default_connection: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 end_time: Optional[pulumi.Input[int]] = None,
+                 disable_sampling: Optional[pulumi.Input[bool]] = None,
+                 group_bies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 hide_timestamp: Optional[pulumi.Input[bool]] = None,
+                 max_delay: Optional[pulumi.Input[int]] = None,
+                 minimum_resolution: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
-                 sort_options: Optional[pulumi.Input[Sequence[pulumi.Input['ViewSortOptionArgs']]]] = None,
-                 start_time: Optional[pulumi.Input[int]] = None,
-                 time_range: Optional[pulumi.Input[int]] = None):
-        """
-        The set of arguments for constructing a View resource.
-        :param pulumi.Input[str] program_text: Signalflow program text for the log view. More info at https://developers.signalfx.com/docs/signalflow-overview.
-        :param pulumi.Input[Sequence[pulumi.Input['ViewColumnArgs']]] columns: The column headers to show on the log view.
-        :param pulumi.Input[str] default_connection: The connection that the log view uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
-        :param pulumi.Input[str] description: Description of the log view.
-        :param pulumi.Input[int] end_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
-        :param pulumi.Input[str] name: Name of the log view.
-        :param pulumi.Input[Sequence[pulumi.Input['ViewSortOptionArgs']]] sort_options: The sorting options configuration to specify if the log view table needs to be sorted in a particular field.
-        :param pulumi.Input[int] start_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
-        :param pulumi.Input[int] time_range: From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
+                 refresh_interval: Optional[pulumi.Input[int]] = None,
+                 timezone: Optional[pulumi.Input[str]] = None,
+                 unit_prefix: Optional[pulumi.Input[str]] = None,
+                 viz_options: Optional[pulumi.Input[Sequence[pulumi.Input['TableChartVizOptionArgs']]]] = None):
+        """
+        The set of arguments for constructing a TableChart resource.
+        :param pulumi.Input[str] program_text: The SignalFlow for your Data Table Chart
+        :param pulumi.Input[str] description: Description of the table chart.
+        :param pulumi.Input[bool] disable_sampling: (false by default) If false, samples a subset of the output MTS, which improves UI performance
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] group_bies: Dimension to group by
+        :param pulumi.Input[bool] hide_timestamp: (false by default) Whether to show the timestamp in the chart
+        :param pulumi.Input[int] max_delay: How long (in seconds) to wait for late datapoints
+        :param pulumi.Input[int] minimum_resolution: The minimum resolution (in seconds) to use for computing the underlying program
+        :param pulumi.Input[str] name: Name of the table chart.
+        :param pulumi.Input[int] refresh_interval: How often (in seconds) to refresh the values of the Table
+        :param pulumi.Input[str] timezone: The property value is a string that denotes the geographic region associated with the time zone, (e.g. Australia/Sydney)
+        :param pulumi.Input[str] unit_prefix: (Metric by default) Must be "Metric" or "Binary"
+        :param pulumi.Input[Sequence[pulumi.Input['TableChartVizOptionArgs']]] viz_options: Plot-level customization options, associated with a publish statement
         """
         pulumi.set(__self__, "program_text", program_text)
-        if columns is not None:
-            pulumi.set(__self__, "columns", columns)
-        if default_connection is not None:
-            pulumi.set(__self__, "default_connection", default_connection)
         if description is not None:
             pulumi.set(__self__, "description", description)
-        if end_time is not None:
-            pulumi.set(__self__, "end_time", end_time)
+        if disable_sampling is not None:
+            pulumi.set(__self__, "disable_sampling", disable_sampling)
+        if group_bies is not None:
+            pulumi.set(__self__, "group_bies", group_bies)
+        if hide_timestamp is not None:
+            pulumi.set(__self__, "hide_timestamp", hide_timestamp)
+        if max_delay is not None:
+            pulumi.set(__self__, "max_delay", max_delay)
+        if minimum_resolution is not None:
+            pulumi.set(__self__, "minimum_resolution", minimum_resolution)
         if name is not None:
             pulumi.set(__self__, "name", name)
-        if sort_options is not None:
-            pulumi.set(__self__, "sort_options", sort_options)
-        if start_time is not None:
-            pulumi.set(__self__, "start_time", start_time)
-        if time_range is not None:
-            pulumi.set(__self__, "time_range", time_range)
+        if refresh_interval is not None:
+            pulumi.set(__self__, "refresh_interval", refresh_interval)
+        if timezone is not None:
+            pulumi.set(__self__, "timezone", timezone)
+        if unit_prefix is not None:
+            pulumi.set(__self__, "unit_prefix", unit_prefix)
+        if viz_options is not None:
+            pulumi.set(__self__, "viz_options", viz_options)
 
     @property
     @pulumi.getter(name="programText")
     def program_text(self) -> pulumi.Input[str]:
         """
-        Signalflow program text for the log view. More info at https://developers.signalfx.com/docs/signalflow-overview.
+        The SignalFlow for your Data Table Chart
         """
         return pulumi.get(self, "program_text")
 
     @program_text.setter
     def program_text(self, value: pulumi.Input[str]):
         pulumi.set(self, "program_text", value)
 
     @property
     @pulumi.getter
-    def columns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ViewColumnArgs']]]]:
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        The column headers to show on the log view.
+        Description of the table chart.
         """
-        return pulumi.get(self, "columns")
+        return pulumi.get(self, "description")
 
-    @columns.setter
-    def columns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ViewColumnArgs']]]]):
-        pulumi.set(self, "columns", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="defaultConnection")
-    def default_connection(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="disableSampling")
+    def disable_sampling(self) -> Optional[pulumi.Input[bool]]:
         """
-        The connection that the log view uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
+        (false by default) If false, samples a subset of the output MTS, which improves UI performance
         """
-        return pulumi.get(self, "default_connection")
+        return pulumi.get(self, "disable_sampling")
 
-    @default_connection.setter
-    def default_connection(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "default_connection", value)
+    @disable_sampling.setter
+    def disable_sampling(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "disable_sampling", value)
 
     @property
-    @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="groupBies")
+    def group_bies(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Description of the log view.
+        Dimension to group by
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "group_bies")
 
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+    @group_bies.setter
+    def group_bies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "group_bies", value)
+
+    @property
+    @pulumi.getter(name="hideTimestamp")
+    def hide_timestamp(self) -> Optional[pulumi.Input[bool]]:
+        """
+        (false by default) Whether to show the timestamp in the chart
+        """
+        return pulumi.get(self, "hide_timestamp")
+
+    @hide_timestamp.setter
+    def hide_timestamp(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "hide_timestamp", value)
+
+    @property
+    @pulumi.getter(name="maxDelay")
+    def max_delay(self) -> Optional[pulumi.Input[int]]:
+        """
+        How long (in seconds) to wait for late datapoints
+        """
+        return pulumi.get(self, "max_delay")
+
+    @max_delay.setter
+    def max_delay(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "max_delay", value)
 
     @property
-    @pulumi.getter(name="endTime")
-    def end_time(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="minimumResolution")
+    def minimum_resolution(self) -> Optional[pulumi.Input[int]]:
         """
-        Seconds since epoch. Used for visualization. Conflicts with `time_range`.
+        The minimum resolution (in seconds) to use for computing the underlying program
         """
-        return pulumi.get(self, "end_time")
+        return pulumi.get(self, "minimum_resolution")
 
-    @end_time.setter
-    def end_time(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "end_time", value)
+    @minimum_resolution.setter
+    def minimum_resolution(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "minimum_resolution", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the log view.
+        Name of the table chart.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter(name="sortOptions")
-    def sort_options(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ViewSortOptionArgs']]]]:
+    @pulumi.getter(name="refreshInterval")
+    def refresh_interval(self) -> Optional[pulumi.Input[int]]:
+        """
+        How often (in seconds) to refresh the values of the Table
+        """
+        return pulumi.get(self, "refresh_interval")
+
+    @refresh_interval.setter
+    def refresh_interval(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "refresh_interval", value)
+
+    @property
+    @pulumi.getter
+    def timezone(self) -> Optional[pulumi.Input[str]]:
         """
-        The sorting options configuration to specify if the log view table needs to be sorted in a particular field.
+        The property value is a string that denotes the geographic region associated with the time zone, (e.g. Australia/Sydney)
         """
-        return pulumi.get(self, "sort_options")
+        return pulumi.get(self, "timezone")
 
-    @sort_options.setter
-    def sort_options(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ViewSortOptionArgs']]]]):
-        pulumi.set(self, "sort_options", value)
+    @timezone.setter
+    def timezone(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "timezone", value)
 
     @property
-    @pulumi.getter(name="startTime")
-    def start_time(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="unitPrefix")
+    def unit_prefix(self) -> Optional[pulumi.Input[str]]:
         """
-        Seconds since epoch. Used for visualization. Conflicts with `time_range`.
+        (Metric by default) Must be "Metric" or "Binary"
         """
-        return pulumi.get(self, "start_time")
+        return pulumi.get(self, "unit_prefix")
 
-    @start_time.setter
-    def start_time(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "start_time", value)
+    @unit_prefix.setter
+    def unit_prefix(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "unit_prefix", value)
 
     @property
-    @pulumi.getter(name="timeRange")
-    def time_range(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="vizOptions")
+    def viz_options(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['TableChartVizOptionArgs']]]]:
         """
-        From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
+        Plot-level customization options, associated with a publish statement
         """
-        return pulumi.get(self, "time_range")
+        return pulumi.get(self, "viz_options")
 
-    @time_range.setter
-    def time_range(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "time_range", value)
+    @viz_options.setter
+    def viz_options(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['TableChartVizOptionArgs']]]]):
+        pulumi.set(self, "viz_options", value)
 
 
 @pulumi.input_type
-class _ViewState:
+class _TableChartState:
     def __init__(__self__, *,
-                 columns: Optional[pulumi.Input[Sequence[pulumi.Input['ViewColumnArgs']]]] = None,
-                 default_connection: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 end_time: Optional[pulumi.Input[int]] = None,
+                 disable_sampling: Optional[pulumi.Input[bool]] = None,
+                 group_bies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 hide_timestamp: Optional[pulumi.Input[bool]] = None,
+                 max_delay: Optional[pulumi.Input[int]] = None,
+                 minimum_resolution: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  program_text: Optional[pulumi.Input[str]] = None,
-                 sort_options: Optional[pulumi.Input[Sequence[pulumi.Input['ViewSortOptionArgs']]]] = None,
-                 start_time: Optional[pulumi.Input[int]] = None,
-                 time_range: Optional[pulumi.Input[int]] = None,
-                 url: Optional[pulumi.Input[str]] = None):
-        """
-        Input properties used for looking up and filtering View resources.
-        :param pulumi.Input[Sequence[pulumi.Input['ViewColumnArgs']]] columns: The column headers to show on the log view.
-        :param pulumi.Input[str] default_connection: The connection that the log view uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
-        :param pulumi.Input[str] description: Description of the log view.
-        :param pulumi.Input[int] end_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
-        :param pulumi.Input[str] name: Name of the log view.
-        :param pulumi.Input[str] program_text: Signalflow program text for the log view. More info at https://developers.signalfx.com/docs/signalflow-overview.
-        :param pulumi.Input[Sequence[pulumi.Input['ViewSortOptionArgs']]] sort_options: The sorting options configuration to specify if the log view table needs to be sorted in a particular field.
-        :param pulumi.Input[int] start_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
-        :param pulumi.Input[int] time_range: From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
-        :param pulumi.Input[str] url: The URL of the log view.
-        """
-        if columns is not None:
-            pulumi.set(__self__, "columns", columns)
-        if default_connection is not None:
-            pulumi.set(__self__, "default_connection", default_connection)
+                 refresh_interval: Optional[pulumi.Input[int]] = None,
+                 timezone: Optional[pulumi.Input[str]] = None,
+                 unit_prefix: Optional[pulumi.Input[str]] = None,
+                 url: Optional[pulumi.Input[str]] = None,
+                 viz_options: Optional[pulumi.Input[Sequence[pulumi.Input['TableChartVizOptionArgs']]]] = None):
+        """
+        Input properties used for looking up and filtering TableChart resources.
+        :param pulumi.Input[str] description: Description of the table chart.
+        :param pulumi.Input[bool] disable_sampling: (false by default) If false, samples a subset of the output MTS, which improves UI performance
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] group_bies: Dimension to group by
+        :param pulumi.Input[bool] hide_timestamp: (false by default) Whether to show the timestamp in the chart
+        :param pulumi.Input[int] max_delay: How long (in seconds) to wait for late datapoints
+        :param pulumi.Input[int] minimum_resolution: The minimum resolution (in seconds) to use for computing the underlying program
+        :param pulumi.Input[str] name: Name of the table chart.
+        :param pulumi.Input[str] program_text: The SignalFlow for your Data Table Chart
+        :param pulumi.Input[int] refresh_interval: How often (in seconds) to refresh the values of the Table
+        :param pulumi.Input[str] timezone: The property value is a string that denotes the geographic region associated with the time zone, (e.g. Australia/Sydney)
+        :param pulumi.Input[str] unit_prefix: (Metric by default) Must be "Metric" or "Binary"
+        :param pulumi.Input[str] url: The URL of the chart.
+        :param pulumi.Input[Sequence[pulumi.Input['TableChartVizOptionArgs']]] viz_options: Plot-level customization options, associated with a publish statement
+        """
         if description is not None:
             pulumi.set(__self__, "description", description)
-        if end_time is not None:
-            pulumi.set(__self__, "end_time", end_time)
+        if disable_sampling is not None:
+            pulumi.set(__self__, "disable_sampling", disable_sampling)
+        if group_bies is not None:
+            pulumi.set(__self__, "group_bies", group_bies)
+        if hide_timestamp is not None:
+            pulumi.set(__self__, "hide_timestamp", hide_timestamp)
+        if max_delay is not None:
+            pulumi.set(__self__, "max_delay", max_delay)
+        if minimum_resolution is not None:
+            pulumi.set(__self__, "minimum_resolution", minimum_resolution)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if program_text is not None:
             pulumi.set(__self__, "program_text", program_text)
-        if sort_options is not None:
-            pulumi.set(__self__, "sort_options", sort_options)
-        if start_time is not None:
-            pulumi.set(__self__, "start_time", start_time)
-        if time_range is not None:
-            pulumi.set(__self__, "time_range", time_range)
+        if refresh_interval is not None:
+            pulumi.set(__self__, "refresh_interval", refresh_interval)
+        if timezone is not None:
+            pulumi.set(__self__, "timezone", timezone)
+        if unit_prefix is not None:
+            pulumi.set(__self__, "unit_prefix", unit_prefix)
         if url is not None:
             pulumi.set(__self__, "url", url)
+        if viz_options is not None:
+            pulumi.set(__self__, "viz_options", viz_options)
 
     @property
     @pulumi.getter
-    def columns(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ViewColumnArgs']]]]:
+    def description(self) -> Optional[pulumi.Input[str]]:
         """
-        The column headers to show on the log view.
+        Description of the table chart.
         """
-        return pulumi.get(self, "columns")
+        return pulumi.get(self, "description")
 
-    @columns.setter
-    def columns(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ViewColumnArgs']]]]):
-        pulumi.set(self, "columns", value)
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
 
     @property
-    @pulumi.getter(name="defaultConnection")
-    def default_connection(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="disableSampling")
+    def disable_sampling(self) -> Optional[pulumi.Input[bool]]:
         """
-        The connection that the log view uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
+        (false by default) If false, samples a subset of the output MTS, which improves UI performance
         """
-        return pulumi.get(self, "default_connection")
+        return pulumi.get(self, "disable_sampling")
 
-    @default_connection.setter
-    def default_connection(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "default_connection", value)
+    @disable_sampling.setter
+    def disable_sampling(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "disable_sampling", value)
 
     @property
-    @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="groupBies")
+    def group_bies(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Description of the log view.
+        Dimension to group by
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "group_bies")
 
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+    @group_bies.setter
+    def group_bies(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "group_bies", value)
+
+    @property
+    @pulumi.getter(name="hideTimestamp")
+    def hide_timestamp(self) -> Optional[pulumi.Input[bool]]:
+        """
+        (false by default) Whether to show the timestamp in the chart
+        """
+        return pulumi.get(self, "hide_timestamp")
+
+    @hide_timestamp.setter
+    def hide_timestamp(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "hide_timestamp", value)
 
     @property
-    @pulumi.getter(name="endTime")
-    def end_time(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="maxDelay")
+    def max_delay(self) -> Optional[pulumi.Input[int]]:
         """
-        Seconds since epoch. Used for visualization. Conflicts with `time_range`.
+        How long (in seconds) to wait for late datapoints
         """
-        return pulumi.get(self, "end_time")
+        return pulumi.get(self, "max_delay")
 
-    @end_time.setter
-    def end_time(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "end_time", value)
+    @max_delay.setter
+    def max_delay(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "max_delay", value)
+
+    @property
+    @pulumi.getter(name="minimumResolution")
+    def minimum_resolution(self) -> Optional[pulumi.Input[int]]:
+        """
+        The minimum resolution (in seconds) to use for computing the underlying program
+        """
+        return pulumi.get(self, "minimum_resolution")
+
+    @minimum_resolution.setter
+    def minimum_resolution(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "minimum_resolution", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the log view.
+        Name of the table chart.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="programText")
     def program_text(self) -> Optional[pulumi.Input[str]]:
         """
-        Signalflow program text for the log view. More info at https://developers.signalfx.com/docs/signalflow-overview.
+        The SignalFlow for your Data Table Chart
         """
         return pulumi.get(self, "program_text")
 
     @program_text.setter
     def program_text(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "program_text", value)
 
     @property
-    @pulumi.getter(name="sortOptions")
-    def sort_options(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ViewSortOptionArgs']]]]:
+    @pulumi.getter(name="refreshInterval")
+    def refresh_interval(self) -> Optional[pulumi.Input[int]]:
         """
-        The sorting options configuration to specify if the log view table needs to be sorted in a particular field.
+        How often (in seconds) to refresh the values of the Table
         """
-        return pulumi.get(self, "sort_options")
+        return pulumi.get(self, "refresh_interval")
 
-    @sort_options.setter
-    def sort_options(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ViewSortOptionArgs']]]]):
-        pulumi.set(self, "sort_options", value)
+    @refresh_interval.setter
+    def refresh_interval(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "refresh_interval", value)
 
     @property
-    @pulumi.getter(name="startTime")
-    def start_time(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter
+    def timezone(self) -> Optional[pulumi.Input[str]]:
         """
-        Seconds since epoch. Used for visualization. Conflicts with `time_range`.
+        The property value is a string that denotes the geographic region associated with the time zone, (e.g. Australia/Sydney)
         """
-        return pulumi.get(self, "start_time")
+        return pulumi.get(self, "timezone")
 
-    @start_time.setter
-    def start_time(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "start_time", value)
+    @timezone.setter
+    def timezone(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "timezone", value)
 
     @property
-    @pulumi.getter(name="timeRange")
-    def time_range(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter(name="unitPrefix")
+    def unit_prefix(self) -> Optional[pulumi.Input[str]]:
         """
-        From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
+        (Metric by default) Must be "Metric" or "Binary"
         """
-        return pulumi.get(self, "time_range")
+        return pulumi.get(self, "unit_prefix")
 
-    @time_range.setter
-    def time_range(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "time_range", value)
+    @unit_prefix.setter
+    def unit_prefix(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "unit_prefix", value)
 
     @property
     @pulumi.getter
     def url(self) -> Optional[pulumi.Input[str]]:
         """
-        The URL of the log view.
+        The URL of the chart.
         """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "url", value)
 
+    @property
+    @pulumi.getter(name="vizOptions")
+    def viz_options(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['TableChartVizOptionArgs']]]]:
+        """
+        Plot-level customization options, associated with a publish statement
+        """
+        return pulumi.get(self, "viz_options")
 
-class View(pulumi.CustomResource):
+    @viz_options.setter
+    def viz_options(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['TableChartVizOptionArgs']]]]):
+        pulumi.set(self, "viz_options", value)
+
+
+class TableChart(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 columns: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewColumnArgs']]]]] = None,
-                 default_connection: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 end_time: Optional[pulumi.Input[int]] = None,
+                 disable_sampling: Optional[pulumi.Input[bool]] = None,
+                 group_bies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 hide_timestamp: Optional[pulumi.Input[bool]] = None,
+                 max_delay: Optional[pulumi.Input[int]] = None,
+                 minimum_resolution: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  program_text: Optional[pulumi.Input[str]] = None,
-                 sort_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewSortOptionArgs']]]]] = None,
-                 start_time: Optional[pulumi.Input[int]] = None,
-                 time_range: Optional[pulumi.Input[int]] = None,
+                 refresh_interval: Optional[pulumi.Input[int]] = None,
+                 timezone: Optional[pulumi.Input[str]] = None,
+                 unit_prefix: Optional[pulumi.Input[str]] = None,
+                 viz_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TableChartVizOptionArgs']]]]] = None,
                  __props__=None):
         """
-        You can add logs data to your Observability Cloud dashboards without turning your logs into metrics first.
-
-        A log view displays log lines in a table form in a dashboard and shows you in detail what is happening and why.
+        This special type of chart displays a data table. This table can be grouped by a dimension.
 
         ## Example
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewColumnArgs']]]] columns: The column headers to show on the log view.
-        :param pulumi.Input[str] default_connection: The connection that the log view uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
-        :param pulumi.Input[str] description: Description of the log view.
-        :param pulumi.Input[int] end_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
-        :param pulumi.Input[str] name: Name of the log view.
-        :param pulumi.Input[str] program_text: Signalflow program text for the log view. More info at https://developers.signalfx.com/docs/signalflow-overview.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewSortOptionArgs']]]] sort_options: The sorting options configuration to specify if the log view table needs to be sorted in a particular field.
-        :param pulumi.Input[int] start_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
-        :param pulumi.Input[int] time_range: From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
+        :param pulumi.Input[str] description: Description of the table chart.
+        :param pulumi.Input[bool] disable_sampling: (false by default) If false, samples a subset of the output MTS, which improves UI performance
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] group_bies: Dimension to group by
+        :param pulumi.Input[bool] hide_timestamp: (false by default) Whether to show the timestamp in the chart
+        :param pulumi.Input[int] max_delay: How long (in seconds) to wait for late datapoints
+        :param pulumi.Input[int] minimum_resolution: The minimum resolution (in seconds) to use for computing the underlying program
+        :param pulumi.Input[str] name: Name of the table chart.
+        :param pulumi.Input[str] program_text: The SignalFlow for your Data Table Chart
+        :param pulumi.Input[int] refresh_interval: How often (in seconds) to refresh the values of the Table
+        :param pulumi.Input[str] timezone: The property value is a string that denotes the geographic region associated with the time zone, (e.g. Australia/Sydney)
+        :param pulumi.Input[str] unit_prefix: (Metric by default) Must be "Metric" or "Binary"
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TableChartVizOptionArgs']]]] viz_options: Plot-level customization options, associated with a publish statement
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ViewArgs,
+                 args: TableChartArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        You can add logs data to your Observability Cloud dashboards without turning your logs into metrics first.
-
-        A log view displays log lines in a table form in a dashboard and shows you in detail what is happening and why.
+        This special type of chart displays a data table. This table can be grouped by a dimension.
 
         ## Example
 
         :param str resource_name: The name of the resource.
-        :param ViewArgs args: The arguments to use to populate this resource's properties.
+        :param TableChartArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ViewArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(TableChartArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 columns: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewColumnArgs']]]]] = None,
-                 default_connection: Optional[pulumi.Input[str]] = None,
                  description: Optional[pulumi.Input[str]] = None,
-                 end_time: Optional[pulumi.Input[int]] = None,
+                 disable_sampling: Optional[pulumi.Input[bool]] = None,
+                 group_bies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 hide_timestamp: Optional[pulumi.Input[bool]] = None,
+                 max_delay: Optional[pulumi.Input[int]] = None,
+                 minimum_resolution: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  program_text: Optional[pulumi.Input[str]] = None,
-                 sort_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewSortOptionArgs']]]]] = None,
-                 start_time: Optional[pulumi.Input[int]] = None,
-                 time_range: Optional[pulumi.Input[int]] = None,
+                 refresh_interval: Optional[pulumi.Input[int]] = None,
+                 timezone: Optional[pulumi.Input[str]] = None,
+                 unit_prefix: Optional[pulumi.Input[str]] = None,
+                 viz_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TableChartVizOptionArgs']]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ViewArgs.__new__(ViewArgs)
+            __props__ = TableChartArgs.__new__(TableChartArgs)
 
-            __props__.__dict__["columns"] = columns
-            __props__.__dict__["default_connection"] = default_connection
             __props__.__dict__["description"] = description
-            __props__.__dict__["end_time"] = end_time
+            __props__.__dict__["disable_sampling"] = disable_sampling
+            __props__.__dict__["group_bies"] = group_bies
+            __props__.__dict__["hide_timestamp"] = hide_timestamp
+            __props__.__dict__["max_delay"] = max_delay
+            __props__.__dict__["minimum_resolution"] = minimum_resolution
             __props__.__dict__["name"] = name
             if program_text is None and not opts.urn:
                 raise TypeError("Missing required property 'program_text'")
             __props__.__dict__["program_text"] = program_text
-            __props__.__dict__["sort_options"] = sort_options
-            __props__.__dict__["start_time"] = start_time
-            __props__.__dict__["time_range"] = time_range
+            __props__.__dict__["refresh_interval"] = refresh_interval
+            __props__.__dict__["timezone"] = timezone
+            __props__.__dict__["unit_prefix"] = unit_prefix
+            __props__.__dict__["viz_options"] = viz_options
             __props__.__dict__["url"] = None
-        alias_opts = pulumi.ResourceOptions(aliases=[pulumi.Alias(type_="signalfx:logs/view:View")])
-        opts = pulumi.ResourceOptions.merge(opts, alias_opts)
-        super(View, __self__).__init__(
-            'signalfx:log/view:View',
+        super(TableChart, __self__).__init__(
+            'signalfx:index/tableChart:TableChart',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            columns: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewColumnArgs']]]]] = None,
-            default_connection: Optional[pulumi.Input[str]] = None,
             description: Optional[pulumi.Input[str]] = None,
-            end_time: Optional[pulumi.Input[int]] = None,
+            disable_sampling: Optional[pulumi.Input[bool]] = None,
+            group_bies: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+            hide_timestamp: Optional[pulumi.Input[bool]] = None,
+            max_delay: Optional[pulumi.Input[int]] = None,
+            minimum_resolution: Optional[pulumi.Input[int]] = None,
             name: Optional[pulumi.Input[str]] = None,
             program_text: Optional[pulumi.Input[str]] = None,
-            sort_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewSortOptionArgs']]]]] = None,
-            start_time: Optional[pulumi.Input[int]] = None,
-            time_range: Optional[pulumi.Input[int]] = None,
-            url: Optional[pulumi.Input[str]] = None) -> 'View':
+            refresh_interval: Optional[pulumi.Input[int]] = None,
+            timezone: Optional[pulumi.Input[str]] = None,
+            unit_prefix: Optional[pulumi.Input[str]] = None,
+            url: Optional[pulumi.Input[str]] = None,
+            viz_options: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TableChartVizOptionArgs']]]]] = None) -> 'TableChart':
         """
-        Get an existing View resource's state with the given name, id, and optional extra
+        Get an existing TableChart resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewColumnArgs']]]] columns: The column headers to show on the log view.
-        :param pulumi.Input[str] default_connection: The connection that the log view uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
-        :param pulumi.Input[str] description: Description of the log view.
-        :param pulumi.Input[int] end_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
-        :param pulumi.Input[str] name: Name of the log view.
-        :param pulumi.Input[str] program_text: Signalflow program text for the log view. More info at https://developers.signalfx.com/docs/signalflow-overview.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ViewSortOptionArgs']]]] sort_options: The sorting options configuration to specify if the log view table needs to be sorted in a particular field.
-        :param pulumi.Input[int] start_time: Seconds since epoch. Used for visualization. Conflicts with `time_range`.
-        :param pulumi.Input[int] time_range: From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
-        :param pulumi.Input[str] url: The URL of the log view.
+        :param pulumi.Input[str] description: Description of the table chart.
+        :param pulumi.Input[bool] disable_sampling: (false by default) If false, samples a subset of the output MTS, which improves UI performance
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] group_bies: Dimension to group by
+        :param pulumi.Input[bool] hide_timestamp: (false by default) Whether to show the timestamp in the chart
+        :param pulumi.Input[int] max_delay: How long (in seconds) to wait for late datapoints
+        :param pulumi.Input[int] minimum_resolution: The minimum resolution (in seconds) to use for computing the underlying program
+        :param pulumi.Input[str] name: Name of the table chart.
+        :param pulumi.Input[str] program_text: The SignalFlow for your Data Table Chart
+        :param pulumi.Input[int] refresh_interval: How often (in seconds) to refresh the values of the Table
+        :param pulumi.Input[str] timezone: The property value is a string that denotes the geographic region associated with the time zone, (e.g. Australia/Sydney)
+        :param pulumi.Input[str] unit_prefix: (Metric by default) Must be "Metric" or "Binary"
+        :param pulumi.Input[str] url: The URL of the chart.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TableChartVizOptionArgs']]]] viz_options: Plot-level customization options, associated with a publish statement
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ViewState.__new__(_ViewState)
+        __props__ = _TableChartState.__new__(_TableChartState)
 
-        __props__.__dict__["columns"] = columns
-        __props__.__dict__["default_connection"] = default_connection
         __props__.__dict__["description"] = description
-        __props__.__dict__["end_time"] = end_time
+        __props__.__dict__["disable_sampling"] = disable_sampling
+        __props__.__dict__["group_bies"] = group_bies
+        __props__.__dict__["hide_timestamp"] = hide_timestamp
+        __props__.__dict__["max_delay"] = max_delay
+        __props__.__dict__["minimum_resolution"] = minimum_resolution
         __props__.__dict__["name"] = name
         __props__.__dict__["program_text"] = program_text
-        __props__.__dict__["sort_options"] = sort_options
-        __props__.__dict__["start_time"] = start_time
-        __props__.__dict__["time_range"] = time_range
+        __props__.__dict__["refresh_interval"] = refresh_interval
+        __props__.__dict__["timezone"] = timezone
+        __props__.__dict__["unit_prefix"] = unit_prefix
         __props__.__dict__["url"] = url
-        return View(resource_name, opts=opts, __props__=__props__)
+        __props__.__dict__["viz_options"] = viz_options
+        return TableChart(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def columns(self) -> pulumi.Output[Optional[Sequence['outputs.ViewColumn']]]:
+    def description(self) -> pulumi.Output[Optional[str]]:
         """
-        The column headers to show on the log view.
+        Description of the table chart.
         """
-        return pulumi.get(self, "columns")
+        return pulumi.get(self, "description")
 
     @property
-    @pulumi.getter(name="defaultConnection")
-    def default_connection(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="disableSampling")
+    def disable_sampling(self) -> pulumi.Output[Optional[bool]]:
         """
-        The connection that the log view uses to fetch data. This could be Splunk Enterprise, Splunk Enterprise Cloud or Observability Cloud.
+        (false by default) If false, samples a subset of the output MTS, which improves UI performance
         """
-        return pulumi.get(self, "default_connection")
+        return pulumi.get(self, "disable_sampling")
 
     @property
-    @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="groupBies")
+    def group_bies(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
-        Description of the log view.
+        Dimension to group by
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "group_bies")
+
+    @property
+    @pulumi.getter(name="hideTimestamp")
+    def hide_timestamp(self) -> pulumi.Output[Optional[bool]]:
+        """
+        (false by default) Whether to show the timestamp in the chart
+        """
+        return pulumi.get(self, "hide_timestamp")
 
     @property
-    @pulumi.getter(name="endTime")
-    def end_time(self) -> pulumi.Output[Optional[int]]:
+    @pulumi.getter(name="maxDelay")
+    def max_delay(self) -> pulumi.Output[Optional[int]]:
         """
-        Seconds since epoch. Used for visualization. Conflicts with `time_range`.
+        How long (in seconds) to wait for late datapoints
         """
-        return pulumi.get(self, "end_time")
+        return pulumi.get(self, "max_delay")
+
+    @property
+    @pulumi.getter(name="minimumResolution")
+    def minimum_resolution(self) -> pulumi.Output[Optional[int]]:
+        """
+        The minimum resolution (in seconds) to use for computing the underlying program
+        """
+        return pulumi.get(self, "minimum_resolution")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        Name of the log view.
+        Name of the table chart.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="programText")
     def program_text(self) -> pulumi.Output[str]:
         """
-        Signalflow program text for the log view. More info at https://developers.signalfx.com/docs/signalflow-overview.
+        The SignalFlow for your Data Table Chart
         """
         return pulumi.get(self, "program_text")
 
     @property
-    @pulumi.getter(name="sortOptions")
-    def sort_options(self) -> pulumi.Output[Optional[Sequence['outputs.ViewSortOption']]]:
+    @pulumi.getter(name="refreshInterval")
+    def refresh_interval(self) -> pulumi.Output[Optional[int]]:
         """
-        The sorting options configuration to specify if the log view table needs to be sorted in a particular field.
+        How often (in seconds) to refresh the values of the Table
         """
-        return pulumi.get(self, "sort_options")
+        return pulumi.get(self, "refresh_interval")
 
     @property
-    @pulumi.getter(name="startTime")
-    def start_time(self) -> pulumi.Output[Optional[int]]:
+    @pulumi.getter
+    def timezone(self) -> pulumi.Output[Optional[str]]:
         """
-        Seconds since epoch. Used for visualization. Conflicts with `time_range`.
+        The property value is a string that denotes the geographic region associated with the time zone, (e.g. Australia/Sydney)
         """
-        return pulumi.get(self, "start_time")
+        return pulumi.get(self, "timezone")
 
     @property
-    @pulumi.getter(name="timeRange")
-    def time_range(self) -> pulumi.Output[Optional[int]]:
+    @pulumi.getter(name="unitPrefix")
+    def unit_prefix(self) -> pulumi.Output[Optional[str]]:
         """
-        From when to display data. Splunk Observability Cloud time syntax (e.g. `"-5m"`, `"-1h"`). Conflicts with `start_time` and `end_time`.
+        (Metric by default) Must be "Metric" or "Binary"
         """
-        return pulumi.get(self, "time_range")
+        return pulumi.get(self, "unit_prefix")
 
     @property
     @pulumi.getter
     def url(self) -> pulumi.Output[str]:
         """
-        The URL of the log view.
+        The URL of the chart.
         """
         return pulumi.get(self, "url")
 
+    @property
+    @pulumi.getter(name="vizOptions")
+    def viz_options(self) -> pulumi.Output[Optional[Sequence['outputs.TableChartVizOption']]]:
+        """
+        Plot-level customization options, associated with a publish statement
+        """
+        return pulumi.get(self, "viz_options")
+
```

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/metric_ruleset.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/metric_ruleset.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/opsgenie/integration.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/opsgenie/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/org_token.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/org_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/outputs.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
 __all__ = [
     'AlertMutingRuleFilter',
+    'AlertMutingRuleRecurrence',
     'DashboardChart',
     'DashboardColumn',
     'DashboardEventOverlay',
     'DashboardEventOverlaySource',
     'DashboardFilter',
     'DashboardGrid',
     'DashboardGroupDashboard',
@@ -120,14 +121,43 @@
         """
         The property to filter.
         """
         return pulumi.get(self, "property")
 
 
 @pulumi.output_type
+class AlertMutingRuleRecurrence(dict):
+    def __init__(__self__, *,
+                 unit: str,
+                 value: int):
+        """
+        :param str unit: The unit of the period. Can be days (d) or weeks (w).
+        :param int value: The amount of time, expressed as an integer, applicable to the unit specified.
+        """
+        pulumi.set(__self__, "unit", unit)
+        pulumi.set(__self__, "value", value)
+
+    @property
+    @pulumi.getter
+    def unit(self) -> str:
+        """
+        The unit of the period. Can be days (d) or weeks (w).
+        """
+        return pulumi.get(self, "unit")
+
+    @property
+    @pulumi.getter
+    def value(self) -> int:
+        """
+        The amount of time, expressed as an integer, applicable to the unit specified.
+        """
+        return pulumi.get(self, "value")
+
+
+@pulumi.output_type
 class DashboardChart(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "chartId":
             suggest = "chart_id"
```

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/pagerduty/get_integration.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/pagerduty/get_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/pagerduty/integration.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/pagerduty/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/provider.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/servicenow/integration.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/servicenow/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/single_value_chart.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/single_value_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/slack/integration.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/slack/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/slo.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/slo.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/team.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/text_chart.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/text_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/time_chart.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/time_chart.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx/victorops/integration.py` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx/victorops/integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx.egg-info/PKG-INFO` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_signalfx
-Version: 7.2.0a1716963243
+Version: 7.2.0a1717136910
 Summary: A Pulumi package for creating and managing SignalFx resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-signalfx
 Keywords: pulumi,signalfx
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_signalfx-7.2.0a1716963243/pulumi_signalfx.egg-info/SOURCES.txt` & `pulumi_signalfx-7.2.0a1717136910/pulumi_signalfx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_signalfx-7.2.0a1716963243/pyproject.toml` & `pulumi_signalfx-7.2.0a1717136910/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_signalfx"
   description = "A Pulumi package for creating and managing SignalFx resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "signalfx"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "7.2.0a1716963243"
+  version = "7.2.0a1717136910"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-signalfx"
 
 [build-system]
```

