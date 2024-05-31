# Comparing `tmp/aimodelshare-0.1.8.tar.gz` & `tmp/aimodelshare-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimodelshare-0.1.8.tar", last modified: Thu Dec 28 09:50:26 2023, max compression
+gzip compressed data, was "aimodelshare-0.1.9.tar", last modified: Thu Dec 28 10:27:47 2023, max compression
```

## Comparing `aimodelshare-0.1.8.tar` & `aimodelshare-0.1.9.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.448721 aimodelshare-0.1.8/
--rw-r--r--   0 root         (0) root         (0)     1134 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       35 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3280 2023-12-28 09:50:26.448721 aimodelshare-0.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1936 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.416718 aimodelshare-0.1.8/aimodelshare/
--rw-r--r--   0 root         (0) root         (0)     2014 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/README.md
--rw-r--r--   0 root         (0) root         (0)      539 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69317 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/aimsonnx.py
--rw-r--r--   0 root         (0) root         (0)    34935 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/api.py
--rw-r--r--   0 root         (0) root         (0)    15188 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/aws.py
--rw-r--r--   0 root         (0) root         (0)     6784 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/aws_client.py
--rw-r--r--   0 root         (0) root         (0)     4825 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/base_image.py
--rw-r--r--   0 root         (0) root         (0)     3055 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/bucketpolicy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.418718 aimodelshare-0.1.8/aimodelshare/color_mappings/
--rw-r--r--   0 root         (0) root         (0)     2728 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/color_mappings/color_mapping_keras.csv
--rw-r--r--   0 root         (0) root         (0)     1960 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/color_mappings/color_mapping_pytorch.csv
--rw-r--r--   0 root         (0) root         (0)     8758 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/containerisation.py
--rw-r--r--   0 root         (0) root         (0)    29609 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/containerization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.419719 aimodelshare-0.1.8/aimodelshare/containerization_templates/
--rw-r--r--   0 root         (0) root         (0)      181 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/containerization_templates/Dockerfile.txt
--rw-r--r--   0 root         (0) root         (0)      687 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/containerization_templates/Dockerfile_PySpark.txt
--rw-r--r--   0 root         (0) root         (0)      532 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/containerization_templates/buildspec.txt
--rw-r--r--   0 root         (0) root         (0)      939 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/containerization_templates/lambda_function.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.420719 aimodelshare-0.1.8/aimodelshare/custom_approach/
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/custom_approach/__init__.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/custom_approach/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3170 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/custom_eval_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.421719 aimodelshare-0.1.8/aimodelshare/data_sharing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/data_sharing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.422719 aimodelshare-0.1.8/aimodelshare/data_sharing/data_sharing_templates/
--rw-r--r--   0 root         (0) root         (0)       77 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/data_sharing/data_sharing_templates/Dockerfile.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/data_sharing/data_sharing_templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      556 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/data_sharing/data_sharing_templates/buildspec.txt
--rw-r--r--   0 root         (0) root         (0)     3855 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/data_sharing/data_sharing_templates/codebuild_policies.txt
--rw-r--r--   0 root         (0) root         (0)      242 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/data_sharing/data_sharing_templates/codebuild_trust_relationship.txt
--rw-r--r--   0 root         (0) root         (0)    22799 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/data_sharing/download_data.py
--rw-r--r--   0 root         (0) root         (0)    13964 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/data_sharing/share_data.py
--rw-r--r--   0 root         (0) root         (0)      236 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/data_sharing/utils.py
--rw-r--r--   0 root         (0) root         (0)    11045 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/deploy_custom_lambda.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.422719 aimodelshare-0.1.8/aimodelshare/documentation/
--rw-r--r--   0 root         (0) root         (0)      638 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.424719 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/
--rw-r--r--   0 root         (0) root         (0)      797 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/__init__.py
--rw-r--r--   0 root         (0) root         (0)       80 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/_version.py
--rw-r--r--   0 root         (0) root         (0)     3099 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/breadcrumbs.html
--rw-r--r--   0 root         (0) root         (0)     6192 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/layout.html
--rw-r--r--   0 root         (0) root         (0)     1529 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/search.html
--rw-r--r--   0 root         (0) root         (0)      513 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/searchbox.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.408717 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.426719 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/css/
--rw-r--r--   0 root         (0) root         (0)       39 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/css/custom.css
--rw-r--r--   0 root         (0) root         (0)       71 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/css/custom.css.map
--rw-r--r--   0 root         (0) root         (0)    43005 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css
--rw-r--r--   0 root         (0) root         (0)   133076 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css.map
--rw-r--r--   0 root         (0) root         (0)    35271 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css
--rw-r--r--   0 root         (0) root         (0)   161215 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css.map
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.427719 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/font/
--rw-r--r--   0 root         (0) root         (0)     8468 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.eot
--rw-r--r--   0 root         (0) root         (0)     5922 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.svg
--rw-r--r--   0 root         (0) root         (0)     8300 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.ttf
--rw-r--r--   0 root         (0) root         (0)     5168 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff
--rw-r--r--   0 root         (0) root         (0)     4344 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.427719 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/js/
--rw-r--r--   0 root         (0) root         (0)     1948 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/js/theme.js
--rwxr-xr-x   0 root         (0) root         (0)      146 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/theme.conf
--rw-r--r--   0 root         (0) root         (0)      804 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/make.bat
--rw-r--r--   0 root         (0) root         (0)       27 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.430719 aimodelshare-0.1.8/aimodelshare/documentation/source/
--rw-r--r--   0 root         (0) root         (0)     1366 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/source/about.rst
--rw-r--r--   0 root         (0) root         (0)     5598 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/source/advanced_features.rst
--rw-r--r--   0 root         (0) root         (0)     8528 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/source/competition.rst
--rw-r--r--   0 root         (0) root         (0)     2028 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/source/conf.py
--rw-r--r--   0 root         (0) root         (0)     3768 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/source/create_credentials.rst
--rw-r--r--   0 root         (0) root         (0)     8854 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/source/example_notebooks.rst
--rw-r--r--   0 root         (0) root         (0)     4727 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/source/functions.rst
--rw-r--r--   0 root         (0) root         (0)    14863 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/source/gettingstarted.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.432720 aimodelshare-0.1.8/aimodelshare/documentation/source/images/
--rw-r--r--   0 root         (0) root         (0)    15684 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/source/images/creds1.png
--rw-r--r--   0 root         (0) root         (0)    80398 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/source/images/creds2.png
--rw-r--r--   0 root         (0) root         (0)   201488 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/source/images/creds3.png
--rw-r--r--   0 root         (0) root         (0)   208089 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/source/images/creds4.png
--rw-r--r--   0 root         (0) root         (0)   123164 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/source/images/creds5.png
--rw-r--r--   0 root         (0) root         (0)    45191 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/source/images/creds_file_example.png
--rw-r--r--   0 root         (0) root         (0)    95857 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/source/images/predict_tab.png
--rw-r--r--   0 root         (0) root         (0)     2452 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/source/index.rst
--rw-r--r--   0 root         (0) root         (0)     6712 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/documentation/source/modelplayground.rst
--rw-r--r--   0 root         (0) root         (0)      318 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    59901 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/generatemodelapi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.433720 aimodelshare-0.1.8/aimodelshare/iam/
--rw-r--r--   0 root         (0) root         (0)     3855 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/iam/codebuild_policy.txt
--rw-r--r--   0 root         (0) root         (0)      242 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/iam/codebuild_trust_relationship.txt
--rw-r--r--   0 root         (0) root         (0)      278 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/iam/lambda_policy.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/iam/lambda_trust_relationship.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.435720 aimodelshare-0.1.8/aimodelshare/json_templates/
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/json_templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2014 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/json_templates/api_json.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.435720 aimodelshare-0.1.8/aimodelshare/json_templates/auth/
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/json_templates/auth/policy.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/json_templates/auth/role.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.436720 aimodelshare-0.1.8/aimodelshare/json_templates/eval/
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/json_templates/eval/policy.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/json_templates/eval/role.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.436720 aimodelshare-0.1.8/aimodelshare/json_templates/function/
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/json_templates/function/policy.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/json_templates/function/role.txt
--rw-r--r--   0 root         (0) root         (0)      316 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/json_templates/integration_response.txt
--rw-r--r--   0 root         (0) root         (0)      278 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/json_templates/lambda_policy_1.txt
--rw-r--r--   0 root         (0) root         (0)      147 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/json_templates/lambda_policy_2.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/json_templates/lambda_role_1.txt
--rw-r--r--   0 root         (0) root         (0)      350 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/json_templates/lambda_role_2.txt
--rw-r--r--   0 root         (0) root         (0)     5216 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/leaderboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.440720 aimodelshare-0.1.8/aimodelshare/main/
--rw-r--r--   0 root         (0) root         (0)     4146 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/main/1.txt
--rw-r--r--   0 root         (0) root         (0)     3616 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/main/1B.txt
--rw-r--r--   0 root         (0) root         (0)     4609 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/main/2.txt
--rw-r--r--   0 root         (0) root         (0)     4110 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/main/3.txt
--rw-r--r--   0 root         (0) root         (0)     4260 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/main/4.txt
--rw-r--r--   0 root         (0) root         (0)     3522 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/main/5.txt
--rw-r--r--   0 root         (0) root         (0)     3518 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/main/6.txt
--rw-r--r--   0 root         (0) root         (0)     4377 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/main/7.txt
--rw-r--r--   0 root         (0) root         (0)     4513 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/main/8.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/main/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10942 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/main/authorization.txt
--rw-r--r--   0 root         (0) root         (0)     3081 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/main/eval_classification.txt
--rw-r--r--   0 root         (0) root         (0)    60314 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/main/eval_lambda.txt
--rw-r--r--   0 root         (0) root         (0)     3111 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/main/eval_regression.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/main/lambda_function.txt
--rw-r--r--   0 root         (0) root         (0)     4941 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/main/nst.txt
--rw-r--r--   0 root         (0) root         (0)    49899 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/model.py
--rw-r--r--   0 root         (0) root         (0)     4311 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/modeluser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.440720 aimodelshare-0.1.8/aimodelshare/placeholders/
--rw-r--r--   0 root         (0) root         (0)     3464 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/placeholders/model.onnx
--rw-r--r--   0 root         (0) root         (0)     2930 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/placeholders/preprocessor.zip
--rw-r--r--   0 root         (0) root         (0)    88713 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/playground.py
--rw-r--r--   0 root         (0) root         (0)     4992 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/postprocessormodules.py
--rw-r--r--   0 root         (0) root         (0)    10912 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/preprocessormodules.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.444721 aimodelshare-0.1.8/aimodelshare/pyspark/
--rw-r--r--   0 root         (0) root         (0)     6529 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/pyspark/1.txt
--rw-r--r--   0 root         (0) root         (0)     6078 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/pyspark/1B.txt
--rw-r--r--   0 root         (0) root         (0)     7055 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/pyspark/2.txt
--rw-r--r--   0 root         (0) root         (0)     6596 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/pyspark/3.txt
--rw-r--r--   0 root         (0) root         (0)     6377 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/pyspark/4.txt
--rw-r--r--   0 root         (0) root         (0)     5988 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/pyspark/5.txt
--rw-r--r--   0 root         (0) root         (0)     5980 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/pyspark/6.txt
--rw-r--r--   0 root         (0) root         (0)     6819 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/pyspark/7.txt
--rw-r--r--   0 root         (0) root         (0)     6906 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/pyspark/8.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/pyspark/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10589 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/pyspark/authorization.txt
--rw-r--r--   0 root         (0) root         (0)     3081 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/pyspark/eval_classification.txt
--rw-r--r--   0 root         (0) root         (0)    51474 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/pyspark/eval_lambda.txt
--rw-r--r--   0 root         (0) root         (0)     3111 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/pyspark/eval_regression.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/pyspark/lambda_function.txt
--rw-r--r--   0 root         (0) root         (0)     7110 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/pyspark/nst.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.444721 aimodelshare-0.1.8/aimodelshare/python/
--rw-r--r--   0 root         (0) root         (0)     1949 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/python/my_preprocessor.py
--rw-r--r--   0 root         (0) root         (0)     2014 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/readme.md
--rw-r--r--   0 root         (0) root         (0)     5793 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/reproducibility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.446721 aimodelshare-0.1.8/aimodelshare/sam/
--rw-r--r--   0 root         (0) root         (0)      182 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/sam/Dockerfile.txt
--rw-r--r--   0 root         (0) root         (0)      708 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/sam/Dockerfile_PySpark.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/sam/__init__.py
--rw-r--r--   0 root         (0) root         (0)      625 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/sam/buildspec.txt
--rw-r--r--   0 root         (0) root         (0)     3855 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/sam/codebuild_policies.txt
--rw-r--r--   0 root         (0) root         (0)      242 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/sam/codebuild_trust_relationship.txt
--rw-r--r--   0 root         (0) root         (0)     5181 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/sam/codepipeline_policies.txt
--rw-r--r--   0 root         (0) root         (0)      245 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/sam/codepipeline_trust_relationship.txt
--rw-r--r--   0 root         (0) root         (0)      217 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/sam/spark-class.txt
--rw-r--r--   0 root         (0) root         (0)     1195 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/sam/template.txt
--rw-r--r--   0 root         (0) root         (0)     3109 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/tools.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/aimodelshare/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.447721 aimodelshare-0.1.8/aimodelshare.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3280 2023-12-28 09:50:26.000000 aimodelshare-0.1.8/aimodelshare.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6377 2023-12-28 09:50:26.000000 aimodelshare-0.1.8/aimodelshare.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 09:50:26.000000 aimodelshare-0.1.8/aimodelshare.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      413 2023-12-28 09:50:26.000000 aimodelshare-0.1.8/aimodelshare.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-12-28 09:50:26.000000 aimodelshare-0.1.8/aimodelshare.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-28 09:50:26.448721 aimodelshare-0.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1320 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 09:50:26.447721 aimodelshare-0.1.8/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3906 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/tests/test_aimsonnx.py
--rw-r--r--   0 root         (0) root         (0)    24574 2023-12-28 09:50:15.000000 aimodelshare-0.1.8/tests/test_playground.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.386463 aimodelshare-0.1.9/
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       35 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3280 2023-12-28 10:27:47.386463 aimodelshare-0.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.356460 aimodelshare-0.1.9/aimodelshare/
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/README.md
+-rw-r--r--   0 root         (0) root         (0)      539 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69282 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/aimsonnx.py
+-rw-r--r--   0 root         (0) root         (0)    34935 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/api.py
+-rw-r--r--   0 root         (0) root         (0)    15188 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/aws.py
+-rw-r--r--   0 root         (0) root         (0)     6784 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/aws_client.py
+-rw-r--r--   0 root         (0) root         (0)     4825 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/base_image.py
+-rw-r--r--   0 root         (0) root         (0)     3055 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/bucketpolicy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.357461 aimodelshare-0.1.9/aimodelshare/color_mappings/
+-rw-r--r--   0 root         (0) root         (0)     2728 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/color_mappings/color_mapping_keras.csv
+-rw-r--r--   0 root         (0) root         (0)     1960 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/color_mappings/color_mapping_pytorch.csv
+-rw-r--r--   0 root         (0) root         (0)     8758 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/containerisation.py
+-rw-r--r--   0 root         (0) root         (0)    29609 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/containerization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.358461 aimodelshare-0.1.9/aimodelshare/containerization_templates/
+-rw-r--r--   0 root         (0) root         (0)      181 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/containerization_templates/Dockerfile.txt
+-rw-r--r--   0 root         (0) root         (0)      687 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/containerization_templates/Dockerfile_PySpark.txt
+-rw-r--r--   0 root         (0) root         (0)      532 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/containerization_templates/buildspec.txt
+-rw-r--r--   0 root         (0) root         (0)      939 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/containerization_templates/lambda_function.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.359461 aimodelshare-0.1.9/aimodelshare/custom_approach/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/custom_approach/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/custom_approach/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3170 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/custom_eval_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.360461 aimodelshare-0.1.9/aimodelshare/data_sharing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/data_sharing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.361461 aimodelshare-0.1.9/aimodelshare/data_sharing/data_sharing_templates/
+-rw-r--r--   0 root         (0) root         (0)       77 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/data_sharing/data_sharing_templates/Dockerfile.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/data_sharing/data_sharing_templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      556 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/data_sharing/data_sharing_templates/buildspec.txt
+-rw-r--r--   0 root         (0) root         (0)     3855 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/data_sharing/data_sharing_templates/codebuild_policies.txt
+-rw-r--r--   0 root         (0) root         (0)      242 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/data_sharing/data_sharing_templates/codebuild_trust_relationship.txt
+-rw-r--r--   0 root         (0) root         (0)    22799 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/data_sharing/download_data.py
+-rw-r--r--   0 root         (0) root         (0)    13964 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/data_sharing/share_data.py
+-rw-r--r--   0 root         (0) root         (0)      236 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/data_sharing/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11045 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/deploy_custom_lambda.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.362461 aimodelshare-0.1.9/aimodelshare/documentation/
+-rw-r--r--   0 root         (0) root         (0)      638 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.364461 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/
+-rw-r--r--   0 root         (0) root         (0)      797 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       80 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/_version.py
+-rw-r--r--   0 root         (0) root         (0)     3099 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/breadcrumbs.html
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/layout.html
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/search.html
+-rw-r--r--   0 root         (0) root         (0)      513 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/searchbox.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.347460 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.365461 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/css/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/css/custom.css
+-rw-r--r--   0 root         (0) root         (0)       71 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/css/custom.css.map
+-rw-r--r--   0 root         (0) root         (0)    43005 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css
+-rw-r--r--   0 root         (0) root         (0)   133076 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css.map
+-rw-r--r--   0 root         (0) root         (0)    35271 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css
+-rw-r--r--   0 root         (0) root         (0)   161215 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css.map
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.366461 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/font/
+-rw-r--r--   0 root         (0) root         (0)     8468 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.eot
+-rw-r--r--   0 root         (0) root         (0)     5922 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.svg
+-rw-r--r--   0 root         (0) root         (0)     8300 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.ttf
+-rw-r--r--   0 root         (0) root         (0)     5168 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff
+-rw-r--r--   0 root         (0) root         (0)     4344 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.367461 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/js/
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/js/theme.js
+-rwxr-xr-x   0 root         (0) root         (0)      146 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/theme.conf
+-rw-r--r--   0 root         (0) root         (0)      804 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/make.bat
+-rw-r--r--   0 root         (0) root         (0)       27 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.369461 aimodelshare-0.1.9/aimodelshare/documentation/source/
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/source/about.rst
+-rw-r--r--   0 root         (0) root         (0)     5598 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/source/advanced_features.rst
+-rw-r--r--   0 root         (0) root         (0)     8528 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/source/competition.rst
+-rw-r--r--   0 root         (0) root         (0)     2028 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)     3768 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/source/create_credentials.rst
+-rw-r--r--   0 root         (0) root         (0)     8854 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/source/example_notebooks.rst
+-rw-r--r--   0 root         (0) root         (0)     4727 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/source/functions.rst
+-rw-r--r--   0 root         (0) root         (0)    14863 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/source/gettingstarted.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.371461 aimodelshare-0.1.9/aimodelshare/documentation/source/images/
+-rw-r--r--   0 root         (0) root         (0)    15684 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/source/images/creds1.png
+-rw-r--r--   0 root         (0) root         (0)    80398 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/source/images/creds2.png
+-rw-r--r--   0 root         (0) root         (0)   201488 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/source/images/creds3.png
+-rw-r--r--   0 root         (0) root         (0)   208089 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/source/images/creds4.png
+-rw-r--r--   0 root         (0) root         (0)   123164 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/source/images/creds5.png
+-rw-r--r--   0 root         (0) root         (0)    45191 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/source/images/creds_file_example.png
+-rw-r--r--   0 root         (0) root         (0)    95857 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/source/images/predict_tab.png
+-rw-r--r--   0 root         (0) root         (0)     2452 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/source/index.rst
+-rw-r--r--   0 root         (0) root         (0)     6712 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/documentation/source/modelplayground.rst
+-rw-r--r--   0 root         (0) root         (0)      318 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    59901 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/generatemodelapi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.372461 aimodelshare-0.1.9/aimodelshare/iam/
+-rw-r--r--   0 root         (0) root         (0)     3855 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/iam/codebuild_policy.txt
+-rw-r--r--   0 root         (0) root         (0)      242 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/iam/codebuild_trust_relationship.txt
+-rw-r--r--   0 root         (0) root         (0)      278 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/iam/lambda_policy.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/iam/lambda_trust_relationship.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.374462 aimodelshare-0.1.9/aimodelshare/json_templates/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/json_templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/json_templates/api_json.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.374462 aimodelshare-0.1.9/aimodelshare/json_templates/auth/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/json_templates/auth/policy.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/json_templates/auth/role.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.374462 aimodelshare-0.1.9/aimodelshare/json_templates/eval/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/json_templates/eval/policy.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/json_templates/eval/role.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.375462 aimodelshare-0.1.9/aimodelshare/json_templates/function/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/json_templates/function/policy.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/json_templates/function/role.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/json_templates/integration_response.txt
+-rw-r--r--   0 root         (0) root         (0)      278 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/json_templates/lambda_policy_1.txt
+-rw-r--r--   0 root         (0) root         (0)      147 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/json_templates/lambda_policy_2.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/json_templates/lambda_role_1.txt
+-rw-r--r--   0 root         (0) root         (0)      350 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/json_templates/lambda_role_2.txt
+-rw-r--r--   0 root         (0) root         (0)     5216 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/leaderboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.378462 aimodelshare-0.1.9/aimodelshare/main/
+-rw-r--r--   0 root         (0) root         (0)     4146 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/main/1.txt
+-rw-r--r--   0 root         (0) root         (0)     3616 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/main/1B.txt
+-rw-r--r--   0 root         (0) root         (0)     4609 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/main/2.txt
+-rw-r--r--   0 root         (0) root         (0)     4110 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/main/3.txt
+-rw-r--r--   0 root         (0) root         (0)     4260 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/main/4.txt
+-rw-r--r--   0 root         (0) root         (0)     3522 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/main/5.txt
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/main/6.txt
+-rw-r--r--   0 root         (0) root         (0)     4377 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/main/7.txt
+-rw-r--r--   0 root         (0) root         (0)     4513 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/main/8.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/main/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10942 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/main/authorization.txt
+-rw-r--r--   0 root         (0) root         (0)     3081 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/main/eval_classification.txt
+-rw-r--r--   0 root         (0) root         (0)    60314 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/main/eval_lambda.txt
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/main/eval_regression.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/main/lambda_function.txt
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/main/nst.txt
+-rw-r--r--   0 root         (0) root         (0)    49899 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/model.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/modeluser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.379462 aimodelshare-0.1.9/aimodelshare/placeholders/
+-rw-r--r--   0 root         (0) root         (0)     3464 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/placeholders/model.onnx
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/placeholders/preprocessor.zip
+-rw-r--r--   0 root         (0) root         (0)    88713 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/playground.py
+-rw-r--r--   0 root         (0) root         (0)     4992 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/postprocessormodules.py
+-rw-r--r--   0 root         (0) root         (0)    10912 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/preprocessormodules.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.383462 aimodelshare-0.1.9/aimodelshare/pyspark/
+-rw-r--r--   0 root         (0) root         (0)     6529 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/pyspark/1.txt
+-rw-r--r--   0 root         (0) root         (0)     6078 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/pyspark/1B.txt
+-rw-r--r--   0 root         (0) root         (0)     7055 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/pyspark/2.txt
+-rw-r--r--   0 root         (0) root         (0)     6596 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/pyspark/3.txt
+-rw-r--r--   0 root         (0) root         (0)     6377 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/pyspark/4.txt
+-rw-r--r--   0 root         (0) root         (0)     5988 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/pyspark/5.txt
+-rw-r--r--   0 root         (0) root         (0)     5980 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/pyspark/6.txt
+-rw-r--r--   0 root         (0) root         (0)     6819 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/pyspark/7.txt
+-rw-r--r--   0 root         (0) root         (0)     6906 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/pyspark/8.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/pyspark/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10589 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/pyspark/authorization.txt
+-rw-r--r--   0 root         (0) root         (0)     3081 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/pyspark/eval_classification.txt
+-rw-r--r--   0 root         (0) root         (0)    51474 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/pyspark/eval_lambda.txt
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/pyspark/eval_regression.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/pyspark/lambda_function.txt
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/pyspark/nst.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.383462 aimodelshare-0.1.9/aimodelshare/python/
+-rw-r--r--   0 root         (0) root         (0)     1949 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/python/my_preprocessor.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/readme.md
+-rw-r--r--   0 root         (0) root         (0)     5793 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/reproducibility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.384462 aimodelshare-0.1.9/aimodelshare/sam/
+-rw-r--r--   0 root         (0) root         (0)      182 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/sam/Dockerfile.txt
+-rw-r--r--   0 root         (0) root         (0)      708 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/sam/Dockerfile_PySpark.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/sam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      625 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/sam/buildspec.txt
+-rw-r--r--   0 root         (0) root         (0)     3855 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/sam/codebuild_policies.txt
+-rw-r--r--   0 root         (0) root         (0)      242 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/sam/codebuild_trust_relationship.txt
+-rw-r--r--   0 root         (0) root         (0)     5181 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/sam/codepipeline_policies.txt
+-rw-r--r--   0 root         (0) root         (0)      245 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/sam/codepipeline_trust_relationship.txt
+-rw-r--r--   0 root         (0) root         (0)      217 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/sam/spark-class.txt
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/sam/template.txt
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/tools.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/aimodelshare/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.385462 aimodelshare-0.1.9/aimodelshare.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3280 2023-12-28 10:27:47.000000 aimodelshare-0.1.9/aimodelshare.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6377 2023-12-28 10:27:47.000000 aimodelshare-0.1.9/aimodelshare.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-28 10:27:47.000000 aimodelshare-0.1.9/aimodelshare.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      413 2023-12-28 10:27:47.000000 aimodelshare-0.1.9/aimodelshare.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-12-28 10:27:47.000000 aimodelshare-0.1.9/aimodelshare.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-12-28 10:27:47.386463 aimodelshare-0.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-28 10:27:47.385462 aimodelshare-0.1.9/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3906 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/tests/test_aimsonnx.py
+-rw-r--r--   0 root         (0) root         (0)    24574 2023-12-28 10:27:37.000000 aimodelshare-0.1.9/tests/test_playground.py
```

### Comparing `aimodelshare-0.1.8/LICENSE` & `aimodelshare-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/PKG-INFO` & `aimodelshare-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimodelshare
-Version: 0.1.8
+Version: 0.1.9
 Summary: Deploy locally saved machine learning models to a live rest API and web-dashboard.  Share it with the world via modelshare.org
 Home-page: https://www.modelshare.org
 Author: Michael Parrott
 Author-email: mikedparrott@modelshare.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `aimodelshare-0.1.8/README.md` & `aimodelshare-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/README.md` & `aimodelshare-0.1.9/aimodelshare/README.md`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/__init__.py` & `aimodelshare-0.1.9/aimodelshare/__init__.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/aimsonnx.py` & `aimodelshare-0.1.9/aimodelshare/aimsonnx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1845,15 +1845,15 @@
     
 def keras_unpack(model):
     
     layers = []
     
     for module in model.layers:
                 
-        if isinstance(module, (keras.engine.functional.Functional, keras.engine.sequential.Sequential)):
+        if isinstance(module, (tf.keras.Model, tf.keras.Sequential)):
             
             layers_out = keras_unpack(module)
             
             layers = layers + layers_out
             
             
         else:
```

### Comparing `aimodelshare-0.1.8/aimodelshare/api.py` & `aimodelshare-0.1.9/aimodelshare/api.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/aws.py` & `aimodelshare-0.1.9/aimodelshare/aws.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/aws_client.py` & `aimodelshare-0.1.9/aimodelshare/aws_client.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/base_image.py` & `aimodelshare-0.1.9/aimodelshare/base_image.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/bucketpolicy.py` & `aimodelshare-0.1.9/aimodelshare/bucketpolicy.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/color_mappings/color_mapping_keras.csv` & `aimodelshare-0.1.9/aimodelshare/color_mappings/color_mapping_keras.csv`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/color_mappings/color_mapping_pytorch.csv` & `aimodelshare-0.1.9/aimodelshare/color_mappings/color_mapping_pytorch.csv`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/containerisation.py` & `aimodelshare-0.1.9/aimodelshare/containerisation.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/containerization.py` & `aimodelshare-0.1.9/aimodelshare/containerization.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/containerization_templates/Dockerfile_PySpark.txt` & `aimodelshare-0.1.9/aimodelshare/containerization_templates/Dockerfile_PySpark.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/containerization_templates/buildspec.txt` & `aimodelshare-0.1.9/aimodelshare/containerization_templates/buildspec.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/containerization_templates/lambda_function.txt` & `aimodelshare-0.1.9/aimodelshare/containerization_templates/lambda_function.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/custom_eval_metrics.py` & `aimodelshare-0.1.9/aimodelshare/custom_eval_metrics.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/data_sharing/data_sharing_templates/buildspec.txt` & `aimodelshare-0.1.9/aimodelshare/data_sharing/data_sharing_templates/buildspec.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/data_sharing/data_sharing_templates/codebuild_policies.txt` & `aimodelshare-0.1.9/aimodelshare/data_sharing/data_sharing_templates/codebuild_policies.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/data_sharing/download_data.py` & `aimodelshare-0.1.9/aimodelshare/data_sharing/download_data.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/data_sharing/share_data.py` & `aimodelshare-0.1.9/aimodelshare/data_sharing/share_data.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/deploy_custom_lambda.py` & `aimodelshare-0.1.9/aimodelshare/deploy_custom_lambda.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/Makefile` & `aimodelshare-0.1.9/aimodelshare/documentation/Makefile`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/__init__.py` & `aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/breadcrumbs.html` & `aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/layout.html` & `aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/search.html` & `aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/searchbox.html` & `aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css` & `aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css.map` & `aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.css.map`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css` & `aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css.map` & `aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/css/theme.min.css.map`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.eot` & `aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.eot`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.svg` & `aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.svg`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.ttf` & `aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.ttf`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff` & `aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff2` & `aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/font/fontello.woff2`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/karma_sphinx_theme/static/js/theme.js` & `aimodelshare-0.1.9/aimodelshare/documentation/karma_sphinx_theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/make.bat` & `aimodelshare-0.1.9/aimodelshare/documentation/make.bat`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/source/about.rst` & `aimodelshare-0.1.9/aimodelshare/documentation/source/about.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/source/advanced_features.rst` & `aimodelshare-0.1.9/aimodelshare/documentation/source/advanced_features.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/source/competition.rst` & `aimodelshare-0.1.9/aimodelshare/documentation/source/competition.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/source/conf.py` & `aimodelshare-0.1.9/aimodelshare/documentation/source/conf.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/source/create_credentials.rst` & `aimodelshare-0.1.9/aimodelshare/documentation/source/create_credentials.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/source/example_notebooks.rst` & `aimodelshare-0.1.9/aimodelshare/documentation/source/example_notebooks.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/source/functions.rst` & `aimodelshare-0.1.9/aimodelshare/documentation/source/functions.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/source/gettingstarted.rst` & `aimodelshare-0.1.9/aimodelshare/documentation/source/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/source/images/creds1.png` & `aimodelshare-0.1.9/aimodelshare/documentation/source/images/creds1.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/source/images/creds2.png` & `aimodelshare-0.1.9/aimodelshare/documentation/source/images/creds2.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/source/images/creds3.png` & `aimodelshare-0.1.9/aimodelshare/documentation/source/images/creds3.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/source/images/creds4.png` & `aimodelshare-0.1.9/aimodelshare/documentation/source/images/creds4.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/source/images/creds5.png` & `aimodelshare-0.1.9/aimodelshare/documentation/source/images/creds5.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/source/images/creds_file_example.png` & `aimodelshare-0.1.9/aimodelshare/documentation/source/images/creds_file_example.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/source/images/predict_tab.png` & `aimodelshare-0.1.9/aimodelshare/documentation/source/images/predict_tab.png`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/source/index.rst` & `aimodelshare-0.1.9/aimodelshare/documentation/source/index.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/documentation/source/modelplayground.rst` & `aimodelshare-0.1.9/aimodelshare/documentation/source/modelplayground.rst`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/generatemodelapi.py` & `aimodelshare-0.1.9/aimodelshare/generatemodelapi.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/iam/codebuild_policy.txt` & `aimodelshare-0.1.9/aimodelshare/iam/codebuild_policy.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/json_templates/api_json.txt` & `aimodelshare-0.1.9/aimodelshare/json_templates/api_json.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/leaderboard.py` & `aimodelshare-0.1.9/aimodelshare/leaderboard.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/main/1.txt` & `aimodelshare-0.1.9/aimodelshare/main/1.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/main/1B.txt` & `aimodelshare-0.1.9/aimodelshare/main/1B.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/main/2.txt` & `aimodelshare-0.1.9/aimodelshare/main/2.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/main/3.txt` & `aimodelshare-0.1.9/aimodelshare/main/3.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/main/4.txt` & `aimodelshare-0.1.9/aimodelshare/main/4.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/main/5.txt` & `aimodelshare-0.1.9/aimodelshare/main/5.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/main/6.txt` & `aimodelshare-0.1.9/aimodelshare/main/6.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/main/7.txt` & `aimodelshare-0.1.9/aimodelshare/main/7.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/main/8.txt` & `aimodelshare-0.1.9/aimodelshare/main/8.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/main/authorization.txt` & `aimodelshare-0.1.9/aimodelshare/main/authorization.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/main/eval_classification.txt` & `aimodelshare-0.1.9/aimodelshare/main/eval_classification.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/main/eval_lambda.txt` & `aimodelshare-0.1.9/aimodelshare/main/eval_lambda.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/main/eval_regression.txt` & `aimodelshare-0.1.9/aimodelshare/main/eval_regression.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/main/nst.txt` & `aimodelshare-0.1.9/aimodelshare/main/nst.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/model.py` & `aimodelshare-0.1.9/aimodelshare/model.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/modeluser.py` & `aimodelshare-0.1.9/aimodelshare/modeluser.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/placeholders/model.onnx` & `aimodelshare-0.1.9/aimodelshare/placeholders/model.onnx`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/placeholders/preprocessor.zip` & `aimodelshare-0.1.9/aimodelshare/placeholders/preprocessor.zip`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/playground.py` & `aimodelshare-0.1.9/aimodelshare/playground.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/postprocessormodules.py` & `aimodelshare-0.1.9/aimodelshare/postprocessormodules.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/preprocessormodules.py` & `aimodelshare-0.1.9/aimodelshare/preprocessormodules.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/pyspark/1.txt` & `aimodelshare-0.1.9/aimodelshare/pyspark/1.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/pyspark/1B.txt` & `aimodelshare-0.1.9/aimodelshare/pyspark/1B.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/pyspark/2.txt` & `aimodelshare-0.1.9/aimodelshare/pyspark/2.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/pyspark/3.txt` & `aimodelshare-0.1.9/aimodelshare/pyspark/3.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/pyspark/4.txt` & `aimodelshare-0.1.9/aimodelshare/pyspark/4.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/pyspark/5.txt` & `aimodelshare-0.1.9/aimodelshare/pyspark/5.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/pyspark/6.txt` & `aimodelshare-0.1.9/aimodelshare/pyspark/6.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/pyspark/7.txt` & `aimodelshare-0.1.9/aimodelshare/pyspark/7.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/pyspark/8.txt` & `aimodelshare-0.1.9/aimodelshare/pyspark/8.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/pyspark/authorization.txt` & `aimodelshare-0.1.9/aimodelshare/pyspark/authorization.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/pyspark/eval_classification.txt` & `aimodelshare-0.1.9/aimodelshare/pyspark/eval_classification.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/pyspark/eval_lambda.txt` & `aimodelshare-0.1.9/aimodelshare/pyspark/eval_lambda.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/pyspark/eval_regression.txt` & `aimodelshare-0.1.9/aimodelshare/pyspark/eval_regression.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/pyspark/nst.txt` & `aimodelshare-0.1.9/aimodelshare/pyspark/nst.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/python/my_preprocessor.py` & `aimodelshare-0.1.9/aimodelshare/python/my_preprocessor.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/readme.md` & `aimodelshare-0.1.9/aimodelshare/readme.md`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/reproducibility.py` & `aimodelshare-0.1.9/aimodelshare/reproducibility.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/sam/Dockerfile_PySpark.txt` & `aimodelshare-0.1.9/aimodelshare/sam/Dockerfile_PySpark.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/sam/buildspec.txt` & `aimodelshare-0.1.9/aimodelshare/sam/buildspec.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/sam/codebuild_policies.txt` & `aimodelshare-0.1.9/aimodelshare/sam/codebuild_policies.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/sam/codepipeline_policies.txt` & `aimodelshare-0.1.9/aimodelshare/sam/codepipeline_policies.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/sam/template.txt` & `aimodelshare-0.1.9/aimodelshare/sam/template.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/tools.py` & `aimodelshare-0.1.9/aimodelshare/tools.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare/utils.py` & `aimodelshare-0.1.9/aimodelshare/utils.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/aimodelshare.egg-info/PKG-INFO` & `aimodelshare-0.1.9/aimodelshare.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimodelshare
-Version: 0.1.8
+Version: 0.1.9
 Summary: Deploy locally saved machine learning models to a live rest API and web-dashboard.  Share it with the world via modelshare.org
 Home-page: https://www.modelshare.org
 Author: Michael Parrott
 Author-email: mikedparrott@modelshare.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `aimodelshare-0.1.8/aimodelshare.egg-info/SOURCES.txt` & `aimodelshare-0.1.9/aimodelshare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/setup.py` & `aimodelshare-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='aimodelshare', #TODO:update
-    version='0.1.8',        #TODO:update
+    version='0.1.9',        #TODO:update
     author="Michael Parrott",
     author_email="mikedparrott@modelshare.org",
     description="Deploy locally saved machine learning models to a live rest API and web-dashboard.  Share it with the world via modelshare.org",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.modelshare.org",
     packages=setuptools.find_packages(),
```

### Comparing `aimodelshare-0.1.8/tests/test_aimsonnx.py` & `aimodelshare-0.1.9/tests/test_aimsonnx.py`

 * *Files identical despite different names*

### Comparing `aimodelshare-0.1.8/tests/test_playground.py` & `aimodelshare-0.1.9/tests/test_playground.py`

 * *Files identical despite different names*

