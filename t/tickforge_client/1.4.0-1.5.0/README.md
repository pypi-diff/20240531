# Comparing `tmp/tickforge_client-1.4.0.tar.gz` & `tmp/tickforge_client-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tickforge_client-1.4.0.tar", max compression
+gzip compressed data, was "tickforge_client-1.5.0.tar", max compression
```

## Comparing `tickforge_client-1.4.0.tar` & `tickforge_client-1.5.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0    10418 2024-05-08 00:08:21.322987 tickforge_client-1.4.0/README.md
--rw-r--r--   0        0        0      726 2024-05-08 00:08:21.335783 tickforge_client-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     6022 2024-05-08 00:08:21.341874 tickforge_client-1.4.0/tickforge_client/__init__.py
--rw-r--r--   0        0        0      636 2024-05-08 00:08:21.344494 tickforge_client-1.4.0/tickforge_client/api/__init__.py
--rw-r--r--   0        0        0    19040 2024-05-08 00:08:21.267912 tickforge_client-1.4.0/tickforge_client/api/auth_api.py
--rw-r--r--   0        0        0     7455 2024-05-08 00:08:21.273214 tickforge_client-1.4.0/tickforge_client/api/builds_api.py
--rw-r--r--   0        0        0     7164 2024-05-08 00:08:21.277152 tickforge_client-1.4.0/tickforge_client/api/db_api.py
--rw-r--r--   0        0        0    17110 2024-05-08 00:08:21.281539 tickforge_client-1.4.0/tickforge_client/api/default_api.py
--rw-r--r--   0        0        0    12503 2024-05-08 00:08:21.284726 tickforge_client-1.4.0/tickforge_client/api/git_api.py
--rw-r--r--   0        0        0     8664 2024-05-08 00:08:21.288866 tickforge_client-1.4.0/tickforge_client/api/github_api.py
--rw-r--r--   0        0        0     6735 2024-05-08 00:08:21.294076 tickforge_client-1.4.0/tickforge_client/api/jobs_api.py
--rw-r--r--   0        0        0    27945 2024-05-08 00:08:21.299287 tickforge_client-1.4.0/tickforge_client/api/metrics_api.py
--rw-r--r--   0        0        0    21793 2024-05-08 00:08:21.304618 tickforge_client-1.4.0/tickforge_client/api/redirects_api.py
--rw-r--r--   0        0        0    23947 2024-05-08 00:08:21.308290 tickforge_client-1.4.0/tickforge_client/api/slack_api.py
--rw-r--r--   0        0        0    59120 2024-05-08 00:08:21.315372 tickforge_client-1.4.0/tickforge_client/api/workspaces_api.py
--rw-r--r--   0        0        0    29482 2024-05-08 00:08:21.349580 tickforge_client-1.4.0/tickforge_client/api_client.py
--rw-r--r--   0        0        0      852 2024-05-08 00:08:21.350843 tickforge_client-1.4.0/tickforge_client/api_response.py
--rw-r--r--   0        0        0    14627 2024-05-08 00:08:21.340061 tickforge_client-1.4.0/tickforge_client/configuration.py
--rw-r--r--   0        0        0     5374 2024-05-08 00:08:21.345944 tickforge_client-1.4.0/tickforge_client/exceptions.py
--rw-r--r--   0        0        0     4163 2024-05-08 00:08:21.343303 tickforge_client-1.4.0/tickforge_client/models/__init__.py
--rw-r--r--   0        0        0     4652 2024-05-08 00:08:20.948458 tickforge_client-1.4.0/tickforge_client/models/always_active.py
--rw-r--r--   0        0        0     4612 2024-02-23 04:03:31.417408 tickforge_client-1.4.0/tickforge_client/models/author_name.py
--rw-r--r--   0        0        0     2483 2024-05-08 00:08:20.957835 tickforge_client-1.4.0/tickforge_client/models/backup.py
--rw-r--r--   0        0        0     2094 2024-05-08 00:08:20.964081 tickforge_client-1.4.0/tickforge_client/models/base_user.py
--rw-r--r--   0        0        0     4582 2024-05-08 00:08:20.969309 tickforge_client-1.4.0/tickforge_client/models/batch_id.py
--rw-r--r--   0        0        0     2348 2024-05-08 00:08:20.974367 tickforge_client-1.4.0/tickforge_client/models/body_bump_app_api_workspaces_app_name_bump_post.py
--rw-r--r--   0        0        0     2663 2024-05-08 00:08:20.979336 tickforge_client-1.4.0/tickforge_client/models/body_qadeploy_api_workspaces_qadeploy_post.py
--rw-r--r--   0        0        0     2257 2024-05-08 00:08:20.984080 tickforge_client-1.4.0/tickforge_client/models/body_qadestroy_api_workspaces_qadestroy_post.py
--rw-r--r--   0        0        0     4572 2024-05-08 00:08:20.988849 tickforge_client-1.4.0/tickforge_client/models/branch.py
--rw-r--r--   0        0        0     2819 2024-05-08 00:08:20.993101 tickforge_client-1.4.0/tickforge_client/models/build_schema.py
--rw-r--r--   0        0        0      957 2024-05-08 00:08:20.996745 tickforge_client-1.4.0/tickforge_client/models/cluster.py
--rw-r--r--   0        0        0     1992 2024-05-08 00:08:21.000060 tickforge_client-1.4.0/tickforge_client/models/code_metric_blob_payload.py
--rw-r--r--   0        0        0     2081 2024-05-08 00:08:21.004606 tickforge_client-1.4.0/tickforge_client/models/code_metric_blob_response.py
--rw-r--r--   0        0        0     2131 2024-05-08 00:08:21.009961 tickforge_client-1.4.0/tickforge_client/models/copy_db_payload.py
--rw-r--r--   0        0        0     2222 2024-05-08 00:08:21.013738 tickforge_client-1.4.0/tickforge_client/models/create_backup_response.py
--rw-r--r--   0        0        0     2664 2024-05-08 00:08:21.017507 tickforge_client-1.4.0/tickforge_client/models/create_build_payload.py
--rw-r--r--   0        0        0     2342 2024-05-08 00:08:21.025496 tickforge_client-1.4.0/tickforge_client/models/create_metric_payload.py
--rw-r--r--   0        0        0     2558 2024-05-08 00:08:21.029253 tickforge_client-1.4.0/tickforge_client/models/create_workspace_payload.py
--rw-r--r--   0        0        0     4602 2024-05-08 00:08:21.032872 tickforge_client-1.4.0/tickforge_client/models/deleted.py
--rw-r--r--   0        0        0     4622 2024-05-08 00:08:21.037831 tickforge_client-1.4.0/tickforge_client/models/display_name.py
--rw-r--r--   0        0        0     4562 2024-05-08 00:08:21.043069 tickforge_client-1.4.0/tickforge_client/models/email.py
--rw-r--r--   0        0        0     4562 2024-05-08 00:08:21.047433 tickforge_client-1.4.0/tickforge_client/models/error.py
--rw-r--r--   0        0        0     4602 2024-05-08 00:08:21.052418 tickforge_client-1.4.0/tickforge_client/models/first_name.py
--rw-r--r--   0        0        0     2377 2024-05-08 00:08:21.056540 tickforge_client-1.4.0/tickforge_client/models/http_validation_error.py
--rw-r--r--   0        0        0     4582 2024-05-08 00:08:21.060466 tickforge_client-1.4.0/tickforge_client/models/image32.py
--rw-r--r--   0        0        0     4602 2024-05-08 00:08:21.065262 tickforge_client-1.4.0/tickforge_client/models/is_admin.py
--rw-r--r--   0        0        0     4622 2024-05-08 00:08:21.070320 tickforge_client-1.4.0/tickforge_client/models/is_app_user.py
--rw-r--r--   0        0        0     4582 2024-05-08 00:08:21.075276 tickforge_client-1.4.0/tickforge_client/models/is_bot.py
--rw-r--r--   0        0        0     4692 2024-05-08 00:08:21.080324 tickforge_client-1.4.0/tickforge_client/models/is_email_confirmed.py
--rw-r--r--   0        0        0     4602 2024-05-08 00:08:21.085256 tickforge_client-1.4.0/tickforge_client/models/is_owner.py
--rw-r--r--   0        0        0     4672 2024-05-08 00:08:21.089602 tickforge_client-1.4.0/tickforge_client/models/is_primary_owner.py
--rw-r--r--   0        0        0     4652 2024-05-08 00:08:21.095776 tickforge_client-1.4.0/tickforge_client/models/is_restricted.py
--rw-r--r--   0        0        0     2704 2024-05-08 00:08:21.099939 tickforge_client-1.4.0/tickforge_client/models/job.py
--rw-r--r--   0        0        0      722 2024-05-08 00:08:21.102924 tickforge_client-1.4.0/tickforge_client/models/job_status.py
--rw-r--r--   0        0        0     4592 2024-05-08 00:08:21.106067 tickforge_client-1.4.0/tickforge_client/models/last_name.py
--rw-r--r--   0        0        0     4573 2024-05-08 00:08:21.110552 tickforge_client-1.4.0/tickforge_client/models/limit.py
--rw-r--r--   0        0        0     3737 2024-05-08 00:08:21.113656 tickforge_client-1.4.0/tickforge_client/models/list_user_response.py
--rw-r--r--   0        0        0     2249 2024-05-08 00:08:21.117276 tickforge_client-1.4.0/tickforge_client/models/metric.py
--rw-r--r--   0        0        0     4612 2024-05-08 00:08:21.120704 tickforge_client-1.4.0/tickforge_client/models/metric_name.py
--rw-r--r--   0        0        0     4602 2024-05-08 00:08:21.123578 tickforge_client-1.4.0/tickforge_client/models/namespace.py
--rw-r--r--   0        0        0     4572 2024-05-08 00:08:21.127167 tickforge_client-1.4.0/tickforge_client/models/offset.py
--rw-r--r--   0        0        0     5185 2024-05-08 00:08:21.131033 tickforge_client-1.4.0/tickforge_client/models/profile.py
--rw-r--r--   0        0        0     4592 2024-05-08 00:08:21.135535 tickforge_client-1.4.0/tickforge_client/models/real_name.py
--rw-r--r--   0        0        0     1869 2024-05-08 00:08:21.138685 tickforge_client-1.4.0/tickforge_client/models/response_metadata.py
--rw-r--r--   0        0        0      760 2024-05-08 00:08:21.142346 tickforge_client-1.4.0/tickforge_client/models/server_timezone.py
--rw-r--r--   0        0        0      735 2024-05-08 00:08:21.144529 tickforge_client-1.4.0/tickforge_client/models/server_type.py
--rw-r--r--   0        0        0     4545 2024-05-08 00:08:21.147922 tickforge_client-1.4.0/tickforge_client/models/size.py
--rw-r--r--   0        0        0     7835 2024-05-08 00:08:21.150969 tickforge_client-1.4.0/tickforge_client/models/slack_member.py
--rw-r--r--   0        0        0     4552 2024-05-08 00:08:21.155433 tickforge_client-1.4.0/tickforge_client/models/team.py
--rw-r--r--   0        0        0     4572 2024-05-08 00:08:21.159306 tickforge_client-1.4.0/tickforge_client/models/team_id.py
--rw-r--r--   0        0        0     4562 2024-05-08 00:08:21.164471 tickforge_client-1.4.0/tickforge_client/models/title.py
--rw-r--r--   0        0        0     1970 2024-05-08 00:08:21.168609 tickforge_client-1.4.0/tickforge_client/models/token_response.py
--rw-r--r--   0        0        0     4532 2024-05-08 00:08:21.172092 tickforge_client-1.4.0/tickforge_client/models/tz.py
--rw-r--r--   0        0        0     4582 2024-05-08 00:08:21.176599 tickforge_client-1.4.0/tickforge_client/models/tz_label.py
--rw-r--r--   0        0        0     4603 2024-05-08 00:08:21.180037 tickforge_client-1.4.0/tickforge_client/models/tz_offset.py
--rw-r--r--   0        0        0     4593 2024-05-08 00:08:21.184197 tickforge_client-1.4.0/tickforge_client/models/updated.py
--rw-r--r--   0        0        0     2508 2024-05-08 00:08:21.188000 tickforge_client-1.4.0/tickforge_client/models/validation_error.py
--rw-r--r--   0        0        0     4733 2024-05-08 00:08:21.190608 tickforge_client-1.4.0/tickforge_client/models/validation_error_loc_inner.py
--rw-r--r--   0        0        0     2442 2024-05-08 00:08:21.193748 tickforge_client-1.4.0/tickforge_client/models/versions_config.py
--rw-r--r--   0        0        0     2706 2024-05-08 00:08:21.196798 tickforge_client-1.4.0/tickforge_client/models/workspace.py
--rw-r--r--   0        0        0     4609 2024-05-08 00:08:21.200222 tickforge_client-1.4.0/tickforge_client/models/workspace_cluster.py
--rw-r--r--   0        0        0     4672 2024-05-08 00:08:21.203641 tickforge_client-1.4.0/tickforge_client/models/x_hub_signature256.py
--rw-r--r--   0        0        0        0 2024-05-08 00:08:21.337500 tickforge_client-1.4.0/tickforge_client/py.typed
--rw-r--r--   0        0        0    13827 2024-05-08 00:08:21.352445 tickforge_client-1.4.0/tickforge_client/rest.py
--rw-r--r--   0        0        0    11377 1970-01-01 00:00:00.000000 tickforge_client-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    10418 2024-05-31 00:07:58.171218 tickforge_client-1.5.0/README.md
+-rw-r--r--   0        0        0      726 2024-05-31 00:07:58.186021 tickforge_client-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6022 2024-05-31 00:07:58.192128 tickforge_client-1.5.0/tickforge_client/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-31 00:07:58.195255 tickforge_client-1.5.0/tickforge_client/api/__init__.py
+-rw-r--r--   0        0        0    19040 2024-05-31 00:07:58.106764 tickforge_client-1.5.0/tickforge_client/api/auth_api.py
+-rw-r--r--   0        0        0     7455 2024-05-31 00:07:58.111209 tickforge_client-1.5.0/tickforge_client/api/builds_api.py
+-rw-r--r--   0        0        0     7164 2024-05-31 00:07:58.115417 tickforge_client-1.5.0/tickforge_client/api/db_api.py
+-rw-r--r--   0        0        0    17110 2024-05-31 00:07:58.119526 tickforge_client-1.5.0/tickforge_client/api/default_api.py
+-rw-r--r--   0        0        0    12503 2024-05-31 00:07:58.123645 tickforge_client-1.5.0/tickforge_client/api/git_api.py
+-rw-r--r--   0        0        0     8664 2024-05-31 00:07:58.127886 tickforge_client-1.5.0/tickforge_client/api/github_api.py
+-rw-r--r--   0        0        0     6735 2024-05-31 00:07:58.131772 tickforge_client-1.5.0/tickforge_client/api/jobs_api.py
+-rw-r--r--   0        0        0    27945 2024-05-31 00:07:58.136618 tickforge_client-1.5.0/tickforge_client/api/metrics_api.py
+-rw-r--r--   0        0        0    21793 2024-05-31 00:07:58.142640 tickforge_client-1.5.0/tickforge_client/api/redirects_api.py
+-rw-r--r--   0        0        0    23947 2024-05-31 00:07:58.147360 tickforge_client-1.5.0/tickforge_client/api/slack_api.py
+-rw-r--r--   0        0        0    59120 2024-05-31 00:07:58.154020 tickforge_client-1.5.0/tickforge_client/api/workspaces_api.py
+-rw-r--r--   0        0        0    29482 2024-05-31 00:07:58.202153 tickforge_client-1.5.0/tickforge_client/api_client.py
+-rw-r--r--   0        0        0      852 2024-05-31 00:07:58.203250 tickforge_client-1.5.0/tickforge_client/api_response.py
+-rw-r--r--   0        0        0    14627 2024-05-31 00:07:58.189646 tickforge_client-1.5.0/tickforge_client/configuration.py
+-rw-r--r--   0        0        0     5374 2024-05-31 00:07:58.196899 tickforge_client-1.5.0/tickforge_client/exceptions.py
+-rw-r--r--   0        0        0     4163 2024-05-31 00:07:58.194027 tickforge_client-1.5.0/tickforge_client/models/__init__.py
+-rw-r--r--   0        0        0     4652 2024-05-31 00:07:57.775278 tickforge_client-1.5.0/tickforge_client/models/always_active.py
+-rw-r--r--   0        0        0     4612 2024-02-23 04:03:31.417408 tickforge_client-1.5.0/tickforge_client/models/author_name.py
+-rw-r--r--   0        0        0     2483 2024-05-31 00:07:57.782873 tickforge_client-1.5.0/tickforge_client/models/backup.py
+-rw-r--r--   0        0        0     2094 2024-05-31 00:07:57.789439 tickforge_client-1.5.0/tickforge_client/models/base_user.py
+-rw-r--r--   0        0        0     4582 2024-05-31 00:07:57.795129 tickforge_client-1.5.0/tickforge_client/models/batch_id.py
+-rw-r--r--   0        0        0     2348 2024-05-31 00:07:57.800800 tickforge_client-1.5.0/tickforge_client/models/body_bump_app_api_workspaces_app_name_bump_post.py
+-rw-r--r--   0        0        0     2663 2024-05-31 00:07:57.806753 tickforge_client-1.5.0/tickforge_client/models/body_qadeploy_api_workspaces_qadeploy_post.py
+-rw-r--r--   0        0        0     2257 2024-05-31 00:07:57.812586 tickforge_client-1.5.0/tickforge_client/models/body_qadestroy_api_workspaces_qadestroy_post.py
+-rw-r--r--   0        0        0     4572 2024-05-31 00:07:57.818764 tickforge_client-1.5.0/tickforge_client/models/branch.py
+-rw-r--r--   0        0        0     2819 2024-05-31 00:07:57.823388 tickforge_client-1.5.0/tickforge_client/models/build_schema.py
+-rw-r--r--   0        0        0      943 2024-05-31 00:07:57.827400 tickforge_client-1.5.0/tickforge_client/models/cluster.py
+-rw-r--r--   0        0        0     1992 2024-05-31 00:07:57.831055 tickforge_client-1.5.0/tickforge_client/models/code_metric_blob_payload.py
+-rw-r--r--   0        0        0     2081 2024-05-31 00:07:57.835569 tickforge_client-1.5.0/tickforge_client/models/code_metric_blob_response.py
+-rw-r--r--   0        0        0     2131 2024-05-31 00:07:57.848977 tickforge_client-1.5.0/tickforge_client/models/copy_db_payload.py
+-rw-r--r--   0        0        0     2222 2024-05-31 00:07:57.858147 tickforge_client-1.5.0/tickforge_client/models/create_backup_response.py
+-rw-r--r--   0        0        0     2664 2024-05-31 00:07:57.866655 tickforge_client-1.5.0/tickforge_client/models/create_build_payload.py
+-rw-r--r--   0        0        0     2342 2024-05-31 00:07:57.870805 tickforge_client-1.5.0/tickforge_client/models/create_metric_payload.py
+-rw-r--r--   0        0        0     2558 2024-05-31 00:07:57.877018 tickforge_client-1.5.0/tickforge_client/models/create_workspace_payload.py
+-rw-r--r--   0        0        0     4602 2024-05-31 00:07:57.881135 tickforge_client-1.5.0/tickforge_client/models/deleted.py
+-rw-r--r--   0        0        0     4622 2024-05-31 00:07:57.885396 tickforge_client-1.5.0/tickforge_client/models/display_name.py
+-rw-r--r--   0        0        0     4562 2024-05-31 00:07:57.890032 tickforge_client-1.5.0/tickforge_client/models/email.py
+-rw-r--r--   0        0        0     4562 2024-05-31 00:07:57.894290 tickforge_client-1.5.0/tickforge_client/models/error.py
+-rw-r--r--   0        0        0     4602 2024-05-31 00:07:57.898998 tickforge_client-1.5.0/tickforge_client/models/first_name.py
+-rw-r--r--   0        0        0     2377 2024-05-31 00:07:57.902266 tickforge_client-1.5.0/tickforge_client/models/http_validation_error.py
+-rw-r--r--   0        0        0     4582 2024-05-31 00:07:57.905945 tickforge_client-1.5.0/tickforge_client/models/image32.py
+-rw-r--r--   0        0        0     4602 2024-05-31 00:07:57.910195 tickforge_client-1.5.0/tickforge_client/models/is_admin.py
+-rw-r--r--   0        0        0     4622 2024-05-31 00:07:57.913985 tickforge_client-1.5.0/tickforge_client/models/is_app_user.py
+-rw-r--r--   0        0        0     4582 2024-05-31 00:07:57.920067 tickforge_client-1.5.0/tickforge_client/models/is_bot.py
+-rw-r--r--   0        0        0     4692 2024-05-31 00:07:57.925256 tickforge_client-1.5.0/tickforge_client/models/is_email_confirmed.py
+-rw-r--r--   0        0        0     4602 2024-05-31 00:07:57.930235 tickforge_client-1.5.0/tickforge_client/models/is_owner.py
+-rw-r--r--   0        0        0     4672 2024-05-31 00:07:57.935138 tickforge_client-1.5.0/tickforge_client/models/is_primary_owner.py
+-rw-r--r--   0        0        0     4652 2024-05-31 00:07:57.939784 tickforge_client-1.5.0/tickforge_client/models/is_restricted.py
+-rw-r--r--   0        0        0     2704 2024-05-31 00:07:57.943949 tickforge_client-1.5.0/tickforge_client/models/job.py
+-rw-r--r--   0        0        0      722 2024-05-31 00:07:57.946692 tickforge_client-1.5.0/tickforge_client/models/job_status.py
+-rw-r--r--   0        0        0     4592 2024-05-31 00:07:57.950348 tickforge_client-1.5.0/tickforge_client/models/last_name.py
+-rw-r--r--   0        0        0     4573 2024-05-31 00:07:57.953731 tickforge_client-1.5.0/tickforge_client/models/limit.py
+-rw-r--r--   0        0        0     3737 2024-05-31 00:07:57.957220 tickforge_client-1.5.0/tickforge_client/models/list_user_response.py
+-rw-r--r--   0        0        0     2249 2024-05-31 00:07:57.960402 tickforge_client-1.5.0/tickforge_client/models/metric.py
+-rw-r--r--   0        0        0     4612 2024-05-31 00:07:57.963847 tickforge_client-1.5.0/tickforge_client/models/metric_name.py
+-rw-r--r--   0        0        0     4602 2024-05-31 00:07:57.967778 tickforge_client-1.5.0/tickforge_client/models/namespace.py
+-rw-r--r--   0        0        0     4572 2024-05-31 00:07:57.971159 tickforge_client-1.5.0/tickforge_client/models/offset.py
+-rw-r--r--   0        0        0     5185 2024-05-31 00:07:57.974631 tickforge_client-1.5.0/tickforge_client/models/profile.py
+-rw-r--r--   0        0        0     4592 2024-05-31 00:07:57.978731 tickforge_client-1.5.0/tickforge_client/models/real_name.py
+-rw-r--r--   0        0        0     1869 2024-05-31 00:07:57.982876 tickforge_client-1.5.0/tickforge_client/models/response_metadata.py
+-rw-r--r--   0        0        0      820 2024-05-31 00:07:57.985480 tickforge_client-1.5.0/tickforge_client/models/server_timezone.py
+-rw-r--r--   0        0        0      735 2024-05-31 00:07:57.987563 tickforge_client-1.5.0/tickforge_client/models/server_type.py
+-rw-r--r--   0        0        0     4545 2024-05-31 00:07:57.991247 tickforge_client-1.5.0/tickforge_client/models/size.py
+-rw-r--r--   0        0        0     7835 2024-05-31 00:07:57.994396 tickforge_client-1.5.0/tickforge_client/models/slack_member.py
+-rw-r--r--   0        0        0     4552 2024-05-31 00:07:57.998592 tickforge_client-1.5.0/tickforge_client/models/team.py
+-rw-r--r--   0        0        0     4572 2024-05-31 00:07:58.003750 tickforge_client-1.5.0/tickforge_client/models/team_id.py
+-rw-r--r--   0        0        0     4562 2024-05-31 00:07:58.007622 tickforge_client-1.5.0/tickforge_client/models/title.py
+-rw-r--r--   0        0        0     1970 2024-05-31 00:07:58.010696 tickforge_client-1.5.0/tickforge_client/models/token_response.py
+-rw-r--r--   0        0        0     4532 2024-05-31 00:07:58.014083 tickforge_client-1.5.0/tickforge_client/models/tz.py
+-rw-r--r--   0        0        0     4582 2024-05-31 00:07:58.018499 tickforge_client-1.5.0/tickforge_client/models/tz_label.py
+-rw-r--r--   0        0        0     4603 2024-05-31 00:07:58.022011 tickforge_client-1.5.0/tickforge_client/models/tz_offset.py
+-rw-r--r--   0        0        0     4593 2024-05-31 00:07:58.025841 tickforge_client-1.5.0/tickforge_client/models/updated.py
+-rw-r--r--   0        0        0     2508 2024-05-31 00:07:58.028959 tickforge_client-1.5.0/tickforge_client/models/validation_error.py
+-rw-r--r--   0        0        0     4733 2024-05-31 00:07:58.032604 tickforge_client-1.5.0/tickforge_client/models/validation_error_loc_inner.py
+-rw-r--r--   0        0        0     2442 2024-05-31 00:07:58.035524 tickforge_client-1.5.0/tickforge_client/models/versions_config.py
+-rw-r--r--   0        0        0     2706 2024-05-31 00:07:58.038520 tickforge_client-1.5.0/tickforge_client/models/workspace.py
+-rw-r--r--   0        0        0     4609 2024-05-31 00:07:58.043066 tickforge_client-1.5.0/tickforge_client/models/workspace_cluster.py
+-rw-r--r--   0        0        0     4672 2024-05-31 00:07:58.046336 tickforge_client-1.5.0/tickforge_client/models/x_hub_signature256.py
+-rw-r--r--   0        0        0        0 2024-05-31 00:07:58.187017 tickforge_client-1.5.0/tickforge_client/py.typed
+-rw-r--r--   0        0        0    13827 2024-05-31 00:07:58.204954 tickforge_client-1.5.0/tickforge_client/rest.py
+-rw-r--r--   0        0        0    11377 1970-01-01 00:00:00.000000 tickforge_client-1.5.0/PKG-INFO
```

### Comparing `tickforge_client-1.4.0/README.md` & `tickforge_client-1.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # tickforge-client
 An API to interact with Uptick Internal Resources
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 1.4.0
+- Package version: 1.5.0
 - Build package: org.openapitools.codegen.languages.PythonPydanticV1ClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

### Comparing `tickforge_client-1.4.0/pyproject.toml` & `tickforge_client-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tickforge_client"
-version = "1.4.0"
+version = "1.5.0"
 description = "Tickforge API"
 authors = ["William Chu <william.chu@uptickhq.com>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/uptick/tickforge"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Tickforge API"]
 include = ["tickforge_client/py.typed"]
```

### Comparing `tickforge_client-1.4.0/tickforge_client/__init__.py` & `tickforge_client-1.5.0/tickforge_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 1.0.0
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.4.0"
+__version__ = "1.5.0"
 
 # import apis into sdk package
 from tickforge_client.api.auth_api import AuthApi
 from tickforge_client.api.builds_api import BuildsApi
 from tickforge_client.api.db_api import DbApi
 from tickforge_client.api.default_api import DefaultApi
 from tickforge_client.api.git_api import GitApi
```

### Comparing `tickforge_client-1.4.0/tickforge_client/api/__init__.py` & `tickforge_client-1.5.0/tickforge_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/api/auth_api.py` & `tickforge_client-1.5.0/tickforge_client/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/api/builds_api.py` & `tickforge_client-1.5.0/tickforge_client/api/builds_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/api/db_api.py` & `tickforge_client-1.5.0/tickforge_client/api/db_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/api/default_api.py` & `tickforge_client-1.5.0/tickforge_client/api/default_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/api/git_api.py` & `tickforge_client-1.5.0/tickforge_client/api/git_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/api/github_api.py` & `tickforge_client-1.5.0/tickforge_client/api/github_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/api/jobs_api.py` & `tickforge_client-1.5.0/tickforge_client/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/api/metrics_api.py` & `tickforge_client-1.5.0/tickforge_client/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/api/redirects_api.py` & `tickforge_client-1.5.0/tickforge_client/api/redirects_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/api/slack_api.py` & `tickforge_client-1.5.0/tickforge_client/api/slack_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/api/workspaces_api.py` & `tickforge_client-1.5.0/tickforge_client/api/workspaces_api.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/api_client.py` & `tickforge_client-1.5.0/tickforge_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.4.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.5.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `tickforge_client-1.4.0/tickforge_client/api_response.py` & `tickforge_client-1.5.0/tickforge_client/api_response.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/configuration.py` & `tickforge_client-1.5.0/tickforge_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.4.0".\
+               "SDK Package Version: 1.5.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `tickforge_client-1.4.0/tickforge_client/exceptions.py` & `tickforge_client-1.5.0/tickforge_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/__init__.py` & `tickforge_client-1.5.0/tickforge_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/always_active.py` & `tickforge_client-1.5.0/tickforge_client/models/always_active.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/author_name.py` & `tickforge_client-1.5.0/tickforge_client/models/author_name.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/backup.py` & `tickforge_client-1.5.0/tickforge_client/models/backup.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/base_user.py` & `tickforge_client-1.5.0/tickforge_client/models/base_user.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/batch_id.py` & `tickforge_client-1.5.0/tickforge_client/models/batch_id.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/body_bump_app_api_workspaces_app_name_bump_post.py` & `tickforge_client-1.5.0/tickforge_client/models/body_bump_app_api_workspaces_app_name_bump_post.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/body_qadeploy_api_workspaces_qadeploy_post.py` & `tickforge_client-1.5.0/tickforge_client/models/body_qadeploy_api_workspaces_qadeploy_post.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/body_qadestroy_api_workspaces_qadestroy_post.py` & `tickforge_client-1.5.0/tickforge_client/models/body_qadestroy_api_workspaces_qadestroy_post.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/branch.py` & `tickforge_client-1.5.0/tickforge_client/models/branch.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/build_schema.py` & `tickforge_client-1.5.0/tickforge_client/models/build_schema.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/cluster.py` & `tickforge_client-1.5.0/tickforge_client/models/cluster.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,23 +25,21 @@
     """
     Name of our EKS Clusters
     """
 
     """
     allowed enum values
     """
-    LUNA = 'luna'
-    BLUE = 'blue'
     SOOTY = 'sooty'
-    THEO = 'theo'
     DEV_MINUS_AU_MINUS_1 = 'dev-au-1'
     STAGING_MINUS_AU_MINUS_1 = 'staging-au-1'
     PROD_MINUS_AU_MINUS_1 = 'prod-au-1'
     PROD_MINUS_AU_MINUS_2 = 'prod-au-2'
     PROD_MINUS_GB_MINUS_1 = 'prod-gb-1'
+    PROD_MINUS_US_MINUS_1 = 'prod-us-1'
     OBSERVABILITY = 'observability'
 
     @classmethod
     def from_json(cls, json_str: str) -> Cluster:
         """Create an instance of Cluster from a JSON string"""
         return Cluster(json.loads(json_str))
```

### Comparing `tickforge_client-1.4.0/tickforge_client/models/code_metric_blob_payload.py` & `tickforge_client-1.5.0/tickforge_client/models/code_metric_blob_payload.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/code_metric_blob_response.py` & `tickforge_client-1.5.0/tickforge_client/models/code_metric_blob_response.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/copy_db_payload.py` & `tickforge_client-1.5.0/tickforge_client/models/copy_db_payload.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/create_backup_response.py` & `tickforge_client-1.5.0/tickforge_client/models/create_backup_response.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/create_build_payload.py` & `tickforge_client-1.5.0/tickforge_client/models/create_build_payload.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/create_metric_payload.py` & `tickforge_client-1.5.0/tickforge_client/models/create_metric_payload.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/create_workspace_payload.py` & `tickforge_client-1.5.0/tickforge_client/models/create_workspace_payload.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/deleted.py` & `tickforge_client-1.5.0/tickforge_client/models/deleted.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/display_name.py` & `tickforge_client-1.5.0/tickforge_client/models/display_name.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/email.py` & `tickforge_client-1.5.0/tickforge_client/models/email.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/error.py` & `tickforge_client-1.5.0/tickforge_client/models/error.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/first_name.py` & `tickforge_client-1.5.0/tickforge_client/models/first_name.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/http_validation_error.py` & `tickforge_client-1.5.0/tickforge_client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/image32.py` & `tickforge_client-1.5.0/tickforge_client/models/image32.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/is_admin.py` & `tickforge_client-1.5.0/tickforge_client/models/is_admin.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/is_app_user.py` & `tickforge_client-1.5.0/tickforge_client/models/is_app_user.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/is_bot.py` & `tickforge_client-1.5.0/tickforge_client/models/is_bot.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/is_email_confirmed.py` & `tickforge_client-1.5.0/tickforge_client/models/is_email_confirmed.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/is_owner.py` & `tickforge_client-1.5.0/tickforge_client/models/is_owner.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/is_primary_owner.py` & `tickforge_client-1.5.0/tickforge_client/models/is_primary_owner.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/is_restricted.py` & `tickforge_client-1.5.0/tickforge_client/models/is_restricted.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/job.py` & `tickforge_client-1.5.0/tickforge_client/models/job.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/job_status.py` & `tickforge_client-1.5.0/tickforge_client/models/job_status.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/last_name.py` & `tickforge_client-1.5.0/tickforge_client/models/last_name.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/limit.py` & `tickforge_client-1.5.0/tickforge_client/models/limit.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/list_user_response.py` & `tickforge_client-1.5.0/tickforge_client/models/list_user_response.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/metric.py` & `tickforge_client-1.5.0/tickforge_client/models/metric.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/metric_name.py` & `tickforge_client-1.5.0/tickforge_client/models/metric_name.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/namespace.py` & `tickforge_client-1.5.0/tickforge_client/models/namespace.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/offset.py` & `tickforge_client-1.5.0/tickforge_client/models/offset.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/profile.py` & `tickforge_client-1.5.0/tickforge_client/models/profile.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/real_name.py` & `tickforge_client-1.5.0/tickforge_client/models/real_name.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/response_metadata.py` & `tickforge_client-1.5.0/tickforge_client/models/response_metadata.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/server_timezone.py` & `tickforge_client-1.5.0/tickforge_client/models/server_timezone.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,14 +30,17 @@
     allowed enum values
     """
     TZ_GB = 'tz_gb'
     TZ_AU = 'tz_au'
     TZ_WA = 'tz_wa'
     TZ_NZ = 'tz_nz'
     TZ_ET = 'tz_et'
+    TZ_PT = 'tz_pt'
+    TZ_CT = 'tz_ct'
+    TZ_MT = 'tz_mt'
 
     @classmethod
     def from_json(cls, json_str: str) -> ServerTimezone:
         """Create an instance of ServerTimezone from a JSON string"""
         return ServerTimezone(json.loads(json_str))
```

### Comparing `tickforge_client-1.4.0/tickforge_client/models/server_type.py` & `tickforge_client-1.5.0/tickforge_client/models/server_type.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/size.py` & `tickforge_client-1.5.0/tickforge_client/models/size.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/slack_member.py` & `tickforge_client-1.5.0/tickforge_client/models/slack_member.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/team.py` & `tickforge_client-1.5.0/tickforge_client/models/team.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/team_id.py` & `tickforge_client-1.5.0/tickforge_client/models/team_id.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/title.py` & `tickforge_client-1.5.0/tickforge_client/models/title.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/token_response.py` & `tickforge_client-1.5.0/tickforge_client/models/token_response.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/tz.py` & `tickforge_client-1.5.0/tickforge_client/models/tz.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/tz_label.py` & `tickforge_client-1.5.0/tickforge_client/models/tz_label.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/tz_offset.py` & `tickforge_client-1.5.0/tickforge_client/models/tz_offset.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/updated.py` & `tickforge_client-1.5.0/tickforge_client/models/updated.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/validation_error.py` & `tickforge_client-1.5.0/tickforge_client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/validation_error_loc_inner.py` & `tickforge_client-1.5.0/tickforge_client/models/validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/versions_config.py` & `tickforge_client-1.5.0/tickforge_client/models/versions_config.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/workspace.py` & `tickforge_client-1.5.0/tickforge_client/models/workspace.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/workspace_cluster.py` & `tickforge_client-1.5.0/tickforge_client/models/workspace_cluster.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/models/x_hub_signature256.py` & `tickforge_client-1.5.0/tickforge_client/models/x_hub_signature256.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/tickforge_client/rest.py` & `tickforge_client-1.5.0/tickforge_client/rest.py`

 * *Files identical despite different names*

### Comparing `tickforge_client-1.4.0/PKG-INFO` & `tickforge_client-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tickforge_client
-Version: 1.4.0
+Version: 1.5.0
 Summary: Tickforge API
 Home-page: https://github.com/uptick/tickforge
 License: NoLicense
 Keywords: OpenAPI,OpenAPI-Generator,Tickforge API
 Author: William Chu
 Author-email: william.chu@uptickhq.com
 Requires-Python: >=3.7,<4.0
@@ -26,15 +26,15 @@
 
 # tickforge-client
 An API to interact with Uptick Internal Resources
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 1.4.0
+- Package version: 1.5.0
 - Build package: org.openapitools.codegen.languages.PythonPydanticV1ClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
```

