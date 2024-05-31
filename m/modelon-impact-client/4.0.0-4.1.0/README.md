# Comparing `tmp/modelon_impact_client-4.0.0.tar.gz` & `tmp/modelon_impact_client-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelon_impact_client-4.0.0.tar", max compression
+gzip compressed data, was "modelon_impact_client-4.1.0.tar", max compression
```

## Comparing `modelon_impact_client-4.0.0.tar` & `modelon_impact_client-4.1.0.tar`

### file list

```diff
@@ -1,79 +1,82 @@
--rw-r--r--   0        0        0     1479 2024-05-17 04:17:21.438211 modelon_impact_client-4.0.0/LICENSE.md
--rw-r--r--   0        0        0     3700 2024-05-17 04:17:21.449211 modelon_impact_client-4.0.0/README.md
--rw-r--r--   0        0        0        0 2024-05-17 04:17:21.324210 modelon_impact_client-4.0.0/modelon/__init__.py
--rw-r--r--   0        0        0        0 2024-05-17 04:17:21.156208 modelon_impact_client-4.0.0/modelon/impact/__init__.py
--rw-r--r--   0        0        0     1035 2024-05-17 04:17:21.417211 modelon_impact_client-4.0.0/modelon/impact/client/__init__.py
--rw-r--r--   0        0        0    28159 2024-05-17 04:17:21.370211 modelon_impact_client-4.0.0/modelon/impact/client/client.py
--rw-r--r--   0        0        0     1949 2024-05-17 04:17:21.218209 modelon_impact_client-4.0.0/modelon/impact/client/configuration.py
--rw-r--r--   0        0        0     1937 2024-05-17 04:17:21.074208 modelon_impact_client-4.0.0/modelon/impact/client/credential_manager.py
--rw-r--r--   0        0        0      119 2024-05-17 04:17:21.398211 modelon_impact_client-4.0.0/modelon/impact/client/entities/__init__.py
--rw-r--r--   0        0        0      640 2024-05-17 04:17:21.322210 modelon_impact_client-4.0.0/modelon/impact/client/entities/asserts.py
--rw-r--r--   0        0        0    27437 2024-05-17 04:17:21.216209 modelon_impact_client-4.0.0/modelon/impact/client/entities/case.py
--rw-r--r--   0        0        0     2260 2024-05-17 04:17:21.233209 modelon_impact_client-4.0.0/modelon/impact/client/entities/content.py
--rw-r--r--   0        0        0     8204 2024-05-17 04:17:21.080208 modelon_impact_client-4.0.0/modelon/impact/client/entities/custom_function.py
--rw-r--r--   0        0        0    26183 2024-05-17 04:17:21.379211 modelon_impact_client-4.0.0/modelon/impact/client/entities/experiment.py
--rw-r--r--   0        0        0     2512 2024-05-17 04:17:21.058207 modelon_impact_client-4.0.0/modelon/impact/client/entities/external_result.py
--rw-r--r--   0        0        0        0 2024-05-17 04:17:21.481212 modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/__init__.py
--rw-r--r--   0        0        0     1249 2024-05-17 04:17:21.307210 modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/case.py
--rw-r--r--   0        0        0      200 2024-05-17 04:17:21.155208 modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/custom_function.py
--rw-r--r--   0        0        0     1305 2024-05-17 04:17:21.405211 modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/experiment.py
--rw-r--r--   0        0        0      192 2024-05-17 04:17:21.418211 modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/external_result.py
--rw-r--r--   0        0        0      186 2024-05-17 04:17:21.140208 modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/model.py
--rw-r--r--   0        0        0      190 2024-05-17 04:17:21.398211 modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/model_executable.py
--rw-r--r--   0        0        0      190 2024-05-17 04:17:21.323210 modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/workspace.py
--rw-r--r--   0        0        0      156 2024-05-17 04:17:21.139208 modelon_impact_client-4.0.0/modelon/impact/client/entities/log.py
--rw-r--r--   0        0        0    16740 2024-05-17 04:17:21.380211 modelon_impact_client-4.0.0/modelon/impact/client/entities/model.py
--rw-r--r--   0        0        0    13656 2024-05-17 04:17:21.368211 modelon_impact_client-4.0.0/modelon/impact/client/entities/model_executable.py
--rw-r--r--   0        0        0    13156 2024-05-17 04:17:21.224209 modelon_impact_client-4.0.0/modelon/impact/client/entities/project.py
--rw-r--r--   0        0        0     1988 2024-05-17 04:17:21.140208 modelon_impact_client-4.0.0/modelon/impact/client/entities/result.py
--rw-r--r--   0        0        0     1479 2024-05-17 04:17:21.316210 modelon_impact_client-4.0.0/modelon/impact/client/entities/status.py
--rw-r--r--   0        0        0    39729 2024-05-17 04:17:21.476212 modelon_impact_client-4.0.0/modelon/impact/client/entities/workspace.py
--rw-r--r--   0        0        0     1531 2024-05-17 04:17:21.372211 modelon_impact_client-4.0.0/modelon/impact/client/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-17 04:17:21.058207 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/__init__.py
--rw-r--r--   0        0        0     5284 2024-05-17 04:17:21.243209 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/asserts.py
--rw-r--r--   0        0        0     4039 2024-05-17 04:17:21.074208 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/expansion.py
--rw-r--r--   0        0        0    11525 2024-05-17 04:17:21.029207 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/extension.py
--rw-r--r--   0        0        0    13950 2024-05-17 04:17:21.446211 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/fmu_based.py
--rw-r--r--   0        0        0        0 2024-05-17 04:17:21.157208 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/interfaces/__init__.py
--rw-r--r--   0        0        0      507 2024-05-17 04:17:21.370211 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/interfaces/definition.py
--rw-r--r--   0        0        0      409 2024-05-17 04:17:21.081208 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/interfaces/expansion.py
--rw-r--r--   0        0        0      188 2024-05-17 04:17:21.017207 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/interfaces/extension.py
--rw-r--r--   0        0        0    21122 2024-05-17 04:17:21.381211 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/model_based.py
--rw-r--r--   0        0        0     2090 2024-05-17 04:17:21.202209 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/modifiers.py
--rw-r--r--   0        0        0     7944 2024-05-17 04:17:21.042207 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/operators.py
--rw-r--r--   0        0        0     1018 2024-05-17 04:17:21.323210 modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/util.py
--rw-r--r--   0        0        0       79 2024-05-17 04:17:21.324210 modelon_impact_client-4.0.0/modelon/impact/client/operations/__init__.py
--rw-r--r--   0        0        0     5814 2024-05-17 04:17:21.382211 modelon_impact_client-4.0.0/modelon/impact/client/operations/base.py
--rw-r--r--   0        0        0     2440 2024-05-17 04:17:21.141208 modelon_impact_client-4.0.0/modelon/impact/client/operations/case.py
--rw-r--r--   0        0        0     2503 2024-05-17 04:17:21.141208 modelon_impact_client-4.0.0/modelon/impact/client/operations/content_import.py
--rw-r--r--   0        0        0     2245 2024-05-17 04:17:21.323210 modelon_impact_client-4.0.0/modelon/impact/client/operations/experiment.py
--rw-r--r--   0        0        0     2409 2024-05-17 04:17:21.420211 modelon_impact_client-4.0.0/modelon/impact/client/operations/external_result_import.py
--rw-r--r--   0        0        0     2720 2024-05-17 04:17:21.131208 modelon_impact_client-4.0.0/modelon/impact/client/operations/fmu_import.py
--rw-r--r--   0        0        0     5846 2024-05-17 04:17:21.486212 modelon_impact_client-4.0.0/modelon/impact/client/operations/model_executable.py
--rw-r--r--   0        0        0     2634 2024-05-17 04:17:21.299210 modelon_impact_client-4.0.0/modelon/impact/client/operations/project_import.py
--rw-r--r--   0        0        0        0 2024-05-17 04:17:21.367210 modelon_impact_client-4.0.0/modelon/impact/client/operations/workspace/__init__.py
--rw-r--r--   0        0        0     2600 2024-05-17 04:17:21.486212 modelon_impact_client-4.0.0/modelon/impact/client/operations/workspace/conversion.py
--rw-r--r--   0        0        0     3627 2024-05-17 04:17:21.487212 modelon_impact_client-4.0.0/modelon/impact/client/operations/workspace/exports.py
--rw-r--r--   0        0        0     2470 2024-05-17 04:17:21.447211 modelon_impact_client-4.0.0/modelon/impact/client/operations/workspace/imports.py
--rw-r--r--   0        0        0     3770 2024-05-17 04:17:21.474212 modelon_impact_client-4.0.0/modelon/impact/client/options.py
--rw-r--r--   0        0        0     5697 2024-05-17 04:17:21.145208 modelon_impact_client-4.0.0/modelon/impact/client/published_workspace_client.py
--rw-r--r--   0        0        0        0 2024-05-17 04:17:21.028207 modelon_impact_client-4.0.0/modelon/impact/client/py.typed
--rw-r--r--   0        0        0        0 2024-05-17 04:17:21.440211 modelon_impact_client-4.0.0/modelon/impact/client/sal/__init__.py
--rw-r--r--   0        0        0      132 2024-05-17 04:17:21.156208 modelon_impact_client-4.0.0/modelon/impact/client/sal/context.py
--rw-r--r--   0        0        0     1544 2024-05-17 04:17:21.093208 modelon_impact_client-4.0.0/modelon/impact/client/sal/custom_function.py
--rw-r--r--   0        0        0      671 2024-05-17 04:17:21.302210 modelon_impact_client-4.0.0/modelon/impact/client/sal/exceptions.py
--rw-r--r--   0        0        0     6787 2024-05-17 04:17:21.447211 modelon_impact_client-4.0.0/modelon/impact/client/sal/experiment.py
--rw-r--r--   0        0        0      630 2024-05-17 04:17:21.074208 modelon_impact_client-4.0.0/modelon/impact/client/sal/exports.py
--rw-r--r--   0        0        0     1476 2024-05-17 04:17:21.278210 modelon_impact_client-4.0.0/modelon/impact/client/sal/external_result.py
--rw-r--r--   0        0        0     3346 2024-05-17 04:17:21.421211 modelon_impact_client-4.0.0/modelon/impact/client/sal/http.py
--rw-r--r--   0        0        0      476 2024-05-17 04:17:21.298210 modelon_impact_client-4.0.0/modelon/impact/client/sal/imports.py
--rw-r--r--   0        0        0     3084 2024-05-17 04:17:21.218209 modelon_impact_client-4.0.0/modelon/impact/client/sal/model_executable.py
--rw-r--r--   0        0        0     4883 2024-05-17 04:17:21.203209 modelon_impact_client-4.0.0/modelon/impact/client/sal/project.py
--rw-r--r--   0        0        0     5353 2024-05-17 04:17:21.370211 modelon_impact_client-4.0.0/modelon/impact/client/sal/request.py
--rw-r--r--   0        0        0     5114 2024-05-17 04:17:21.407211 modelon_impact_client-4.0.0/modelon/impact/client/sal/response.py
--rw-r--r--   0        0        0     3284 2024-05-17 04:17:21.058207 modelon_impact_client-4.0.0/modelon/impact/client/sal/service.py
--rw-r--r--   0        0        0      885 2024-05-17 04:17:21.319210 modelon_impact_client-4.0.0/modelon/impact/client/sal/uri.py
--rw-r--r--   0        0        0      454 2024-05-17 04:17:21.384211 modelon_impact_client-4.0.0/modelon/impact/client/sal/users.py
--rw-r--r--   0        0        0    13616 2024-05-17 04:17:21.383211 modelon_impact_client-4.0.0/modelon/impact/client/sal/workspace.py
--rw-r--r--   0        0        0     1479 2024-05-17 04:23:56.357321 modelon_impact_client-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     4674 1970-01-01 00:00:00.000000 modelon_impact_client-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1479 2024-05-31 07:46:46.684333 modelon_impact_client-4.1.0/LICENSE.md
+-rw-r--r--   0        0        0     3700 2024-05-31 07:46:46.691333 modelon_impact_client-4.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-31 07:46:46.611332 modelon_impact_client-4.1.0/modelon/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 07:46:46.483331 modelon_impact_client-4.1.0/modelon/impact/__init__.py
+-rw-r--r--   0        0        0     1035 2024-05-31 07:46:46.676333 modelon_impact_client-4.1.0/modelon/impact/client/__init__.py
+-rw-r--r--   0        0        0    28159 2024-05-31 07:46:46.649332 modelon_impact_client-4.1.0/modelon/impact/client/client.py
+-rw-r--r--   0        0        0     1949 2024-05-31 07:46:46.537331 modelon_impact_client-4.1.0/modelon/impact/client/configuration.py
+-rw-r--r--   0        0        0     1937 2024-05-31 07:46:46.410330 modelon_impact_client-4.1.0/modelon/impact/client/credential_manager.py
+-rw-r--r--   0        0        0      119 2024-05-31 07:46:46.666333 modelon_impact_client-4.1.0/modelon/impact/client/entities/__init__.py
+-rw-r--r--   0        0        0      640 2024-05-31 07:46:46.609332 modelon_impact_client-4.1.0/modelon/impact/client/entities/asserts.py
+-rw-r--r--   0        0        0    25104 2024-05-31 07:46:46.536331 modelon_impact_client-4.1.0/modelon/impact/client/entities/case.py
+-rw-r--r--   0        0        0     2260 2024-05-31 07:46:46.550331 modelon_impact_client-4.1.0/modelon/impact/client/entities/content.py
+-rw-r--r--   0        0        0     3235 2024-05-31 07:46:46.605332 modelon_impact_client-4.1.0/modelon/impact/client/entities/custom_artifact.py
+-rw-r--r--   0        0        0     8550 2024-05-31 07:46:46.415330 modelon_impact_client-4.1.0/modelon/impact/client/entities/custom_function.py
+-rw-r--r--   0        0        0    26183 2024-05-31 07:46:46.659333 modelon_impact_client-4.1.0/modelon/impact/client/entities/experiment.py
+-rw-r--r--   0        0        0     2512 2024-05-31 07:46:46.394330 modelon_impact_client-4.1.0/modelon/impact/client/entities/external_result.py
+-rw-r--r--   0        0        0     2934 2024-05-31 07:46:46.425330 modelon_impact_client-4.1.0/modelon/impact/client/entities/file_uri.py
+-rw-r--r--   0        0        0        0 2024-05-31 07:46:46.709333 modelon_impact_client-4.1.0/modelon/impact/client/entities/interfaces/__init__.py
+-rw-r--r--   0        0        0     1249 2024-05-31 07:46:46.593332 modelon_impact_client-4.1.0/modelon/impact/client/entities/interfaces/case.py
+-rw-r--r--   0        0        0      788 2024-05-31 07:46:46.425330 modelon_impact_client-4.1.0/modelon/impact/client/entities/interfaces/custom_artifact.py
+-rw-r--r--   0        0        0      200 2024-05-31 07:46:46.476331 modelon_impact_client-4.1.0/modelon/impact/client/entities/interfaces/custom_function.py
+-rw-r--r--   0        0        0     1305 2024-05-31 07:46:46.670333 modelon_impact_client-4.1.0/modelon/impact/client/entities/interfaces/experiment.py
+-rw-r--r--   0        0        0      192 2024-05-31 07:46:46.676333 modelon_impact_client-4.1.0/modelon/impact/client/entities/interfaces/external_result.py
+-rw-r--r--   0        0        0      186 2024-05-31 07:46:46.462330 modelon_impact_client-4.1.0/modelon/impact/client/entities/interfaces/model.py
+-rw-r--r--   0        0        0      190 2024-05-31 07:46:46.666333 modelon_impact_client-4.1.0/modelon/impact/client/entities/interfaces/model_executable.py
+-rw-r--r--   0        0        0      190 2024-05-31 07:46:46.610332 modelon_impact_client-4.1.0/modelon/impact/client/entities/interfaces/workspace.py
+-rw-r--r--   0        0        0      156 2024-05-31 07:46:46.461331 modelon_impact_client-4.1.0/modelon/impact/client/entities/log.py
+-rw-r--r--   0        0        0    16740 2024-05-31 07:46:46.660333 modelon_impact_client-4.1.0/modelon/impact/client/entities/model.py
+-rw-r--r--   0        0        0    13656 2024-05-31 07:46:46.647332 modelon_impact_client-4.1.0/modelon/impact/client/entities/model_executable.py
+-rw-r--r--   0        0        0    13156 2024-05-31 07:46:46.545331 modelon_impact_client-4.1.0/modelon/impact/client/entities/project.py
+-rw-r--r--   0        0        0     1988 2024-05-31 07:46:46.462330 modelon_impact_client-4.1.0/modelon/impact/client/entities/result.py
+-rw-r--r--   0        0        0     1479 2024-05-31 07:46:46.602332 modelon_impact_client-4.1.0/modelon/impact/client/entities/status.py
+-rw-r--r--   0        0        0    40304 2024-05-31 07:46:46.707333 modelon_impact_client-4.1.0/modelon/impact/client/entities/workspace.py
+-rw-r--r--   0        0        0     1531 2024-05-31 07:46:46.651332 modelon_impact_client-4.1.0/modelon/impact/client/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-31 07:46:46.394330 modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/__init__.py
+-rw-r--r--   0        0        0     5284 2024-05-31 07:46:46.554331 modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/asserts.py
+-rw-r--r--   0        0        0     4039 2024-05-31 07:46:46.410330 modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/expansion.py
+-rw-r--r--   0        0        0    11525 2024-05-31 07:46:46.368329 modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/extension.py
+-rw-r--r--   0        0        0    13950 2024-05-31 07:46:46.689333 modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/fmu_based.py
+-rw-r--r--   0        0        0        0 2024-05-31 07:46:46.485331 modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/interfaces/__init__.py
+-rw-r--r--   0        0        0      507 2024-05-31 07:46:46.649332 modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/interfaces/definition.py
+-rw-r--r--   0        0        0      409 2024-05-31 07:46:46.416330 modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/interfaces/expansion.py
+-rw-r--r--   0        0        0      188 2024-05-31 07:46:46.358329 modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/interfaces/extension.py
+-rw-r--r--   0        0        0    21122 2024-05-31 07:46:46.661332 modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/model_based.py
+-rw-r--r--   0        0        0     2090 2024-05-31 07:46:46.523331 modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/modifiers.py
+-rw-r--r--   0        0        0     7944 2024-05-31 07:46:46.380329 modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/operators.py
+-rw-r--r--   0        0        0     1018 2024-05-31 07:46:46.609332 modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/util.py
+-rw-r--r--   0        0        0       79 2024-05-31 07:46:46.610332 modelon_impact_client-4.1.0/modelon/impact/client/operations/__init__.py
+-rw-r--r--   0        0        0     5814 2024-05-31 07:46:46.662333 modelon_impact_client-4.1.0/modelon/impact/client/operations/base.py
+-rw-r--r--   0        0        0     2440 2024-05-31 07:46:46.463330 modelon_impact_client-4.1.0/modelon/impact/client/operations/case.py
+-rw-r--r--   0        0        0     2503 2024-05-31 07:46:46.463330 modelon_impact_client-4.1.0/modelon/impact/client/operations/content_import.py
+-rw-r--r--   0        0        0     2245 2024-05-31 07:46:46.610332 modelon_impact_client-4.1.0/modelon/impact/client/operations/experiment.py
+-rw-r--r--   0        0        0     2409 2024-05-31 07:46:46.677333 modelon_impact_client-4.1.0/modelon/impact/client/operations/external_result_import.py
+-rw-r--r--   0        0        0     2720 2024-05-31 07:46:46.455330 modelon_impact_client-4.1.0/modelon/impact/client/operations/fmu_import.py
+-rw-r--r--   0        0        0     5846 2024-05-31 07:46:46.712333 modelon_impact_client-4.1.0/modelon/impact/client/operations/model_executable.py
+-rw-r--r--   0        0        0     2634 2024-05-31 07:46:46.583332 modelon_impact_client-4.1.0/modelon/impact/client/operations/project_import.py
+-rw-r--r--   0        0        0        0 2024-05-31 07:46:46.646332 modelon_impact_client-4.1.0/modelon/impact/client/operations/workspace/__init__.py
+-rw-r--r--   0        0        0     2600 2024-05-31 07:46:46.713333 modelon_impact_client-4.1.0/modelon/impact/client/operations/workspace/conversion.py
+-rw-r--r--   0        0        0     3627 2024-05-31 07:46:46.714333 modelon_impact_client-4.1.0/modelon/impact/client/operations/workspace/exports.py
+-rw-r--r--   0        0        0     2470 2024-05-31 07:46:46.690333 modelon_impact_client-4.1.0/modelon/impact/client/operations/workspace/imports.py
+-rw-r--r--   0        0        0     3770 2024-05-31 07:46:46.706333 modelon_impact_client-4.1.0/modelon/impact/client/options.py
+-rw-r--r--   0        0        0     5697 2024-05-31 07:46:46.467331 modelon_impact_client-4.1.0/modelon/impact/client/published_workspace_client.py
+-rw-r--r--   0        0        0        0 2024-05-31 07:46:46.368329 modelon_impact_client-4.1.0/modelon/impact/client/py.typed
+-rw-r--r--   0        0        0        0 2024-05-31 07:46:46.685333 modelon_impact_client-4.1.0/modelon/impact/client/sal/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-31 07:46:46.484331 modelon_impact_client-4.1.0/modelon/impact/client/sal/context.py
+-rw-r--r--   0        0        0     1544 2024-05-31 07:46:46.426330 modelon_impact_client-4.1.0/modelon/impact/client/sal/custom_function.py
+-rw-r--r--   0        0        0      671 2024-05-31 07:46:46.588332 modelon_impact_client-4.1.0/modelon/impact/client/sal/exceptions.py
+-rw-r--r--   0        0        0     6787 2024-05-31 07:46:46.689333 modelon_impact_client-4.1.0/modelon/impact/client/sal/experiment.py
+-rw-r--r--   0        0        0      630 2024-05-31 07:46:46.409330 modelon_impact_client-4.1.0/modelon/impact/client/sal/exports.py
+-rw-r--r--   0        0        0     1476 2024-05-31 07:46:46.570332 modelon_impact_client-4.1.0/modelon/impact/client/sal/external_result.py
+-rw-r--r--   0        0        0     3346 2024-05-31 07:46:46.678333 modelon_impact_client-4.1.0/modelon/impact/client/sal/http.py
+-rw-r--r--   0        0        0      476 2024-05-31 07:46:46.582332 modelon_impact_client-4.1.0/modelon/impact/client/sal/imports.py
+-rw-r--r--   0        0        0     3084 2024-05-31 07:46:46.539331 modelon_impact_client-4.1.0/modelon/impact/client/sal/model_executable.py
+-rw-r--r--   0        0        0     4883 2024-05-31 07:46:46.524331 modelon_impact_client-4.1.0/modelon/impact/client/sal/project.py
+-rw-r--r--   0        0        0     5353 2024-05-31 07:46:46.649332 modelon_impact_client-4.1.0/modelon/impact/client/sal/request.py
+-rw-r--r--   0        0        0     5114 2024-05-31 07:46:46.671333 modelon_impact_client-4.1.0/modelon/impact/client/sal/response.py
+-rw-r--r--   0        0        0     3284 2024-05-31 07:46:46.395330 modelon_impact_client-4.1.0/modelon/impact/client/sal/service.py
+-rw-r--r--   0        0        0      885 2024-05-31 07:46:46.605332 modelon_impact_client-4.1.0/modelon/impact/client/sal/uri.py
+-rw-r--r--   0        0        0      454 2024-05-31 07:46:46.664332 modelon_impact_client-4.1.0/modelon/impact/client/sal/users.py
+-rw-r--r--   0        0        0    13616 2024-05-31 07:46:46.663333 modelon_impact_client-4.1.0/modelon/impact/client/sal/workspace.py
+-rw-r--r--   0        0        0     1479 2024-05-31 07:50:48.414890 modelon_impact_client-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4674 1970-01-01 00:00:00.000000 modelon_impact_client-4.1.0/PKG-INFO
```

### Comparing `modelon_impact_client-4.0.0/LICENSE.md` & `modelon_impact_client-4.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/README.md` & `modelon_impact_client-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/__init__.py` & `modelon_impact_client-4.1.0/modelon/impact/client/__init__.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/client.py` & `modelon_impact_client-4.1.0/modelon/impact/client/client.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/configuration.py` & `modelon_impact_client-4.1.0/modelon/impact/client/configuration.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/credential_manager.py` & `modelon_impact_client-4.1.0/modelon/impact/client/credential_manager.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/entities/asserts.py` & `modelon_impact_client-4.1.0/modelon/impact/client/entities/asserts.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/entities/case.py` & `modelon_impact_client-4.1.0/modelon/impact/client/entities/case.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 import logging
-import os
-import tempfile
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Text, Tuple, Union
 
 from modelon.impact.client import exceptions
 from modelon.impact.client.entities.asserts import assert_successful_operation
+from modelon.impact.client.entities.custom_artifact import CustomArtifact
 from modelon.impact.client.entities.custom_function import CustomFunction
 from modelon.impact.client.entities.external_result import ExternalResult
 from modelon.impact.client.entities.interfaces.case import CaseReference
 from modelon.impact.client.entities.log import Log
 from modelon.impact.client.entities.model import (
     Model,
     SimpleModelicaExperimentDefinition,
@@ -20,15 +19,14 @@
 from modelon.impact.client.entities.result import Result
 from modelon.impact.client.entities.status import CaseStatus
 from modelon.impact.client.operations.base import BaseOperation
 from modelon.impact.client.operations.case import CaseOperation
 from modelon.impact.client.sal.experiment import ResultFormat
 
 if TYPE_CHECKING:
-    from modelon.impact.client.sal.experiment import ExperimentService
     from modelon.impact.client.sal.service import Service
 
 logger = logging.getLogger(__name__)
 
 
 def _assert_case_is_complete(
     status: CaseStatus, operation_name: str = "Operation"
@@ -205,93 +203,14 @@
         return self._analysis["simulation_log_level"]
 
     @simulation_log_level.setter
     def simulation_log_level(self, simulation_log_level: str) -> None:
         self._analysis["simulation_log_level"] = simulation_log_level
 
 
-class CustomArtifact:
-    """CustomArtifact class."""
-
-    def __init__(
-        self,
-        workspace_id: str,
-        experiment_id: str,
-        case_id: str,
-        artifact_id: str,
-        download_as: str,
-        exp_sal: ExperimentService,
-    ):
-        self._workspace_id = workspace_id
-        self._exp_id = experiment_id
-        self._case_id = case_id
-        self._artifact_id = artifact_id
-        self._download_as = download_as
-        self._exp_sal = exp_sal
-
-    @property
-    def id(self) -> str:
-        """Id of the custom artifact."""
-        return self._artifact_id
-
-    @property
-    def download_as(self) -> str:
-        """File name for the downloaded artifact."""
-        return self._download_as
-
-    def download(self, path: Optional[str] = None) -> str:
-        """Downloads a custom artifact. Returns the local path to the downloaded
-        artifact.
-
-        Args:
-            path: The local path to the directory to store the downloaded custom
-                artifact. Default: None. If no path is given, custom artifact
-                will be downloaded in a temporary directory.
-
-        Returns:
-            path: Local path to the downloaded custom artifact.
-
-        Example::
-
-            artifact_path = artifact.download()
-            artifact_path = artifact.download('/home/Downloads')
-
-        """
-        artifact, _ = self._exp_sal.case_artifact_get(
-            self._workspace_id, self._exp_id, self._case_id, self.id
-        )
-        if path is None:
-            path = os.path.join(tempfile.gettempdir(), "impact-downloads")
-        os.makedirs(path, exist_ok=True)
-        artifact_path = os.path.join(path, self.download_as)
-        with open(artifact_path, mode="wb") as f:
-            f.write(artifact)
-        return artifact_path
-
-    def get_data(self) -> Union[Text, bytes]:
-        """Returns the custom artifact stream.
-
-        Returns:
-            artifact: The artifact byte stream.
-
-        Example::
-
-            artifact = case.get_artifact("ABCD")
-            data = artifact.get_data() # may raise exception on communication error
-            with open(artifact.download_as, "wb") as f:
-                f.write(data)
-
-        """
-        result_stream, _ = self._exp_sal.case_artifact_get(
-            self._workspace_id, self._exp_id, self._case_id, self.id
-        )
-
-        return result_stream
-
-
 class CaseMeta:
     """Class containing Case meta."""
 
     __slots__ = ["_data"]
 
     def __init__(self, data: Dict[str, Any]):
         self._data = data
@@ -390,14 +309,15 @@
         info: Dict[str, Any],
     ):
         self._case_id = case_id
         self._workspace_id = workspace_id
         self._exp_id = exp_id
         self._sal = service
         self._info = info
+        super().__init__(case_id, workspace_id, exp_id, service, info)
 
     def __eq__(self, obj: object) -> bool:
         return isinstance(obj, Case) and obj._case_id == self._case_id
 
     def __repr__(self) -> str:
         return f"Case with id '{self._case_id}'"
```

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/entities/content.py` & `modelon_impact_client-4.1.0/modelon/impact/client/entities/content.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/entities/custom_function.py` & `modelon_impact_client-4.1.0/modelon/impact/client/entities/custom_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
+from modelon.impact.client.entities.file_uri import FileURI, get_resource_URI_from_str
 from modelon.impact.client.entities.interfaces.case import CaseInterface, CaseReference
 from modelon.impact.client.entities.interfaces.custom_function import (
     CustomFunctionInterface,
 )
 from modelon.impact.client.entities.interfaces.experiment import (
     ExperimentInterface,
     ExperimentReference,
@@ -34,14 +35,15 @@
             int,
         ),
         "String": (str,),
         "Boolean": (bool,),
         "Enumeration": (str,),
         "CaseResult": (CaseInterface,),
         "ExperimentResult": (ExperimentInterface,),
+        "FileURI": (FileURI,),
     }
 
     def __init__(self, name: str, value: Any, value_type: str, valid_values: List[Any]):
         self._name = name
         self._value = value
         self._value_type = value_type
         self._valid_values = valid_values
@@ -77,14 +79,16 @@
     def as_raw_dict(self) -> Dict[str, Any]:
         new_dict = {}
         for key, value in self.items():
             if isinstance(value, ExperimentInterface):
                 new_dict[key] = value.id
             elif isinstance(value, CaseInterface):
                 new_dict[key] = f"{value.experiment_id}/{value.id}"
+            elif isinstance(value, FileURI):
+                new_dict[key] = str(value)
             else:
                 new_dict[key] = value
         return new_dict
 
 
 class CustomFunction(CustomFunctionInterface):
     """Class containing CustomFunction functionalities."""
@@ -153,14 +157,16 @@
                 experiment_id, case_id = value.split("/")
                 case_info = self._sal.experiment.case_get(
                     self._workspace_id, experiment_id, case_id
                 )
                 parameter.value = CaseReference(
                     case_id, self._workspace_id, experiment_id, self._sal, case_info
                 )
+            elif parameter.type == "FileURI" and isinstance(value, str):
+                parameter.value = get_resource_URI_from_str(value)
             else:
                 parameter.value = value
 
         return new
 
     @property
     def parameter_values(self) -> ParameterDict:
```

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/entities/experiment.py` & `modelon_impact_client-4.1.0/modelon/impact/client/entities/experiment.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/entities/external_result.py` & `modelon_impact_client-4.1.0/modelon/impact/client/entities/external_result.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/case.py` & `modelon_impact_client-4.1.0/modelon/impact/client/entities/interfaces/case.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/entities/interfaces/experiment.py` & `modelon_impact_client-4.1.0/modelon/impact/client/entities/interfaces/experiment.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/entities/model.py` & `modelon_impact_client-4.1.0/modelon/impact/client/entities/model.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/entities/model_executable.py` & `modelon_impact_client-4.1.0/modelon/impact/client/entities/model_executable.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/entities/project.py` & `modelon_impact_client-4.1.0/modelon/impact/client/entities/project.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/entities/result.py` & `modelon_impact_client-4.1.0/modelon/impact/client/entities/result.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/entities/status.py` & `modelon_impact_client-4.1.0/modelon/impact/client/entities/status.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/entities/workspace.py` & `modelon_impact_client-4.1.0/modelon/impact/client/entities/workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 from modelon.impact.client.configuration import Experimental
 from modelon.impact.client.entities.custom_function import CustomFunction
 from modelon.impact.client.entities.experiment import Experiment
 from modelon.impact.client.entities.external_result import ExternalResult
+from modelon.impact.client.entities.file_uri import ModelicaResourceURI
 from modelon.impact.client.entities.interfaces.workspace import WorkspaceInterface
 from modelon.impact.client.entities.model import Model
 from modelon.impact.client.entities.model_executable import ModelExecutable
 from modelon.impact.client.entities.project import Project, VcsUri
 from modelon.impact.client.exceptions import (
     NoAssociatedPublishedWorkspaceError,
     RemotePublishedWorkspaceLinkError,
@@ -1269,7 +1270,26 @@
             )
             return None
         return PublishedWorkspace(
             published_workspaces[0]["id"],
             definition=PublishedWorkspaceDefinition.from_dict(published_workspaces[0]),
             service=self._sal,
         )
+
+    @Experimental
+    def get_modelica_resource_uri(
+        self, library: str, resource_path: str
+    ) -> ModelicaResourceURI:
+        """Returns a ModelicaResourceURI class.
+
+        Returns:
+            The ModelicaResourceURI class object.
+
+        Example::
+
+            modelica_resource_ref = workspace.get_modelica_resource_uri(
+                library,
+                resource_path
+            )
+
+        """
+        return ModelicaResourceURI(library=library, resource_path=resource_path)
```

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/exceptions.py` & `modelon_impact_client-4.1.0/modelon/impact/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/asserts.py` & `modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/asserts.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/expansion.py` & `modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/expansion.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/extension.py` & `modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/extension.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/fmu_based.py` & `modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/fmu_based.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/model_based.py` & `modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/model_based.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/modifiers.py` & `modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/modifiers.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/operators.py` & `modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/operators.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/experiment_definition/util.py` & `modelon_impact_client-4.1.0/modelon/impact/client/experiment_definition/util.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/operations/base.py` & `modelon_impact_client-4.1.0/modelon/impact/client/operations/base.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/operations/case.py` & `modelon_impact_client-4.1.0/modelon/impact/client/operations/case.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/operations/content_import.py` & `modelon_impact_client-4.1.0/modelon/impact/client/operations/content_import.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/operations/experiment.py` & `modelon_impact_client-4.1.0/modelon/impact/client/operations/experiment.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/operations/external_result_import.py` & `modelon_impact_client-4.1.0/modelon/impact/client/operations/external_result_import.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/operations/fmu_import.py` & `modelon_impact_client-4.1.0/modelon/impact/client/operations/fmu_import.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/operations/model_executable.py` & `modelon_impact_client-4.1.0/modelon/impact/client/operations/model_executable.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/operations/project_import.py` & `modelon_impact_client-4.1.0/modelon/impact/client/operations/project_import.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/operations/workspace/conversion.py` & `modelon_impact_client-4.1.0/modelon/impact/client/operations/workspace/conversion.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/operations/workspace/exports.py` & `modelon_impact_client-4.1.0/modelon/impact/client/operations/workspace/exports.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/operations/workspace/imports.py` & `modelon_impact_client-4.1.0/modelon/impact/client/operations/workspace/imports.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/options.py` & `modelon_impact_client-4.1.0/modelon/impact/client/options.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/published_workspace_client.py` & `modelon_impact_client-4.1.0/modelon/impact/client/published_workspace_client.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/sal/custom_function.py` & `modelon_impact_client-4.1.0/modelon/impact/client/sal/custom_function.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/sal/exceptions.py` & `modelon_impact_client-4.1.0/modelon/impact/client/sal/exceptions.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/sal/experiment.py` & `modelon_impact_client-4.1.0/modelon/impact/client/sal/experiment.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/sal/exports.py` & `modelon_impact_client-4.1.0/modelon/impact/client/sal/exports.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/sal/external_result.py` & `modelon_impact_client-4.1.0/modelon/impact/client/sal/external_result.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/sal/http.py` & `modelon_impact_client-4.1.0/modelon/impact/client/sal/http.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/sal/model_executable.py` & `modelon_impact_client-4.1.0/modelon/impact/client/sal/model_executable.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/sal/project.py` & `modelon_impact_client-4.1.0/modelon/impact/client/sal/project.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/sal/request.py` & `modelon_impact_client-4.1.0/modelon/impact/client/sal/request.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/sal/response.py` & `modelon_impact_client-4.1.0/modelon/impact/client/sal/response.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/sal/service.py` & `modelon_impact_client-4.1.0/modelon/impact/client/sal/service.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/sal/uri.py` & `modelon_impact_client-4.1.0/modelon/impact/client/sal/uri.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/modelon/impact/client/sal/workspace.py` & `modelon_impact_client-4.1.0/modelon/impact/client/sal/workspace.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-4.0.0/pyproject.toml` & `modelon_impact_client-4.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "modelon-impact-client"
 packages = [
     { include = "modelon" },
 ]
-version = "4.0.0"
+version = "4.1.0"
 description = "Client library for easy scripting against Modelon Impact"
 readme = "README.md"
 homepage = "https://www.modelon.com/modelon-impact"
 repository = "https://github.com/modelon-community/impact-client-python"
 documentation = "https://modelon-impact-client.readthedocs.io"
 license = "BSD"
 authors = [
```

### Comparing `modelon_impact_client-4.0.0/PKG-INFO` & `modelon_impact_client-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelon-impact-client
-Version: 4.0.0
+Version: 4.1.0
 Summary: Client library for easy scripting against Modelon Impact
 Home-page: https://www.modelon.com/modelon-impact
 License: BSD
 Keywords: impact,client,API
 Author: WEP
 Author-email: impact@modelon.com
 Requires-Python: >=3.8.0,<4.0.0
```

