# Comparing `tmp/dbt_platform_helper-8.4.1.tar.gz` & `tmp/dbt_platform_helper-8.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_platform_helper-8.4.1.tar", max compression
+gzip compressed data, was "dbt_platform_helper-8.5.0.tar", max compression
```

## Comparing `dbt_platform_helper-8.4.1.tar` & `dbt_platform_helper-8.5.0.tar`

### file list

```diff
@@ -1,92 +1,94 @@
--rw-r--r--   0        0        0     1090 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/LICENSE
--rw-r--r--   0        0        0    17907 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/COMMANDS.md
--rw-r--r--   0        0        0     1762 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/README.md
--rw-r--r--   0        0        0        0 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/__init__.py
--rw-r--r--   0        0        0     4522 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/addon-plans.yml
--rw-r--r--   0        0        0     1315 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/addons-template-map.yml
--rw-r--r--   0        0        0        0 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/commands/__init__.py
--rw-r--r--   0        0        0     9957 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/commands/application.py
--rwxr-xr-x   0        0        0     3226 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/commands/check_cloudformation.py
--rw-r--r--   0        0        0    11192 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/commands/codebase.py
--rw-r--r--   0        0        0    14847 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/commands/conduit.py
--rw-r--r--   0        0        0    11480 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/commands/config.py
--rwxr-xr-x   0        0        0    16297 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/commands/copilot.py
--rwxr-xr-x   0        0        0    35037 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/commands/dns.py
--rw-r--r--   0        0        0    11417 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/commands/environment.py
--rw-r--r--   0        0        0      853 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/commands/generate.py
--rw-r--r--   0        0        0     6674 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/commands/pipeline.py
--rwxr-xr-x   0        0        0     3860 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/commands/secrets.py
--rw-r--r--   0        0        0        0 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/custom_resources/__init__.py
--rw-r--r--   0        0        0     2396 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/custom_resources/s3_object.py
--rw-r--r--   0        0        0      342 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/default-extensions.yml
--rw-r--r--   0        0        0      499 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/exceptions.py
--rw-r--r--   0        0        0      369 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/jinja2_tags.py
--rw-r--r--   0        0        0      158 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/.copilot/config.yml
--rwxr-xr-x   0        0        0      164 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/.copilot/image_build_run.sh
--rwxr-xr-x   0        0        0      121 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/.copilot/phases/build.sh
--rwxr-xr-x   0        0        0      123 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/.copilot/phases/install.sh
--rwxr-xr-x   0        0        0      126 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/.copilot/phases/post_build.sh
--rwxr-xr-x   0        0        0      125 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/.copilot/phases/pre_build.sh
--rw-r--r--   0        0        0     1081 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/COMMANDS.md.jinja
--rw-r--r--   0        0        0      618 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addon-instructions.txt
--rw-r--r--   0        0        0      412 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/README.md
--rw-r--r--   0        0        0      734 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/env/addons.parameters.yml
--rw-r--r--   0        0        0    26381 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/env/aurora-postgres.yml
--rw-r--r--   0        0        0     6064 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/env/monitoring.yml
--rw-r--r--   0        0        0    10853 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/env/opensearch.yml
--rw-r--r--   0        0        0    25624 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/env/rds-postgres.yml
--rw-r--r--   0        0        0     7613 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/env/redis-cluster.yml
--rw-r--r--   0        0        0     7626 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/env/s3.yml
--rw-r--r--   0        0        0     3658 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/env/vpc.yml
--rw-r--r--   0        0        0      956 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml
--rw-r--r--   0        0        0     2403 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/svc/s3-policy.yml
--rw-r--r--   0        0        0      893 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/svc/subscription-filter.yml
--rw-r--r--   0        0        0     1836 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/ci-codebuild-role-policy.json
--rw-r--r--   0        0        0      197 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/create-codebuild-role.json
--rw-r--r--   0        0        0     1180 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/custom-codebuild-role-policy.json
--rw-r--r--   0        0        0      781 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/env/manifest.yml
--rw-r--r--   0        0        0      169 2024-05-23 15:08:58.454227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/env/overrides/.gitignore
--rw-r--r--   0        0        0      443 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/env/overrides/README.md
--rw-r--r--   0        0        0      284 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/env/overrides/bin/override.ts
--rw-r--r--   0        0        0      339 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/env/overrides/cdk.json
--rw-r--r--   0        0        0     1760 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/env/overrides/log_resource_policy.json
--rw-r--r--   0        0        0   155387 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/env/overrides/package-lock.json
--rw-r--r--   0        0        0      536 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/env/overrides/package.json
--rw-r--r--   0        0        0     1910 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/env/overrides/stack.ts
--rw-r--r--   0        0        0      710 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/env/overrides/tsconfig.json
--rw-r--r--   0        0        0      259 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/env/terraform-overrides/cfn.patches.yml
--rw-r--r--   0        0        0     1959 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/manifest.yml
--rw-r--r--   0        0        0      169 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/overrides/.gitignore
--rw-r--r--   0        0        0      227 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/overrides/bin/override.ts
--rw-r--r--   0        0        0      287 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.deploy.yml
--rw-r--r--   0        0        0      781 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml
--rw-r--r--   0        0        0      339 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/overrides/cdk.json
--rw-r--r--   0        0        0   152518 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json
--rw-r--r--   0        0        0      536 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json
--rw-r--r--   0        0        0    20142 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts
--rw-r--r--   0        0        0      651 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json
--rw-r--r--   0        0        0     1205 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts
--rw-r--r--   0        0        0     3178 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/environments/buildspec.yml
--rw-r--r--   0        0        0     1778 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/environments/manifest.yml
--rw-r--r--   0        0        0      617 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml
--rw-r--r--   0        0        0      741 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/svc/maintenance_pages/default.html
--rw-r--r--   0        0        0      783 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/svc/maintenance_pages/migration.html
--rw-r--r--   0        0        0     2881 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/svc/manifest-backend.yml
--rw-r--r--   0        0        0     3921 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/svc/manifest-public.yml
--rw-r--r--   0        0        0      386 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/templates/svc/overrides/cfn.patches.yml
--rw-r--r--   0        0        0        0 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/utils/__init__.py
--rw-r--r--   0        0        0     3555 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/utils/application.py
--rw-r--r--   0        0        0    10297 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/utils/aws.py
--rw-r--r--   0        0        0     2943 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/utils/click.py
--rw-r--r--   0        0        0     1053 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/utils/cloudformation.py
--rw-r--r--   0        0        0      484 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/utils/cloudfoundry.py
--rw-r--r--   0        0        0     1720 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/utils/files.py
--rw-r--r--   0        0        0      384 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/utils/git.py
--rw-r--r--   0        0        0      507 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/utils/manifests.py
--rw-r--r--   0        0        0      115 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/utils/messages.py
--rw-r--r--   0        0        0      469 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/utils/template.py
--rw-r--r--   0        0        0    15115 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/utils/validation.py
--rw-r--r--   0        0        0     6695 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/dbt_platform_helper/utils/versioning.py
--rwxr-xr-x   0        0        0     1930 2024-05-23 15:08:58.464227 dbt_platform_helper-8.4.1/platform_helper.py
--rw-r--r--   0        0        0     1392 2024-05-23 15:08:58.474226 dbt_platform_helper-8.4.1/pyproject.toml
--rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 dbt_platform_helper-8.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-05-31 11:33:46.381025 dbt_platform_helper-8.5.0/LICENSE
+-rw-r--r--   0        0        0    20115 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/COMMANDS.md
+-rw-r--r--   0        0        0     1762 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/README.md
+-rw-r--r--   0        0        0        0 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/__init__.py
+-rw-r--r--   0        0        0     4522 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/addon-plans.yml
+-rw-r--r--   0        0        0     1315 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/addons-template-map.yml
+-rw-r--r--   0        0        0        0 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/commands/__init__.py
+-rw-r--r--   0        0        0     9957 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/commands/application.py
+-rwxr-xr-x   0        0        0     3226 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/commands/check_cloudformation.py
+-rw-r--r--   0        0        0    11192 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/commands/codebase.py
+-rw-r--r--   0        0        0    15007 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/commands/conduit.py
+-rw-r--r--   0        0        0    11480 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/commands/config.py
+-rwxr-xr-x   0        0        0    16297 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/commands/copilot.py
+-rwxr-xr-x   0        0        0    35037 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/commands/dns.py
+-rw-r--r--   0        0        0    11417 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/commands/environment.py
+-rw-r--r--   0        0        0      853 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/commands/generate.py
+-rwxr-xr-x   0        0        0     3748 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/commands/notify.py
+-rw-r--r--   0        0        0     6674 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/commands/pipeline.py
+-rwxr-xr-x   0        0        0     3860 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/commands/secrets.py
+-rw-r--r--   0        0        0        0 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/custom_resources/__init__.py
+-rw-r--r--   0        0        0     2396 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/custom_resources/s3_object.py
+-rw-r--r--   0        0        0      342 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/default-extensions.yml
+-rw-r--r--   0        0        0      499 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/exceptions.py
+-rw-r--r--   0        0        0      369 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/jinja2_tags.py
+-rw-r--r--   0        0        0      158 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/.copilot/config.yml
+-rwxr-xr-x   0        0        0      164 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/.copilot/image_build_run.sh
+-rwxr-xr-x   0        0        0      121 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/.copilot/phases/build.sh
+-rwxr-xr-x   0        0        0      123 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/.copilot/phases/install.sh
+-rwxr-xr-x   0        0        0      126 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/.copilot/phases/post_build.sh
+-rwxr-xr-x   0        0        0      125 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/.copilot/phases/pre_build.sh
+-rw-r--r--   0        0        0     1081 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/COMMANDS.md.jinja
+-rw-r--r--   0        0        0      618 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addon-instructions.txt
+-rw-r--r--   0        0        0      412 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/README.md
+-rw-r--r--   0        0        0      734 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml
+-rw-r--r--   0        0        0    26381 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml
+-rw-r--r--   0        0        0     6064 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/env/monitoring.yml
+-rw-r--r--   0        0        0    10853 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/env/opensearch.yml
+-rw-r--r--   0        0        0    25624 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml
+-rw-r--r--   0        0        0     7613 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml
+-rw-r--r--   0        0        0     7626 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/env/s3.yml
+-rw-r--r--   0        0        0     3658 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/env/vpc.yml
+-rw-r--r--   0        0        0      956 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml
+-rw-r--r--   0        0        0     2403 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml
+-rw-r--r--   0        0        0      893 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml
+-rw-r--r--   0        0        0     1836 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json
+-rw-r--r--   0        0        0      197 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/create-codebuild-role.json
+-rw-r--r--   0        0        0     1180 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json
+-rw-r--r--   0        0        0      781 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/env/manifest.yml
+-rw-r--r--   0        0        0      169 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/env/overrides/.gitignore
+-rw-r--r--   0        0        0      443 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/env/overrides/README.md
+-rw-r--r--   0        0        0      284 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/env/overrides/bin/override.ts
+-rw-r--r--   0        0        0      339 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/env/overrides/cdk.json
+-rw-r--r--   0        0        0     1760 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json
+-rw-r--r--   0        0        0   155387 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/env/overrides/package-lock.json
+-rw-r--r--   0        0        0      536 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/env/overrides/package.json
+-rw-r--r--   0        0        0     1910 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/env/overrides/stack.ts
+-rw-r--r--   0        0        0      710 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/env/overrides/tsconfig.json
+-rw-r--r--   0        0        0      259 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/env/terraform-overrides/cfn.patches.yml
+-rw-r--r--   0        0        0     1959 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml
+-rw-r--r--   0        0        0      169 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/overrides/.gitignore
+-rw-r--r--   0        0        0      227 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/overrides/bin/override.ts
+-rw-r--r--   0        0        0      287 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.deploy.yml
+-rw-r--r--   0        0        0      781 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml
+-rw-r--r--   0        0        0      339 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/overrides/cdk.json
+-rw-r--r--   0        0        0   152518 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json
+-rw-r--r--   0        0        0      536 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json
+-rw-r--r--   0        0        0    20142 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts
+-rw-r--r--   0        0        0      651 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json
+-rw-r--r--   0        0        0     1205 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts
+-rw-r--r--   0        0        0     3178 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml
+-rw-r--r--   0        0        0     1778 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml
+-rw-r--r--   0        0        0      617 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml
+-rw-r--r--   0        0        0      741 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html
+-rw-r--r--   0        0        0      783 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html
+-rw-r--r--   0        0        0     2881 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/svc/manifest-backend.yml
+-rw-r--r--   0        0        0     3921 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/svc/manifest-public.yml
+-rw-r--r--   0        0        0      386 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/templates/svc/overrides/cfn.patches.yml
+-rw-r--r--   0        0        0        0 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/utils/__init__.py
+-rw-r--r--   0        0        0     3555 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/utils/application.py
+-rw-r--r--   0        0        0     1294 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/utils/arn_parser.py
+-rw-r--r--   0        0        0    10297 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/utils/aws.py
+-rw-r--r--   0        0        0     2943 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/utils/click.py
+-rw-r--r--   0        0        0     1053 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/utils/cloudformation.py
+-rw-r--r--   0        0        0      484 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/utils/cloudfoundry.py
+-rw-r--r--   0        0        0     1720 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/utils/files.py
+-rw-r--r--   0        0        0      384 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/utils/git.py
+-rw-r--r--   0        0        0      507 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/utils/manifests.py
+-rw-r--r--   0        0        0      115 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/utils/messages.py
+-rw-r--r--   0        0        0      469 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/utils/template.py
+-rw-r--r--   0        0        0    15115 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/utils/validation.py
+-rw-r--r--   0        0        0     6695 2024-05-31 11:33:46.391025 dbt_platform_helper-8.5.0/dbt_platform_helper/utils/versioning.py
+-rwxr-xr-x   0        0        0     2049 2024-05-31 11:33:46.401025 dbt_platform_helper-8.5.0/platform_helper.py
+-rw-r--r--   0        0        0     1392 2024-05-31 11:33:46.401025 dbt_platform_helper-8.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 dbt_platform_helper-8.5.0/PKG-INFO
```

### Comparing `dbt_platform_helper-8.4.1/LICENSE` & `dbt_platform_helper-8.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/COMMANDS.md` & `dbt_platform_helper-8.5.0/dbt_platform_helper/COMMANDS.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 - [platform-helper environment generate](#platform-helper-environment-generate)
 - [platform-helper generate](#platform-helper-generate)
 - [platform-helper pipeline](#platform-helper-pipeline)
 - [platform-helper pipeline generate](#platform-helper-pipeline-generate)
 - [platform-helper secrets](#platform-helper-secrets)
 - [platform-helper secrets copy](#platform-helper-secrets-copy)
 - [platform-helper secrets list](#platform-helper-secrets-list)
+- [platform-helper notify](#platform-helper-notify)
+- [platform-helper notify environment-progress](#platform-helper-notify-environment-progress)
+- [platform-helper notify add-comment](#platform-helper-notify-add-comment)
 
 # platform-helper
 
 ## Usage
 
 ```
 platform-helper <command> [--version] 
@@ -59,14 +62,15 @@
 - [`codebase` ↪](#platform-helper-codebase)
 - [`conduit` ↪](#platform-helper-conduit)
 - [`config` ↪](#platform-helper-config)
 - [`copilot` ↪](#platform-helper-copilot)
 - [`domain` ↪](#platform-helper-domain)
 - [`environment` ↪](#platform-helper-environment)
 - [`generate` ↪](#platform-helper-generate)
+- [`notify` ↪](#platform-helper-notify)
 - [`pipeline` ↪](#platform-helper-pipeline)
 - [`secrets` ↪](#platform-helper-secrets)
 
 # platform-helper application
 
 [↩ Parent](#platform-helper)
 
@@ -824,7 +828,95 @@
 - `app <text>`
 - `env <text>`
 
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
+
+# platform-helper notify
+
+[↩ Parent](#platform-helper)
+
+    Send Slack notifications
+
+## Usage
+
+```
+platform-helper notify (environment-progress|add-comment) 
+```
+
+## Options
+
+- `--help <boolean>` _Defaults to False._
+  - Show this message and exit.
+
+## Commands
+
+- [`add-comment` ↪](#platform-helper-notify-add-comment)
+- [`environment-progress` ↪](#platform-helper-notify-environment-progress)
+
+# platform-helper notify environment-progress
+
+[↩ Parent](#platform-helper-notify)
+
+    Send environment progress notifications
+
+## Usage
+
+```
+platform-helper notify environment-progress <slack_channel_id> <slack_token> 
+                                            <message> 
+                                            [--build-arn <build_arn>] 
+                                            [--repository <repository>] 
+                                            [--commit-sha <commit_sha>] 
+                                            [--slack-ref <slack_ref>] 
+```
+
+## Arguments
+
+- `slack-channel-id <text>`
+- `slack-token <text>`
+- `message <text>`
+
+## Options
+
+- `--build-arn <text>`
+
+- `--repository <text>`
+
+- `--commit-sha <text>`
+
+- `--slack-ref <text>`
+  - Slack message reference
+- `--help <boolean>` _Defaults to False._
+  - Show this message and exit.
+
+# platform-helper notify add-comment
+
+[↩ Parent](#platform-helper-notify)
+
+    Add comment to a notification
+
+## Usage
+
+```
+platform-helper notify add-comment <slack_channel_id> <slack_token> 
+                                   <slack_ref> <message> 
+                                   [--title <title>] [--send-to-main-channel <send_to_main_channel>] 
+```
+
+## Arguments
+
+- `slack-channel-id <text>`
+- `slack-token <text>`
+- `slack-ref <text>`
+- `message <text>`
+
+## Options
+
+- `--title <text>`
+  - Message title
+- `--send-to-main-channel <boolean>` _Defaults to False._
+  - Send to main channel
+- `--help <boolean>` _Defaults to False._
+  - Show this message and exit.
```

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/README.md` & `dbt_platform_helper-8.5.0/dbt_platform_helper/README.md`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/addon-plans.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/addon-plans.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/addons-template-map.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/addons-template-map.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/commands/application.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/commands/application.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/commands/check_cloudformation.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/commands/check_cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/commands/codebase.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/commands/codebase.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/commands/conduit.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/commands/conduit.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,14 +93,16 @@
 
 
 def get_parameter_name(
     app: Application, env: str, addon_type: str, addon_name: str, access: str
 ) -> str:
     if addon_type == "postgres":
         return f"/copilot/{app.name}/{env}/conduits/{normalise_secret_name(addon_name)}_{access.upper()}"
+    elif addon_type == "redis" or addon_type == "opensearch":
+        return f"/copilot/{app.name}/{env}/conduits/{normalise_secret_name(addon_name)}_ENDPOINT"
     else:
         return f"/copilot/{app.name}/{env}/conduits/{normalise_secret_name(addon_name)}"
 
 
 def get_or_create_task_name(
     app: Application, env: str, addon_name: str, parameter_name: str
 ) -> str:
```

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/commands/config.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/commands/config.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/commands/copilot.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/commands/copilot.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/commands/dns.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/commands/dns.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/commands/environment.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/commands/environment.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/commands/generate.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/commands/generate.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/commands/pipeline.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/commands/pipeline.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/commands/secrets.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/commands/secrets.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/custom_resources/s3_object.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/custom_resources/s3_object.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/COMMANDS.md.jinja` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/COMMANDS.md.jinja`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addon-instructions.txt` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addon-instructions.txt`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/env/addons.parameters.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/env/aurora-postgres.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/env/monitoring.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/env/monitoring.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/env/opensearch.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/env/opensearch.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/env/rds-postgres.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/env/redis-cluster.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/env/s3.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/env/s3.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/env/vpc.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/env/vpc.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/svc/s3-policy.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/addons/svc/subscription-filter.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/ci-codebuild-role-policy.json` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/custom-codebuild-role-policy.json` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/env/manifest.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/env/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/env/overrides/log_resource_policy.json` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/env/overrides/package-lock.json` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/env/overrides/package-lock.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/env/overrides/package.json` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/env/overrides/package.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/env/overrides/stack.ts` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/env/overrides/stack.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/env/overrides/tsconfig.json` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/env/overrides/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/manifest.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/environments/buildspec.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/environments/manifest.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/svc/maintenance_pages/default.html` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/svc/maintenance_pages/migration.html` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/svc/manifest-backend.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/svc/manifest-backend.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/templates/svc/manifest-public.yml` & `dbt_platform_helper-8.5.0/dbt_platform_helper/templates/svc/manifest-public.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/utils/application.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/utils/application.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/utils/aws.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/utils/aws.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/utils/click.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/utils/click.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/utils/cloudformation.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/utils/cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/utils/files.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/utils/files.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/utils/validation.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/utils/validation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/dbt_platform_helper/utils/versioning.py` & `dbt_platform_helper-8.5.0/dbt_platform_helper/utils/versioning.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.4.1/platform_helper.py` & `dbt_platform_helper-8.5.0/platform_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from dbt_platform_helper.commands.conduit import conduit as conduit_commands
 from dbt_platform_helper.commands.config import config as config_commands
 from dbt_platform_helper.commands.copilot import copilot as copilot_commands
 from dbt_platform_helper.commands.dns import cdn as cdn_commands
 from dbt_platform_helper.commands.dns import domain as domain_commands
 from dbt_platform_helper.commands.environment import environment as environment_commands
 from dbt_platform_helper.commands.generate import generate as generate_commands
+from dbt_platform_helper.commands.notify import notify as notify_commands
 from dbt_platform_helper.commands.pipeline import pipeline as pipeline_commands
 from dbt_platform_helper.commands.secrets import secrets as secrets_commands
 from dbt_platform_helper.utils.click import ClickDocOptGroup
 
 
 @click.group(cls=ClickDocOptGroup)
 @click.version_option(
@@ -38,10 +39,11 @@
 platform_helper.add_command(config_commands)
 platform_helper.add_command(copilot_commands)
 platform_helper.add_command(domain_commands)
 platform_helper.add_command(environment_commands)
 platform_helper.add_command(generate_commands)
 platform_helper.add_command(pipeline_commands)
 platform_helper.add_command(secrets_commands)
+platform_helper.add_command(notify_commands)
 
 if __name__ == "__main__":
     platform_helper()
```

### Comparing `dbt_platform_helper-8.4.1/pyproject.toml` & `dbt_platform_helper-8.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "dbt-platform-helper"
-version = "8.4.1"
+version = "8.5.0"
 description = "Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot."
 authors = ["Department for Business and Trade Platform Team <sre-team@digital.trade.gov.uk>"]
 license = "MIT"
 readme = "dbt_platform_helper/README.md"
 packages = [
     { include = "dbt_platform_helper" },
     { include = "platform_helper.py" }
```

### Comparing `dbt_platform_helper-8.4.1/PKG-INFO` & `dbt_platform_helper-8.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-platform-helper
-Version: 8.4.1
+Version: 8.5.0
 Summary: Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot.
 License: MIT
 Author: Department for Business and Trade Platform Team
 Author-email: sre-team@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

