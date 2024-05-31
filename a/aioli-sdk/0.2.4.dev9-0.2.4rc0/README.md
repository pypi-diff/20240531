# Comparing `tmp/aioli_sdk-0.2.4.dev9.tar.gz` & `tmp/aioli_sdk-0.2.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioli_sdk-0.2.4.dev9.tar", last modified: Mon May 27 07:14:30 2024, max compression
+gzip compressed data, was "aioli_sdk-0.2.4rc0.tar", last modified: Thu May 30 17:47:31 2024, max compression
```

## Comparing `aioli_sdk-0.2.4.dev9.tar` & `aioli_sdk-0.2.4rc0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-27 07:14:30.547164 aioli_sdk-0.2.4.dev9/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-05-27 07:14:30.547164 aioli_sdk-0.2.4.dev9/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-27 07:14:30.539164 aioli_sdk-0.2.4.dev9/aioli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/__version__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-27 07:14:30.539164 aioli_sdk-0.2.4.dev9/aioli/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/cli/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1644 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/cli/_util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8497 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/cli/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13159 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/cli/deployment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/cli/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14935 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/cli/model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8210 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/cli/registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7221 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/cli/render.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/cli/role.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5304 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/cli/sso.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-27 07:14:30.539164 aioli_sdk-0.2.4.dev9/aioli/cli/test/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/cli/test/conftest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31029 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/cli/test/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6629 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/cli/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3103 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/cli/version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-27 07:14:30.543164 aioli_sdk-0.2.4.dev9/aioli/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/common/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-27 07:14:30.543164 aioli_sdk-0.2.4.dev9/aioli/common/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/common/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/common/api/_util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18000 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/common/api/authentication.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8098 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/common/api/certs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3671 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/common/api/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10969 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/common/api/request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8655 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/common/check.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/common/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8480 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/common/declarative_argparse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/common/requests.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4706 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/common/util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2272 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/aioli/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-27 07:14:30.547164 aioli_sdk-0.2.4.dev9/aioli_sdk.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-05-27 07:14:30.000000 aioli_sdk-0.2.4.dev9/aioli_sdk.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2482 2024-05-27 07:14:30.000000 aioli_sdk-0.2.4.dev9/aioli_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-27 07:14:30.000000 aioli_sdk-0.2.4.dev9/aioli_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-05-27 07:14:30.000000 aioli_sdk-0.2.4.dev9/aioli_sdk.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-27 07:14:28.000000 aioli_sdk-0.2.4.dev9/aioli_sdk.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-05-27 07:14:30.000000 aioli_sdk-0.2.4.dev9/aioli_sdk.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-05-27 07:14:30.000000 aioli_sdk-0.2.4.dev9/aioli_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-27 07:14:30.543164 aioli_sdk-0.2.4.dev9/aiolirest/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3218 2024-05-27 07:14:27.000000 aioli_sdk-0.2.4.dev9/aiolirest/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-27 07:14:30.543164 aioli_sdk-0.2.4.dev9/aiolirest/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-05-27 07:14:27.000000 aioli_sdk-0.2.4.dev9/aiolirest/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22813 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/api/authentication_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    84659 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/api/deployments_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10515 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/api/information_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    91193 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/api/packaged_models_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    66586 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/api/registries_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43082 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/api/roles_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   105944 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/api/templates_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    61885 2024-05-27 07:14:27.000000 aioli_sdk-0.2.4.dev9/aiolirest/api/users_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25050 2024-05-27 07:14:27.000000 aioli_sdk-0.2.4.dev9/aiolirest/api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-05-27 07:14:27.000000 aioli_sdk-0.2.4.dev9/aiolirest/api_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14926 2024-05-27 07:14:27.000000 aioli_sdk-0.2.4.dev9/aiolirest/configuration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5597 2024-05-27 07:14:27.000000 aioli_sdk-0.2.4.dev9/aiolirest/exceptions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-27 07:14:30.547164 aioli_sdk-0.2.4.dev9/aiolirest/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2280 2024-05-27 07:14:27.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3384 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/auto_scaling_template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3986 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/autoscaling.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3662 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/configuration_resources.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7356 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/deployment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4309 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/deployment_model_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5068 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/deployment_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5178 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/deployment_state.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2788 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/error_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3775 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/event_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3261 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/failure_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2642 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/login_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/login_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2820 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/model_auth_token.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4130 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/model_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2970 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/observability.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6263 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/packaged_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5740 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/packaged_model_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2940 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/resource_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3366 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/resources_template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2747 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/role.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2836 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/role_assignment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3296 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/role_assignments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/security.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2649 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/success_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5551 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/trained_model_registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5294 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/trained_model_registry_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3932 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2663 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/user_patch_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3387 2024-05-27 07:14:26.000000 aioli_sdk-0.2.4.dev9/aiolirest/models/user_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-27 07:14:27.000000 aioli_sdk-0.2.4.dev9/aiolirest/py.typed
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8440 2024-05-27 07:14:27.000000 aioli_sdk-0.2.4.dev9/aiolirest/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-27 07:14:30.547164 aioli_sdk-0.2.4.dev9/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2404 2024-05-27 07:09:02.000000 aioli_sdk-0.2.4.dev9/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 17:47:31.710608 aioli_sdk-0.2.4rc0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1418 2024-05-30 17:47:31.710608 aioli_sdk-0.2.4rc0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 17:47:31.702607 aioli_sdk-0.2.4rc0/aioli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/__version__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 17:47:31.702607 aioli_sdk-0.2.4rc0/aioli/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/cli/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1644 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/cli/_util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8532 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/cli/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14634 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/cli/deployment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/cli/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13780 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/cli/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8210 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/cli/registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7221 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/cli/render.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/cli/role.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5304 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/cli/sso.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 17:47:31.702607 aioli_sdk-0.2.4rc0/aioli/cli/test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/cli/test/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30332 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/cli/test/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6629 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/cli/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3290 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/cli/version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 17:47:31.702607 aioli_sdk-0.2.4rc0/aioli/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/common/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 17:47:31.702607 aioli_sdk-0.2.4rc0/aioli/common/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/common/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/common/api/_util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18000 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/common/api/authentication.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8098 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/common/api/certs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3671 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/common/api/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10969 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/common/api/request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8655 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/common/check.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/common/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8480 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/common/declarative_argparse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/common/requests.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4706 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/common/util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2272 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/aioli/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 17:47:31.710608 aioli_sdk-0.2.4rc0/aioli_sdk.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1418 2024-05-30 17:47:31.000000 aioli_sdk-0.2.4rc0/aioli_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2482 2024-05-30 17:47:31.000000 aioli_sdk-0.2.4rc0/aioli_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-30 17:47:31.000000 aioli_sdk-0.2.4rc0/aioli_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-05-30 17:47:31.000000 aioli_sdk-0.2.4rc0/aioli_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-30 17:47:29.000000 aioli_sdk-0.2.4rc0/aioli_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-05-30 17:47:31.000000 aioli_sdk-0.2.4rc0/aioli_sdk.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-05-30 17:47:31.000000 aioli_sdk-0.2.4rc0/aioli_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 17:47:31.706607 aioli_sdk-0.2.4rc0/aiolirest/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3217 2024-05-30 17:47:28.000000 aioli_sdk-0.2.4rc0/aiolirest/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 17:47:31.706607 aioli_sdk-0.2.4rc0/aiolirest/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-05-30 17:47:28.000000 aioli_sdk-0.2.4rc0/aiolirest/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22812 2024-05-30 17:47:28.000000 aioli_sdk-0.2.4rc0/aiolirest/api/authentication_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    84658 2024-05-30 17:47:28.000000 aioli_sdk-0.2.4rc0/aiolirest/api/deployments_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10514 2024-05-30 17:47:28.000000 aioli_sdk-0.2.4rc0/aiolirest/api/information_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    92236 2024-05-30 17:47:28.000000 aioli_sdk-0.2.4rc0/aiolirest/api/packaged_models_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    66585 2024-05-30 17:47:28.000000 aioli_sdk-0.2.4rc0/aiolirest/api/registries_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43081 2024-05-30 17:47:28.000000 aioli_sdk-0.2.4rc0/aiolirest/api/roles_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   105943 2024-05-30 17:47:28.000000 aioli_sdk-0.2.4rc0/aiolirest/api/templates_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    61884 2024-05-30 17:47:28.000000 aioli_sdk-0.2.4rc0/aiolirest/api/users_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25049 2024-05-30 17:47:28.000000 aioli_sdk-0.2.4rc0/aiolirest/api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-05-30 17:47:28.000000 aioli_sdk-0.2.4rc0/aiolirest/api_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14924 2024-05-30 17:47:28.000000 aioli_sdk-0.2.4rc0/aiolirest/configuration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5596 2024-05-30 17:47:28.000000 aioli_sdk-0.2.4rc0/aiolirest/exceptions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-30 17:47:31.710608 aioli_sdk-0.2.4rc0/aiolirest/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2279 2024-05-30 17:47:28.000000 aioli_sdk-0.2.4rc0/aiolirest/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3383 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/auto_scaling_template.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3985 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/autoscaling.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3661 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/configuration_resources.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7355 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/deployment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4308 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/deployment_model_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5067 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/deployment_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5177 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/deployment_state.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2787 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/error_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3774 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/event_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3260 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/failure_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2641 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/login_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2535 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/login_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/model_auth_token.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4129 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/model_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2969 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/observability.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6262 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/packaged_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5739 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/packaged_model_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2939 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/resource_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3365 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/resources_template.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2746 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/role.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2835 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/role_assignment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3295 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/role_assignments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2904 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/security.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2648 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/success_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5550 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/trained_model_registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5293 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/trained_model_registry_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3931 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2662 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/user_patch_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3386 2024-05-30 17:47:27.000000 aioli_sdk-0.2.4rc0/aiolirest/models/user_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-30 17:47:28.000000 aioli_sdk-0.2.4rc0/aiolirest/py.typed
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8439 2024-05-30 17:47:28.000000 aioli_sdk-0.2.4rc0/aiolirest/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-30 17:47:31.710608 aioli_sdk-0.2.4rc0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2403 2024-05-30 17:40:29.000000 aioli_sdk-0.2.4rc0/setup.py
```

### Comparing `aioli_sdk-0.2.4.dev9/PKG-INFO` & `aioli_sdk-0.2.4rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.2.4.dev9
+Version: 0.2.4rc0
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli_sdk-0.2.4.dev9/aioli/cli/_util.py` & `aioli_sdk-0.2.4rc0/aioli/cli/_util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli/cli/cli.py` & `aioli_sdk-0.2.4rc0/aioli/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # © Copyright 2023-2024 Hewlett Packard Enterprise Development LP
 import hashlib
 import json
 import os
 import socket
 import ssl
 import sys
-from argparse import ArgumentDefaultsHelpFormatter, ArgumentError, ArgumentParser
+from argparse import (
+    ArgumentDefaultsHelpFormatter,
+    ArgumentError,
+    ArgumentParser,
+    Namespace,
+)
 from typing import List, Optional, Sequence, Union, cast
 
 import argcomplete
 import argcomplete.completers
 from OpenSSL import SSL, crypto
 from termcolor import colored
 from urllib3.exceptions import MaxRetryError, SSLError
@@ -97,73 +102,15 @@
 
         v = vars(parsed_args)
         if not v.get("func"):
             parser.print_usage()
             parser.exit(2, "{}: no subcommand specified\n".format(parser.prog))
 
         try:
-            # Configure the CLI's Cert singleton.
-            certs.cli_cert = certs.default_load(parsed_args.controller)
-
-            try:
-                check_version(parsed_args)
-            except SSLError:
-                # An SSLError usually means that we queried a controller over HTTPS and got an
-                # untrusted cert, so allow the user to store and trust the current cert. (It
-                # could also mean that we tried to talk HTTPS on the HTTP port, but distinguishing
-                # that based on the exception is annoying, and we'll figure that out in the next
-                # step anyway.)
-                addr = api.parse_master_address(parsed_args.controller)
-                check_not_none(addr.hostname)
-                check_not_none(addr.port)
-                try:
-                    ctx = SSL.Context(SSL.TLSv1_2_METHOD)
-                    conn = SSL.Connection(ctx, socket.socket())
-                    conn.set_tlsext_host_name(cast(str, addr.hostname).encode())
-                    conn.connect(cast(Sequence[Union[str, int]], (addr.hostname, addr.port)))
-                    conn.do_handshake()
-                    peer_cert_chain = conn.get_peer_cert_chain()
-                    if peer_cert_chain is None or len(peer_cert_chain) == 0:
-                        # Peer presented no cert.  It seems unlikely that this is possible after
-                        # do_handshake() succeeded, but checking for None makes mypy happy.
-                        raise crypto.Error()
-                    cert_pem_data = [
-                        crypto.dump_certificate(crypto.FILETYPE_PEM, cert).decode()
-                        for cert in peer_cert_chain
-                    ]
-                except crypto.Error:
-                    die(
-                        "Tried to connect over HTTPS but couldn't get a certificate from the "
-                        "controller; consider using HTTP"
-                    )
-
-                # Compute the fingerprint of the certificate; this is the same as the output of
-                # `openssl x509 -fingerprint -sha256 -inform pem -noout -in <cert>`.
-                cert_hash = hashlib.sha256(ssl.PEM_cert_to_DER_cert(cert_pem_data[0])).hexdigest()
-                cert_fingerprint = ":".join(chunks(cert_hash, 2))
-
-                if not render.yes_or_no(
-                    "The controller sent an untrusted certificate chain with this SHA256 "
-                    "fingerprint:\n"
-                    "{}\nDo you want to trust this certificate from now on?".format(
-                        cert_fingerprint
-                    )
-                ):
-                    die("Unable to verify controller certificate")
-
-                joined_certs = "".join(cert_pem_data)
-                certs.CertStore(certs.default_store()).set_cert(
-                    parsed_args.controller, joined_certs
-                )
-                # Reconfigure the CLI's Cert singleton, but preserve the certificate name.
-                old_cert_name = certs.cli_cert.name
-                certs.cli_cert = certs.Cert(cert_pem=joined_certs, name=old_cert_name)
-
-                check_version(parsed_args)
-
+            configure_certificate_for_controller(parsed_args)
             parsed_args.func(parsed_args)
         except KeyboardInterrupt as e:
             raise e
         except (
             api.errors.BadRequestException,
             api.errors.BadResponseException,
             MaxRetryError,
@@ -197,14 +144,77 @@
                 )
         except Exception:
             die(f"Failed to {parsed_args.func.__name__}", always_print_traceback=True)
     except KeyboardInterrupt:
         die("Interrupting...", exit_code=3)
 
 
+def configure_certificate_for_controller(parsed_args: Namespace) -> None:
+    # Configure the CLI's Cert singleton.
+    certs.cli_cert = certs.default_load(parsed_args.controller)
+
+    try:
+        # check_version doesn't require credentials, so we can use it to verify the certificate.
+        check_version(parsed_args)
+    except SSLError:
+        # An SSLError usually means that we queried a controller over HTTPS and got an
+        # untrusted cert, so allow the user to store and trust the current cert. (It
+        # could also mean that we tried to talk HTTPS on the HTTP port, but distinguishing
+        # that based on the exception is annoying, and we'll figure that out in the next
+        # step anyway.)
+        addr = api.parse_master_address(parsed_args.controller)
+        check_not_none(addr.hostname)
+        check_not_none(addr.port)
+        try:
+            ctx = SSL.Context(SSL.TLSv1_2_METHOD)
+            conn = SSL.Connection(ctx, socket.socket())
+            conn.set_tlsext_host_name(cast(str, addr.hostname).encode())
+            conn.connect(cast(Sequence[Union[str, int]], (addr.hostname, addr.port)))
+            conn.do_handshake()
+            peer_cert_chain = conn.get_peer_cert_chain()
+            if peer_cert_chain is None or len(peer_cert_chain) == 0:
+                # Peer presented no cert.  It seems unlikely that this is possible after
+                # do_handshake() succeeded, but checking for None makes mypy happy.
+                raise crypto.Error()
+            cert_pem_data = [
+                crypto.dump_certificate(crypto.FILETYPE_PEM, cert).decode()
+                for cert in peer_cert_chain
+            ]
+        except crypto.Error:
+            die(
+                "Tried to connect over HTTPS but couldn't get a certificate from the "
+                "controller; consider using HTTP"
+            )
+
+        # Compute the fingerprint of the certificate; this is the same as the output of
+        # `openssl x509 -fingerprint -sha256 -inform pem -noout -in <cert>`.
+        cert_hash = hashlib.sha256(ssl.PEM_cert_to_DER_cert(cert_pem_data[0])).hexdigest()
+        cert_fingerprint = ":".join(chunks(cert_hash, 2))
+
+        if not render.yes_or_no(
+            "The controller sent an untrusted certificate chain with this SHA256 "
+            "fingerprint:\n"
+            "{}\nDo you want to trust this certificate from now on?".format(cert_fingerprint)
+        ):
+            die("Unable to verify controller certificate")
+
+        joined_certs = "".join(cert_pem_data)
+        certs.CertStore(certs.default_store()).set_cert(parsed_args.controller, joined_certs)
+        # Reconfigure the CLI's Cert singleton, but preserve the certificate name.
+        old_cert_name = certs.cli_cert.name
+        certs.cli_cert = certs.Cert(cert_pem=joined_certs, name=old_cert_name)
+
+        try:
+            # let's try that again now that we have reconfigured with the certificate
+            # information supplied by the controller.
+            check_version(parsed_args)
+        except SSLError:
+            die("Failed to verify the controller certificate")
+
+
 def extract_message(e: ApiException) -> Optional[str]:
     decoder = json.JSONDecoder()
     try:
         body_obj = decoder.decode(e.body)
         return str(body_obj["message"])
     except json.JSONDecodeError:
         return None
```

### Comparing `aioli_sdk-0.2.4.dev9/aioli/cli/deployment.py` & `aioli_sdk-0.2.4rc0/aioli/cli/deployment.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,92 +42,116 @@
     # For a more useful display, replace the model ID with its name
     packaged_models_api = aiolirest.PackagedModelsApi(session)
     deployment.model = packaged_models_api.models_id_get(deployment.model).name
 
     d = deployment.to_dict()
     # Remove clusterName for now - INF-243
     d.pop("clusterName")
+
+    # Get the model version for the deployment
+    deployment_model_versions = packaged_models_api.models_versions_get(deployment.model)
+    for r in deployment_model_versions:
+        if r.deployment_id == d["id"]:
+            d["version"] = r.mdl_version
     if args.json:
         render.print_json(d)
     else:
         print(render.format_object_as_yaml(d))
 
 
 @authentication.required
 def list_deployments(args: Namespace) -> None:
     with cli.setup_session(args) as session:
         api_instance = aiolirest.DeploymentsApi(session)
         response = api_instance.deployments_get()
-
     model_api = aiolirest.PackagedModelsApi(session)
 
     if args.json:
         format_json(response, model_api)
     else:
         format_deployments(response, args, model_api)
 
 
 def format_json(response: List[Deployment], model_api: aiolirest.PackagedModelsApi) -> None:
     deps = []
     for d in response:
         # Don't use the d.to_json() method as it adds backslash escapes for double quote
         m_dict = d.to_dict()
-        m_dict.pop("id")
         m_dict.pop("modifiedAt")
         # Use model name instead of id
         model = model_api.models_id_get(d.model)
+        deployment_model_versions = model_api.models_versions_get(model.name)
+        for r in deployment_model_versions:
+            if r.deployment_id == m_dict["id"]:
+                m_dict["version"] = r.mdl_version
+        m_dict.pop("id")
         m_dict["model"] = model.name
         m_dict.pop("clusterName", None)
         deps.append(m_dict)
-
     render.print_json(deps)
 
 
 def format_deployments(
     response: List[Deployment],
     args: Namespace,
     packaged_models_api: aiolirest.PackagedModelsApi,
 ) -> None:
     def format_deployment(e: Deployment, models_api: aiolirest.PackagedModelsApi) -> List[Any]:
         model = models_api.models_id_get(e.model)
         state = e.state
+        total_failures = 0
+
         if state is None:
             state = DeploymentState()
+        else:
+            failure_info = state.failure_info
+            if failure_info:
+                total_failures = len(failure_info)
 
         secondary_state = e.secondary_state
         if secondary_state is None:
             secondary_state = DeploymentState()
 
         assert e.security is not None
 
         auto_scaling = e.auto_scaling
         if auto_scaling is None:
             auto_scaling = Autoscaling()
 
+        if total_failures > 1:
+            e.status = f"{e.status}\n({total_failures} errors)"
+        elif total_failures == 1:
+            e.status = f"{e.status}\n({total_failures} error)"
+
+        deployment_model_versions = models_api.models_versions_get(model.name)
+        version = next(r.mdl_version for r in deployment_model_versions if r.deployment_id == e.id)
         result = [
             e.name,
             model.name,
+            version,
             e.namespace,
             e.status,
             e.security.authentication_required,
             state.status,
             state.traffic_percentage,
         ]
 
         return result
 
     headers = [
         "Name",
         "Model",
+        "Version",
         "Namespace",
         "Status",
         "Auth Required",
         "State",
         "Traffic %",
     ]
+
     values = [format_deployment(r, packaged_models_api) for r in response]
     render.tabulate_or_csv(headers, values, args.csv)
 
 
 @authentication.required
 def create(args: Namespace) -> None:
     with cli.setup_session(args) as session:
@@ -333,15 +357,22 @@
             "create a deployment",
             [
                 Arg(
                     "name",
                     help="The name of the deployment. Must begin with a letter, but may contain "
                     "letters, numbers, and hyphen",
                 ),
-                Arg("--model", help="Model to be deployed", required="true"),
+                Arg(
+                    "--model",
+                    help=(
+                        "The package model id, name or versioned-name (evaluated in that "
+                        "order) to be deployed"
+                    ),
+                    required="true",
+                ),
             ]
             + common_deployment_args,
         ),
         # dashboard command.
         Cmd(
             "dashboard",
             dashboard,
@@ -377,15 +408,21 @@
             [
                 Arg("deploymentname", help="The name of the deployment"),
                 Arg(
                     "--name",
                     help="The new name of the deployment. Must begin with a letter, but may "
                     "contain letters, numbers, and hyphen",
                 ),
-                Arg("--model", help="Model to be deployed"),
+                Arg(
+                    "--model",
+                    help=(
+                        "The package model id, name or versioned-name (evaluated in that "
+                        "order) to be deployed"
+                    ),
+                ),
                 Arg("--pause", action="store_true", help="Pause the deployment"),
                 Arg("--resume", action="store_true", help="Resume the deployment"),
             ]
             + common_deployment_args,
         ),
         Cmd(
             "delete",
```

### Comparing `aioli_sdk-0.2.4.dev9/aioli/cli/errors.py` & `aioli_sdk-0.2.4rc0/aioli/cli/errors.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli/cli/model.py` & `aioli_sdk-0.2.4rc0/aioli/cli/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # © Copyright 2023-2024 Hewlett Packard Enterprise Development LP
-import re
 from argparse import Namespace
 from typing import Any, List
 
-from pydantic import StrictInt
-
 import aiolirest
 from aioli import cli
 from aioli.cli import render
 from aioli.cli.registry import lookup_registry_name_by_id
 from aioli.common import api
 from aioli.common.api import authentication
 from aioli.common.api.errors import NotFoundException, VersionRequiredException
@@ -101,78 +98,48 @@
             environment=construct_environment(args),
             modelFormat=args.format,
             arguments=construct_arguments(args),
         )
         api_instance.models_post(r)
 
 
-def lookup_model(name: str, args: Namespace, api: aiolirest.PackagedModelsApi) -> PackagedModel:
+def lookup_model(name: str, api: aiolirest.PackagedModelsApi) -> PackagedModel:
     # From the database, get the model record. If the model exists in multiple versions,
     # then sufficient version information must be part of the request.
-    model_count = 0
-    models: List[PackagedModel] = api.models_get()
-    for r in models:
-        if r.name == name:
-            model = r
-            model_count += 1
-
-    if model_count == 1:
-        return model  # Found a single version of the specified model
-    if model_count > 1 and not args.version:
-        raise_version_required(name, model_count)
-
-    if model_count == 0:
-        # The specified model does not exist; extract the version suffix if any
-        regexp = re.compile(r"^(.+)\.[Vv](\d+)$")
-        m = regexp.match(name)
-        if m is None:
-            raise NotFoundException(
-                f"model {name} not found. Model versions may optionally be specified "
-                "using the suffix '.v#', for example, '.v1', '.v100'"
-            )
-        name = m.group(1)
-        version = m.group(2)
-
-    # if there is an explicit version specified, then use that
-    if args.version:
-        version = args.version
-
-    return lookup_model_and_version(name, version, models)
+    models: List[PackagedModel] = api.models_get(name)
+    if len(models):
+        return models[0]
+
+    raise NotFoundException(
+        f"model {name} not found. Model versions may optionally be specified "
+        "using the suffix '.v#', for example, '.v1', '.v100'"
+    )
 
 
 def raise_version_required(name: str, count: int) -> None:
     raise VersionRequiredException(f"specify a version as model {name} exists in {count} versions")
 
 
-def lookup_model_and_version(name: str, version: str, models: List[PackagedModel]) -> PackagedModel:
-    # The version may optionally be expressed with a prefix of 'v'
-    version_no_prefix: str = version.lstrip("vV")
-    for r in models:
-        if r.name == name and r.version == StrictInt(version_no_prefix):
-            return r
-    raise NotFoundException(f"model {name} version {version} not found")
-
-
 @authentication.required
 def dashboard(args: Namespace) -> None:
     with cli.setup_session(args) as session:
         api_instance = aiolirest.PackagedModelsApi(session)
 
-    model = lookup_model(args.name, args, api_instance)
+    model = lookup_model(args.name, api_instance)
 
     observability = api_instance.models_id_observability_get(model.id)
     launch_dashboard(args, observability.dashboard_url)
 
 
 @authentication.required
 def show_model(args: Namespace) -> None:
     with cli.setup_session(args) as session:
         api_instance = aiolirest.PackagedModelsApi(session)
 
-    model = lookup_model(args.name, args, api_instance)
+    model = lookup_model(args.name, api_instance)
     registries_api = aiolirest.RegistriesApi(session)
 
     rname = lookup_registry_name_by_id(model.registry, registries_api)
 
     d = model.to_dict()
     d["registry"] = rname
 
@@ -182,15 +149,15 @@
         print(render.format_object_as_yaml(d))
 
 
 @authentication.required
 def update(args: Namespace) -> None:
     with cli.setup_session(args) as session:
         api_instance = aiolirest.PackagedModelsApi(session)
-        found = lookup_model(args.modelname, args, api_instance)
+        found = lookup_model(args.modelname, api_instance)
         request = PackagedModelRequest(
             description=found.description,
             image=found.image,
             name=found.name,
             registry=found.registry,
             url=found.url,
             arguments=found.arguments,
@@ -258,36 +225,36 @@
         api_instance.models_id_put(found.id, request, _headers=headers)
 
 
 @authentication.required
 def delete_model(args: Namespace) -> None:
     with cli.setup_session(args) as session:
         api_instance = aiolirest.PackagedModelsApi(session)
-        found = lookup_model_and_version(args.name, args.version, api_instance.models_get())
+        found = lookup_model(args.name, api_instance)
 
         assert found.id is not None
         api_instance.models_id_delete(found.id)
 
 
 @authentication.required
 def auth_token(args: Namespace) -> None:
     with cli.setup_session(args) as session:
         api_instance = aiolirest.PackagedModelsApi(session)
-        found = lookup_model(args.name, args, api_instance)
+        found = lookup_model(args.name, api_instance)
         assert found.id is not None
         response = api_instance.models_id_token_get(found.id)
     t = response.to_dict()
     print(render.format_object_as_yaml(t))
 
 
 @authentication.required
 def list_versions(args: Namespace) -> None:
     with cli.setup_session(args) as session:
         api_instance = aiolirest.PackagedModelsApi(session)
-        found = lookup_model(args.name, args, api_instance)
+        found = lookup_model(args.name, api_instance)
         assert found.id is not None
         response = api_instance.models_versions_get(found.id)
 
     def format_versions(e: DeploymentModelVersion) -> List[Any]:
         result = [
             e.deployed,
             e.native_app_name,
@@ -335,14 +302,22 @@
     Arg("--limits-memory", help="Memory limit"),
     Arg("--limits-gpu", help="GPU limit"),
     Arg("--requests-cpu", help="CPU request"),
     Arg("--requests-memory", help="Memory request"),
     Arg("--requests-gpu", help="GPU request"),
 ]
 
+VERSIONED_MODEL_HELP_MSG = (
+    "The packaged model id, name or versioned-name (evaluated in that order). "
+    "A versioned-name is the package model name with suffix of the version "
+    "with the format 'name.V###' where '###' is the version number. For example, "
+    "a model named 'my-model' with a version of '23' would be represented by "
+    "versioned-name of: my-model.V23"
+)
+
 main_cmd = Cmd(
     "m|odel|s",
     None,
     "manage packaged models",
     [
         # Inspection commands.
         Cmd(
@@ -374,78 +349,84 @@
         Cmd(
             "dashboard",
             dashboard,
             "launch the packaged model dashboard",
             [
                 Arg(
                     "name",
-                    help="The name of the packaged model.",
+                    help=VERSIONED_MODEL_HELP_MSG,
                 ),
-                Arg("--version", help="The packaged model version to show"),
             ],
         ),
         # Show command.
         Cmd(
             "show",
             show_model,
             "show a packaged model",
             [
                 Arg(
                     "name",
-                    help="The name of the packaged model.",
+                    help=VERSIONED_MODEL_HELP_MSG,
                 ),
                 Group(
                     Arg("--yaml", action="store_true", help="print as YAML", default=True),
                     Arg("--json", action="store_true", help="print as JSON"),
                 ),
-                Arg("--version", help="The packaged model version to show"),
             ],
         ),
         # Update command
         Cmd(
             "update",
             update,
             "modify a packaged model",
             [
-                Arg("modelname", help="The name of the packaged model"),
+                Arg(
+                    "modelname",
+                    help=VERSIONED_MODEL_HELP_MSG,
+                ),
                 Arg(
                     "--name",
                     help="The new name of the packaged model. Must begin with a letter, but may "
                     "contain letters, numbers, and hyphen",
                 ),
                 Arg("--image", help="Docker container image servicing the packaged model"),
-                Arg("--version", help="The packaged model version to update"),
             ]
             + common_model_args,
         ),
         Cmd(
             "delete",
             delete_model,
             "delete a packaged model",
             [
-                Arg("name", help="The name of the packaged model"),
-                Arg("version", help="The packaged model version to delete"),
+                Arg(
+                    "name",
+                    help=VERSIONED_MODEL_HELP_MSG,
+                ),
             ],
         ),
         Cmd(
             "token",
             auth_token,
             "get packaged model auth token",
             [
-                Arg("name", help="The name of the packaged model"),
-                Arg("--version", help="The version of the packaged model"),
+                Arg(
+                    "name",
+                    help=VERSIONED_MODEL_HELP_MSG,
+                ),
             ],
         ),
         Cmd(
             "versions lv",
             list_versions,
             "list of deployment versions for a packaged model",
             [
                 Arg("--csv", action="store_true", help="print as CSV"),
-                Arg("name", help="The name of the packaged model"),
-                Arg("--version", help="The version of the packaged model"),
+                Arg(
+                    "name",
+                    help=VERSIONED_MODEL_HELP_MSG,
+                ),
             ],
         ),
     ],
 )
 
 args_description = [main_cmd]  # type: List[Any]
```

### Comparing `aioli_sdk-0.2.4.dev9/aioli/cli/registry.py` & `aioli_sdk-0.2.4rc0/aioli/cli/registry.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli/cli/render.py` & `aioli_sdk-0.2.4rc0/aioli/cli/render.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli/cli/role.py` & `aioli_sdk-0.2.4rc0/aioli/cli/role.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli/cli/sso.py` & `aioli_sdk-0.2.4rc0/aioli/cli/sso.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli/cli/test/conftest.py` & `aioli_sdk-0.2.4rc0/aioli/cli/test/conftest.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli/cli/test/test_cli.py` & `aioli_sdk-0.2.4rc0/aioli/cli/test/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -323,29 +323,14 @@
         assert yaml_output == yaml_output2, "Expect the same output using .v1"
 
         yaml_output2 = subprocess.check_output(
             ["aioli", "model", "show", "iris-tf-keras.V1"]
         ).decode("utf-8")
         assert yaml_output == yaml_output2, "Expect the same output using .V1"
 
-        yaml_output2 = subprocess.check_output(
-            ["aioli", "model", "show", "iris-tf-keras", "--version", "1"]
-        ).decode("utf-8")
-        assert yaml_output == yaml_output2, "Expect the same output using --version 1"
-
-        yaml_output2 = subprocess.check_output(
-            ["aioli", "model", "show", "iris-tf-keras", "--version", "v1"]
-        ).decode("utf-8")
-        assert yaml_output == yaml_output2, "Expect the same output using --version v1"
-
-        yaml_output2 = subprocess.check_output(
-            ["aioli", "model", "show", "iris-tf-keras", "--version", "V1"]
-        ).decode("utf-8")
-        assert yaml_output == yaml_output2, "Expect the same output using --version V1"
-
     # fmt: off
     def test_model_list_json(self, setup_login: None) -> None:
         expected = (
             '[\n'    # noqa: Q000
             '  {\n'  # noqa: Q000
             '    "arguments": [\n'
             '      "arg1",\n'
@@ -398,27 +383,27 @@
             "openllm       | the model description |         1 | "
             "s3://demo-bento-registry/iris-tf-keras |"
             "                                      | bento-registry1"
         )
         actual = subprocess.check_output(["aioli", "model", "list"]).decode("utf-8")
 
         assert (actual.find(expected)) > 0
-        assert os.system("aioli model delete openllm 1") == 0
+        assert os.system("aioli model delete openllm.v1") == 0
 
     def test_model_update_bad_model_name(self, setup_login: None) -> None:
         # Attempt to update model specifying the version incorrectly. Here we specify
         # a suffix of ".1", and not ".v1" which would specify the name & version.
         # assert (os.system("aioli model update iris-tf-keras.1") == 0)
         try:
             subprocess.check_output(
                 ["aioli", "model", "update", "iris-tf-keras.1"], stderr=subprocess.STDOUT
             )
         except subprocess.CalledProcessError as e:
             assert e.returncode == 1
-            expected = "Failed to modify a packaged model: model iris-tf-keras.1 not found"
+            expected = "Failed to modify a packaged model: model 'iris-tf-keras.1' does not exist."
             actual: str = e.output.decode("utf-8")
             assert actual.find(expected) == 0
 
     def test_model_update(self, setup_login: None) -> None:
         # Update existing model entry and test for expected values
         assert (
             os.system(
@@ -468,16 +453,15 @@
             )
             == 256
         )
 
         # Create a third version of the model using the second version
         assert (
             os.system(
-                "aioli model update iris-tf-keras --name iris-tf-keras "
-                "--version 2 "
+                "aioli model update iris-tf-keras.v2 --name iris-tf-keras "
                 "--registry bento-registry1 "
                 "--url s3://demo-bento-registry/iris-tf-keras_updated_v3 "
                 "--image fictional.registry.example/updated_imagename "
                 '--description "the updated model description"'
             )
             == 0
         )
@@ -491,16 +475,15 @@
         )
         assert (actual.find(expected)) > 0
 
         # Create a fourth with a new name of the model using the second version
         # (specifying the version with the optional v{n} format)
         assert (
             os.system(
-                "aioli model update iris-tf-keras --name iris-tf-keras-v4 "
-                "--version v2 "
+                "aioli model update iris-tf-keras.v2 --name iris-tf-keras-v4 "
                 "--registry bento-registry1 "
                 "--url s3://demo-bento-registry/iris-tf-keras_updated_v3 "
                 "--image fictional.registry.example/updated_imagename "
                 '--description "the updated model description"'
             )
             == 0
         )
@@ -523,15 +506,15 @@
                 "--authentication-required false "
                 "iris-tf-keras-deployment"
             )
             == 0
         )
         actual = subprocess.check_output(["aioli", "deployment", "list"]).decode("utf-8")
         expected = (
-            "iris-tf-keras-deployment | iris-tf-keras | aioli       "
+            "iris-tf-keras-deployment | iris-tf-keras |         3 | aioli       "
             "| Deploying | False           | Deploying |           0"
         )
 
         assert actual.find(expected) > 0
 
     def test_deployment_list_csv(self, setup_login: None) -> None:
         csv_output = subprocess.check_output(["aioli", "deployment", "list", "--csv"]).decode(
@@ -561,16 +544,17 @@
                 "--authentication-required true "
                 "--model iris-tf-keras "
                 "iris-tf-keras-deployment"
             )
             == 0
         )
         actual = subprocess.check_output(["aioli", "deployment", "list"]).decode("utf-8")
+
         expected = (
-            "iris-tf-keras-deployment | iris-tf-keras | aioli       "
+            "iris-tf-keras-deployment | iris-tf-keras |         3 | aioli       "
             "| Deploying | True            | Deploying |           0"
         )
         assert actual.find(expected) > 0
 
         # Disallow --pause and --resume at the same time
         proc = subprocess.run(
             [
@@ -617,15 +601,16 @@
             '    "state": {\n'
             '      "endpoint": "",\n'
             '      "modelId": "",\n'
             '      "nativeAppName": "",\n'
             '      "status": "Deploying",\n'
             '      "trafficPercentage": 0\n'
             '    },\n'  # noqa: Q000
-            '    "status": "Deploying"\n'
+            '    "status": "Deploying",\n'
+            '    "version": "3"\n'
             '  }\n'  # noqa: Q000
             ']\n'    # noqa: Q000
         )
         actual = subprocess.check_output(["aioli", "deployment", "list", "--json"]).decode("utf-8")
         assert actual == expected
     # fmt: on
 
@@ -706,19 +691,19 @@
         assert other_found
 
     def test_deployment_delete(self, setup_login: None) -> None:
         assert os.system("aioli deployment delete iris-tf-keras-deployment") == 0
         assert os.system("aioli deployment delete iris-tf-keras-deployment-2") == 0
 
     def test_model_delete(self, setup_login: None) -> None:
-        assert os.system("aioli model delete iris-tf-keras1 1") == 0
-        assert os.system("aioli model delete iris-tf-keras 1") == 0
-        assert os.system("aioli model delete iris-tf-keras 2") == 0
-        assert os.system("aioli model delete iris-tf-keras 3") == 0
-        assert os.system("aioli model delete iris-tf-keras-v4 1") == 0
+        assert os.system("aioli model delete iris-tf-keras1") == 0
+        assert os.system("aioli model delete iris-tf-keras.v1") == 0
+        assert os.system("aioli model delete iris-tf-keras.v2") == 0
+        assert os.system("aioli model delete iris-tf-keras.v3") == 0
+        assert os.system("aioli model delete iris-tf-keras-v4.v1") == 0
 
     def test_registry_delete(self, setup_login: None) -> None:
         # Delete the registry entry
         assert os.system("aioli registry delete bento-registry1") == 0
 
     def test_user_list(self, setup_login: None) -> None:
         # Test the user table header fields
```

### Comparing `aioli_sdk-0.2.4.dev9/aioli/cli/user.py` & `aioli_sdk-0.2.4rc0/aioli/cli/user.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli/cli/version.py` & `aioli_sdk-0.2.4rc0/aioli/cli/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -73,15 +73,19 @@
             ),
             file=sys.stderr,
         )
     elif version.Version(client_version) > version.Version(controller_version):
         print(
             termcolor.colored(
                 "Controller version {} is less than CLI version {}. "
-                "Consider upgrading the controller.".format(controller_version, client_version),
+                "This CLI may utilize features not supported by an older "
+                "controller. Install a compatible CLI with: "
+                " pip install aioli-sdk=={}".format(
+                    controller_version, client_version, controller_version
+                ),
                 "yellow",
             ),
             file=sys.stderr,
         )
 
 
 def describe_version(parsed_args: argparse.Namespace) -> None:
```

### Comparing `aioli_sdk-0.2.4.dev9/aioli/common/api/authentication.py` & `aioli_sdk-0.2.4rc0/aioli/common/api/authentication.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli/common/api/certs.py` & `aioli_sdk-0.2.4rc0/aioli/common/api/certs.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli/common/api/errors.py` & `aioli_sdk-0.2.4rc0/aioli/common/api/errors.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli/common/api/request.py` & `aioli_sdk-0.2.4rc0/aioli/common/api/request.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli/common/check.py` & `aioli_sdk-0.2.4rc0/aioli/common/check.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli/common/constants.py` & `aioli_sdk-0.2.4rc0/aioli/common/constants.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli/common/declarative_argparse.py` & `aioli_sdk-0.2.4rc0/aioli/common/declarative_argparse.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli/common/requests.py` & `aioli_sdk-0.2.4rc0/aioli/common/requests.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli/common/util.py` & `aioli_sdk-0.2.4rc0/aioli/common/util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli/util.py` & `aioli_sdk-0.2.4rc0/aioli/util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aioli_sdk.egg-info/PKG-INFO` & `aioli_sdk-0.2.4rc0/aioli_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.2.4.dev9
+Version: 0.2.4rc0
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli_sdk-0.2.4.dev9/aioli_sdk.egg-info/SOURCES.txt` & `aioli_sdk-0.2.4rc0/aioli_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/__init__.py` & `aioli_sdk-0.2.4rc0/aiolirest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/api/authentication_api.py` & `aioli_sdk-0.2.4rc0/aiolirest/api/authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/api/deployments_api.py` & `aioli_sdk-0.2.4rc0/aiolirest/api/deployments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/api/information_api.py` & `aioli_sdk-0.2.4rc0/aiolirest/api/information_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/api/packaged_models_api.py` & `aioli_sdk-0.2.4rc0/aiolirest/api/packaged_models_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -54,14 +54,15 @@
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
     def models_get(
         self,
+        model_ref: Annotated[Optional[StrictStr], Field(description="PackagedModel ID, Name or versioned Name (evaluated in that order)")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -71,14 +72,16 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> List[PackagedModel]:
         """Get all models.
 
         Return the properties of all configured models.
 
+        :param model_ref: PackagedModel ID, Name or versioned Name (evaluated in that order)
+        :type model_ref: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -94,14 +97,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._models_get_serialize(
+            model_ref=model_ref,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -119,14 +123,15 @@
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
     def models_get_with_http_info(
         self,
+        model_ref: Annotated[Optional[StrictStr], Field(description="PackagedModel ID, Name or versioned Name (evaluated in that order)")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -136,14 +141,16 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[List[PackagedModel]]:
         """Get all models.
 
         Return the properties of all configured models.
 
+        :param model_ref: PackagedModel ID, Name or versioned Name (evaluated in that order)
+        :type model_ref: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -159,14 +166,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._models_get_serialize(
+            model_ref=model_ref,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -184,14 +192,15 @@
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
     def models_get_without_preload_content(
         self,
+        model_ref: Annotated[Optional[StrictStr], Field(description="PackagedModel ID, Name or versioned Name (evaluated in that order)")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -201,14 +210,16 @@
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Get all models.
 
         Return the properties of all configured models.
 
+        :param model_ref: PackagedModel ID, Name or versioned Name (evaluated in that order)
+        :type model_ref: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -224,14 +235,15 @@
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._models_get_serialize(
+            model_ref=model_ref,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -244,14 +256,15 @@
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
     def _models_get_serialize(
         self,
+        model_ref,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -265,14 +278,18 @@
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
+        if model_ref is not None:
+            
+            _query_params.append(('model-ref', model_ref))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/api/registries_api.py` & `aioli_sdk-0.2.4rc0/aiolirest/api/registries_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/api/roles_api.py` & `aioli_sdk-0.2.4rc0/aiolirest/api/roles_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/api/templates_api.py` & `aioli_sdk-0.2.4rc0/aiolirest/api/templates_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/api/users_api.py` & `aioli_sdk-0.2.4rc0/aiolirest/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/api_client.py` & `aioli_sdk-0.2.4rc0/aiolirest/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/api_response.py` & `aioli_sdk-0.2.4rc0/aiolirest/api_response.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/configuration.py` & `aioli_sdk-0.2.4rc0/aiolirest/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -385,15 +385,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.2.4-dev9\n"\
+               "Version of the API: 0.2.4-rc0\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/exceptions.py` & `aioli_sdk-0.2.4rc0/aiolirest/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/__init__.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/auto_scaling_template.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/auto_scaling_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/autoscaling.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/autoscaling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/configuration_resources.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/configuration_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/deployment.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/deployment_model_version.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/deployment_model_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/deployment_request.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/deployment_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/deployment_state.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/deployment_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/error_response.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/event_info.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/event_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/failure_info.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/failure_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/login_request.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/login_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/login_response.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/login_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/model_auth_token.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/model_auth_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/model_response.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/model_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/observability.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/observability.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/packaged_model.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/packaged_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/packaged_model_request.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/packaged_model_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/resource_profile.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/resource_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/resources_template.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/resources_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/role.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/role_assignment.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/role_assignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/role_assignments.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/role_assignments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/security.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/security.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/success_response.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/success_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/trained_model_registry.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/trained_model_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/trained_model_registry_request.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/trained_model_registry_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/user.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/user_patch_request.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/user_patch_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/models/user_request.py` & `aioli_sdk-0.2.4rc0/aiolirest/models/user_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/aiolirest/rest.py` & `aioli_sdk-0.2.4rc0/aiolirest/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev9
+    The version of the OpenAPI document: 0.2.4-rc0
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev9/setup.py` & `aioli_sdk-0.2.4rc0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as readme:
     markdown_description = "".join(readme.readlines())
 
 setuptools.setup(
     name="aioli-sdk",
-    version="0.2.4-dev9",
+    version="0.2.4-rc0",
     author="HPE AI Solutions",
     # author_email="hello@determined.ai",
     url="https://github.com/determined-ai/aioli",
     description="Aioli (AI OnLine Inference), a platform for deploying AI models at scale.",
     long_description = markdown_description,
     long_description_content_type = "text/markdown",
     license="Apache License 2.0",
```

