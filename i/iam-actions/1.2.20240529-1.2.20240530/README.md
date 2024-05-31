# Comparing `tmp/iam_actions-1.2.20240529.tar.gz` & `tmp/iam_actions-1.2.20240530.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240529.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240530.tar", max compression
```

## Comparing `iam_actions-1.2.20240529.tar` & `iam_actions-1.2.20240530.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/LICENSE
--rw-r--r--   0        0        0     2302 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/README.md
--rw-r--r--   0        0        0      228 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/__init__.py
--rw-r--r--   0        0        0  4854274 2024-05-29 02:28:01.721773 iam_actions-1.2.20240529/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-05-29 02:26:14.473893 iam_actions-1.2.20240529/iam_actions/generate/services.py
--rw-r--r--   0        0        0   632109 2024-05-29 02:28:01.721773 iam_actions-1.2.20240529/iam_actions/policies.json
--rw-r--r--   0        0        0   209748 2024-05-29 02:28:01.721773 iam_actions-1.2.20240529/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   613075 2024-05-29 02:28:01.721773 iam_actions-1.2.20240529/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-05-29 02:28:02.397773 iam_actions-1.2.20240529/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240529/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240529/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/LICENSE
+-rw-r--r--   0        0        0     2302 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/README.md
+-rw-r--r--   0        0        0      228 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4858362 2024-05-30 02:26:24.977529 iam_actions-1.2.20240530/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-05-30 02:24:52.417094 iam_actions-1.2.20240530/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   632940 2024-05-30 02:26:24.977529 iam_actions-1.2.20240530/iam_actions/policies.json
+-rw-r--r--   0        0        0   209776 2024-05-30 02:26:24.977529 iam_actions-1.2.20240530/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   613908 2024-05-30 02:26:24.977529 iam_actions-1.2.20240530/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-05-30 02:26:25.677532 iam_actions-1.2.20240530/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240530/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240530/PKG-INFO
```

### Comparing `iam_actions-1.2.20240529/LICENSE` & `iam_actions-1.2.20240530/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240529/README.md` & `iam_actions-1.2.20240530/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240529/iam_actions/actions.json` & `iam_actions-1.2.20240530/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974612964554742%*

 * *Differences: {"'application-signals'": "OrderedDict([('ListServiceDependencies', OrderedDict([('access_level', "*

 * *                          "'Undocumented'), ('action', 'ListServiceDependencies'), "*

 * *                          "('condition_keys', []), ('description', 'Not Documented by AWS'), "*

 * *                          "('orphan', False), ('resources', [])])), "*

 * *                          "('UpdateServiceLevelObjective', OrderedDict([('access_level', "*

 * *                          "'Undocumented'), ('action', 'UpdateServiceLe […]*

```diff
@@ -5169,14 +5169,136 @@
             "action": "UpdateReportDefinition",
             "condition_keys": [],
             "description": "Grants permission to update an existing Application Cost Profiler Report configuration",
             "orphan": false,
             "resources": []
         }
     },
+    "application-signals": {
+        "BatchGetServiceLevelObjectiveBudgetReport": {
+            "access_level": "Undocumented",
+            "action": "BatchGetServiceLevelObjectiveBudgetReport",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateServiceLevelObjective": {
+            "access_level": "Undocumented",
+            "action": "CreateServiceLevelObjective",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteServiceLevelObjective": {
+            "access_level": "Undocumented",
+            "action": "DeleteServiceLevelObjective",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetService": {
+            "access_level": "Undocumented",
+            "action": "GetService",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetServiceLevelObjective": {
+            "access_level": "Undocumented",
+            "action": "GetServiceLevelObjective",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListServiceDependencies": {
+            "access_level": "Undocumented",
+            "action": "ListServiceDependencies",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListServiceDependents": {
+            "access_level": "Undocumented",
+            "action": "ListServiceDependents",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListServiceLevelObjectives": {
+            "access_level": "Undocumented",
+            "action": "ListServiceLevelObjectives",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListServiceOperations": {
+            "access_level": "Undocumented",
+            "action": "ListServiceOperations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListServices": {
+            "access_level": "Undocumented",
+            "action": "ListServices",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListTagsForResource": {
+            "access_level": "Undocumented",
+            "action": "ListTagsForResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StartDiscovery": {
+            "access_level": "Undocumented",
+            "action": "StartDiscovery",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "TagResource": {
+            "access_level": "Undocumented",
+            "action": "TagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateServiceLevelObjective": {
+            "access_level": "Undocumented",
+            "action": "UpdateServiceLevelObjective",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        }
+    },
     "application-transformation": {
         "GetContainerization": {
             "access_level": "Undocumented",
             "action": "GetContainerization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
@@ -76085,18 +76207,18 @@
             "description": "Grants permission to retrieve one or more workflows",
             "orphan": false,
             "resources": [
                 "workflow"
             ]
         },
         "BatchPutDataQualityStatisticAnnotation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "BatchPutDataQualityStatisticAnnotation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to annotate datapoints over time for a specific data quality statistic",
             "orphan": false,
             "resources": []
         },
         "BatchStopJobRun": {
             "access_level": "Write",
             "action": "BatchStopJobRun",
             "condition_keys": [],
@@ -76707,28 +76829,31 @@
             "action": "DeregisterDataPreview",
             "condition_keys": [],
             "description": "Grants permission to terminate Glue Studio Notebook session",
             "orphan": false,
             "resources": []
         },
         "DescribeConnectionType": {
-            "access_level": "Undocumented",
+            "access_level": "Permissions management",
             "action": "DescribeConnectionType",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe connection type in glue studio",
             "orphan": false,
             "resources": []
         },
         "DescribeEntity": {
-            "access_level": "Undocumented",
+            "access_level": "Permissions management",
             "action": "DescribeEntity",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe entity in glue studio",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "catalog",
+                "connection"
+            ]
         },
         "GetBlueprint": {
             "access_level": "Read",
             "action": "GetBlueprint",
             "condition_keys": [],
             "description": "Grants permission to retrieve a blueprint",
             "orphan": false,
@@ -76905,26 +77030,26 @@
             "action": "GetDataPreviewStatement",
             "condition_keys": [],
             "description": "Grants permission to get Data Preview Statement",
             "orphan": false,
             "resources": []
         },
         "GetDataQualityModel": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetDataQualityModel",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve the retraining status of the model",
             "orphan": false,
             "resources": []
         },
         "GetDataQualityModelResult": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetDataQualityModelResult",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve the latest predictions for a statistic from the model",
             "orphan": false,
             "resources": []
         },
         "GetDataQualityResult": {
             "access_level": "Read",
             "action": "GetDataQualityResult",
             "condition_keys": [],
@@ -77577,18 +77702,18 @@
             "action": "ListColumnStatisticsTaskRuns",
             "condition_keys": [],
             "description": "Grants permission to list all Column Statistics run-ids that have been executed for the account",
             "orphan": false,
             "resources": []
         },
         "ListConnectionTypes": {
-            "access_level": "Undocumented",
+            "access_level": "Permissions management",
             "action": "ListConnectionTypes",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list connection types in glue studio",
             "orphan": false,
             "resources": []
         },
         "ListCrawlers": {
             "access_level": "List",
             "action": "ListCrawlers",
             "condition_keys": [],
@@ -77649,44 +77774,47 @@
             "description": "Grants permission to retrieve a list of Data Quality rulesets",
             "orphan": false,
             "resources": [
                 "dataQualityRuleset"
             ]
         },
         "ListDataQualityStatisticAnnotations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListDataQualityStatisticAnnotations",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve annotations for a data quality statistic",
             "orphan": false,
             "resources": []
         },
         "ListDataQualityStatistics": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListDataQualityStatistics",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to retrieve data quality statistics and annotations associated with it",
             "orphan": false,
             "resources": []
         },
         "ListDevEndpoints": {
             "access_level": "List",
             "action": "ListDevEndpoints",
             "condition_keys": [],
             "description": "Grants permission to retrieve all development endpoints",
             "orphan": false,
             "resources": []
         },
         "ListEntities": {
-            "access_level": "Undocumented",
+            "access_level": "Permissions management",
             "action": "ListEntities",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list entities in glue studio",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "catalog",
+                "connection"
+            ]
         },
         "ListJobs": {
             "access_level": "List",
             "action": "ListJobs",
             "condition_keys": [],
             "description": "Grants permission to retrieve all current jobs",
             "orphan": false,
@@ -77814,18 +77942,18 @@
             "description": "Grants permission to update catalog encryption settings",
             "orphan": false,
             "resources": [
                 "catalog"
             ]
         },
         "PutDataQualityProfileAnnotation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PutDataQualityProfileAnnotation",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to annotate all datapoints for a profile",
             "orphan": false,
             "resources": []
         },
         "PutResourcePolicy": {
             "access_level": "Permissions management",
             "action": "PutResourcePolicy",
             "condition_keys": [],
@@ -77864,20 +77992,23 @@
             "orphan": false,
             "resources": [
                 "registry",
                 "schema"
             ]
         },
         "RefreshOAuth2Tokens": {
-            "access_level": "Undocumented",
+            "access_level": "Permissions management",
             "action": "RefreshOAuth2Tokens",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to refresh the oauth2 tokens for connection during job execution",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "catalog",
+                "connection"
+            ]
         },
         "RegisterSchemaVersion": {
             "access_level": "Write",
             "action": "RegisterSchemaVersion",
             "condition_keys": [],
             "description": "Grants permission to create a new schema version",
             "orphan": false,
@@ -161641,28 +161772,38 @@
             "description": "Grants permission to return the estimated number of decision tasks in the specified task list",
             "orphan": false,
             "resources": [
                 "domain"
             ]
         },
         "DeleteActivityType": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteActivityType",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "swf:activityType.name",
+                "swf:activityType.version"
+            ],
+            "description": "Grants permission to delete the specified activity type",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "domain"
+            ]
         },
         "DeleteWorkflowType": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteWorkflowType",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "swf:workflowType.name",
+                "swf:workflowType.version"
+            ],
+            "description": "Grants permission to delete the specified workflow type",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "domain"
+            ]
         },
         "DeprecateActivityType": {
             "access_level": "Write",
             "action": "DeprecateActivityType",
             "condition_keys": [
                 "swf:activityType.name",
                 "swf:activityType.version"
```

### Comparing `iam_actions-1.2.20240529/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240530/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240529/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240530/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240529/iam_actions/generate/generate.py` & `iam_actions-1.2.20240530/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240529/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240530/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240529/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240530/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240529/iam_actions/generate/services.py` & `iam_actions-1.2.20240530/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240529/iam_actions/policies.json` & `iam_actions-1.2.20240530/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997489959839359%*

 * *Differences: {"'serviceMap'": "{'AWS Payments': {'ARNRegex': '^arn:aws:payments:::.+:.+'}, 'Amazon CloudWatch "*

 * *                 "Application Signals': OrderedDict([('StringPrefix', 'application-signals'), "*

 * *                 "('Actions', ['BatchGetServiceLevelObjectiveBudgetReport', "*

 * *                 "'CreateServiceLevelObjective', 'DeleteServiceLevelObjective', 'GetService', "*

 * *                 "'GetServiceLevelObjective', 'ListServiceDependencies', 'ListServiceDependents', "*

 * *                 "'ListServiceLevelObjectiv […]*

```diff
@@ -8378,15 +8378,15 @@
                 "payment-cryptography:RequestAlias",
                 "payment-cryptography:ResourceAliases",
                 "payment-cryptography:WrappingKeyIdentifier"
             ]
         },
         "AWS Payments": {
             "ARNFormat": "arn:aws:payments::${Account}:${ResourceType}:${ResourceId}",
-            "ARNRegex": "^arn:aws:payments::[0-9]{12}:.+:.+",
+            "ARNRegex": "^arn:aws:payments:::.+:.+",
             "Actions": [
                 "CreatePaymentInstrument",
                 "DeletePaymentInstrument",
                 "GetPaymentInstrument",
                 "GetPaymentStatus",
                 "ListPaymentInstruments",
                 "ListPaymentPreferences",
@@ -12326,14 +12326,42 @@
             "StringPrefix": "applicationinsights",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
+        "Amazon CloudWatch Application Signals": {
+            "ARNFormat": "arn:aws:application-signals:${Region}:${Account}:slo/{ServiceLevelObjectivesName}",
+            "ARNRegex": "^arn:aws:application-signals:.+:.+:.+",
+            "Actions": [
+                "BatchGetServiceLevelObjectiveBudgetReport",
+                "CreateServiceLevelObjective",
+                "DeleteServiceLevelObjective",
+                "GetService",
+                "GetServiceLevelObjective",
+                "ListServiceDependencies",
+                "ListServiceDependents",
+                "ListServiceLevelObjectives",
+                "ListServiceOperations",
+                "ListServices",
+                "ListTagsForResource",
+                "StartDiscovery",
+                "TagResource",
+                "UntagResource",
+                "UpdateServiceLevelObjective"
+            ],
+            "HasResource": true,
+            "StringPrefix": "application-signals",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
+        },
         "Amazon CloudWatch Evidently": {
             "ARNFormat": "arn:aws:evidently:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:evidently:.+:.+:.+",
             "Actions": [
                 "BatchEvaluateFeature",
                 "CreateExperiment",
                 "CreateFeature",
```

### Comparing `iam_actions-1.2.20240529/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240530/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974747474747475%*

 * *Differences: {"'application-signals'": 'OrderedDict()'}*

```diff
@@ -501,14 +501,15 @@
     "application-autoscaling": {
         "ScalableTarget": {
             "arn_pattern": "arn:*:application-autoscaling:*:*:scalable-target/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "application-cost-profiler": {},
+    "application-signals": {},
     "application-transformation": {},
     "applicationinsights": {},
     "appmesh": {
         "gatewayRoute": {
             "arn_pattern": "arn:*:appmesh:*:*:mesh/*/virtualGateway/*/gatewayRoute/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
```

### Comparing `iam_actions-1.2.20240529/iam_actions/services.json` & `iam_actions-1.2.20240530/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973695286195288%*

 * *Differences: {"'application-signals'": "OrderedDict([('Actions', ['BatchGetServiceLevelObjectiveBudgetReport', "*

 * *                          "'CreateServiceLevelObjective', 'DeleteServiceLevelObjective', "*

 * *                          "'GetService', 'GetServiceLevelObjective', 'ListServiceDependencies', "*

 * *                          "'ListServiceDependents', 'ListServiceLevelObjectives', "*

 * *                          "'ListServiceOperations', 'ListServices', 'ListTagsForResource', "*

 * *                          "'StartDiscovery', ' […]*

```diff
@@ -878,14 +878,48 @@
         ],
         "ConditionKeys": [],
         "HasResource": false,
         "ServiceNames": [
             "AWS Application Cost Profiler Service"
         ]
     },
+    "application-signals": {
+        "ARNFormats": [
+            "arn:aws:application-signals:${Region}:${Account}:slo/{ServiceLevelObjectivesName}"
+        ],
+        "ARNRegexes": [
+            "^arn:aws:application-signals:.+:.+:.+"
+        ],
+        "Actions": [
+            "BatchGetServiceLevelObjectiveBudgetReport",
+            "CreateServiceLevelObjective",
+            "DeleteServiceLevelObjective",
+            "GetService",
+            "GetServiceLevelObjective",
+            "ListServiceDependencies",
+            "ListServiceDependents",
+            "ListServiceLevelObjectives",
+            "ListServiceOperations",
+            "ListServices",
+            "ListTagsForResource",
+            "StartDiscovery",
+            "TagResource",
+            "UntagResource",
+            "UpdateServiceLevelObjective"
+        ],
+        "ConditionKeys": [
+            "aws:RequestTag/${TagKey}",
+            "aws:ResourceTag/${TagKey}",
+            "aws:TagKeys"
+        ],
+        "HasResource": true,
+        "ServiceNames": [
+            "Amazon CloudWatch Application Signals"
+        ]
+    },
     "application-transformation": {
         "ARNFormats": [
             "arn:${Partition}:application-transformation:${Region}:${Account}:${ResourceType}"
         ],
         "ARNRegexes": [
             "^arn:${Partition}:application-transformation:.+:.+:.+"
         ],
@@ -16853,15 +16887,15 @@
         ]
     },
     "payments": {
         "ARNFormats": [
             "arn:aws:payments::${Account}:${ResourceType}:${ResourceId}"
         ],
         "ARNRegexes": [
-            "^arn:aws:payments::[0-9]{12}:.+:.+"
+            "^arn:aws:payments:::.+:.+"
         ],
         "Actions": [
             "CreatePaymentInstrument",
             "DeletePaymentInstrument",
             "GetPaymentInstrument",
             "GetPaymentStatus",
             "ListPaymentInstruments",
```

### Comparing `iam_actions-1.2.20240529/pyproject.toml` & `iam_actions-1.2.20240530/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240529"
+version = "1.2.20240530"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240529/setup.py` & `iam_actions-1.2.20240530/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240529',
+    'version': '1.2.20240530',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240529/PKG-INFO` & `iam_actions-1.2.20240530/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240529
+Version: 1.2.20240530
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

