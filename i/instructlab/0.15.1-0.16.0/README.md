# Comparing `tmp/instructlab-0.15.1.tar.gz` & `tmp/instructlab-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructlab-0.15.1.tar", last modified: Thu May 23 18:28:38 2024, max compression
+gzip compressed data, was "instructlab-0.16.0.tar", last modified: Fri May 31 15:43:26 2024, max compression
```

## Comparing `instructlab-0.15.1.tar` & `instructlab-0.16.0.tar`

### file list

```diff
@@ -1,195 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.923701 instructlab-0.15.1/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-23 18:28:35.000000 instructlab-0.15.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/actionlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/mergify.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/actionlint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/e2e.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/image-cuda.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/lint.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/.github/workflows/matchers/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/matchers/pylint.json
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/spellcheck.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/stale_bot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-23 18:28:35.000000 instructlab-0.15.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-23 18:28:35.000000 instructlab-0.15.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-23 18:28:35.000000 instructlab-0.15.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-23 18:28:35.000000 instructlab-0.15.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-23 18:28:35.000000 instructlab-0.15.1/.markdownlint-cli2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-23 18:28:35.000000 instructlab-0.15.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    21523 2024-05-23 18:28:35.000000 instructlab-0.15.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-23 18:28:35.000000 instructlab-0.15.1/.spellcheck-en-custom.txt
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-23 18:28:35.000000 instructlab-0.15.1/.spellcheck.yml
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-23 18:28:35.000000 instructlab-0.15.1/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/CONTRIBUTING/
--rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-05-23 18:28:35.000000 instructlab-0.15.1/CONTRIBUTING/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-23 18:28:35.000000 instructlab-0.15.1/CONTRIBUTING/FIRST_TIME_CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-23 18:28:35.000000 instructlab-0.15.1/CONTRIBUTOR_ROLES.md
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-23 18:28:35.000000 instructlab-0.15.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-23 18:28:35.000000 instructlab-0.15.1/MAINTAINERS.md
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-23 18:28:35.000000 instructlab-0.15.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    30417 2024-05-23 18:28:38.923701 instructlab-0.15.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27980 2024-05-23 18:28:35.000000 instructlab-0.15.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-23 18:28:35.000000 instructlab-0.15.1/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-23 18:28:35.000000 instructlab-0.15.1/TROUBLESHOOTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/containers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/containers/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2240 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/bin/debug-llama
--rwxr-xr-x   0 runner    (1001) docker     (127)     2079 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/bin/debug-pytorch
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/containers/cuda/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/cuda/Containerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.899701 instructlab-0.15.1/containers/hpu/
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/hpu/Containerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.903701 instructlab-0.15.1/containers/rocm/
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/rocm/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/rocm/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      618 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/rocm/gfx-version.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1480 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/rocm/remove-gfx.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-23 18:28:35.000000 instructlab-0.15.1/containers/sitecustomize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.903701 instructlab-0.15.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/STABLE.md
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/ci.md
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/containerization.md
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/converting_GGUF.md
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/demo-slides.md
--rw-r--r--   0 runner    (1001) docker     (127)    14107 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/gpu-acceleration.md
--rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/habana-gaudi.md
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/release-strategy.md
--rw-r--r--   0 runner    (1001) docker     (127)    90583 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/workflow.png
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-23 18:28:35.000000 instructlab-0.15.1/docs/workflow.puml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-23 18:28:35.000000 instructlab-0.15.1/governance.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.903701 instructlab-0.15.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    32510 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/Training_a_LoRA_With_Instruct_Lab.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.903701 instructlab-0.15.1/notebooks/images/
--rw-r--r--   0 runner    (1001) docker     (127)    83152 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/collab-copy-path.png
--rw-r--r--   0 runner    (1001) docker     (127)    89046 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/collab-file-upload-button.png
--rw-r--r--   0 runner    (1001) docker     (127)   165712 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/collab-folder-icon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.907701 instructlab-0.15.1/notebooks/images/kaggle/
--rw-r--r--   0 runner    (1001) docker     (127)   233502 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/clear-outputs.png
--rw-r--r--   0 runner    (1001) docker     (127)    58512 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/copy-file-path.png
--rw-r--r--   0 runner    (1001) docker     (127)    20354 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/create-new-nb.png
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/create.png
--rw-r--r--   0 runner    (1001) docker     (127)    18475 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/file-click.png
--rw-r--r--   0 runner    (1001) docker     (127)    23953 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/import-nb.png
--rw-r--r--   0 runner    (1001) docker     (127)   170886 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/input-drop-files.png
--rw-r--r--   0 runner    (1001) docker     (127)    21422 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/input-upload.png
--rw-r--r--   0 runner    (1001) docker     (127)    73216 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/input.png
--rw-r--r--   0 runner    (1001) docker     (127)    34311 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/new-dataset.png
--rw-r--r--   0 runner    (1001) docker     (127)    27504 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/select-accelerator-p100.png
--rw-r--r--   0 runner    (1001) docker     (127)   294162 2024-05-23 18:28:35.000000 instructlab-0.15.1/notebooks/images/kaggle/select-accelerator.png
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-23 18:28:35.000000 instructlab-0.15.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-23 18:28:35.000000 instructlab-0.15.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-23 18:28:35.000000 instructlab-0.15.1/requirements-hpu.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-23 18:28:35.000000 instructlab-0.15.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.907701 instructlab-0.15.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5262 2024-05-23 18:28:35.000000 instructlab-0.15.1/scripts/basic-workflow-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    11088 2024-05-23 18:28:35.000000 instructlab-0.15.1/scripts/functional-tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1091 2024-05-23 18:28:35.000000 instructlab-0.15.1/scripts/ruff.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.907701 instructlab-0.15.1/scripts/test-data/
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-23 18:28:35.000000 instructlab-0.15.1/scripts/test-data/basic-workflow-fixture-qna.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:28:38.923701 instructlab-0.15.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.891701 instructlab-0.15.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.911702 instructlab-0.15.1/src/instructlab/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 18:28:38.000000 instructlab-0.15.1/src/instructlab/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.911702 instructlab-0.15.1/src/instructlab/chat/
--rw-r--r--   0 runner    (1001) docker     (127)    19642 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/chat/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.911702 instructlab-0.15.1/src/instructlab/generator/
--rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/generator/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23232 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/generator/generate_data.py
--rw-r--r--   0 runner    (1001) docker     (127)   110936 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/generator/seed_tasks.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/generator/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    44198 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/lab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.911702 instructlab-0.15.1/src/instructlab/llamacpp/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/llamacpp/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/llamacpp/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/llamacpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    60403 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/llamacpp/llamacpp_convert_to_gguf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)  1361544 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/llamacpp/quantize
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.915701 instructlab-0.15.1/src/instructlab/mlx_explore/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/mlx_explore/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/mlx_explore/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/mlx_explore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10556 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/mlx_explore/gguf_convert_to_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/mlx_explore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.891701 instructlab-0.15.1/src/instructlab/schema/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.915701 instructlab-0.15.1/src/instructlab/schema/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/schema/v1/compositional_skills.json
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/schema/v1/knowledge.json
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/schema/v1/version.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.915701 instructlab-0.15.1/src/instructlab/schema/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/schema/v2/compositional_skills.json
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/schema/v2/knowledge.json
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/schema/v2/version.json
--rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.915701 instructlab-0.15.1/src/instructlab/train/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13425 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/linux_train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.919701 instructlab-0.15.1/src/instructlab/train/lora_mlx/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/make_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.919701 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/mixtral.py
--rw-r--r--   0 runner    (1001) docker     (127)    11484 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/models/phi2.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/prepare_model.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/train/lora_mlx/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-05-23 18:28:35.000000 instructlab-0.15.1/src/instructlab/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.923701 instructlab-0.15.1/src/instructlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    30417 2024-05-23 18:28:38.000000 instructlab-0.15.1/src/instructlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-23 18:28:38.000000 instructlab-0.15.1/src/instructlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:28:38.000000 instructlab-0.15.1/src/instructlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 18:28:38.000000 instructlab-0.15.1/src/instructlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-23 18:28:38.000000 instructlab-0.15.1/src/instructlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 18:28:38.000000 instructlab-0.15.1/src/instructlab.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.919701 instructlab-0.15.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_lab.py
--rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_lab_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_lab_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_lab_generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_lab_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    16370 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_lab_train.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.923701 instructlab-0.15.1/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/testdata/invalid_yaml.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/testdata/knowledge_valid.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/testdata/skill_incomplete.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/testdata/skill_invalid_answer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/testdata/skill_valid_answer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.923701 instructlab-0.15.1/tests/testdata/temp_repo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:28:38.923701 instructlab-0.15.1/tests/testdata/temp_repo/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/testdata/temp_repo/docs/skill-wiki.md
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/testdata/temp_repo/knowledge-wiki.md
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-23 18:28:35.000000 instructlab-0.15.1/tests/testdata/testdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-23 18:28:35.000000 instructlab-0.15.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.780833 instructlab-0.16.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-31 15:43:22.000000 instructlab-0.16.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.752833 instructlab-0.16.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.752833 instructlab-0.16.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-31 15:43:22.000000 instructlab-0.16.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-31 15:43:22.000000 instructlab-0.16.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-31 15:43:22.000000 instructlab-0.16.0/.github/ISSUE_TEMPLATE/team_recommend.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-31 15:43:22.000000 instructlab-0.16.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 15:43:22.000000 instructlab-0.16.0/.github/actionlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-31 15:43:22.000000 instructlab-0.16.0/.github/mergify.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.756833 instructlab-0.16.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-31 15:43:22.000000 instructlab-0.16.0/.github/workflows/actionlint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-31 15:43:22.000000 instructlab-0.16.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-31 15:43:22.000000 instructlab-0.16.0/.github/workflows/e2e.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-31 15:43:22.000000 instructlab-0.16.0/.github/workflows/image-cuda.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-31 15:43:22.000000 instructlab-0.16.0/.github/workflows/lint.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.756833 instructlab-0.16.0/.github/workflows/matchers/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-31 15:43:22.000000 instructlab-0.16.0/.github/workflows/matchers/pylint.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-31 15:43:22.000000 instructlab-0.16.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-31 15:43:22.000000 instructlab-0.16.0/.github/workflows/spellcheck.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-31 15:43:22.000000 instructlab-0.16.0/.github/workflows/stale_bot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-05-31 15:43:22.000000 instructlab-0.16.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-31 15:43:22.000000 instructlab-0.16.0/.github/workflows/validate-notebooks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-31 15:43:22.000000 instructlab-0.16.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-31 15:43:22.000000 instructlab-0.16.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-31 15:43:22.000000 instructlab-0.16.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-31 15:43:22.000000 instructlab-0.16.0/.markdownlint-cli2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-31 15:43:22.000000 instructlab-0.16.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    21523 2024-05-31 15:43:22.000000 instructlab-0.16.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-31 15:43:22.000000 instructlab-0.16.0/.spellcheck-en-custom.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-31 15:43:22.000000 instructlab-0.16.0/.spellcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-31 15:43:22.000000 instructlab-0.16.0/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.756833 instructlab-0.16.0/CONTRIBUTING/
+-rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-05-31 15:43:22.000000 instructlab-0.16.0/CONTRIBUTING/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-31 15:43:22.000000 instructlab-0.16.0/CONTRIBUTING/FIRST_TIME_CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-31 15:43:22.000000 instructlab-0.16.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-31 15:43:22.000000 instructlab-0.16.0/MAINTAINERS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-31 15:43:22.000000 instructlab-0.16.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    30604 2024-05-31 15:43:26.780833 instructlab-0.16.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    28124 2024-05-31 15:43:22.000000 instructlab-0.16.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-31 15:43:22.000000 instructlab-0.16.0/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-31 15:43:22.000000 instructlab-0.16.0/TROUBLESHOOTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.756833 instructlab-0.16.0/containers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-31 15:43:22.000000 instructlab-0.16.0/containers/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.756833 instructlab-0.16.0/containers/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2240 2024-05-31 15:43:22.000000 instructlab-0.16.0/containers/bin/debug-llama
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2079 2024-05-31 15:43:22.000000 instructlab-0.16.0/containers/bin/debug-pytorch
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.756833 instructlab-0.16.0/containers/cuda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-31 15:43:22.000000 instructlab-0.16.0/containers/cuda/Containerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.756833 instructlab-0.16.0/containers/hpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-31 15:43:22.000000 instructlab-0.16.0/containers/hpu/Containerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.756833 instructlab-0.16.0/containers/rocm/
+-rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-05-31 15:43:22.000000 instructlab-0.16.0/containers/rocm/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-31 15:43:22.000000 instructlab-0.16.0/containers/rocm/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      618 2024-05-31 15:43:22.000000 instructlab-0.16.0/containers/rocm/gfx-version.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1480 2024-05-31 15:43:22.000000 instructlab-0.16.0/containers/rocm/remove-gfx.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-31 15:43:22.000000 instructlab-0.16.0/containers/sitecustomize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.760833 instructlab-0.16.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-31 15:43:22.000000 instructlab-0.16.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-31 15:43:22.000000 instructlab-0.16.0/docs/ci.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-31 15:43:22.000000 instructlab-0.16.0/docs/converting_GGUF.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-31 15:43:22.000000 instructlab-0.16.0/docs/demo-slides.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14107 2024-05-31 15:43:22.000000 instructlab-0.16.0/docs/gpu-acceleration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8891 2024-05-31 15:43:22.000000 instructlab-0.16.0/docs/habana-gaudi.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-31 15:43:22.000000 instructlab-0.16.0/docs/release-strategy.md
+-rw-r--r--   0 runner    (1001) docker     (127)    90583 2024-05-31 15:43:22.000000 instructlab-0.16.0/docs/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-31 15:43:22.000000 instructlab-0.16.0/docs/workflow.puml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.760833 instructlab-0.16.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-05-31 15:43:22.000000 instructlab-0.16.0/notebooks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32510 2024-05-31 15:43:22.000000 instructlab-0.16.0/notebooks/Training_a_LoRA_With_Instruct_Lab.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.760833 instructlab-0.16.0/notebooks/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    83152 2024-05-31 15:43:22.000000 instructlab-0.16.0/notebooks/images/collab-copy-path.png
+-rw-r--r--   0 runner    (1001) docker     (127)    89046 2024-05-31 15:43:22.000000 instructlab-0.16.0/notebooks/images/collab-file-upload-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)   165712 2024-05-31 15:43:22.000000 instructlab-0.16.0/notebooks/images/collab-folder-icon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.764833 instructlab-0.16.0/notebooks/images/kaggle/
+-rw-r--r--   0 runner    (1001) docker     (127)   233502 2024-05-31 15:43:22.000000 instructlab-0.16.0/notebooks/images/kaggle/clear-outputs.png
+-rw-r--r--   0 runner    (1001) docker     (127)    58512 2024-05-31 15:43:22.000000 instructlab-0.16.0/notebooks/images/kaggle/copy-file-path.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20354 2024-05-31 15:43:22.000000 instructlab-0.16.0/notebooks/images/kaggle/create-new-nb.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-05-31 15:43:22.000000 instructlab-0.16.0/notebooks/images/kaggle/create.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18475 2024-05-31 15:43:22.000000 instructlab-0.16.0/notebooks/images/kaggle/file-click.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23953 2024-05-31 15:43:22.000000 instructlab-0.16.0/notebooks/images/kaggle/import-nb.png
+-rw-r--r--   0 runner    (1001) docker     (127)   170886 2024-05-31 15:43:22.000000 instructlab-0.16.0/notebooks/images/kaggle/input-drop-files.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21422 2024-05-31 15:43:22.000000 instructlab-0.16.0/notebooks/images/kaggle/input-upload.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73216 2024-05-31 15:43:22.000000 instructlab-0.16.0/notebooks/images/kaggle/input.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34311 2024-05-31 15:43:22.000000 instructlab-0.16.0/notebooks/images/kaggle/new-dataset.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27504 2024-05-31 15:43:22.000000 instructlab-0.16.0/notebooks/images/kaggle/select-accelerator-p100.png
+-rw-r--r--   0 runner    (1001) docker     (127)   294162 2024-05-31 15:43:22.000000 instructlab-0.16.0/notebooks/images/kaggle/select-accelerator.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-31 15:43:22.000000 instructlab-0.16.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-31 15:43:22.000000 instructlab-0.16.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-31 15:43:22.000000 instructlab-0.16.0/requirements-hpu.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-31 15:43:22.000000 instructlab-0.16.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.764833 instructlab-0.16.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5257 2024-05-31 15:43:22.000000 instructlab-0.16.0/scripts/basic-workflow-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10833 2024-05-31 15:43:22.000000 instructlab-0.16.0/scripts/functional-tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1091 2024-05-31 15:43:22.000000 instructlab-0.16.0/scripts/ruff.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.764833 instructlab-0.16.0/scripts/test-data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-31 15:43:22.000000 instructlab-0.16.0/scripts/test-data/basic-workflow-fixture-qna.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      992 2024-05-31 15:43:22.000000 instructlab-0.16.0/scripts/validate_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:43:26.780833 instructlab-0.16.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.748833 instructlab-0.16.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.764833 instructlab-0.16.0/src/instructlab/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-31 15:43:26.000000 instructlab-0.16.0/src/instructlab/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.768833 instructlab-0.16.0/src/instructlab/chat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/chat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20488 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/chat/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.768833 instructlab-0.16.0/src/instructlab/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/generator/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25291 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/generator/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110936 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/generator/seed_tasks.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/generator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45026 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/lab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.768833 instructlab-0.16.0/src/instructlab/llamacpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/llamacpp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/llamacpp/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/llamacpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60422 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/llamacpp/llamacpp_convert_to_gguf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.768833 instructlab-0.16.0/src/instructlab/mlx_explore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/mlx_explore/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/mlx_explore/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/mlx_explore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10556 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/mlx_explore/gguf_convert_to_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/mlx_explore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.748833 instructlab-0.16.0/src/instructlab/schema/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.772833 instructlab-0.16.0/src/instructlab/schema/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/schema/v1/compositional_skills.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/schema/v1/knowledge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/schema/v1/version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.772833 instructlab-0.16.0/src/instructlab/schema/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/schema/v2/compositional_skills.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/schema/v2/knowledge.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/schema/v2/version.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/sysinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.772833 instructlab-0.16.0/src/instructlab/train/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13425 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/linux_train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.772833 instructlab-0.16.0/src/instructlab/train/lora_mlx/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/make_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.776833 instructlab-0.16.0/src/instructlab/train/lora_mlx/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/models/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/models/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/models/mixtral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11484 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/models/phi2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/prepare_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/train/lora_mlx/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20599 2024-05-31 15:43:22.000000 instructlab-0.16.0/src/instructlab/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.776833 instructlab-0.16.0/src/instructlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    30604 2024-05-31 15:43:26.000000 instructlab-0.16.0/src/instructlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-05-31 15:43:26.000000 instructlab-0.16.0/src/instructlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:43:26.000000 instructlab-0.16.0/src/instructlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 15:43:26.000000 instructlab-0.16.0/src/instructlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-31 15:43:26.000000 instructlab-0.16.0/src/instructlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 15:43:26.000000 instructlab-0.16.0/src/instructlab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.776833 instructlab-0.16.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/test_lab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10293 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/test_lab_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/test_lab_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/test_lab_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/test_lab_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16564 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/test_lab_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.776833 instructlab-0.16.0/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/testdata/invalid_yaml.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/testdata/knowledge_valid.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/testdata/skill_incomplete.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/testdata/skill_invalid_answer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16722 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/testdata/skill_too_long_answer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/testdata/skill_valid_answer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.776833 instructlab-0.16.0/tests/testdata/temp_repo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:43:26.776833 instructlab-0.16.0/tests/testdata/temp_repo/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/testdata/temp_repo/docs/skill-wiki.md
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/testdata/temp_repo/knowledge-wiki.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-31 15:43:22.000000 instructlab-0.16.0/tests/testdata/testdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-31 15:43:22.000000 instructlab-0.16.0/tox.ini
```

### Comparing `instructlab-0.15.1/.github/ISSUE_TEMPLATE/bug_report.md` & `instructlab-0.16.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/.github/mergify.yml` & `instructlab-0.16.0/.github/mergify.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pull_request_rules:
 - name: auto-merge
-  description: automatic merge for main with > 1 approved reviews, all requested reviews have given feedback, not held, and CI is successful
+  description: automatic merge for main with >= 2 approved reviews, all requested reviews have given feedback, not held, and CI is successful
   conditions:
-    - "#approved-reviews-by>=1"
+    - "#approved-reviews-by>=2"
     - "#review-requested=0"
     - "#changes-requested-reviews-by=0"
     - or:
       - base=main
       - base~=release-.*
     - label!=hold
     - label!=do-not-merge
@@ -46,14 +46,22 @@
           - files~='.*\.md'
           - files='.markdownlint-cli2.yaml'
         - check-success=markdown-lint
       - and:
         - -files~='.*\.md'
         - -files='.markdownlint-cli2.yaml'
 
+    - or:
+      - and:
+        - or:
+          - files~='notebooks/.*\.ipynb$'
+        - check-success=validate-notebook
+      - and:
+        - -files~='notebooks/.*\.ipynb$'
+
   actions:
     merge:
       method: merge
     delete_head_branch:
 
 - name: label-cicd
   description: Automatically apply CI/CD label
@@ -149,7 +157,39 @@
 - name: backport release-v0.14
   actions:
     backport:
       branches:
         - release-v0.14
   conditions:
     - label=backport-release-v0.14
+
+- name: Apply ci-failure label if any CI checks have failed
+  conditions:
+      - "#check-failure>0"
+  actions:
+    label:
+      add:
+        - ci-failure
+
+- name: Remove ci-failure label if no failures are present
+  conditions:
+      - "#check-failure=0"
+  actions:
+    label:
+      remove:
+        - ci-failure
+
+- name: Apply 'one-approval' label if one of the maintainer approved the PR
+  conditions:
+      - "#approved-reviews-by=1"
+  actions:
+    label:
+      add:
+        - one-approval
+
+- name: Remove 'one-approval' label if the approval was reset
+  conditions:
+      - "#approved-reviews-by!=1"
+  actions:
+    label:
+      remove:
+        - one-approval
```

### Comparing `instructlab-0.15.1/.github/workflows/actionlint.yml` & `instructlab-0.16.0/.github/workflows/actionlint.yml`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
       - "main"
       - "release-**"
     paths:
       - '.github/**'
   pull_request:
     branches:
       - "main"
-      - '.github/**'
+      - "release-**"
     paths:
       - '.github/**'
 
 defaults:
   run:
     shell: bash
```

### Comparing `instructlab-0.15.1/.github/workflows/e2e.yml` & `instructlab-0.16.0/.github/workflows/e2e.yml`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         with:
           path: ~/.cache/huggingface
           # config contains DEFAULT_MODEL
           key: huggingface-${{ hashFiles('src/instructlab/config.py') }}
 
       - name: Install ilab
         run: |
-          export PATH="/home/runner/.local/bin:/usr/local/cuda-12.4/bin:$PATH"
+          export PATH="/home/runner/.local/bin:/usr/local/cuda/bin:$PATH"
           python3 -m venv venv
           . venv/bin/activate
           sed 's/\[.*\]//' requirements.txt > constraints.txt
           python3 -m pip cache remove llama_cpp_python
           CMAKE_ARGS="-DLLAMA_CUBLAS=on" python3 -m pip install --no-binary llama_cpp_python -c constraints.txt llama_cpp_python
           # needed for --4-bit-quant option to ilab train
           python3 -m pip install bitsandbytes
```

### Comparing `instructlab-0.15.1/.github/workflows/image-cuda.yml` & `instructlab-0.16.0/.github/workflows/image-cuda.yml`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/.github/workflows/lint.yml` & `instructlab-0.16.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/.github/workflows/matchers/pylint.json` & `instructlab-0.16.0/.github/workflows/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/.github/workflows/pypi.yaml` & `instructlab-0.16.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/.github/workflows/spellcheck.yaml` & `instructlab-0.16.0/.github/workflows/spellcheck.yaml`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/.github/workflows/stale_bot.yml` & `instructlab-0.16.0/.github/workflows/stale_bot.yml`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/.github/workflows/test.yml` & `instructlab-0.16.0/.github/workflows/test.yml`

 * *Files 6% similar despite different names*

```diff
@@ -124,21 +124,37 @@
             **/pyproject.toml
             **/requirements*.txt
 
       - name: Remove llama-cpp-python from cache
         run: |
           pip cache remove llama_cpp_python
 
+      - name: Run tox docs target (expect failure since tox is not present)
+        run: make man
+        continue-on-error: true
+
+      - name: Run tox docs target
+        id: tox-docs
+        run: make man || echo "status=failed" >> "$GITHUB_OUTPUT"
+        continue-on-error: true
+
+      - name: Check for 'make man' failure
+        run: |
+          if [[ "${{ steps.tox-docs.outputs.status }}" != "failed" ]]; then
+            echo "'make man' did not fail as expected"
+            exit 1
+          fi
+
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install tox
 
       - name: Run tox docs target
-        run: tox -e docs
+        run: make man
 
       - name: Check that man pages were generated
         uses: andstor/file-existence-action@v3
         with:
           files: 'man/*.1'
           fail: true
```

### Comparing `instructlab-0.15.1/.gitignore` & `instructlab-0.16.0/.gitignore`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/.pylintrc` & `instructlab-0.16.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/.spellcheck-en-custom.txt` & `instructlab-0.16.0/.spellcheck-en-custom.txt`

 * *Files 21% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 DKMS
 dr
 Dropdown
 env
 EPEL
 Eval
 Finetuning
+frontend
 Gaudi
 GFX
 GGUF
 GiB
 GitHub
 Gmail
 gpu
@@ -54,14 +55,16 @@
 Kai
 Kubernetes
 lignment
 LLM
 llms
 LLVM
 lora
+md
+Mergify
 Merlinite
 Miniforge
 Mixtral
 mlx
 MLX
 MPS
 Nvidia
@@ -72,16 +75,18 @@
 orchestrator
 ots
 Pareja
 PEFT
 PlantUML
 Podman
 pre
+preceeds
 preprint
 pyenv
+PyPi
 PyPI
 PyTorch
 qlora
 quantized
 Quantizing
 Radeon
 RDNA
```

### Comparing `instructlab-0.15.1/.spellcheck.yml` & `instructlab-0.16.0/.spellcheck.yml`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/CONTRIBUTING/CONTRIBUTING.md` & `instructlab-0.16.0/CONTRIBUTING/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/CONTRIBUTING/FIRST_TIME_CONTRIBUTORS.md` & `instructlab-0.16.0/CONTRIBUTING/FIRST_TIME_CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/LICENSE` & `instructlab-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/Makefile` & `instructlab-0.16.0/Makefile`

 * *Files 13% similar despite different names*

```diff
@@ -41,34 +41,37 @@
 help: ## Display this help.
 	@awk 'BEGIN {FS = ":.*##"; printf "\nUsage:\n  make \033[36m<target>\033[0m\n"} /^[a-zA-Z_0-9-]+:.*?##/ { printf "  \033[36m%-15s\033[0m %s\n", $$1, $$2 } /^##@/ { printf "\n\033[1m%s\033[0m\n", substr($$0, 5) } ' $(MAKEFILE_LIST)
 
 ##@ Build
 
 .PHONY: images
 images: ## Get the current controller, set the path, and build the Containerfile image. (auto-detect the compatible controller)
-	@if lspci -d '10DE:*:0300'| grep -q "NVIDIA"; then \
+	@if ! command -v lspci &> /dev/null; then \
+		echo "ERROR: Unable to detect GPU, lspci is not installed" >&2; \
+		exit 2; \
+	elif lspci -d '10DE:*:0300'| grep -q "NVIDIA"; then \
 		$(MAKE) cuda; \
 	elif lspci -d '1002:*:0300' | grep -q "AMD"; then \
 		$(MAKE) rocm; \
 	else \
 		echo "ERROR: Unable to detect AMD / Nvidia GPU" >&2; \
 		exit 2; \
 	fi
 
 .PHONY: cuda
-cuda: $(CUDA_DEPS)  ## Build container for NVidia CUDA
+cuda: check-engine $(CUDA_DEPS)  ## Build container for NVidia CUDA
 	$(CENGINE) build $(BUILD_ARGS) \
 		-t $(CONTAINER_PREFIX):$@ \
 		-f $(CUDA_CONTAINERFILE) \
 		.
 
 # The base container uses uids beyond 65535. Rootless builds may not work
 # unless the user account has extended subordinate ids up to 2**24 - 1.
 .PHONY: hpu
-hpu: $(HPU_DEPS)  ## Build container for Intel Gaudi HPU
+hpu: $(HPU_DEPS) check-engine ## Build container for Intel Gaudi HPU
 	$(CENGINE) build $(BUILD_ARGS) \
 		-t $(CONTAINER_PREFIX):$@ \
 		-f $< \
 		.
 
 define build-rocm =
 	@echo "Building ROCm container for GPU arch '$(1)', version '$(2)'"
@@ -78,15 +81,15 @@
 		-t $(CONTAINER_PREFIX):rocm-$(1) \
 		-t $(CONTAINER_PREFIX):rocm \
 		-f $(ROCM_CONTAINERFILE) \
 		.
 endef
 
 .PHONY: rocm
-rocm:   ## Build container for AMD ROCm (auto-detect the ROCm GPU arch)
+rocm: check-rocm  ## Build container for AMD ROCm (auto-detect the ROCm GPU arch)
 	@# amdgpu-arch requires clang-tools-extra and rocm-hip-devel to work
 	@# rocminfo parsing is more messy, but requires less dependencies.
 	@arch=$(shell rocminfo | grep -o -m1 'gfx[1-9][0-9a-f]*'); \
 	    if test -z $$arch; then echo "Unable to detect AMD GPU arch"; exit 2; fi; \
 	    echo "Auto-detected GPU arch '$$arch'"; \
 	    $(MAKE) rocm-$${arch}
 
@@ -119,44 +122,42 @@
 	$(call build-rocm,gfx906,9.0.6)
 
 .PHONY: rocm-gfx900
 rocm-gfx900: $(ROCM_DEPS)  ## Build container for AMD ROCm gfx900 (untested)
 	$(call build-rocm,gfx900,9.0.0)
 
 .PHONY: rocm-toolbox
-toolbox-rocm:  ## Create AMD ROCm toolbox from container
+toolbox-rocm: check-toolbox ## Create AMD ROCm toolbox from container
 	toolbox create --image $(CONTAINER_PREFIX):rocm $(TOOLBOX)
 
 .PHONY: toolbox-rm
-toolbox-rm:  ## Stop and remove toolbox container
+toolbox-rm: check-toolbox ## Stop and remove toolbox container
 	toolbox rm -f $(TOOLBOX)
 
 ##@ Development
 
 .PHONY: tests
-tests: ## Run tox -e unit against code
+tests: check-tox ## Run tox -e unit against code
 	tox -e py3-unit
 
 .PHONY: verify
-verify: ## Run tox -e fmt,lint,spellcheck against code
+verify: check-tox ## Run tox -e fmt,lint,spellcheck against code
 	tox p -e ruff,fastlint,spellcheck
 
 .PHONY: spellcheck-sort
-spellcheck-sort: .spellcheck-en-custom.txt
+spellcheck-sort: .spellcheck-en-custom.txt ## Sort spellcheck directory
 	sort -d -o $< $<
 
 .PHONY: man
-man:
+man: check-tox
 	tox -e docs
 
 .PHONY: docs
 docs: man ## Run tox -e docs against code
 
-##@ Linting
-
 #
 # If you want to see the full commands, run:
 #   NOISY_BUILD=y make
 #
 ifeq ($(NOISY_BUILD),)
     ECHO_PREFIX=@
     CMD_PREFIX=@
@@ -164,10 +165,26 @@
 else
     ECHO_PREFIX=@\#
     CMD_PREFIX=
     PIPE_DEV_NULL=
 endif
 
 .PHONY: md-lint
-md-lint: ## Lint markdown files
+md-lint: check-engine ## Lint markdown files
 	$(ECHO_PREFIX) printf "  %-12s ./...\n" "[MD LINT]"
-	$(CMD_PREFIX) podman run --rm -v $(CURDIR):/workdir --security-opt label=disable docker.io/davidanson/markdownlint-cli2:v0.12.1 > /dev/null
+	$(CMD_PREFIX) $(CENGINE) run --rm -v $(CURDIR):/workdir --security-opt label=disable docker.io/davidanson/markdownlint-cli2:v0.12.1 > /dev/null
+
+.PHONY: check-tox
+check-tox:
+	@command -v tox &> /dev/null || (echo "'tox' is not installed" && exit 1)
+
+.PHONY: check-toolbox
+check-toolbox:
+	@command -v toolbox &> /dev/null || (echo "'toolbox' is not installed" && exit 1)
+
+.PHONY: check-engine
+check-engine:
+	@command -v $(CENGINE) &> /dev/null || (echo "'$(CENGINE)' container engine is not installed, you can override it with the 'CENGINE' variable" && exit 1)
+
+.PHONY: check-rocm
+check-rocm:
+	@command -v rocm &> /dev/null || (echo "'rocm' is not installed" && exit 1)
```

### Comparing `instructlab-0.15.1/PKG-INFO` & `instructlab-0.16.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructlab
-Version: 0.15.1
+Version: 0.16.0
 Summary: CLI for interacting with InstructLab
 Author-email: TBD <jon@example.com>
 License: Apache-2.0 AND MIT
 Project-URL: homepage, https://instructlab.io
 Project-URL: source, https://github.com/instructlab/instructlab
 Project-URL: issues, https://github.com/instructlab/instructlab/issues
 Classifier: Development Status :: 3 - Alpha
@@ -25,14 +25,15 @@
 License-File: LICENSE
 Requires-Dist: click<9.0.0,>=8.1.7
 Requires-Dist: click-didyoumean<0.4.0,>=0.3.0
 Requires-Dist: datasets<3.0.0,>=2.18.0
 Requires-Dist: gguf<0.7.0,>=0.6.0
 Requires-Dist: GitPython<4.0.0,>=3.1.42
 Requires-Dist: httpx<1.0.0,>=0.25.0
+Requires-Dist: instructlab-quantize>=0.1.0
 Requires-Dist: jsonschema<5.0.0,>=4.21.1
 Requires-Dist: llama_cpp_python[server]==0.2.75
 Requires-Dist: mlx<0.6.0,>=0.5.1; sys_platform == "darwin" and platform_machine == "arm64"
 Requires-Dist: numpy<2.0.0,>=1.23.5; python_version == "3.10"
 Requires-Dist: numpy<2.0.0,>=1.26.4; python_version != "3.10"
 Requires-Dist: openai<2.0.0,>=1.13.3
 Requires-Dist: peft<0.10.0,>=0.9.0
@@ -65,38 +66,31 @@
 ## 📖 Contents
 
 - [Welcome to the InstructLab CLI](#welcome-to-the-instructlab-cli)
 - [❓ What is `ilab`](#-what-is-ilab)
 - [📋 Requirements](#-requirements)
 - [✅ Getting started](#-getting-started)
   - [🧰 Installing `ilab`](#-installing-ilab)
-    - [To install with no GPU acceleration and PyTorch without CUDA bindings](#to-install-with-no-gpu-acceleration-and-pytorch-without-cuda-bindings)
-    - [To install with AMD ROCm](#to-install-with-amd-rocm)
-    - [To install with Apple Metal on M1/M2/M3 Mac](#to-install-with-apple-metal-on-m1m2m3-mac)
-    - [To install with Nvidia CUDA](#to-install-with-nvidia-cuda)
-    - [Example output](#example-output)
-    - [Bash (version 4.4 or newer)](#bash-version-44-or-newer)
-    - [Zsh](#zsh)
-    - [Fish](#fish)
+    - [Install with no GPU acceleration and PyTorch without CUDA bindings](#install-using-pytorch-without-cuda-bindings-and-no-gpu-acceleration)
+    - [Install with AMD ROCm](#install-with-amd-rocm)
+    - [Install with Apple Metal on M1/M2/M3 Macs](#install-with-apple-metal-on-m1m2m3-macs)
+    - [Install with Nvidia CUDA](#install-with-nvidia-cuda)
   - [🏗️ Initialize `ilab`](#️-initialize-ilab)
-    - [Example output](#example-output-1)
-    - [Example output](#example-output-2)
   - [📥 Download the model](#-download-the-model)
   - [🍴 Serving the model](#-serving-the-model)
   - [📣 Chat with the model (Optional)](#-chat-with-the-model-optional)
 - [💻 Creating new knowledge or skills and training the model](#-creating-new-knowledge-or-skills-and-training-the-model)
   - [🎁 Contribute knowledge or compositional skills](#-contribute-knowledge-or-compositional-skills)
   - [📜 List and validate your new data](#-list-and-validate-your-new-data)
   - [🚀 Generate a synthetic dataset](#-generate-a-synthetic-dataset)
-    - [Example output](#example-output-3)
-  - [👩‍🏫 Train the model](#-train-the-model)
+  - [👩‍🏫 Training the model](#-training-the-model)
     - [Train the model locally on Linux](#train-the-model-locally-on-linux)
-    - [Train the model locally on an M-series Mac](#train-the-model-locally-on-an-m-series-mac)
-    - [Training the model locally with GPU acceleration](#training-the-model-locally-with-gpu-acceleration)
-    - [Training the model in the cloud](#training-the-model-in-the-cloud)
+    - [Train the model locally on M-series Macs](#train-the-model-locally-on-an-m-series-mac)
+    - [Train the model locally with GPU acceleration](#train-the-model-locally-with-gpu-acceleration)
+    - [Train the model in the cloud](#train-the-model-in-the-cloud)
   - [📜 Test the newly trained model](#-test-the-newly-trained-model)
   - [🍴 Serve the newly trained model](#-serve-the-newly-trained-model)
 - [📣 Chat with the new model (not optional this time)](#-chat-with-the-new-model-not-optional-this-time)
 - [🎁 Submit your new knowledge or skills](#-submit-your-new-knowledge-or-skills)
 - [📬 Contributing](#-contributing)
 
 ## Welcome to the InstructLab CLI
@@ -143,15 +137,15 @@
 - **🍎 Apple M1/M2/M3 Mac or 🐧 Linux system** (tested on Fedora). We anticipate support for more operating systems in the future.
 - C++ compiler
 - Python 3.9+ (<3.12 for PyTorch JIT)
 - Approximately 60GB disk space (entire process)
 
 > **NOTE:** PyTorch 2.2.1 does not support `torch.compile` with Python 3.12. On Fedora 39+, install `python3.11-devel` and create the virtual env with `python3.11` if you wish to use PyTorch's JIT compiler.
 <!-- -->
-> **NOTE:** When installing the `ilab` CLI on macOS, you may have to run the `xcode select --install` command to install the required packages previously listed.
+> **NOTE:** When installing the `ilab` CLI on macOS, you may have to run the `xcode select --install` command, installing the required packages previously listed.
 
 ## ✅ Getting started
 
 ### 🧰 Installing `ilab`
 
 1. When installing on Fedora Linux, install C++, Python 3.9+, and other necessary tools by running the following command:
 
@@ -172,73 +166,81 @@
    ```shell
    mkdir instructlab
    cd instructlab
    ```
 
    > **NOTE:** The following steps in this document use [Python venv](https://docs.python.org/3/library/venv.html) for virtual environments. However, if you use another tool such as [pyenv](https://github.com/pyenv/pyenv) or [Conda Miniforge](https://github.com/conda-forge/miniforge) for managing Python environments on your machine continue to use that tool instead. Otherwise, you may have issues with packages that are installed but not found in `venv`.
 
-3. Install and activate your `venv` environment by running the following command:
+3. There are a few ways you can locally install the `ilab` CLI. Select your preferred installation method from the following instructions. You can then install `ilab` and activate your `venv` environment.
 
    > **NOTE**: ⏳ `pip install` may take some time, depending on your internet connection. In case installation fails with error ``unsupported instruction `vpdpbusd'``, append `-C cmake.args="-DLLAMA_NATIVE=off"` to `pip install` command.
 
    See [the GPU acceleration documentation](./docs/gpu-acceleration.md) for how to
-   to enable hardware acceleration for inference and training on AMD ROCm,
+   to enable hardware acceleration for interaction and training on AMD ROCm,
    Apple Metal Performance Shaders (MPS), and Nvidia CUDA.
 
-   #### To install with no GPU acceleration and PyTorch without CUDA bindings
+   #### Install using PyTorch without CUDA bindings and no GPU acceleration
 
-   ```shell
-   python3 -m venv --upgrade-deps venv
-   source venv/bin/activate
-   (venv) $ pip cache remove llama_cpp_python
-   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable --extra-index-url=https://download.pytorch.org/whl/cpu
-   ```
-
-   #### To install with AMD ROCm
-
-   ```shell
-   python3 -m venv --upgrade-deps venv
-   source venv/bin/activate
-   (venv) $ pip cache remove llama_cpp_python
-   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable \
-       --extra-index-url https://download.pytorch.org/whl/rocm6.0 \
-       -C cmake.args="-DLLAMA_HIPBLAS=on" \
-       -C cmake.args="-DAMDGPU_TARGETS=all" \
-       -C cmake.args="-DCMAKE_C_COMPILER=/opt/rocm/llvm/bin/clang" \
-       -C cmake.args="-DCMAKE_CXX_COMPILER=/opt/rocm/llvm/bin/clang++" \
-       -C cmake.args="-DCMAKE_PREFIX_PATH=/opt/rocm"
-   ```
-
-   On Fedora 40+, use `-DCMAKE_C_COMPILER=clang-17` and `-DCMAKE_CXX_COMPILER=clang++-17`.
-
-   #### To install with Apple Metal on M1/M2/M3 Mac
-
-   ```shell
-   python3 -m venv --upgrade-deps venv
-   source venv/bin/activate
-   (venv) $ pip cache remove llama_cpp_python
-   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable -C cmake.args="-DLLAMA_METAL=on"
-   ```
-
-   #### To install with Nvidia CUDA
-
-   ```shell
-   python3 -m venv --upgrade-deps venv
-   source venv/bin/activate
-   (venv) $ pip cache remove llama_cpp_python
-   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable -C cmake.args="-DLLAMA_CUBLAS=on"
+      ```shell
+      python3 -m venv --upgrade-deps venv
+      source venv/bin/activate
+      (venv) $ pip cache remove llama_cpp_python
+      (venv) $ pip install instructlab --extra-index-url=https://download.pytorch.org/whl/cpu
+      ```
+
+      > **NOTE**: *Additional Build Argument for Intel Macs*
+      >
+      > If you have an Mac with an Intel CPU, you must add a prefix of
+      > `CMAKE_ARGS="-DLLAMA_METAL=off"` to the `pip install` command to ensure
+      > that the build is done without Apple M-series GPU support.
+      >
+      > `(venv) $ CMAKE_ARGS="-DLLAMA_METAL=off" pip install ...`
+
+   #### Install with AMD ROCm
+
+      ```shell
+      python3 -m venv --upgrade-deps venv
+      source venv/bin/activate
+      (venv) $ pip cache remove llama_cpp_python
+      (venv) $ pip install instructlab \
+         --extra-index-url https://download.pytorch.org/whl/rocm6.0 \
+         -C cmake.args="-DLLAMA_HIPBLAS=on" \
+         -C cmake.args="-DAMDGPU_TARGETS=all" \
+         -C cmake.args="-DCMAKE_C_COMPILER=/opt/rocm/llvm/bin/clang" \
+         -C cmake.args="-DCMAKE_CXX_COMPILER=/opt/rocm/llvm/bin/clang++" \
+         -C cmake.args="-DCMAKE_PREFIX_PATH=/opt/rocm"
+      ```
+
+      On Fedora 40+, use `-DCMAKE_C_COMPILER=clang-17` and `-DCMAKE_CXX_COMPILER=clang++-17`.
+
+   #### Install with Apple Metal on M1/M2/M3 Macs
+
+      ```shell
+      python3 -m venv --upgrade-deps venv
+      source venv/bin/activate
+      (venv) $ pip cache remove llama_cpp_python
+      (venv) $ pip install instructlab
+      ```
+
+   #### Install with Nvidia CUDA
+
+      ```shell
+      python3 -m venv --upgrade-deps venv
+      source venv/bin/activate
+      (venv) $ pip cache remove llama_cpp_python
+      (venv) $ pip install instructlab -C cmake.args="-DLLAMA_CUBLAS=on"
    ```
 
 4. From your `venv` environment, verify `ilab` is installed correctly, by running the `ilab` command.
 
    ```shell
    ilab
    ```
 
-   #### Example output
+   *Example output of the `ilab` command*
 
    ```shell
    (venv) $ ilab
    Usage: ilab [OPTIONS] COMMAND [ARGS]...
 
    CLI for interacting with InstructLab.
 
@@ -265,15 +267,15 @@
 
    > **IMPORTANT:** every `ilab` command needs to be run from within your Python virtual environment. To enter the Python environment, run the following command:
 
    ```shell
    source venv/bin/activate
    ```
 
-5. You may optionally enable tab completion for the `ilab` command.
+5. Optional: You can enable tab completion for the `ilab` command.
 
    #### Bash (version 4.4 or newer)
 
    Enable tab completion in `bash` with the following command:
 
    ```sh
    eval "$(_ILAB_COMPLETE=bash_source ilab)"
@@ -322,29 +324,29 @@
 
 1. Initialize `ilab` by running the following command:
 
    ```shell
    ilab init
    ```
 
-   #### Example output
+   *Example output*
 
    ```shell
    Welcome to InstructLab CLI. This guide will help you set up your environment.
    Please provide the following values to initiate the environment [press Enter for defaults]:
    Path to taxonomy repo [taxonomy]: <ENTER>
    ```
 
 2. When prompted by the interface, press **Enter** to add a new default `config.yaml` file.
 
 3. When prompted, clone the `https://github.com/instructlab/taxonomy.git` repository into the current directory by typing **y**.
 
    **Optional**: If you want to point to an existing local clone of the `taxonomy` repository, you can pass the path interactively or alternatively with the `--taxonomy-path` flag.
 
-   #### Example output
+   *Example output after initializing `ilab`*
 
    ```shell
    (venv) $ ilab init
    Welcome to InstructLab CLI. This guide will help you set up your environment.
    Please provide the following values to initiate the environment [press Enter for defaults]:
    Path to taxonomy repo [taxonomy]: <ENTER>
    `taxonomy` seems to not exists or is empty. Should I clone https://github.com/instructlab/taxonomy.git for you? [y/N]: y
@@ -363,21 +365,21 @@
    ```shell
    git clone --recurse-submodules https://github.com/instructlab/taxonomy.git
    git pull --recurse-submodules
    ```
 
 ### 📥 Download the model
 
-- Run the `ilab download`command.
+- Run the `ilab download` command.
 
   ```shell
   ilab download
   ```
 
-  `ilab download` will download a pre-trained [model](https://huggingface.co/instructlab/) (~4.4G) from HuggingFace and store it in a `models` directory:
+  `ilab download` downloads a compact pre-trained version of the [model](https://huggingface.co/instructlab/) (~4.4G) from HuggingFace and store it in a `models` directory:
 
   ```shell
   (venv) $ ilab download
   Downloading model from instructlab/merlinite-7b-lab-GGUF@main to models...
   (venv) $ ls models
   merlinite-7b-lab-Q4_K_M.gguf
   ```
@@ -465,15 +467,15 @@
 
    ```shell
    ilab generate
    ```
 
    > **NOTE:** ⏳ This can take from 15 minutes to 1+ hours to complete, depending on your computing resources.
 
-   #### Example output
+   *Example output of `ilab generate`*
 
    ```shell
    (venv) $ ilab generate
    INFO 2024-02-29 19:09:48,804 lab.py:250 Generating model 'ggml-merlinite-7b-lab-Q4_K_M' using 10 CPUs,
    taxonomy: '/home/username/instructlab/taxonomy' and seed 'seed_tasks.json'
 
    0%|##########| 0/100 Cannot find prompt.txt. Using default prompt.
@@ -498,19 +500,19 @@
    **Optional**: It is also possible to run the generate step against a different model via an
    OpenAI-compatible API. For example, the one spawned by `ilab serve` or any remote or locally hosted LLM (e.g. via [`ollama`](https://ollama.com/), [`LM Studio`](https://lmstudio.ai), etc.). Run the following command:
 
    ```shell
    ilab generate --endpoint-url http://localhost:8000/v1
    ```
 
-### 👩‍🏫 Train the model
+### 👩‍🏫 Training the model
 
-There are three options to train the model on your synthetic data-enhanced dataset.
+There are many options for training the model with your synthetic data-enhanced dataset.
 
-> **Note:** **Every** `ilab` command needs to be run from within your Python virtual environment.
+> **Note:** **Every** `ilab` command needs to run from within your Python virtual environment.
 
 #### Train the model locally on Linux
 
 ```shell
 ilab train
 ```
 
@@ -540,23 +542,23 @@
 (venv) $ ls instructlab-merlinite-7b-lab-mlx-q
 adapters-010.npz        adapters-050.npz        adapters-090.npz        config.json             tokenizer.model
 adapters-020.npz        adapters-060.npz        adapters-100.npz        model.safetensors       tokenizer_config.json
 adapters-030.npz        adapters-070.npz        adapters.npz            special_tokens_map.json
 adapters-040.npz        adapters-080.npz        added_tokens.json       tokenizer.jso
 ```
 
-#### Training the model locally with GPU acceleration
+#### Train the model locally with GPU acceleration
 
 Training has experimental support for GPU acceleration with Nvidia CUDA or AMD ROCm. Please see [the GPU acceleration documentation](./docs/gpu-acceleration.md) for more details. At present, hardware acceleration requires a data center GPU or high-end consumer GPU with at least 18 GB free memory.
 
 ```shell
 ilab train --device=cuda
 ```
 
-#### Training the model in the cloud
+#### Train the model in the cloud
 
 Follow the instructions in [Training](./notebooks/README.md).
 
 ⏳ Approximate amount of time taken on each platform:
 
 - *Google Colab*: **5-10 minutes** with a T4 GPU
 - *Kaggle*: **~30 minutes** with a P100 GPU.
@@ -592,20 +594,20 @@
    ilab convert
    ```
 
 3. Serve the newly trained model locally via `ilab serve` command with the `--model-path`
 argument to specify your new model:
 
    ```shell
-   ilab serve --model-path <New model name>
+   ilab serve --model-path <new model path>
    ```
 
-   Which model should you select to serve? After running the `ilab convert` command, a few files and directories are generated. The one you will want to serve will end in `.gguf`
-   and will exist in a directory with the suffix `fused-pt`. For example:
-   `instructlab-merlinite-7b-lab-mlx-q-fused-pt/ggml-model-Q4_K_M.gguf`
+   Which model should you select to serve? After running the `ilab convert` command, some files and a directory are generated. The model you will want to serve ends with an extension of `.gguf`
+   and exists in a directory with the suffix `trained`. For example:
+   `instructlab-merlinite-7b-lab-trained/instructlab-merlinite-7b-lab-Q4_K_M.gguf`.
 
 ## 📣 Chat with the new model (not optional this time)
 
 - Try the fine-tuned model out live using the chat interface, and see if the results are better than the untrained version of the model with chat by running the following command:
 
    ```shell
    ilab chat -m <New model name>
```

### Comparing `instructlab-0.15.1/README.md` & `instructlab-0.16.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,38 +9,31 @@
 ## 📖 Contents
 
 - [Welcome to the InstructLab CLI](#welcome-to-the-instructlab-cli)
 - [❓ What is `ilab`](#-what-is-ilab)
 - [📋 Requirements](#-requirements)
 - [✅ Getting started](#-getting-started)
   - [🧰 Installing `ilab`](#-installing-ilab)
-    - [To install with no GPU acceleration and PyTorch without CUDA bindings](#to-install-with-no-gpu-acceleration-and-pytorch-without-cuda-bindings)
-    - [To install with AMD ROCm](#to-install-with-amd-rocm)
-    - [To install with Apple Metal on M1/M2/M3 Mac](#to-install-with-apple-metal-on-m1m2m3-mac)
-    - [To install with Nvidia CUDA](#to-install-with-nvidia-cuda)
-    - [Example output](#example-output)
-    - [Bash (version 4.4 or newer)](#bash-version-44-or-newer)
-    - [Zsh](#zsh)
-    - [Fish](#fish)
+    - [Install with no GPU acceleration and PyTorch without CUDA bindings](#install-using-pytorch-without-cuda-bindings-and-no-gpu-acceleration)
+    - [Install with AMD ROCm](#install-with-amd-rocm)
+    - [Install with Apple Metal on M1/M2/M3 Macs](#install-with-apple-metal-on-m1m2m3-macs)
+    - [Install with Nvidia CUDA](#install-with-nvidia-cuda)
   - [🏗️ Initialize `ilab`](#️-initialize-ilab)
-    - [Example output](#example-output-1)
-    - [Example output](#example-output-2)
   - [📥 Download the model](#-download-the-model)
   - [🍴 Serving the model](#-serving-the-model)
   - [📣 Chat with the model (Optional)](#-chat-with-the-model-optional)
 - [💻 Creating new knowledge or skills and training the model](#-creating-new-knowledge-or-skills-and-training-the-model)
   - [🎁 Contribute knowledge or compositional skills](#-contribute-knowledge-or-compositional-skills)
   - [📜 List and validate your new data](#-list-and-validate-your-new-data)
   - [🚀 Generate a synthetic dataset](#-generate-a-synthetic-dataset)
-    - [Example output](#example-output-3)
-  - [👩‍🏫 Train the model](#-train-the-model)
+  - [👩‍🏫 Training the model](#-training-the-model)
     - [Train the model locally on Linux](#train-the-model-locally-on-linux)
-    - [Train the model locally on an M-series Mac](#train-the-model-locally-on-an-m-series-mac)
-    - [Training the model locally with GPU acceleration](#training-the-model-locally-with-gpu-acceleration)
-    - [Training the model in the cloud](#training-the-model-in-the-cloud)
+    - [Train the model locally on M-series Macs](#train-the-model-locally-on-an-m-series-mac)
+    - [Train the model locally with GPU acceleration](#train-the-model-locally-with-gpu-acceleration)
+    - [Train the model in the cloud](#train-the-model-in-the-cloud)
   - [📜 Test the newly trained model](#-test-the-newly-trained-model)
   - [🍴 Serve the newly trained model](#-serve-the-newly-trained-model)
 - [📣 Chat with the new model (not optional this time)](#-chat-with-the-new-model-not-optional-this-time)
 - [🎁 Submit your new knowledge or skills](#-submit-your-new-knowledge-or-skills)
 - [📬 Contributing](#-contributing)
 
 ## Welcome to the InstructLab CLI
@@ -87,15 +80,15 @@
 - **🍎 Apple M1/M2/M3 Mac or 🐧 Linux system** (tested on Fedora). We anticipate support for more operating systems in the future.
 - C++ compiler
 - Python 3.9+ (<3.12 for PyTorch JIT)
 - Approximately 60GB disk space (entire process)
 
 > **NOTE:** PyTorch 2.2.1 does not support `torch.compile` with Python 3.12. On Fedora 39+, install `python3.11-devel` and create the virtual env with `python3.11` if you wish to use PyTorch's JIT compiler.
 <!-- -->
-> **NOTE:** When installing the `ilab` CLI on macOS, you may have to run the `xcode select --install` command to install the required packages previously listed.
+> **NOTE:** When installing the `ilab` CLI on macOS, you may have to run the `xcode select --install` command, installing the required packages previously listed.
 
 ## ✅ Getting started
 
 ### 🧰 Installing `ilab`
 
 1. When installing on Fedora Linux, install C++, Python 3.9+, and other necessary tools by running the following command:
 
@@ -116,73 +109,81 @@
    ```shell
    mkdir instructlab
    cd instructlab
    ```
 
    > **NOTE:** The following steps in this document use [Python venv](https://docs.python.org/3/library/venv.html) for virtual environments. However, if you use another tool such as [pyenv](https://github.com/pyenv/pyenv) or [Conda Miniforge](https://github.com/conda-forge/miniforge) for managing Python environments on your machine continue to use that tool instead. Otherwise, you may have issues with packages that are installed but not found in `venv`.
 
-3. Install and activate your `venv` environment by running the following command:
+3. There are a few ways you can locally install the `ilab` CLI. Select your preferred installation method from the following instructions. You can then install `ilab` and activate your `venv` environment.
 
    > **NOTE**: ⏳ `pip install` may take some time, depending on your internet connection. In case installation fails with error ``unsupported instruction `vpdpbusd'``, append `-C cmake.args="-DLLAMA_NATIVE=off"` to `pip install` command.
 
    See [the GPU acceleration documentation](./docs/gpu-acceleration.md) for how to
-   to enable hardware acceleration for inference and training on AMD ROCm,
+   to enable hardware acceleration for interaction and training on AMD ROCm,
    Apple Metal Performance Shaders (MPS), and Nvidia CUDA.
 
-   #### To install with no GPU acceleration and PyTorch without CUDA bindings
+   #### Install using PyTorch without CUDA bindings and no GPU acceleration
 
-   ```shell
-   python3 -m venv --upgrade-deps venv
-   source venv/bin/activate
-   (venv) $ pip cache remove llama_cpp_python
-   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable --extra-index-url=https://download.pytorch.org/whl/cpu
-   ```
-
-   #### To install with AMD ROCm
-
-   ```shell
-   python3 -m venv --upgrade-deps venv
-   source venv/bin/activate
-   (venv) $ pip cache remove llama_cpp_python
-   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable \
-       --extra-index-url https://download.pytorch.org/whl/rocm6.0 \
-       -C cmake.args="-DLLAMA_HIPBLAS=on" \
-       -C cmake.args="-DAMDGPU_TARGETS=all" \
-       -C cmake.args="-DCMAKE_C_COMPILER=/opt/rocm/llvm/bin/clang" \
-       -C cmake.args="-DCMAKE_CXX_COMPILER=/opt/rocm/llvm/bin/clang++" \
-       -C cmake.args="-DCMAKE_PREFIX_PATH=/opt/rocm"
-   ```
-
-   On Fedora 40+, use `-DCMAKE_C_COMPILER=clang-17` and `-DCMAKE_CXX_COMPILER=clang++-17`.
-
-   #### To install with Apple Metal on M1/M2/M3 Mac
-
-   ```shell
-   python3 -m venv --upgrade-deps venv
-   source venv/bin/activate
-   (venv) $ pip cache remove llama_cpp_python
-   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable -C cmake.args="-DLLAMA_METAL=on"
-   ```
-
-   #### To install with Nvidia CUDA
-
-   ```shell
-   python3 -m venv --upgrade-deps venv
-   source venv/bin/activate
-   (venv) $ pip cache remove llama_cpp_python
-   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable -C cmake.args="-DLLAMA_CUBLAS=on"
+      ```shell
+      python3 -m venv --upgrade-deps venv
+      source venv/bin/activate
+      (venv) $ pip cache remove llama_cpp_python
+      (venv) $ pip install instructlab --extra-index-url=https://download.pytorch.org/whl/cpu
+      ```
+
+      > **NOTE**: *Additional Build Argument for Intel Macs*
+      >
+      > If you have an Mac with an Intel CPU, you must add a prefix of
+      > `CMAKE_ARGS="-DLLAMA_METAL=off"` to the `pip install` command to ensure
+      > that the build is done without Apple M-series GPU support.
+      >
+      > `(venv) $ CMAKE_ARGS="-DLLAMA_METAL=off" pip install ...`
+
+   #### Install with AMD ROCm
+
+      ```shell
+      python3 -m venv --upgrade-deps venv
+      source venv/bin/activate
+      (venv) $ pip cache remove llama_cpp_python
+      (venv) $ pip install instructlab \
+         --extra-index-url https://download.pytorch.org/whl/rocm6.0 \
+         -C cmake.args="-DLLAMA_HIPBLAS=on" \
+         -C cmake.args="-DAMDGPU_TARGETS=all" \
+         -C cmake.args="-DCMAKE_C_COMPILER=/opt/rocm/llvm/bin/clang" \
+         -C cmake.args="-DCMAKE_CXX_COMPILER=/opt/rocm/llvm/bin/clang++" \
+         -C cmake.args="-DCMAKE_PREFIX_PATH=/opt/rocm"
+      ```
+
+      On Fedora 40+, use `-DCMAKE_C_COMPILER=clang-17` and `-DCMAKE_CXX_COMPILER=clang++-17`.
+
+   #### Install with Apple Metal on M1/M2/M3 Macs
+
+      ```shell
+      python3 -m venv --upgrade-deps venv
+      source venv/bin/activate
+      (venv) $ pip cache remove llama_cpp_python
+      (venv) $ pip install instructlab
+      ```
+
+   #### Install with Nvidia CUDA
+
+      ```shell
+      python3 -m venv --upgrade-deps venv
+      source venv/bin/activate
+      (venv) $ pip cache remove llama_cpp_python
+      (venv) $ pip install instructlab -C cmake.args="-DLLAMA_CUBLAS=on"
    ```
 
 4. From your `venv` environment, verify `ilab` is installed correctly, by running the `ilab` command.
 
    ```shell
    ilab
    ```
 
-   #### Example output
+   *Example output of the `ilab` command*
 
    ```shell
    (venv) $ ilab
    Usage: ilab [OPTIONS] COMMAND [ARGS]...
 
    CLI for interacting with InstructLab.
 
@@ -209,15 +210,15 @@
 
    > **IMPORTANT:** every `ilab` command needs to be run from within your Python virtual environment. To enter the Python environment, run the following command:
 
    ```shell
    source venv/bin/activate
    ```
 
-5. You may optionally enable tab completion for the `ilab` command.
+5. Optional: You can enable tab completion for the `ilab` command.
 
    #### Bash (version 4.4 or newer)
 
    Enable tab completion in `bash` with the following command:
 
    ```sh
    eval "$(_ILAB_COMPLETE=bash_source ilab)"
@@ -266,29 +267,29 @@
 
 1. Initialize `ilab` by running the following command:
 
    ```shell
    ilab init
    ```
 
-   #### Example output
+   *Example output*
 
    ```shell
    Welcome to InstructLab CLI. This guide will help you set up your environment.
    Please provide the following values to initiate the environment [press Enter for defaults]:
    Path to taxonomy repo [taxonomy]: <ENTER>
    ```
 
 2. When prompted by the interface, press **Enter** to add a new default `config.yaml` file.
 
 3. When prompted, clone the `https://github.com/instructlab/taxonomy.git` repository into the current directory by typing **y**.
 
    **Optional**: If you want to point to an existing local clone of the `taxonomy` repository, you can pass the path interactively or alternatively with the `--taxonomy-path` flag.
 
-   #### Example output
+   *Example output after initializing `ilab`*
 
    ```shell
    (venv) $ ilab init
    Welcome to InstructLab CLI. This guide will help you set up your environment.
    Please provide the following values to initiate the environment [press Enter for defaults]:
    Path to taxonomy repo [taxonomy]: <ENTER>
    `taxonomy` seems to not exists or is empty. Should I clone https://github.com/instructlab/taxonomy.git for you? [y/N]: y
@@ -307,21 +308,21 @@
    ```shell
    git clone --recurse-submodules https://github.com/instructlab/taxonomy.git
    git pull --recurse-submodules
    ```
 
 ### 📥 Download the model
 
-- Run the `ilab download`command.
+- Run the `ilab download` command.
 
   ```shell
   ilab download
   ```
 
-  `ilab download` will download a pre-trained [model](https://huggingface.co/instructlab/) (~4.4G) from HuggingFace and store it in a `models` directory:
+  `ilab download` downloads a compact pre-trained version of the [model](https://huggingface.co/instructlab/) (~4.4G) from HuggingFace and store it in a `models` directory:
 
   ```shell
   (venv) $ ilab download
   Downloading model from instructlab/merlinite-7b-lab-GGUF@main to models...
   (venv) $ ls models
   merlinite-7b-lab-Q4_K_M.gguf
   ```
@@ -409,15 +410,15 @@
 
    ```shell
    ilab generate
    ```
 
    > **NOTE:** ⏳ This can take from 15 minutes to 1+ hours to complete, depending on your computing resources.
 
-   #### Example output
+   *Example output of `ilab generate`*
 
    ```shell
    (venv) $ ilab generate
    INFO 2024-02-29 19:09:48,804 lab.py:250 Generating model 'ggml-merlinite-7b-lab-Q4_K_M' using 10 CPUs,
    taxonomy: '/home/username/instructlab/taxonomy' and seed 'seed_tasks.json'
 
    0%|##########| 0/100 Cannot find prompt.txt. Using default prompt.
@@ -442,19 +443,19 @@
    **Optional**: It is also possible to run the generate step against a different model via an
    OpenAI-compatible API. For example, the one spawned by `ilab serve` or any remote or locally hosted LLM (e.g. via [`ollama`](https://ollama.com/), [`LM Studio`](https://lmstudio.ai), etc.). Run the following command:
 
    ```shell
    ilab generate --endpoint-url http://localhost:8000/v1
    ```
 
-### 👩‍🏫 Train the model
+### 👩‍🏫 Training the model
 
-There are three options to train the model on your synthetic data-enhanced dataset.
+There are many options for training the model with your synthetic data-enhanced dataset.
 
-> **Note:** **Every** `ilab` command needs to be run from within your Python virtual environment.
+> **Note:** **Every** `ilab` command needs to run from within your Python virtual environment.
 
 #### Train the model locally on Linux
 
 ```shell
 ilab train
 ```
 
@@ -484,23 +485,23 @@
 (venv) $ ls instructlab-merlinite-7b-lab-mlx-q
 adapters-010.npz        adapters-050.npz        adapters-090.npz        config.json             tokenizer.model
 adapters-020.npz        adapters-060.npz        adapters-100.npz        model.safetensors       tokenizer_config.json
 adapters-030.npz        adapters-070.npz        adapters.npz            special_tokens_map.json
 adapters-040.npz        adapters-080.npz        added_tokens.json       tokenizer.jso
 ```
 
-#### Training the model locally with GPU acceleration
+#### Train the model locally with GPU acceleration
 
 Training has experimental support for GPU acceleration with Nvidia CUDA or AMD ROCm. Please see [the GPU acceleration documentation](./docs/gpu-acceleration.md) for more details. At present, hardware acceleration requires a data center GPU or high-end consumer GPU with at least 18 GB free memory.
 
 ```shell
 ilab train --device=cuda
 ```
 
-#### Training the model in the cloud
+#### Train the model in the cloud
 
 Follow the instructions in [Training](./notebooks/README.md).
 
 ⏳ Approximate amount of time taken on each platform:
 
 - *Google Colab*: **5-10 minutes** with a T4 GPU
 - *Kaggle*: **~30 minutes** with a P100 GPU.
@@ -536,20 +537,20 @@
    ilab convert
    ```
 
 3. Serve the newly trained model locally via `ilab serve` command with the `--model-path`
 argument to specify your new model:
 
    ```shell
-   ilab serve --model-path <New model name>
+   ilab serve --model-path <new model path>
    ```
 
-   Which model should you select to serve? After running the `ilab convert` command, a few files and directories are generated. The one you will want to serve will end in `.gguf`
-   and will exist in a directory with the suffix `fused-pt`. For example:
-   `instructlab-merlinite-7b-lab-mlx-q-fused-pt/ggml-model-Q4_K_M.gguf`
+   Which model should you select to serve? After running the `ilab convert` command, some files and a directory are generated. The model you will want to serve ends with an extension of `.gguf`
+   and exists in a directory with the suffix `trained`. For example:
+   `instructlab-merlinite-7b-lab-trained/instructlab-merlinite-7b-lab-Q4_K_M.gguf`.
 
 ## 📣 Chat with the new model (not optional this time)
 
 - Try the fine-tuned model out live using the chat interface, and see if the results are better than the untrained version of the model with chat by running the following command:
 
    ```shell
    ilab chat -m <New model name>
```

### Comparing `instructlab-0.15.1/TROUBLESHOOTING.md` & `instructlab-0.16.0/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/containers/bin/debug-llama` & `instructlab-0.16.0/containers/bin/debug-llama`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/containers/bin/debug-pytorch` & `instructlab-0.16.0/containers/bin/debug-pytorch`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/containers/cuda/Containerfile` & `instructlab-0.16.0/containers/cuda/Containerfile`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # SPDX-License-Identifier: Apache-2.0
 
-FROM nvcr.io/nvidia/cuda:12.3.2-devel-ubi9
-RUN dnf install -y python3.11 git python3-pip make automake gcc gcc-c++
+FROM nvcr.io/nvidia/cuda:12.4.1-devel-ubi9
+RUN dnf install -y python3.11 python3.11-devel git python3-pip make automake gcc gcc-c++
 WORKDIR /instructlab
 RUN python3.11 -m ensurepip
-RUN dnf install -y gcc
 RUN rpm -ivh https://dl.fedoraproject.org/pub/epel/epel-release-latest-9.noarch.rpm
 RUN dnf config-manager --add-repo https://developer.download.nvidia.com/compute/cuda/repos/rhel9/x86_64/cuda-rhel9.repo && dnf repolist && dnf config-manager --set-enabled cuda-rhel9-x86_64 && dnf config-manager --set-enabled cuda && dnf config-manager --set-enabled epel && dnf update -y
 RUN dnf install -y libcudnn8 nvidia-driver-NVML nvidia-driver-cuda-libs
 RUN python3.11 -m pip install --force-reinstall nvidia-cuda-nvcc-cu12
 RUN export LD_LIBRARY_PATH="$LD_LIBRARY_PATH:/usr/local/cuda/lib64:/usr/local/cuda/extras/CUPTI/lib64" \
     && export CUDA_HOME=/usr/local/cuda \
     && export PATH="/usr/local/cuda/bin:$PATH" \
     && export XLA_TARGET=cuda120 \
     && export XLA_FLAGS=--xla_gpu_cuda_data_dir=/usr/local/cuda
 
 ARG GIT_TAG=stable
-RUN CMAKE_ARGS="-DLLAMA_CUBLAS=on" CFLAGS="-mno-avx" python3.11 -m pip install -r https://raw.githubusercontent.com/instructlab/instructlab/${GIT_TAG}/requirements.txt --force-reinstall --no-cache-dir llama-cpp-python
+RUN if [[ "$(uname -m)" != "aarch64" ]]; then export CFLAGS="-mno-avx"; fi && \
+    CMAKE_ARGS="-DLLAMA_CUBLAS=on" python3.11 -m pip install -r https://raw.githubusercontent.com/instructlab/instructlab/${GIT_TAG}/requirements.txt --force-reinstall --no-cache-dir llama-cpp-python
 RUN python3.11 -m pip install git+https://github.com/instructlab/instructlab.git@${GIT_TAG}
 
 CMD ["/bin/bash"]
```

### Comparing `instructlab-0.15.1/containers/hpu/Containerfile` & `instructlab-0.16.0/containers/hpu/Containerfile`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/containers/rocm/Containerfile` & `instructlab-0.16.0/containers/rocm/Containerfile`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/containers/rocm/README.md` & `instructlab-0.16.0/containers/rocm/README.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/containers/rocm/gfx-version.sh` & `instructlab-0.16.0/containers/rocm/gfx-version.sh`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/containers/rocm/remove-gfx.sh` & `instructlab-0.16.0/containers/rocm/remove-gfx.sh`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/containers/sitecustomize.py` & `instructlab-0.16.0/containers/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/docs/README.md` & `instructlab-0.16.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/docs/ci.md` & `instructlab-0.16.0/docs/ci.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/docs/converting_GGUF.md` & `instructlab-0.16.0/docs/converting_GGUF.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/docs/demo-slides.md` & `instructlab-0.16.0/docs/demo-slides.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/docs/gpu-acceleration.md` & `instructlab-0.16.0/docs/gpu-acceleration.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/docs/habana-gaudi.md` & `instructlab-0.16.0/docs/habana-gaudi.md`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
 ```shell
 ./habanalabs-installer.sh validate
 ```
 
 ## Habana Lab's PyTorch stack
 
-Habana Labs comes with a modified fork of PyTorch that is build with Intel's oneAPI Math Kernel Library (oneMKL). The actual HPU bindings and helpers are provided by the the `habana_framework` package. Imports of `habana_framework` sub-packages register `hpu` device support, `torch.hpu` module, and `dynamo` backends.
+Habana Labs comes with a modified fork of PyTorch that is build with Intel's oneAPI Math Kernel Library (oneMKL). The actual HPU bindings and helpers are provided by the `habana_framework` package. Imports of `habana_framework` sub-packages register `hpu` device support, `torch.hpu` module, and `dynamo` backends.
 
 The [`SFTTrainer`](https://huggingface.co/docs/trl/sft_trainer) from `trl` does not work with Habana stack. Instead the `GaudiSFTTrainer` from [optimum-habana](https://huggingface.co/docs/optimum/habana/index) is needed. The version on PyPI is currently broken, but the HabanaAI [optimum-habana-fork](https://github.com/HabanaAI/optimum-habana-fork) works.
 
 ## Install and run InstructLab with Intel Gaudi
 
 Install `InstructLab` from checkout with additional dependencies:
```

### Comparing `instructlab-0.15.1/docs/workflow.png` & `instructlab-0.16.0/docs/workflow.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/docs/workflow.puml` & `instructlab-0.16.0/docs/workflow.puml`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/notebooks/README.md` & `instructlab-0.16.0/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/notebooks/Training_a_LoRA_With_Instruct_Lab.ipynb` & `instructlab-0.16.0/notebooks/Training_a_LoRA_With_Instruct_Lab.ipynb`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/notebooks/images/collab-copy-path.png` & `instructlab-0.16.0/notebooks/images/collab-copy-path.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/notebooks/images/collab-file-upload-button.png` & `instructlab-0.16.0/notebooks/images/collab-file-upload-button.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/notebooks/images/collab-folder-icon.png` & `instructlab-0.16.0/notebooks/images/collab-folder-icon.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/notebooks/images/kaggle/clear-outputs.png` & `instructlab-0.16.0/notebooks/images/kaggle/clear-outputs.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/notebooks/images/kaggle/copy-file-path.png` & `instructlab-0.16.0/notebooks/images/kaggle/copy-file-path.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/notebooks/images/kaggle/create-new-nb.png` & `instructlab-0.16.0/notebooks/images/kaggle/create-new-nb.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/notebooks/images/kaggle/create.png` & `instructlab-0.16.0/notebooks/images/kaggle/create.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/notebooks/images/kaggle/file-click.png` & `instructlab-0.16.0/notebooks/images/kaggle/file-click.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/notebooks/images/kaggle/import-nb.png` & `instructlab-0.16.0/notebooks/images/kaggle/import-nb.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/notebooks/images/kaggle/input-drop-files.png` & `instructlab-0.16.0/notebooks/images/kaggle/input-drop-files.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/notebooks/images/kaggle/input-upload.png` & `instructlab-0.16.0/notebooks/images/kaggle/input-upload.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/notebooks/images/kaggle/input.png` & `instructlab-0.16.0/notebooks/images/kaggle/input.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/notebooks/images/kaggle/new-dataset.png` & `instructlab-0.16.0/notebooks/images/kaggle/new-dataset.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/notebooks/images/kaggle/select-accelerator-p100.png` & `instructlab-0.16.0/notebooks/images/kaggle/select-accelerator-p100.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/notebooks/images/kaggle/select-accelerator.png` & `instructlab-0.16.0/notebooks/images/kaggle/select-accelerator.png`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/pyproject.toml` & `instructlab-0.16.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 dependencies = {file = ["requirements.txt"]}
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["instructlab", "instructlab.chat", "instructlab.generator", "instructlab.train", "instructlab.train.lora_mlx", "instructlab.train.lora_mlx.models", "instructlab.llamacpp", "instructlab.mlx_explore", "instructlab.schema.v1", "instructlab.schema.v2"]
 
 [tool.setuptools.package-data]
-"instructlab.llamacpp" = ["quantize"]
 "instructlab.schema.v1" = ["*.json"]
 "instructlab.schema.v2" = ["*.json"]
 
 [tool.check-wheel-contents]
 # W002 - Wheel contains duplicate files:
 #  instructlab/mlx_explore/LICENSE
 #  instructlab/train/lora_mlx/LICENSE
```

### Comparing `instructlab-0.15.1/requirements-hpu.txt` & `instructlab-0.16.0/requirements-hpu.txt`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/requirements.txt` & `instructlab-0.16.0/requirements.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 datasets>=2.18.0,<3.0.0
 gguf>=0.6.0,<0.7.0
 GitPython>=3.1.42,<4.0.0
 # Linux: 4-bit quantization with BitsAndBytes is not ready to use, yet.
 # see https://github.com/instructlab/instructlab/issues/579
 # bitsandbytes; sys_platform=='linux' and platform_machine=='x86_64'
 httpx>=0.25.0,<1.0.0
+instructlab-quantize>=0.1.0
 jsonschema>=4.21.1,<5.0.0
 llama_cpp_python[server]==0.2.75
 mlx>=0.5.1,<0.6.0; sys_platform == 'darwin' and platform_machine == 'arm64'
 # HabanaLabs / Intel Gaudi env comes with Python 3.10 and slightly older
 # versions of some dependencies. Use '3.10' as an indicator.
 # Habana installer has NumPy 1.23.5
 numpy>=1.23.5,<2.0.0 ; python_version == '3.10'
```

### Comparing `instructlab-0.15.1/scripts/basic-workflow-tests.sh` & `instructlab-0.16.0/scripts/basic-workflow-tests.sh`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 test_smoke() {
     task Smoke test InstructLab
     ilab | grep --color 'Usage: ilab'
 }
 
 test_init() {
     task Initializing ilab
-    [ -f config.yaml ] || printf "taxonomy\ny" | ilab init
+    [ -f config.yaml ] || ilab init --non-interactive
 
     step Checking config.yaml
     cat config.yaml | grep merlinite
 }
 
 test_download() {
     task Download the model
```

### Comparing `instructlab-0.15.1/scripts/functional-tests.sh` & `instructlab-0.16.0/scripts/functional-tests.sh`

 * *Files 3% similar despite different names*

```diff
@@ -36,28 +36,31 @@
     done
     rm -f "$TEST_CTX_SIZE_LAB_SERVE_LOG_FILE" \
         "$TEST_CTX_SIZE_LAB_CHAT_LOG_FILE" \
         test_session_history
     rm -rf test_taxonomy
     # revert port change from test_bind_port()
     sed -i.bak 's/9999/8000/g' config.yaml
-    rm -f config.yaml.bak
     # revert model name change from test_model_print()
     sed -i.bak "s/baz/merlinite-7b-lab-Q4_K_M/g" config.yaml
-    mv models/foo.gguf models/merlinite-7b-lab-Q4_K_M.gguf
+    mv models/foo.gguf models/merlinite-7b-lab-Q4_K_M.gguf || true
+    rm -f config.yaml.bak
     set -e
 }
 
 trap 'cleanup "$?"' EXIT QUIT INT TERM
 
 rm -f config.yaml
 
 # print version
 ilab --version
 
+# print system information
+ilab sysinfo
+
 # pipe 3 carriage returns to ilab init to get past the prompts
 echo -e "\n\n\n" | ilab init
 
 # Enable Debug in func tests
 sed -i.bak -e 's/log_level:.*/log_level: DEBUG/g;' config.yaml
 
 # It looks like GitHub action MacOS runner does not have graphics
@@ -289,15 +292,22 @@
         send "hello!\r"
         sleep 5
         send "\003"
         expect {
             "Disconnected from client (via refresh/close)" { exit 1 }
         }
         send "exit\r"
-        expect eof
+        expect {
+            "Traceback (most recent call last):" { set exp_result 1 }
+            default { set exp_result 0 }
+        }
+        if { $exp_result != 0 } {
+            puts stderr "Error: ilab chat command failed"
+            exit 1
+        }
     '
 }
 
 test_server_welcome_message(){
     # test that the server welcome message is displayed
     ilab serve &
     PID_SERVE=$!
@@ -330,36 +340,20 @@
         expect {
             -re "Welcome to InstructLab Chat w/ \\\u001b\\\[1mMODELS/FOO\\.GGUF" { exit 0 }
             eof { catch wait result; exit [lindex $result 3] }
             timeout { exit 1 }
         }
     '
 
-    # validate that we print the model from the CLI
+    # validate that we fail on invalid model
     expect -c '
         set timeout 30
         spawn ilab chat -m bar
         expect {
-            -re "Welcome to InstructLab Chat w/ \\\u001b\\\[1mBAR\\\u001b\\\[0m" { exit 0 }
-            eof { catch wait result; exit [lindex $result 3] }
-            timeout { exit 1 }
-        }
-    '
-
-    # validate that we print the model from the config
-    expect -c '
-        exec sed -i.bak "s/merlinite-7b-lab-Q4_K_M/baz/g" config.yaml
-        spawn ilab chat
-        expect {
-            -re "Welcome to InstructLab Chat w/ \\\u001b\\\[1mBAZ\\\u001b\\\[0m" {
-                exec sed -i.bak "s/baz/merlinite-7b-lab-Q4_K_M/g" config.yaml
-                exit 0
-            }
-            eof { catch wait result; exit [lindex $result 3] }
-            timeout { exit 1 }
+           "Executing chat failed with: Model bar is not served by the server. These are the served models: ['models/foo.gguf']" { exit 0 }
         }
     '
 
     # If we don't specify a model, validate that we print the model reported
     # by the server since it is different from the config.
     expect -c '
         spawn ilab chat
```

### Comparing `instructlab-0.15.1/scripts/ruff.sh` & `instructlab-0.16.0/scripts/ruff.sh`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/scripts/test-data/basic-workflow-fixture-qna.yaml` & `instructlab-0.16.0/scripts/test-data/basic-workflow-fixture-qna.yaml`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/chat/chat.py` & `instructlab-0.16.0/src/instructlab/chat/chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from rich.markdown import Markdown
 from rich.panel import Panel
 from rich.text import Text
 import httpx
 import openai
 
 # Local
-from ..config import DEFAULT_API_KEY, DEFAULT_CONNECTION_TIMEOUT
+from ..config import DEFAULT_CONNECTION_TIMEOUT, DEFAULT_MODEL_OLD
 from ..utils import get_sysprompt
 
 HELP_MD = """
 Help / TL;DR
 - `/q`: **q**uit
 - `/h`: show **h**elp
 - `/a assistant`: **a**mend **a**ssistant (i.e., model)
@@ -68,15 +68,15 @@
     def __init__(
         self,
         model,
         client,
         vi_mode=False,
         prompt=True,
         vertical_overflow="ellipsis",
-        loaded={},
+        loaded=None,
         log_file=None,
         greedy_mode=False,
         max_tokens=None,
     ):
         self.client = client
         self.model = model
         self.vi_mode = vi_mode
@@ -108,18 +108,18 @@
         )
 
     def _sys_print(self, *args, **kwargs):
         self.console.print(Panel(*args, title="system", **kwargs))
 
     def log_message(self, msg):
         if self.log_file:
-            with open(self.log_file, "a") as fp:
+            with open(self.log_file, "a", encoding="utf-8") as fp:
                 fp.write(msg)
 
-    def greet(self, help=False, new=False, session_name="new session"):
+    def greet(self, help=False, new=False, session_name="new session"):  # pylint: disable=redefined-builtin
         side_info_str = (" (type `/h` for help)" if help else "") + (
             f" ({session_name})" if new else ""
         )
         self._sys_print(
             Markdown(
                 f"Welcome to InstructLab Chat w/ **{self.model.upper()}**"
                 + side_info_str
@@ -140,18 +140,18 @@
                     else []
                 ),  # loaded context/session file
                 # TODO: Fix openai package to fix the openai error.
                 # *([] if openai.proxy is None else [('#d08770 bold', "[proxied]")]), # indicate prox
             ]
         )
 
-    def _handle_quit(self, content):
+    def _handle_quit(self, _):
         raise ChatQuitException
 
-    def _handle_help(self, content):
+    def _handle_help(self, _):
         self._sys_print(Markdown(HELP_MD))
         raise KeyboardInterrupt
 
     def _handle_multiline(self, content):
         temp = content == "/m"  # soft multiline only for next prompt
         self.multiline = not self.multiline
         self.multiline_mode = 1 if not temp else 2
@@ -203,37 +203,37 @@
 
     def _handle_new_session(self, content):
         hard = content == "/N"  # hard new ignores loaded context/session
         self._reset_session(hard=hard)
         self.greet(new=True)
         raise KeyboardInterrupt
 
-    def __handle_replay(self, content, display_wrapper=(lambda x: x)):
+    def __handle_replay(self, content, display_wrapper=lambda x: x):
         # if the history is empty, then return
         if (
             len(self.info["messages"]) == 1
             and self.info["messages"][0]["role"] == "system"
         ):
             raise KeyboardInterrupt
         cs = content.split()
         try:
             i = 1 if len(cs) == 1 else int(cs[1]) * 2 - 1
             if abs(i) >= len(self.info["messages"]):
                 raise IndexError
-        except (IndexError, ValueError):
+        except (IndexError, ValueError) as exc:
             self.console.print(
                 display_wrapper("Invalid index: " + content), style="bold red"
             )
-            raise KeyboardInterrupt
+            raise KeyboardInterrupt from exc
         if len(self.info["messages"]) > abs(i):
             self.console.print(display_wrapper(self.info["messages"][-i]["content"]))
         raise KeyboardInterrupt
 
     def _handle_display(self, content):
-        return self.__handle_replay(content, display_wrapper=(lambda x: Panel(x)))
+        return self.__handle_replay(content, display_wrapper=lambda x: Panel(x))  # pylint: disable=unnecessary-lambda
 
     def _load_session_history(self, content=None):
         data = self.info["messages"]
         if content is not None:
             data = content["messages"]
         for m in data:
             if m["role"] == "user":
@@ -262,15 +262,15 @@
             self._sys_print(
                 Markdown(
                     "**WARNING**: The second argument `filepath` is missing in the `/s filepath` command."
                 )
             )
             raise KeyboardInterrupt
         filepath = cs[1]
-        with open(filepath, "w") as outfile:
+        with open(filepath, "w", encoding="utf-8") as outfile:
             json.dump(self.info["messages"], outfile, indent=4)
         raise KeyboardInterrupt
 
     def _handle_load_session(self, content):
         cs = content.split()
         if len(cs) < 2:
             self._sys_print(
@@ -283,15 +283,15 @@
         if not os.path.exists(filepath):
             self._sys_print(
                 Markdown(
                     f"**WARNING**: File `{filepath}` specified in the `/l filepath` or `/L filepath` command does not exist."
                 )
             )
             raise KeyboardInterrupt
-        with open(filepath, "r") as session:
+        with open(filepath, "r", encoding="utf-8") as session:
             messages = json.loads(session.read())
         if content[:2] == "/L":
             self.loaded["name"] = filepath
             self.loaded["messages"] = messages
             self._reset_session()
             self.greet(new=True)
         else:
@@ -406,41 +406,41 @@
             raise ChatException("API Key Error") from e
         except openai.RateLimitError as e:
             self.console.print(
                 "Rate limit or maximum monthly limit exceeded", style="bold red"
             )
             self.info["messages"].pop()
             raise ChatException("Rate limit exceeded") from e
-        except openai.APIConnectionError:
+        except openai.APIConnectionError as e:
             self.console.print("Connection error, try again...", style="red bold")
             self.info["messages"].pop()
-            raise KeyboardInterrupt
+            raise KeyboardInterrupt from e
         except KeyboardInterrupt as e:
             raise e
         except httpx.RemoteProtocolError as e:
             self.console.print("Connection to the server was closed", style="bold red")
             self.info["messages"].pop()
             raise ChatException("Connection to the server was closed") from e
-        except:
+        except Exception as e:
             self.console.print("Unknown error", style="bold red")
-            raise ChatException(f"Unknown error: {sys.exc_info()[0]}")
+            raise ChatException(f"Unknown error: {sys.exc_info()[0]}") from e
 
         response_content = Text()
         panel = (
             Panel(response_content, title=self.model, subtitle_align="right")
             if box
             else response_content
         )
         subtitle = None
         with Live(
             panel,
             console=self.console,
             refresh_per_second=5,
             vertical_overflow=self.vertical_overflow,
-        ) as live:
+        ):
             start_time = time.time()
             for chunk in response:
                 chunk_message = chunk.choices[0].delta
                 if chunk_message.content:
                     response_content.append(chunk_message.content)
 
                 if box:
@@ -478,14 +478,27 @@
     verify = not tls_insecure
     client = OpenAI(
         base_url=api_base,
         api_key=api_key,
         timeout=DEFAULT_CONNECTION_TIMEOUT,
         http_client=httpx.Client(cert=cert, verify=verify),
     )
+    # ensure the model specified exists on the server. with backends like vllm, this is crucial.
+    model_list = client.models.list().data
+    model_ids = []
+    for m in model_list:
+        model_ids.append(m.id)
+    if not any(model == m for m in model_ids):
+        if model == DEFAULT_MODEL_OLD:
+            logger.info(
+                f"Model {model} is not a full path. Try running ilab init or edit your config to have the full model path for serving, chatting, and generation."
+            )
+        raise ChatException(
+            f"Model {model} is not served by the server. These are the served models: {model_ids}"
+        )
 
     # Load context/session
     loaded = {}
 
     # Context config file
     # global CONTEXTS
     # CONTEXTS = config["contexts"]
@@ -496,18 +509,18 @@
     loaded["messages"] = [{"role": "system", "content": CONTEXTS[context]}]
 
     # Session from CLI
     if session is not None:
         loaded["name"] = os.path.basename(session.name).strip(".json")
         try:
             loaded["messages"] = json.loads(session.read())
-        except json.JSONDecodeError:
+        except json.JSONDecodeError as exc:
             raise ChatException(
                 f"Session file {session.name} is not a valid JSON file."
-            )
+            ) from exc
 
     log_file = None
     if config.logs_dir:
         date_suffix = (
             datetime.datetime.now().replace(microsecond=0).isoformat().replace(":", "_")
         )
         os.makedirs(config.logs_dir, exist_ok=True)
@@ -534,17 +547,17 @@
 
     # Use the input question to start with
     if len(question) > 0:
         question = " ".join(question)
         if not qq:
             print(f"{PROMPT_PREFIX}{question}")
         try:
-            ccb.start_prompt(logger, content=question, box=(not qq))
+            ccb.start_prompt(logger, content=question, box=not qq)
         except ChatException as exc:
-            raise ChatException(f"API issue found while executing chat: {exc}")
+            raise ChatException(f"API issue found while executing chat: {exc}") from exc
         except (ChatQuitException, KeyboardInterrupt, EOFError):
             return
 
     if qq:
         return
 
     # load the history
@@ -554,12 +567,12 @@
     # Start chatting
     while True:
         try:
             ccb.start_prompt(logger)
         except KeyboardInterrupt:
             continue
         except ChatException as exc:
-            raise ChatException(f"API issue found while executing chat: {exc}")
-        except httpx.RemoteProtocolError:
-            raise ChatException(f"Connection to the server was closed")
+            raise ChatException(f"API issue found while executing chat: {exc}") from exc
+        except httpx.RemoteProtocolError as exc:
+            raise ChatException("Connection to the server was closed") from exc
         except (ChatQuitException, EOFError):
             return
```

### Comparing `instructlab-0.15.1/src/instructlab/client.py` & `instructlab-0.16.0/src/instructlab/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # SPDX-License-Identifier: Apache-2.0
+# pylint: disable=duplicate-code
 
 # Standard
 from typing import Optional
 
 # Third Party
 from openai import OpenAI, OpenAIError
 import httpx
```

### Comparing `instructlab-0.15.1/src/instructlab/config.py` & `instructlab-0.16.0/src/instructlab/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # SPDX-License-Identifier: Apache-2.0
 
 # Standard
+from os import path
+from re import match
 from typing import Optional
 
 # Third Party
 from pydantic import (
     BaseModel,
     ConfigDict,
     PositiveInt,
@@ -13,16 +15,18 @@
     field_validator,
 )
 import httpx
 import yaml
 
 DEFAULT_API_KEY = "no_api_key"
 DEFAULT_CONFIG = "config.yaml"
-DEFAULT_MODEL = "merlinite-7b-lab-Q4_K_M"
-DEFAULT_MODEL_PATH = f"models/{DEFAULT_MODEL}.gguf"
+# TODO: Consolidate --model and --model-path into one --model-path flag since we always need a path now
+DEFAULT_MODEL_OLD = "merlinite-7b-lab-Q4_K_M"
+DEFAULT_MODEL = "models/merlinite-7b-lab-Q4_K_M.gguf"
+DEFAULT_MODEL_PATH = "models/merlinite-7b-lab-Q4_K_M.gguf"
 DEFAULT_TAXONOMY_REPO = "https://github.com/instructlab/taxonomy.git"
 DEFAULT_TAXONOMY_PATH = "taxonomy"
 DEFAULT_TAXONOMY_BASE = "origin/main"
 DEFAULT_YAML_RULES = "yaml_rules.yaml"
 MAX_CONTEXT_SIZE = 4096
 # TODO: these constants should be removed, they should not leak out
 DEFAULT_NUM_CPUS = 10
@@ -186,7 +190,11 @@
     with open(config_file, "w", encoding="utf-8") as yamlfile:
         yaml.safe_dump(get_dict(cfg), stream=yamlfile)
 
 
 def get_api_base(host_port):
     """Returns server API URL, based on the provided host_port"""
     return f"http://{host_port}/v1"
+
+
+def get_model_family(forced, model_path):
+    return forced if forced else match(r"^\w*", path.basename(model_path)).group(0)
```

### Comparing `instructlab-0.15.1/src/instructlab/generator/README.md` & `instructlab-0.16.0/src/instructlab/generator/README.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/generator/generate_data.py` & `instructlab-0.16.0/src/instructlab/generator/generate_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,21 @@
 # Third Party
 from jinja2 import Template
 from rouge_score import rouge_scorer
 import click
 import tqdm
 
 # Local
-from ..config import DEFAULT_MULTIPROCESSING_START_METHOD
-from ..utils import chunk_document, read_taxonomy
+from ..config import DEFAULT_MULTIPROCESSING_START_METHOD, get_model_family
+from ..utils import (
+    chunk_document,
+    max_seed_example_tokens,
+    num_chars_from_tokens,
+    read_taxonomy,
+)
 from . import utils
 from .utils import GenerateException
 
 DEFAULT_PROMPT_TEMPLATE_MERLINITE = """\
 You are asked to come up with a set of 5 diverse task instructions under {{taxonomy}}{{" for the task \\"%s\\""|format(task_description)  if task_description}}. These task instructions will be given to a GPT model and we will evaluate the GPT model for completing the instructions.
 
 Here are the requirements:
@@ -294,26 +299,43 @@
         # Hard-coded to maximize length.
         # Requests will be automatically adjusted.
         max_tokens=3072,
         top_p=top_p,
         stop=["* Task 5"],
     )
     request_start = time.time()
-    results = utils.openai_completion(
-        api_base=api_base,
-        api_key=api_key,
-        prompts=batch_inputs,
-        model_name=model_name,
-        tls_insecure=tls_insecure,
-        tls_client_cert=tls_client_cert,
-        tls_client_key=tls_client_key,
-        tls_client_passwd=tls_client_passwd,
-        batch_size=request_batch_size,
-        decoding_args=decoding_args,
-    )
+    try:
+        results = utils.openai_completion(
+            api_base=api_base,
+            api_key=api_key,
+            prompts=batch_inputs,
+            model_name=model_name,
+            tls_insecure=tls_insecure,
+            tls_client_cert=tls_client_cert,
+            tls_client_key=tls_client_key,
+            tls_client_passwd=tls_client_passwd,
+            batch_size=request_batch_size,
+            decoding_args=decoding_args,
+        )
+    except GenerateException as exc:
+        # Attempt to log and gracefully recover from exceeding the server's
+        # maximum context length. This won't work for all servers.
+        #
+        # Both llama_cpp_python and vllm use this exact string in their error
+        # responses when exceeding the model's max content length. Other
+        # OpenAI-compatible servers may as well, but no guarantees.
+        if "model's maximum context length" in str(exc):
+            logger.warn(
+                "Generated prompt exceeded the server's maximum context length. "
+                "If you see this warning many times during generation, lower "
+                "the length of your example question and answers or raise the "
+                "server's maximum context size using `max_ctx_size`."
+            )
+            return [], 0
+        raise exc
     request_duration = time.time() - request_start
 
     post_process_start = time.time()
     instruction_data = []
     for result in results:
         new_instructions, discarded = post_process_gpt3_response(
             num_prompt_instructions, result, output_file_discarded
@@ -358,14 +380,15 @@
     chunk_word_count=None,
     server_ctx_size=None,
     tls_client_cert: Optional[str] = None,
     tls_client_key: Optional[str] = None,
     tls_client_passwd: Optional[str] = None,
 ):
     seed_instruction_data = []
+    machine_seed_instruction_data = []
     generate_start = time.time()
 
     if not os.path.exists(output_dir):
         os.mkdir(output_dir)
 
     # check taxonomy first then seed_tasks_path
     # throw an error if both not found
@@ -373,14 +396,30 @@
     if taxonomy and os.path.exists(taxonomy):
         seed_instruction_data = read_taxonomy(
             logger, taxonomy, taxonomy_base, yaml_rules
         )
     else:
         raise SystemExit(f"Error: taxonomy ({taxonomy}) does not exist.")
 
+    prompt_template = check_prompt_file(
+        prompt_file_path, get_model_family(model_family, model_name)
+    )
+    max_seed_tokens = max_seed_example_tokens(server_ctx_size, len(prompt_template))
+    max_seed_chars = num_chars_from_tokens(max_seed_tokens)
+    for seed_example in seed_instruction_data:
+        if (
+            len(seed_example["instruction"])
+            + len(seed_example["input"])
+            + len(seed_example["output"])
+            >= max_seed_chars
+        ):
+            raise SystemExit(
+                f"Error: An example in the taxonomy path {seed_example['taxonomy_path']} is too long for the server context size of {server_ctx_size}. Ensure the total number of characters across the combined question, answer, and context is less than {max_seed_chars} for each example or use a server with a larger context size."
+            )
+
     seeds = len(seed_instruction_data)
     logger.debug(f"Loaded {seeds} human-written seed instructions from {taxonomy}")
     if not seeds:
         raise SystemExit("Nothing to generate. Exiting.")
 
     def unescape(s):
         return bytes(s, "utf-8").decode("utf-8")
@@ -445,15 +484,14 @@
     all_instructions = [d["instruction"] for d in seed_instruction_data] + [
         d["instruction"] for d in machine_instruction_data
     ]
     all_instruction_tokens = [
         scorer._tokenizer.tokenize(inst) for inst in all_instructions
     ]
 
-    prompt_template = check_prompt_file(prompt_file_path, model_family)
     if console_output:
         print(
             "Synthesizing new instructions. If you aren't satisfied with the generated instructions, interrupt training (Ctrl-C) and try adjusting your YAML files. Adding more examples may help."
         )
 
     mpctx = multiprocessing.get_context(DEFAULT_MULTIPROCESSING_START_METHOD)
 
@@ -465,15 +503,15 @@
 
         # Pick taxonomy path
         selected_taxonomy = all_taxonomy_paths[request_idx % len(all_taxonomy_paths)]
         logger.info(f"Selected taxonomy path {selected_taxonomy}")
         # Filter the pool
         instruction_data_pool = [
             e
-            for e in seed_instruction_data + machine_instruction_data
+            for e in seed_instruction_data + machine_seed_instruction_data
             if e["taxonomy_path"] == selected_taxonomy
         ]
         instruction_data, discarded = get_instructions_from_model(
             logger,
             request_idx,
             instruction_data_pool,
             prompt_template,
@@ -514,14 +552,19 @@
             if max(rouge_scores) > rouge_threshold:
                 total_rouged += 1
                 continue
             keep += 1
             # Comment out extra info not currently being used:
             # instruction_data_entry["most_similar_instructions"] = most_similar_instructions
             # instruction_data_entry["avg_similarity_score"] = float(np.mean(rouge_scores))
+
+            # Only add sufficiently small instructions to our machine seeds
+            if len(new_instruction_tokens) <= max_seed_tokens:
+                machine_seed_instruction_data.append(instruction_data_entry)
+
             machine_instruction_data.append(instruction_data_entry)
             all_instructions.append(instruction_data_entry["instruction"])
             all_instruction_tokens.append(new_instruction_tokens)
             if console_output:
                 print(
                     f"Q> {instruction_data_entry['instruction']}\nI> {instruction_data_entry['input']}\nA> {instruction_data_entry['output']}\n"
                 )
```

### Comparing `instructlab-0.15.1/src/instructlab/generator/seed_tasks.jsonl` & `instructlab-0.16.0/src/instructlab/generator/seed_tasks.jsonl`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/generator/utils.py` & `instructlab-0.16.0/src/instructlab/generator/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import sys
 
 # Third Party
 from openai import OpenAI, OpenAIError
 import httpx
 
 # Local
-from ..config import DEFAULT_API_KEY
+from ..config import DEFAULT_API_KEY, DEFAULT_MODEL_OLD
 from ..utils import get_sysprompt
 
 StrOrOpenAIObject = Union[str, object]
 
 
 class GenerateException(Exception):
     """An exception raised during generate step."""
@@ -129,14 +129,29 @@
         verify = not tls_insecure
         client = OpenAI(
             base_url=api_base,
             api_key=api_key,
             http_client=httpx.Client(cert=cert, verify=verify),
         )
 
+        # ensure the model specified exists on the server. with backends like vllm, this is crucial.
+        model_list = client.models.list().data
+        model_ids = []
+        for model in model_list:
+            model_ids.append(model.id)
+        if not any(model_name == m for m in model_ids):
+            if model_name == DEFAULT_MODEL_OLD:
+                logging.info(
+                    "Model %s is not a full path. Try running ilab init or edit your config to have the full model path for serving, chatting, and generation.",
+                    model_name,
+                )
+            raise GenerateException(
+                f"Model {model_name} is not served by the server. These are the served models {model_ids}"
+            )
+
         messages = [
             {"role": "system", "content": get_sysprompt()},
             {"role": "user", "content": prompt_batch[batch_id]},
         ]
 
         # Inference the model
         try:
```

### Comparing `instructlab-0.15.1/src/instructlab/lab.py` & `instructlab-0.16.0/src/instructlab/lab.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-License-Identifier: Apache-2.0
 
 # pylint: disable=too-many-lines
 
 # Standard
 from glob import glob
-from os.path import basename, dirname, exists, splitext
+from os.path import basename, dirname, exists
 import json
 import logging
 import multiprocessing
 import os
 import shutil
 import sys
 import typing
@@ -20,15 +20,16 @@
 from huggingface_hub import logging as hf_logging
 from huggingface_hub import snapshot_download
 import click
 import yaml
 
 # Local
 # NOTE: Subcommands are using local imports to speed up startup time.
-from . import config, utils
+from . import config, log, utils
+from .sysinfo import get_sysinfo
 
 # 'fork' is unsafe and incompatible with some hardware accelerators.
 # Python 3.14 will switch to 'spawn' on all platforms.
 multiprocessing.set_start_method(
     config.DEFAULT_MULTIPROCESSING_START_METHOD, force=True
 )
 
@@ -42,17 +43,30 @@
 
 
 class Lab:
     """Lab object holds high-level information about ilab CLI"""
 
     def __init__(self, config_obj: config.Config):
         self.config = config_obj
-        FORMAT = "%(levelname)s %(asctime)s %(filename)s:%(lineno)d %(message)s"
-        logging.basicConfig(format=FORMAT)
+
+        # Set up logging for the Lab class
         self.logger = logging.getLogger(__name__)
+
+        # Create a formatter
+        formatter = log.CustomFormatter(log.FORMAT)
+
+        # Create a handler and set the formatter
+        handler = logging.StreamHandler()
+        handler.setFormatter(formatter)
+
+        logging.basicConfig(
+            format=log.FORMAT,
+            handlers=[handler],
+        )
+
         self.logger.setLevel(self.config.general.log_level.upper())
 
 
 @click.group(cls=DYMGroup)
 @click.option(
     "--config",
     "config_file",
@@ -65,18 +79,21 @@
 @click.pass_context
 # pylint: disable=redefined-outer-name
 def cli(ctx, config_file):
     """CLI for interacting with InstructLab.
 
     If this is your first time running InstructLab, it's best to start with `ilab init` to create the environment.
     """
-    # ilab init or "--help" have no config file
+    # ilab init or "--help" have no config file. ilab sysinfo does not need one.
     # CliRunner does fill ctx.invoke_subcommand in option callbacks. We have
     # to validate config_file here.
-    if ctx.invoked_subcommand != "init" and "--help" not in sys.argv[1:]:
+    if (
+        ctx.invoked_subcommand not in {"init", "sysinfo"}
+        and "--help" not in sys.argv[1:]
+    ):
         if config_file == "DEFAULT":
             config_obj = config.get_default_config()
         elif not os.path.isfile(config_file):
             config_obj = None
             ctx.fail(
                 f"`{config_file}` does not exists, please run `ilab init` "
                 "or point to a valid configuration file using `--config=<path>`."
@@ -194,17 +211,16 @@
     models_dir = dirname(model_path)
     if interactive and exists(models_dir):
         model_path = utils.expand_path(
             click.prompt("Path to your model", default=model_path)
         )
     click.echo(f"Generating `{config.DEFAULT_CONFIG}` in the current directory...")
     cfg = config.get_default_config()
-    model = splitext(basename(model_path))[0]
-    cfg.chat.model = model
-    cfg.generate.model = model
+    cfg.chat.model = model_path
+    cfg.generate.model = model_path
     cfg.serve.model_path = model_path
     cfg.generate.taxonomy_path = taxonomy_path
     cfg.generate.taxonomy_base = taxonomy_base
     config.write_config(cfg)
 
     click.echo(
         "Initialization completed successfully, you're ready to start using `ilab`. Enjoy!"
@@ -287,14 +303,16 @@
 utils.make_lab_diff_aliases(cli, diff)
 
 
 @cli.command()
 @click.option(
     "--model-path",
     type=click.Path(),
+    default=config.DEFAULT_MODEL_PATH,
+    show_default=True,
     help="Path to the model used during generation.",
 )
 @click.option(
     "--gpu-layers",
     type=click.INT,
     help="The number of layers to put on the GPU. The rest will be on the CPU. Defaults to -1 to move all to GPU.",
 )
@@ -303,24 +321,26 @@
     "--max-ctx-size",
     type=click.INT,
     help="The context size is the maximum number of tokens considered by the model, for both the prompt and response. Defaults to 4096.",
 )
 @click.option(
     "--model-family",
     type=str,
-    default="merlinite",
-    help="Model family is used to specify which chat template to serve with",
+    help="Force model family to specify which chat template to serve with",
 )
 @click.pass_context
 def serve(ctx, model_path, gpu_layers, num_threads, max_ctx_size, model_family):
     """Start a local server"""
     # pylint: disable=C0415
     # Local
     from .server import ServerException, server
 
+    # Redirect server stdout and stderr to the logger
+    log.stdout_stderr_to_logger(ctx.obj.logger)
+
     ctx.obj.logger.info(
         f"Using model '{model_path}' with {gpu_layers} gpu-layers and {max_ctx_size} max context size."
     )
 
     try:
         host = ctx.obj.config.serve.host_port.split(":")[0]
         port = int(ctx.obj.config.serve.host_port.split(":")[1])
@@ -445,16 +465,15 @@
     "--tls-client-passwd",
     type=click.STRING,
     default="",
     help="TLS client certificate password.",
 )
 @click.option(
     "--model-family",
-    default="merlinite",
-    help="model family to use when picking a generation template",
+    help="Force model family to use when picking a generation template",
 )
 @click.pass_context
 def generate(
     ctx,
     model,
     num_cpus,
     num_instructions,
@@ -564,14 +583,16 @@
     "question",
     nargs=-1,
     type=click.UNPROCESSED,
 )
 @click.option(
     "-m",
     "--model",
+    default=config.DEFAULT_MODEL,
+    show_default=True,
     help="Model name to print in chat process",
 )
 @click.option(
     "-c",
     "--context",
     default="default",
     show_default=True,
@@ -634,17 +655,15 @@
     "--tls-client-passwd",
     type=click.STRING,
     default="",
     help="TLS client certificate password.",
 )
 @click.option(
     "--model-family",
-    default="merlinite",
-    show_default=True,
-    help="model family to use when picking a chat template",
+    help="Force model family to use when picking a chat template",
 )
 @click.pass_context
 def chat(
     ctx,
     question,
     model,
     context,
@@ -797,16 +816,16 @@
 )
 @click.pass_context
 def download(ctx, repository, release, filename, model_dir, hf_token):
     """Download the model(s) to train"""
     click.echo(f"Downloading model from {repository}@{release} to {model_dir}...")
     if hf_token == "" and "instructlab" not in repository:
         raise ValueError(
-            """HF_TOKEN var needs to be set in your environment to download HF Model. 
-            Alternatively, the token can be passed with --hf-token flag. 
+            """HF_TOKEN var needs to be set in your environment to download HF Model.
+            Alternatively, the token can be passed with --hf-token flag.
             The HF Token is used to authenticate your identity to the Hugging Face Hub."""
         )
     try:
         if ctx.obj is not None:
             hf_logging.set_verbosity(ctx.obj.config.general.log_level.upper())
         files = list_repo_files(repo_id=repository, token=hf_token)
         if any(".safetensors" in string for string in files):
@@ -1053,19 +1072,26 @@
             model_name=model_name,
             num_epochs=num_epochs,
             device=device,
             four_bit_quant=four_bit_quant,
         )
 
         training_results_dir = "./training_results"
-        os.makedirs(training_results_dir, exist_ok=True)
 
         final_results_dir = training_results_dir + "/final"
         os.makedirs(final_results_dir, exist_ok=True)
 
+        gguf_models_dir = "./models"
+        if not os.path.isdir(gguf_models_dir):
+            os.mkdir(gguf_models_dir)
+        gguf_models_file = os.path.join(gguf_models_dir, "ggml-model-f16.gguf")
+        # Remove previously trained model, its taking up space we may need in the next step
+        if os.path.isfile(gguf_models_file):
+            os.remove(gguf_models_file)
+
         # TODO: Figure out what to do when there are multiple checkpoint dirs.
         # Right now it's just copying files from the first one numerically not necessarily the best one
         added_tokens_file = glob(
             training_results_dir + "/checkpoint-*/added_tokens.json"
         )
         special_tokens_map = glob(
             training_results_dir + "/checkpoint-*/special_tokens_map.json"
@@ -1092,32 +1118,33 @@
         shutil.copy(tokenizer_config_json[0], final_results_dir)
         print("Copied ", tokenizer_config_json[0], "to ", final_results_dir)
         shutil.copy(config_json[0], final_results_dir)
         print("Copied ", config_json[0], "to ", final_results_dir)
         shutil.copy(generation_config_json[0], final_results_dir)
         print("Copied ", generation_config_json[0], "to ", final_results_dir)
         for file in safe_tensors:
-            shutil.copy(file, final_results_dir)
-            print("Copied ", file, "to ", final_results_dir)
+            shutil.move(file, final_results_dir)
+            print("Moved ", file, "to ", final_results_dir)
 
         if four_bit_quant:
             print(
                 "SKIPPING CONVERSION to gguf. This is unsupported with --4-bit-quant. "
                 + "See https://github.com/instructlab/instructlab/issues/579."
             )
             return
 
-        convert_llama_to_gguf(model=final_results_dir, pad_vocab=True)
+        gguf_file_path = convert_llama_to_gguf(model=final_results_dir, pad_vocab=True)
+
+        # Remove safetensors files to save space, were done with them here
+        # and the huggingface lib has them cached
+        for file in glob(final_results_dir + "/*.safetensors"):
+            os.remove(file)
+
+        shutil.move(gguf_file_path, gguf_models_file)
 
-        gguf_models_dir = "./models"
-        if not os.path.isdir(gguf_models_dir):
-            os.mkdir(gguf_models_dir)
-        shutil.copy(final_results_dir + "/ggml-model-f16.gguf", gguf_models_dir)
-        # cleanup original copy of model
-        os.remove(final_results_dir + "/ggml-model-f16.gguf")
         # cleanup checkpoint dir since it's name is unpredictable
         # TODO: figure out how checkpoint dirs should be cleaned up
         # checkpoint_dirs = glob(training_results_dir + "/checkpoint*")
         # shutil.rmtree(checkpoint_dirs[0])
     else:
         # Local
         from .mlx_explore.gguf_convert_to_mlx import load
@@ -1282,29 +1309,30 @@
     show_default=True,
 )
 @utils.macos_requirement(echo_func=click.secho, exit_exception=click.exceptions.Exit)
 @click.pass_context
 def convert(ctx, model_dir, adapter_file, skip_de_quantize, skip_quantize, model_name):
     """Converts model to GGUF"""
     # pylint: disable=C0415
+    # Third Party
+    from instructlab_quantize import run_quantize  # pylint: disable=import-error
+
     # Local
     from .llamacpp.llamacpp_convert_to_gguf import convert_llama_to_gguf
     from .train.lora_mlx.convert import convert_between_mlx_and_pytorch
     from .train.lora_mlx.fuse import fine_tune
 
     # compute model name from model-dir if not supplied
     if model_name is None:
         mlx_q_suffix = "-mlx-q"
         model_name = model_dir.split("/")[-1]
         model_name = model_name.replace(mlx_q_suffix, "")
 
     if adapter_file is None:
         adapter_file = os.path.join(model_dir, "adapters.npz")
-    cli_dir = os.path.dirname(os.path.abspath(__file__))
-
     source_model_dir = model_dir
     model_dir_fused = f"{source_model_dir}-fused"
 
     # this combines adapter with the original model to produce the updated model
     fine_tune(
         model=source_model_dir,
         save_path=model_dir_fused,
@@ -1335,13 +1363,18 @@
     for file in glob(os.path.join(model_dir_fused_pt, "*.safetensors")):
         os.remove(file)
 
     # quantize to 4-bit GGUF (optional)
     if not skip_quantize:
         gguf_model_dir = f"{model_dir_fused_pt}/{model_name}.gguf"
         gguf_model_q_dir = f"{model_dir_fused_pt}/{model_name}-Q4_K_M.gguf"
-        script = os.path.join(cli_dir, "llamacpp/quantize")
-        cmd = f"{script} {gguf_model_dir} {gguf_model_q_dir} Q4_K_M"
-        os.system("{}".format(cmd))
+        run_quantize(gguf_model_dir, gguf_model_q_dir, "Q4_K_M")
 
     ctx.obj.logger.info(f"deleting {model_dir_fused_pt}/{model_name}.gguf...")
     os.remove(os.path.join(model_dir_fused_pt, f"{model_name}.gguf"))
+
+
+@cli.command
+def sysinfo():
+    """Print system information"""
+    for key, value in get_sysinfo().items():
+        print(f"{key}: {value}")
```

### Comparing `instructlab-0.15.1/src/instructlab/llamacpp/LICENSE` & `instructlab-0.16.0/src/instructlab/llamacpp/LICENSE`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/llamacpp/README.md` & `instructlab-0.16.0/src/instructlab/llamacpp/README.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/llamacpp/llamacpp_convert_to_gguf.py` & `instructlab-0.16.0/src/instructlab/llamacpp/llamacpp_convert_to_gguf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1739,7 +1739,8 @@
         vocab,
         special_vocab,
         concurrency=concurrency,
         endianess=endianess,
         pad_vocab=pad_vocab,
     )
     print(f"Wrote {outfile}")
+    return outfile
```

### Comparing `instructlab-0.15.1/src/instructlab/mlx_explore/LICENSE` & `instructlab-0.16.0/src/instructlab/mlx_explore/LICENSE`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/mlx_explore/README.md` & `instructlab-0.16.0/src/instructlab/mlx_explore/README.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/mlx_explore/gguf_convert_to_mlx.py` & `instructlab-0.16.0/src/instructlab/mlx_explore/gguf_convert_to_mlx.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/mlx_explore/utils.py` & `instructlab-0.16.0/src/instructlab/mlx_explore/utils.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/schema/v1/compositional_skills.json` & `instructlab-0.16.0/src/instructlab/schema/v1/compositional_skills.json`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/schema/v1/knowledge.json` & `instructlab-0.16.0/src/instructlab/schema/v1/knowledge.json`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/schema/v2/compositional_skills.json` & `instructlab-0.16.0/src/instructlab/schema/v2/compositional_skills.json`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/schema/v2/knowledge.json` & `instructlab-0.16.0/src/instructlab/schema/v2/knowledge.json`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/server.py` & `instructlab-0.16.0/src/instructlab/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from llama_cpp.server.settings import Settings
 from uvicorn import Config
 import llama_cpp.server.app as llama_app
 import uvicorn
 
 # Local
 from .client import ClientException, list_models
-from .config import get_api_base
+from .config import get_api_base, get_model_family
 
 templates = [
     {
         "model": "merlinite",
         "template": "{% for message in messages %}\n{% if message['role'] == 'user' %}\n{{ '<|user|>\n' + message['content'] }}\n{% elif message['role'] == 'system' %}\n{{ '<|system|>\n' + message['content'] }}\n{% elif message['role'] == 'assistant' %}\n{{ '<|assistant|>\n' + message['content'] + eos_token }}\n{% endif %}\n{% if loop.last and add_generation_prompt %}\n{{ '<|assistant|>' }}\n{% endif %}\n{% endfor %}",
     },
     {
@@ -177,15 +177,15 @@
             return
         raise ServerException(f"failed creating the server application: {exc}") from exc
 
     template = ""
     eos_token = "<|endoftext|>"
     bos_token = ""
     for template_dict in templates:
-        if template_dict["model"] == model_family:
+        if template_dict["model"] == get_model_family(model_family, model_path):
             template = template_dict["template"]
             if template_dict["model"] == "mixtral":
                 eos_token = "</s>"
                 bos_token = "<s>"
     try:
         llama_app._llama_proxy._current_model.chat_handler = (
             llama_chat_format.Jinja2ChatFormatter(
@@ -219,14 +219,15 @@
     s = Server(config)
 
     # If this is not the main process, this is the temp server process that ran in the background
     # after `ilab chat` was executed.
     # In this case, we want to redirect stdout to null to avoid cluttering the chat with messages
     # returned by the server.
     if is_temp_server_running():
+        # TODO: redirect temp server logs to a file instead of hidding the logs completely
         # Redirect stdout and stderr to null
         with (
             open(os.devnull, "w", encoding="utf-8") as f,
             redirect_stdout(f),
             redirect_stderr(f),
         ):
             s.run()
```

### Comparing `instructlab-0.15.1/src/instructlab/train/linux_train.py` & `instructlab-0.16.0/src/instructlab/train/linux_train.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/train/lora_mlx/LICENSE` & `instructlab-0.16.0/src/instructlab/train/lora_mlx/LICENSE`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/train/lora_mlx/README.md` & `instructlab-0.16.0/src/instructlab/train/lora_mlx/README.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/train/lora_mlx/convert.py` & `instructlab-0.16.0/src/instructlab/train/lora_mlx/convert.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/train/lora_mlx/fuse.py` & `instructlab-0.16.0/src/instructlab/train/lora_mlx/fuse.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/train/lora_mlx/lora.py` & `instructlab-0.16.0/src/instructlab/train/lora_mlx/lora.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/train/lora_mlx/make_data.py` & `instructlab-0.16.0/src/instructlab/train/lora_mlx/make_data.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/train/lora_mlx/models/README.md` & `instructlab-0.16.0/src/instructlab/train/lora_mlx/models/README.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/train/lora_mlx/models/llama.py` & `instructlab-0.16.0/src/instructlab/train/lora_mlx/models/llama.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/train/lora_mlx/models/lora.py` & `instructlab-0.16.0/src/instructlab/train/lora_mlx/models/lora.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/train/lora_mlx/models/mixtral.py` & `instructlab-0.16.0/src/instructlab/train/lora_mlx/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/train/lora_mlx/models/models.py` & `instructlab-0.16.0/src/instructlab/train/lora_mlx/models/models.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/train/lora_mlx/models/phi2.py` & `instructlab-0.16.0/src/instructlab/train/lora_mlx/models/phi2.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/train/lora_mlx/prepare_model.py` & `instructlab-0.16.0/src/instructlab/train/lora_mlx/prepare_model.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/train/lora_mlx/utils.py` & `instructlab-0.16.0/src/instructlab/train/lora_mlx/utils.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/src/instructlab/utils.py` & `instructlab-0.16.0/src/instructlab/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from functools import cache, wraps
 from logging import Logger
 from pathlib import Path
 from typing import Any, Dict, List, Mapping, Optional, Union
 import copy
 import glob
 import json
-import logging
 import os
 import platform
 import re
 import subprocess
 import tempfile
 
 # Third Party
@@ -32,19 +31,14 @@
 rules:
   line-length:
     max: 120
 """
 
 DEFAULT_CHUNK_OVERLAP = 100
 
-logging.basicConfig(
-    level=logging.INFO,
-    format="%(levelname)s %(asctime)s %(filename)s:%(lineno)d %(message)s",
-)
-
 
 class TaxonomyReadingException(Exception):
     """An exception raised during reading of the taxonomy."""
 
 
 def macos_requirement(echo_func, exit_exception):
     """Adds a check for MacOS before running a method.
@@ -243,14 +237,55 @@
     return int(num_words * 1.3)  # 1 word ~ 1.3 token
 
 
 def num_chars_from_tokens(num_tokens) -> int:
     return int(num_tokens * 4)  # 1 token ~ 4 English character
 
 
+def num_tokens_from_chars(num_chars) -> int:
+    return int(num_chars / 4)  # 1 token ~ 4 English character
+
+
+def max_seed_example_tokens(server_ctx_size, prompt_num_chars) -> int:
+    """
+    Estimates the maximum number of tokens any seed example can have based
+    on the server context size and number of characters in the selected prompt.
+
+    A lot has to fit into the given server context size:
+      - The prompt itself, which can vary in size a bit based on model family and knowledge vs skill
+      - Two seed examples, which we append to the prompt template.
+      - A knowledge document chunk, if this is a knowledge example.
+      - The generated completion, which can vary substantially in length.
+
+    This is an attempt to roughly estimate the maximum size any seed example
+    (question + answer + context values from the yaml) should be to even have
+    a hope of not often exceeding the server's maximum context size.
+
+    NOTE: This does not take into account knowledge document chunks. It's meant
+    to calculate the maximum size that any seed example should be, whether knowledge
+    or skill. Knowledge seed examples will want to stay well below this limit.
+
+    NOTE: This is a very simplistic calculation, and examples with lots of numbers
+    or punctuation may have quite a different token count than the estimates here,
+    depending on the model (and thus tokenizer) in use. That's ok, as it's only
+    meant to be a rough estimate.
+
+    Args:
+        server_ctx_size (int): Size of the server context, in tokens.
+        prompt_num_chars (int): Number of characters in the prompt (not including the examples)
+    """
+    # Ensure we have at least 1024 tokens available for a response.
+    max_seed_tokens = server_ctx_size - 1024
+    # Subtract the number of tokens in our prompt template
+    max_seed_tokens = max_seed_tokens - num_tokens_from_chars(prompt_num_chars)
+    # Divide number of characters by 2, since we insert 2 examples
+    max_seed_tokens = int(max_seed_tokens / 2)
+    return max_seed_tokens
+
+
 def chunk_document(documents: List, server_ctx_size, chunk_word_count) -> List[str]:
     """
     Iterates over the documents and splits them into chunks based on the word count provided by the user.
     Args:
         documents (dict): List of documents retrieved from git (can also consist of a single document).
         server_ctx_size (int): Context window size of server.
         chunk_word_count (int): Maximum number of words to chunk a document.
@@ -428,14 +463,20 @@
     try:
         with open(file_path, "r", encoding="utf-8") as file:
             contents = yaml.safe_load(file)
         if not contents:
             logger.warn(f"Skipping {file_path} because it is empty!")
             warnings += 1
             return None, warnings, errors
+        if not isinstance(contents, Mapping):
+            logger.error(
+                f"{file_path} is not valid. The top-level element is not an object with key-value pairs."
+            )
+            errors += 1
+            return None, warnings, errors
 
         # do general YAML linting if specified
         version = get_version(contents)
         if version > 1:  # no linting for version 1 yaml
             if yaml_rules is not None:
                 is_file = os.path.isfile(yaml_rules)
                 if is_file:
```

### Comparing `instructlab-0.15.1/src/instructlab.egg-info/PKG-INFO` & `instructlab-0.16.0/src/instructlab.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructlab
-Version: 0.15.1
+Version: 0.16.0
 Summary: CLI for interacting with InstructLab
 Author-email: TBD <jon@example.com>
 License: Apache-2.0 AND MIT
 Project-URL: homepage, https://instructlab.io
 Project-URL: source, https://github.com/instructlab/instructlab
 Project-URL: issues, https://github.com/instructlab/instructlab/issues
 Classifier: Development Status :: 3 - Alpha
@@ -25,14 +25,15 @@
 License-File: LICENSE
 Requires-Dist: click<9.0.0,>=8.1.7
 Requires-Dist: click-didyoumean<0.4.0,>=0.3.0
 Requires-Dist: datasets<3.0.0,>=2.18.0
 Requires-Dist: gguf<0.7.0,>=0.6.0
 Requires-Dist: GitPython<4.0.0,>=3.1.42
 Requires-Dist: httpx<1.0.0,>=0.25.0
+Requires-Dist: instructlab-quantize>=0.1.0
 Requires-Dist: jsonschema<5.0.0,>=4.21.1
 Requires-Dist: llama_cpp_python[server]==0.2.75
 Requires-Dist: mlx<0.6.0,>=0.5.1; sys_platform == "darwin" and platform_machine == "arm64"
 Requires-Dist: numpy<2.0.0,>=1.23.5; python_version == "3.10"
 Requires-Dist: numpy<2.0.0,>=1.26.4; python_version != "3.10"
 Requires-Dist: openai<2.0.0,>=1.13.3
 Requires-Dist: peft<0.10.0,>=0.9.0
@@ -65,38 +66,31 @@
 ## 📖 Contents
 
 - [Welcome to the InstructLab CLI](#welcome-to-the-instructlab-cli)
 - [❓ What is `ilab`](#-what-is-ilab)
 - [📋 Requirements](#-requirements)
 - [✅ Getting started](#-getting-started)
   - [🧰 Installing `ilab`](#-installing-ilab)
-    - [To install with no GPU acceleration and PyTorch without CUDA bindings](#to-install-with-no-gpu-acceleration-and-pytorch-without-cuda-bindings)
-    - [To install with AMD ROCm](#to-install-with-amd-rocm)
-    - [To install with Apple Metal on M1/M2/M3 Mac](#to-install-with-apple-metal-on-m1m2m3-mac)
-    - [To install with Nvidia CUDA](#to-install-with-nvidia-cuda)
-    - [Example output](#example-output)
-    - [Bash (version 4.4 or newer)](#bash-version-44-or-newer)
-    - [Zsh](#zsh)
-    - [Fish](#fish)
+    - [Install with no GPU acceleration and PyTorch without CUDA bindings](#install-using-pytorch-without-cuda-bindings-and-no-gpu-acceleration)
+    - [Install with AMD ROCm](#install-with-amd-rocm)
+    - [Install with Apple Metal on M1/M2/M3 Macs](#install-with-apple-metal-on-m1m2m3-macs)
+    - [Install with Nvidia CUDA](#install-with-nvidia-cuda)
   - [🏗️ Initialize `ilab`](#️-initialize-ilab)
-    - [Example output](#example-output-1)
-    - [Example output](#example-output-2)
   - [📥 Download the model](#-download-the-model)
   - [🍴 Serving the model](#-serving-the-model)
   - [📣 Chat with the model (Optional)](#-chat-with-the-model-optional)
 - [💻 Creating new knowledge or skills and training the model](#-creating-new-knowledge-or-skills-and-training-the-model)
   - [🎁 Contribute knowledge or compositional skills](#-contribute-knowledge-or-compositional-skills)
   - [📜 List and validate your new data](#-list-and-validate-your-new-data)
   - [🚀 Generate a synthetic dataset](#-generate-a-synthetic-dataset)
-    - [Example output](#example-output-3)
-  - [👩‍🏫 Train the model](#-train-the-model)
+  - [👩‍🏫 Training the model](#-training-the-model)
     - [Train the model locally on Linux](#train-the-model-locally-on-linux)
-    - [Train the model locally on an M-series Mac](#train-the-model-locally-on-an-m-series-mac)
-    - [Training the model locally with GPU acceleration](#training-the-model-locally-with-gpu-acceleration)
-    - [Training the model in the cloud](#training-the-model-in-the-cloud)
+    - [Train the model locally on M-series Macs](#train-the-model-locally-on-an-m-series-mac)
+    - [Train the model locally with GPU acceleration](#train-the-model-locally-with-gpu-acceleration)
+    - [Train the model in the cloud](#train-the-model-in-the-cloud)
   - [📜 Test the newly trained model](#-test-the-newly-trained-model)
   - [🍴 Serve the newly trained model](#-serve-the-newly-trained-model)
 - [📣 Chat with the new model (not optional this time)](#-chat-with-the-new-model-not-optional-this-time)
 - [🎁 Submit your new knowledge or skills](#-submit-your-new-knowledge-or-skills)
 - [📬 Contributing](#-contributing)
 
 ## Welcome to the InstructLab CLI
@@ -143,15 +137,15 @@
 - **🍎 Apple M1/M2/M3 Mac or 🐧 Linux system** (tested on Fedora). We anticipate support for more operating systems in the future.
 - C++ compiler
 - Python 3.9+ (<3.12 for PyTorch JIT)
 - Approximately 60GB disk space (entire process)
 
 > **NOTE:** PyTorch 2.2.1 does not support `torch.compile` with Python 3.12. On Fedora 39+, install `python3.11-devel` and create the virtual env with `python3.11` if you wish to use PyTorch's JIT compiler.
 <!-- -->
-> **NOTE:** When installing the `ilab` CLI on macOS, you may have to run the `xcode select --install` command to install the required packages previously listed.
+> **NOTE:** When installing the `ilab` CLI on macOS, you may have to run the `xcode select --install` command, installing the required packages previously listed.
 
 ## ✅ Getting started
 
 ### 🧰 Installing `ilab`
 
 1. When installing on Fedora Linux, install C++, Python 3.9+, and other necessary tools by running the following command:
 
@@ -172,73 +166,81 @@
    ```shell
    mkdir instructlab
    cd instructlab
    ```
 
    > **NOTE:** The following steps in this document use [Python venv](https://docs.python.org/3/library/venv.html) for virtual environments. However, if you use another tool such as [pyenv](https://github.com/pyenv/pyenv) or [Conda Miniforge](https://github.com/conda-forge/miniforge) for managing Python environments on your machine continue to use that tool instead. Otherwise, you may have issues with packages that are installed but not found in `venv`.
 
-3. Install and activate your `venv` environment by running the following command:
+3. There are a few ways you can locally install the `ilab` CLI. Select your preferred installation method from the following instructions. You can then install `ilab` and activate your `venv` environment.
 
    > **NOTE**: ⏳ `pip install` may take some time, depending on your internet connection. In case installation fails with error ``unsupported instruction `vpdpbusd'``, append `-C cmake.args="-DLLAMA_NATIVE=off"` to `pip install` command.
 
    See [the GPU acceleration documentation](./docs/gpu-acceleration.md) for how to
-   to enable hardware acceleration for inference and training on AMD ROCm,
+   to enable hardware acceleration for interaction and training on AMD ROCm,
    Apple Metal Performance Shaders (MPS), and Nvidia CUDA.
 
-   #### To install with no GPU acceleration and PyTorch without CUDA bindings
+   #### Install using PyTorch without CUDA bindings and no GPU acceleration
 
-   ```shell
-   python3 -m venv --upgrade-deps venv
-   source venv/bin/activate
-   (venv) $ pip cache remove llama_cpp_python
-   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable --extra-index-url=https://download.pytorch.org/whl/cpu
-   ```
-
-   #### To install with AMD ROCm
-
-   ```shell
-   python3 -m venv --upgrade-deps venv
-   source venv/bin/activate
-   (venv) $ pip cache remove llama_cpp_python
-   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable \
-       --extra-index-url https://download.pytorch.org/whl/rocm6.0 \
-       -C cmake.args="-DLLAMA_HIPBLAS=on" \
-       -C cmake.args="-DAMDGPU_TARGETS=all" \
-       -C cmake.args="-DCMAKE_C_COMPILER=/opt/rocm/llvm/bin/clang" \
-       -C cmake.args="-DCMAKE_CXX_COMPILER=/opt/rocm/llvm/bin/clang++" \
-       -C cmake.args="-DCMAKE_PREFIX_PATH=/opt/rocm"
-   ```
-
-   On Fedora 40+, use `-DCMAKE_C_COMPILER=clang-17` and `-DCMAKE_CXX_COMPILER=clang++-17`.
-
-   #### To install with Apple Metal on M1/M2/M3 Mac
-
-   ```shell
-   python3 -m venv --upgrade-deps venv
-   source venv/bin/activate
-   (venv) $ pip cache remove llama_cpp_python
-   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable -C cmake.args="-DLLAMA_METAL=on"
-   ```
-
-   #### To install with Nvidia CUDA
-
-   ```shell
-   python3 -m venv --upgrade-deps venv
-   source venv/bin/activate
-   (venv) $ pip cache remove llama_cpp_python
-   (venv) $ pip install git+https://github.com/instructlab/instructlab.git@stable -C cmake.args="-DLLAMA_CUBLAS=on"
+      ```shell
+      python3 -m venv --upgrade-deps venv
+      source venv/bin/activate
+      (venv) $ pip cache remove llama_cpp_python
+      (venv) $ pip install instructlab --extra-index-url=https://download.pytorch.org/whl/cpu
+      ```
+
+      > **NOTE**: *Additional Build Argument for Intel Macs*
+      >
+      > If you have an Mac with an Intel CPU, you must add a prefix of
+      > `CMAKE_ARGS="-DLLAMA_METAL=off"` to the `pip install` command to ensure
+      > that the build is done without Apple M-series GPU support.
+      >
+      > `(venv) $ CMAKE_ARGS="-DLLAMA_METAL=off" pip install ...`
+
+   #### Install with AMD ROCm
+
+      ```shell
+      python3 -m venv --upgrade-deps venv
+      source venv/bin/activate
+      (venv) $ pip cache remove llama_cpp_python
+      (venv) $ pip install instructlab \
+         --extra-index-url https://download.pytorch.org/whl/rocm6.0 \
+         -C cmake.args="-DLLAMA_HIPBLAS=on" \
+         -C cmake.args="-DAMDGPU_TARGETS=all" \
+         -C cmake.args="-DCMAKE_C_COMPILER=/opt/rocm/llvm/bin/clang" \
+         -C cmake.args="-DCMAKE_CXX_COMPILER=/opt/rocm/llvm/bin/clang++" \
+         -C cmake.args="-DCMAKE_PREFIX_PATH=/opt/rocm"
+      ```
+
+      On Fedora 40+, use `-DCMAKE_C_COMPILER=clang-17` and `-DCMAKE_CXX_COMPILER=clang++-17`.
+
+   #### Install with Apple Metal on M1/M2/M3 Macs
+
+      ```shell
+      python3 -m venv --upgrade-deps venv
+      source venv/bin/activate
+      (venv) $ pip cache remove llama_cpp_python
+      (venv) $ pip install instructlab
+      ```
+
+   #### Install with Nvidia CUDA
+
+      ```shell
+      python3 -m venv --upgrade-deps venv
+      source venv/bin/activate
+      (venv) $ pip cache remove llama_cpp_python
+      (venv) $ pip install instructlab -C cmake.args="-DLLAMA_CUBLAS=on"
    ```
 
 4. From your `venv` environment, verify `ilab` is installed correctly, by running the `ilab` command.
 
    ```shell
    ilab
    ```
 
-   #### Example output
+   *Example output of the `ilab` command*
 
    ```shell
    (venv) $ ilab
    Usage: ilab [OPTIONS] COMMAND [ARGS]...
 
    CLI for interacting with InstructLab.
 
@@ -265,15 +267,15 @@
 
    > **IMPORTANT:** every `ilab` command needs to be run from within your Python virtual environment. To enter the Python environment, run the following command:
 
    ```shell
    source venv/bin/activate
    ```
 
-5. You may optionally enable tab completion for the `ilab` command.
+5. Optional: You can enable tab completion for the `ilab` command.
 
    #### Bash (version 4.4 or newer)
 
    Enable tab completion in `bash` with the following command:
 
    ```sh
    eval "$(_ILAB_COMPLETE=bash_source ilab)"
@@ -322,29 +324,29 @@
 
 1. Initialize `ilab` by running the following command:
 
    ```shell
    ilab init
    ```
 
-   #### Example output
+   *Example output*
 
    ```shell
    Welcome to InstructLab CLI. This guide will help you set up your environment.
    Please provide the following values to initiate the environment [press Enter for defaults]:
    Path to taxonomy repo [taxonomy]: <ENTER>
    ```
 
 2. When prompted by the interface, press **Enter** to add a new default `config.yaml` file.
 
 3. When prompted, clone the `https://github.com/instructlab/taxonomy.git` repository into the current directory by typing **y**.
 
    **Optional**: If you want to point to an existing local clone of the `taxonomy` repository, you can pass the path interactively or alternatively with the `--taxonomy-path` flag.
 
-   #### Example output
+   *Example output after initializing `ilab`*
 
    ```shell
    (venv) $ ilab init
    Welcome to InstructLab CLI. This guide will help you set up your environment.
    Please provide the following values to initiate the environment [press Enter for defaults]:
    Path to taxonomy repo [taxonomy]: <ENTER>
    `taxonomy` seems to not exists or is empty. Should I clone https://github.com/instructlab/taxonomy.git for you? [y/N]: y
@@ -363,21 +365,21 @@
    ```shell
    git clone --recurse-submodules https://github.com/instructlab/taxonomy.git
    git pull --recurse-submodules
    ```
 
 ### 📥 Download the model
 
-- Run the `ilab download`command.
+- Run the `ilab download` command.
 
   ```shell
   ilab download
   ```
 
-  `ilab download` will download a pre-trained [model](https://huggingface.co/instructlab/) (~4.4G) from HuggingFace and store it in a `models` directory:
+  `ilab download` downloads a compact pre-trained version of the [model](https://huggingface.co/instructlab/) (~4.4G) from HuggingFace and store it in a `models` directory:
 
   ```shell
   (venv) $ ilab download
   Downloading model from instructlab/merlinite-7b-lab-GGUF@main to models...
   (venv) $ ls models
   merlinite-7b-lab-Q4_K_M.gguf
   ```
@@ -465,15 +467,15 @@
 
    ```shell
    ilab generate
    ```
 
    > **NOTE:** ⏳ This can take from 15 minutes to 1+ hours to complete, depending on your computing resources.
 
-   #### Example output
+   *Example output of `ilab generate`*
 
    ```shell
    (venv) $ ilab generate
    INFO 2024-02-29 19:09:48,804 lab.py:250 Generating model 'ggml-merlinite-7b-lab-Q4_K_M' using 10 CPUs,
    taxonomy: '/home/username/instructlab/taxonomy' and seed 'seed_tasks.json'
 
    0%|##########| 0/100 Cannot find prompt.txt. Using default prompt.
@@ -498,19 +500,19 @@
    **Optional**: It is also possible to run the generate step against a different model via an
    OpenAI-compatible API. For example, the one spawned by `ilab serve` or any remote or locally hosted LLM (e.g. via [`ollama`](https://ollama.com/), [`LM Studio`](https://lmstudio.ai), etc.). Run the following command:
 
    ```shell
    ilab generate --endpoint-url http://localhost:8000/v1
    ```
 
-### 👩‍🏫 Train the model
+### 👩‍🏫 Training the model
 
-There are three options to train the model on your synthetic data-enhanced dataset.
+There are many options for training the model with your synthetic data-enhanced dataset.
 
-> **Note:** **Every** `ilab` command needs to be run from within your Python virtual environment.
+> **Note:** **Every** `ilab` command needs to run from within your Python virtual environment.
 
 #### Train the model locally on Linux
 
 ```shell
 ilab train
 ```
 
@@ -540,23 +542,23 @@
 (venv) $ ls instructlab-merlinite-7b-lab-mlx-q
 adapters-010.npz        adapters-050.npz        adapters-090.npz        config.json             tokenizer.model
 adapters-020.npz        adapters-060.npz        adapters-100.npz        model.safetensors       tokenizer_config.json
 adapters-030.npz        adapters-070.npz        adapters.npz            special_tokens_map.json
 adapters-040.npz        adapters-080.npz        added_tokens.json       tokenizer.jso
 ```
 
-#### Training the model locally with GPU acceleration
+#### Train the model locally with GPU acceleration
 
 Training has experimental support for GPU acceleration with Nvidia CUDA or AMD ROCm. Please see [the GPU acceleration documentation](./docs/gpu-acceleration.md) for more details. At present, hardware acceleration requires a data center GPU or high-end consumer GPU with at least 18 GB free memory.
 
 ```shell
 ilab train --device=cuda
 ```
 
-#### Training the model in the cloud
+#### Train the model in the cloud
 
 Follow the instructions in [Training](./notebooks/README.md).
 
 ⏳ Approximate amount of time taken on each platform:
 
 - *Google Colab*: **5-10 minutes** with a T4 GPU
 - *Kaggle*: **~30 minutes** with a P100 GPU.
@@ -592,20 +594,20 @@
    ilab convert
    ```
 
 3. Serve the newly trained model locally via `ilab serve` command with the `--model-path`
 argument to specify your new model:
 
    ```shell
-   ilab serve --model-path <New model name>
+   ilab serve --model-path <new model path>
    ```
 
-   Which model should you select to serve? After running the `ilab convert` command, a few files and directories are generated. The one you will want to serve will end in `.gguf`
-   and will exist in a directory with the suffix `fused-pt`. For example:
-   `instructlab-merlinite-7b-lab-mlx-q-fused-pt/ggml-model-Q4_K_M.gguf`
+   Which model should you select to serve? After running the `ilab convert` command, some files and a directory are generated. The model you will want to serve ends with an extension of `.gguf`
+   and exists in a directory with the suffix `trained`. For example:
+   `instructlab-merlinite-7b-lab-trained/instructlab-merlinite-7b-lab-Q4_K_M.gguf`.
 
 ## 📣 Chat with the new model (not optional this time)
 
 - Try the fine-tuned model out live using the chat interface, and see if the results are better than the untrained version of the model with chat by running the following command:
 
    ```shell
    ilab chat -m <New model name>
```

### Comparing `instructlab-0.15.1/src/instructlab.egg-info/SOURCES.txt` & `instructlab-0.16.0/src/instructlab.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,57 +4,56 @@
 .isort.cfg
 .markdownlint-cli2.yaml
 .pre-commit-config.yaml
 .pylintrc
 .spellcheck-en-custom.txt
 .spellcheck.yml
 CODE_OF_CONDUCT.md
-CONTRIBUTOR_ROLES.md
 LICENSE
 MAINTAINERS.md
 Makefile
 README.md
 SECURITY.md
 TROUBLESHOOTING.md
-governance.md
 pyproject.toml
 requirements-dev.txt
 requirements-hpu.txt
 requirements.txt
 tox.ini
 .github/PULL_REQUEST_TEMPLATE.md
 .github/actionlint.yaml
 .github/mergify.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
+.github/ISSUE_TEMPLATE/team_recommend.md
 .github/workflows/actionlint.yml
 .github/workflows/docs.yml
 .github/workflows/e2e.yml
 .github/workflows/image-cuda.yml
 .github/workflows/lint.yml
 .github/workflows/pypi.yaml
 .github/workflows/spellcheck.yaml
 .github/workflows/stale_bot.yml
 .github/workflows/test.yml
+.github/workflows/validate-notebooks.yml
 .github/workflows/matchers/pylint.json
 CONTRIBUTING/CONTRIBUTING.md
 CONTRIBUTING/FIRST_TIME_CONTRIBUTORS.md
+containers/README.md
 containers/sitecustomize.py
 containers/bin/debug-llama
 containers/bin/debug-pytorch
 containers/cuda/Containerfile
 containers/hpu/Containerfile
 containers/rocm/Containerfile
 containers/rocm/README.md
 containers/rocm/gfx-version.sh
 containers/rocm/remove-gfx.sh
 docs/README.md
-docs/STABLE.md
 docs/ci.md
-docs/containerization.md
 docs/converting_GGUF.md
 docs/demo-slides.md
 docs/gpu-acceleration.md
 docs/habana-gaudi.md
 docs/release-strategy.md
 docs/workflow.png
 docs/workflow.puml
@@ -74,41 +73,44 @@
 notebooks/images/kaggle/input.png
 notebooks/images/kaggle/new-dataset.png
 notebooks/images/kaggle/select-accelerator-p100.png
 notebooks/images/kaggle/select-accelerator.png
 scripts/basic-workflow-tests.sh
 scripts/functional-tests.sh
 scripts/ruff.sh
+scripts/validate_notebook.py
 scripts/test-data/basic-workflow-fixture-qna.yaml
 src/instructlab/__init__.py
 src/instructlab/__main__.py
 src/instructlab/_version.py
 src/instructlab/client.py
 src/instructlab/common.py
 src/instructlab/config.py
 src/instructlab/lab.py
+src/instructlab/log.py
 src/instructlab/server.py
+src/instructlab/sysinfo.py
 src/instructlab/utils.py
 src/instructlab.egg-info/PKG-INFO
 src/instructlab.egg-info/SOURCES.txt
 src/instructlab.egg-info/dependency_links.txt
 src/instructlab.egg-info/entry_points.txt
 src/instructlab.egg-info/requires.txt
 src/instructlab.egg-info/top_level.txt
+src/instructlab/chat/__init__.py
 src/instructlab/chat/chat.py
 src/instructlab/generator/README.md
 src/instructlab/generator/__init__.py
 src/instructlab/generator/generate_data.py
 src/instructlab/generator/seed_tasks.jsonl
 src/instructlab/generator/utils.py
 src/instructlab/llamacpp/LICENSE
 src/instructlab/llamacpp/README.md
 src/instructlab/llamacpp/__init__.py
 src/instructlab/llamacpp/llamacpp_convert_to_gguf.py
-src/instructlab/llamacpp/quantize
 src/instructlab/mlx_explore/LICENSE
 src/instructlab/mlx_explore/README.md
 src/instructlab/mlx_explore/__init__.py
 src/instructlab/mlx_explore/gguf_convert_to_mlx.py
 src/instructlab/mlx_explore/utils.py
 src/instructlab/schema/v1/compositional_skills.json
 src/instructlab/schema/v1/knowledge.json
@@ -149,11 +151,12 @@
 tests/test_lab_train.py
 tests/test_notebooks.py
 tests/test_utils.py
 tests/testdata/invalid_yaml.yaml
 tests/testdata/knowledge_valid.yaml
 tests/testdata/skill_incomplete.yaml
 tests/testdata/skill_invalid_answer.yaml
+tests/testdata/skill_too_long_answer.yaml
 tests/testdata/skill_valid_answer.yaml
 tests/testdata/testdata.py
 tests/testdata/temp_repo/knowledge-wiki.md
 tests/testdata/temp_repo/docs/skill-wiki.md
```

### Comparing `instructlab-0.15.1/src/instructlab.egg-info/requires.txt` & `instructlab-0.16.0/src/instructlab.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 click<9.0.0,>=8.1.7
 click-didyoumean<0.4.0,>=0.3.0
 datasets<3.0.0,>=2.18.0
 gguf<0.7.0,>=0.6.0
 GitPython<4.0.0,>=3.1.42
 httpx<1.0.0,>=0.25.0
+instructlab-quantize>=0.1.0
 jsonschema<5.0.0,>=4.21.1
 llama_cpp_python[server]==0.2.75
 openai<2.0.0,>=1.13.3
 peft<0.10.0,>=0.9.0
 prompt-toolkit<4.0.0,>=3.0.38
 pydantic<3.0.0,>=2.6.0
 pydantic_yaml<2.0.0,>=1.2.0
```

### Comparing `instructlab-0.15.1/tests/conftest.py` & `instructlab-0.16.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/tests/taxonomy.py` & `instructlab-0.16.0/tests/taxonomy.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/tests/test_config.py` & `instructlab-0.16.0/tests/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,24 +13,24 @@
         self.tmpdir = tmpdir
 
     def _assert_defaults(self, cfg):
         assert cfg.general is not None
         assert cfg.general.log_level == "INFO"
 
         assert cfg.chat is not None
-        assert cfg.chat.model == "merlinite-7b-lab-Q4_K_M"
+        assert cfg.chat.model == "models/merlinite-7b-lab-Q4_K_M.gguf"
         assert not cfg.chat.vi_mode
         assert cfg.chat.visible_overflow
         assert cfg.chat.context == "default"
         assert cfg.chat.session is None
         assert cfg.chat.logs_dir == "data/chatlogs"
         assert not cfg.chat.greedy_mode
 
         assert cfg.generate is not None
-        assert cfg.generate.model == "merlinite-7b-lab-Q4_K_M"
+        assert cfg.generate.model == "models/merlinite-7b-lab-Q4_K_M.gguf"
         assert cfg.generate.taxonomy_path == "taxonomy"
         assert cfg.generate.taxonomy_base == "origin/main"
         assert cfg.generate.num_cpus == 10
         assert cfg.generate.num_instructions == 100
         assert cfg.generate.chunk_word_count == 1000
         assert cfg.generate.output_dir == "generated"
         assert cfg.generate.prompt_file == "prompt.txt"
@@ -48,17 +48,17 @@
         self._assert_defaults(cfg)
 
     def test_minimal_config(self):
         config_path = self.tmpdir.join("config.yaml")
         with open(config_path, "w", encoding="utf-8") as config_file:
             config_file.write(
                 """chat:
-  model: merlinite-7b-lab-Q4_K_M
+  model: models/merlinite-7b-lab-Q4_K_M.gguf
 generate:
-  model: merlinite-7b-lab-Q4_K_M
+  model: models/merlinite-7b-lab-Q4_K_M.gguf
   taxonomy_base: origin/main
   taxonomy_path: taxonomy
 serve:
   model_path: models/merlinite-7b-lab-Q4_K_M.gguf
 """
             )
         cfg = config.read_config(config_path)
@@ -71,20 +71,20 @@
             config_file.write(
                 """general:
   log_level: INFO
 chat:
   context: default
   greedy_mode: false
   logs_dir: data/chatlogs
-  model: merlinite-7b-lab-Q4_K_M
+  model: models/merlinite-7b-lab-Q4_K_M.gguf
   session: null
   vi_mode: false
   visible_overflow: true
 generate:
-  model: merlinite-7b-lab-Q4_K_M
+  model: models/merlinite-7b-lab-Q4_K_M.gguf
   num_cpus: 10
   num_instructions: 100
   output_dir: generated
   prompt_file: prompt.txt
   seed_file: seed_tasks.json
   taxonomy_base: origin/main
   taxonomy_path: taxonomy
@@ -102,17 +102,17 @@
 
     def test_config_unexpected_fields(self):
         print(dir(self.tmpdir))
         config_path = self.tmpdir.join("config.yaml")
         with open(config_path, "w", encoding="utf-8") as config_file:
             config_file.write(
                 """chat:
-  model: merlinite-7b-lab-Q4_K_M
+  model: models/merlinite-7b-lab-Q4_K_M.gguf
 generate:
-  model: merlinite-7b-lab-Q4_K_M
+  model: models/merlinite-7b-lab-Q4_K_M.gguf
   taxonomy_base: origin/main
   taxonomy_path: taxonomy
 serve:
   model_path: models/merlinite-7b-lab-Q4_K_M.gguf
 unexpected:
   field: value
 """
@@ -141,15 +141,15 @@
     def test_config_missing_required_fields(self):
         config_path = self.tmpdir.join("config.yaml")
         with open(config_path, "w", encoding="utf-8") as config_file:
             config_file.write(
                 """general:
   log_level: INFO
 generate:
-  model: merlinite-7b-lab-Q4_K_M
+  model: models/merlinite-7b-lab-Q4_K_M.gguf
 """
             )
         with pytest.raises(
             config.ConfigException,
             match=r"""4 errors in [\/\w-]+config.yaml:
 - missing chat: field required
 - missing generate->taxonomy_path: field required
```

### Comparing `instructlab-0.15.1/tests/test_lab.py` & `instructlab-0.16.0/tests/test_lab.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/tests/test_lab_diff.py` & `instructlab-0.16.0/tests/test_lab_diff.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/tests/test_lab_download.py` & `instructlab-0.16.0/tests/test_lab_download.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/tests/test_lab_generate.py` & `instructlab-0.16.0/tests/test_lab_generate.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 # Third Party
 from click.testing import CliRunner
 import pytest
 
 # First Party
 from instructlab import lab
+from instructlab.config import get_default_config, write_config
 from instructlab.generator.generate_data import generate_data
 from instructlab.generator.utils import GenerateException
 
 # Local
 from .taxonomy import MockTaxonomy
 from .testdata import testdata
 
@@ -157,14 +158,49 @@
                     )
                 assert "There was a problem connecting to the OpenAI server" in str(
                     exc.value
                 )
                 get_instructions_from_model.assert_called_once()
                 mt.teardown()
 
+    def test_new_data_too_long(self):
+        runner = CliRunner()
+        with open("tests/testdata/skill_too_long_answer.yaml", "rb") as qnafile:
+            with runner.isolated_filesystem():
+                cfg_file = "small_ctx_config.yaml"
+                smaller_ctx = 3072
+                config = get_default_config()
+                config.serve.max_ctx_size = smaller_ctx
+                write_config(config, config_file=cfg_file)
+                mt = MockTaxonomy(pathlib.Path("taxonomy"))
+                mt.create_untracked(
+                    "compositional_skills/tracked/qna.yaml", qnafile.read()
+                )
+                result = runner.invoke(
+                    lab.cli,
+                    [
+                        "--config",
+                        cfg_file,
+                        "generate",
+                        "--taxonomy-base",
+                        "main",
+                        "--taxonomy-path",
+                        mt.root,
+                        "--endpoint-url",
+                        "localhost:8000",
+                        "--server-ctx-size",
+                        smaller_ctx,
+                    ],
+                )
+                assert (
+                    result.exit_code == 1
+                ), "command finished with an unexpected exit code"
+                assert "too long for the server context size" in result.output
+                mt.teardown()
+
     @patch(
         "instructlab.generator.generate_data.get_instructions_from_model",
         return_value=(testdata.generate_data_return_value, 0),
     )
     def test_generate_no_error(self, get_instructions_from_model):
         with open("tests/testdata/skill_valid_answer.yaml", "rb") as qnafile:
             with CliRunner().isolated_filesystem():
```

### Comparing `instructlab-0.15.1/tests/test_lab_init.py` & `instructlab-0.16.0/tests/test_lab_init.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/tests/test_lab_train.py` & `instructlab-0.16.0/tests/test_lab_train.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,27 +45,30 @@
     ]:
         with open(CHECKPOINT_DIR + f_path, "w", encoding=ENCODING) as f:
             f.write("{}")
     os.makedirs(MERGED_MODEL_DIR)
     for f_path in ["/config.json", "/generation_config.json", "/1.safetensors"]:
         with open(MERGED_MODEL_DIR + f_path, "w", encoding=ENCODING) as f:
             f.write("{}")
-    os.makedirs(FINAL_RESULTS_DIR)
-    with open(LINUX_GGUF_FILE, "w", encoding=ENCODING) as f:
-        f.write("{}")
 
 
 def setup_load():
     os.makedirs(MODEL_DIR)
 
 
 def is_arm_mac():
     return sys.platform == "darwin" and platform.machine() == "arm64"
 
 
+def mock_convert_llama_to_gguf(model, pad_vocab):
+    with open(LINUX_GGUF_FILE, "w", encoding="utf-8") as fp:
+        fp.write(str(model) + str(pad_vocab))
+    return LINUX_GGUF_FILE
+
+
 @pytest.mark.usefixtures("mock_mlx_package")
 class TestLabTrain:
     """Test collection for `ilab train` command."""
 
     @patch("instructlab.lab.utils.is_macos_with_m_chip", return_value=True)
     @patch("instructlab.mlx_explore.gguf_convert_to_mlx.load")
     @patch("instructlab.train.lora_mlx.make_data.make_data")
@@ -336,15 +339,18 @@
             convert_between_mlx_and_pytorch_mock.assert_not_called()
             make_data_mock.assert_called_once()
             fetch_tokenizer_from_hub_mock.assert_not_called()
             is_macos_with_m_chip_mock.assert_called_once()
 
     @patch("instructlab.lab.utils.is_macos_with_m_chip", return_value=False)
     @patch.object(linux_train, "linux_train")
-    @patch("instructlab.llamacpp.llamacpp_convert_to_gguf.convert_llama_to_gguf")
+    @patch(
+        "instructlab.llamacpp.llamacpp_convert_to_gguf.convert_llama_to_gguf",
+        side_effect=mock_convert_llama_to_gguf,
+    )
     def test_train_linux(
         self,
         convert_llama_to_gguf_mock,
         linux_train_mock,
         is_macos_with_m_chip_mock,
     ):
         runner = CliRunner()
@@ -377,15 +383,18 @@
             assert not linux_train_mock.call_args[1]["four_bit_quant"]
             assert len(linux_train_mock.call_args[1]) == 7
             is_macos_with_m_chip_mock.assert_called_once()
             assert not os.path.isfile(LINUX_GGUF_FILE)
 
     @patch("instructlab.lab.utils.is_macos_with_m_chip", return_value=False)
     @patch("instructlab.train.linux_train.linux_train")
-    @patch("instructlab.llamacpp.llamacpp_convert_to_gguf.convert_llama_to_gguf")
+    @patch(
+        "instructlab.llamacpp.llamacpp_convert_to_gguf.convert_llama_to_gguf",
+        side_effect=mock_convert_llama_to_gguf,
+    )
     def test_num_epochs(
         self, convert_llama_to_gguf_mock, linux_train_mock, is_macos_with_m_chip_mock
     ):
         runner = CliRunner()
         with runner.isolated_filesystem():
             setup_input_dir()
             setup_linux_dir()
```

### Comparing `instructlab-0.15.1/tests/test_notebooks.py` & `instructlab-0.16.0/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/tests/test_utils.py` & `instructlab-0.16.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/tests/testdata/invalid_yaml.yaml` & `instructlab-0.16.0/tests/testdata/invalid_yaml.yaml`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/tests/testdata/knowledge_valid.yaml` & `instructlab-0.16.0/tests/testdata/knowledge_valid.yaml`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/tests/testdata/temp_repo/docs/skill-wiki.md` & `instructlab-0.16.0/tests/testdata/temp_repo/docs/skill-wiki.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/tests/testdata/temp_repo/knowledge-wiki.md` & `instructlab-0.16.0/tests/testdata/temp_repo/knowledge-wiki.md`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/tests/testdata/testdata.py` & `instructlab-0.16.0/tests/testdata/testdata.py`

 * *Files identical despite different names*

### Comparing `instructlab-0.15.1/tox.ini` & `instructlab-0.16.0/tox.ini`

 * *Files identical despite different names*

