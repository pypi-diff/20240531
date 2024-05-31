# Comparing `tmp/itwinai-0.0.1.tar.gz` & `tmp/itwinai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itwinai-0.0.1.tar", last modified: Fri May  3 15:31:15 2024, max compression
+gzip compressed data, was "itwinai-0.0.2.tar", last modified: Fri May 31 14:41:50 2024, max compression
```

## Comparing `itwinai-0.0.1.tar` & `itwinai-0.0.2.tar`

### file list

```diff
@@ -1,255 +1,280 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.696772 itwinai-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-03 15:31:10.000000 itwinai-0.0.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.660773 itwinai-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-03 15:31:10.000000 itwinai-0.0.1/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.660773 itwinai-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-03 15:31:10.000000 itwinai-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-03 15:31:10.000000 itwinai-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-03 15:31:10.000000 itwinai-0.0.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-03 15:31:10.000000 itwinai-0.0.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-03 15:31:10.000000 itwinai-0.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.660773 itwinai-0.0.1/.github/linters/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-03 15:31:10.000000 itwinai-0.0.1/.github/linters/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-03 15:31:10.000000 itwinai-0.0.1/.github/linters/.jscpd.json
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-03 15:31:10.000000 itwinai-0.0.1/.github/linters/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-03 15:31:10.000000 itwinai-0.0.1/.github/linters/mlc_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.660773 itwinai-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-03 15:31:10.000000 itwinai-0.0.1/.github/workflows/check-links.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-03 15:31:10.000000 itwinai-0.0.1/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-03 15:31:10.000000 itwinai-0.0.1/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-03 15:31:10.000000 itwinai-0.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-03 15:31:10.000000 itwinai-0.0.1/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-03 15:31:10.000000 itwinai-0.0.1/.github/workflows/sqaaas.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-05-03 15:31:10.000000 itwinai-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 15:31:10.000000 itwinai-0.0.1/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-03 15:31:10.000000 itwinai-0.0.1/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.660773 itwinai-0.0.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-03 15:31:10.000000 itwinai-0.0.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-03 15:31:10.000000 itwinai-0.0.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-03 15:31:10.000000 itwinai-0.0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-03 15:31:10.000000 itwinai-0.0.1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-03 15:31:10.000000 itwinai-0.0.1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-03 15:31:10.000000 itwinai-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-03 15:31:10.000000 itwinai-0.0.1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-03 15:31:10.000000 itwinai-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-03 15:31:10.000000 itwinai-0.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-03 15:31:15.696772 itwinai-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-05-03 15:31:10.000000 itwinai-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.664773 itwinai-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/3dgan_doc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/advanced_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/basic_comp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/basic_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/getting_started_with_itwinai.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/hpc_setup.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/intermediate_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/itwinai.cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/itwinai.cluster.rst
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/itwinai.components.rst
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/itwinai.loggers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/itwinai.parser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/itwinai.pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/itwinai.serialization.rst
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/itwinai.tf.modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/itwinai.torch.modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/itwinai.types.rst
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/itwinai.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/local_setup.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/mnist_doc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-03 15:31:10.000000 itwinai-0.0.1/docs/use_cases.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.652773 itwinai-0.0.1/env-files/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.668773 itwinai-0.0.1/env-files/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-03 15:31:10.000000 itwinai-0.0.1/env-files/tensorflow/createEnvJSCTF.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-03 15:31:10.000000 itwinai-0.0.1/env-files/tensorflow/generic_tf.sh
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-03 15:31:10.000000 itwinai-0.0.1/env-files/tensorflow/tensorflow-2.10.yml
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-03 15:31:10.000000 itwinai-0.0.1/env-files/tensorflow/tensorflow-2.11.yml
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-03 15:31:10.000000 itwinai-0.0.1/env-files/tensorflow/tensorflow-2.13-cpu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-03 15:31:10.000000 itwinai-0.0.1/env-files/tensorflow/tensorflow-2.13.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.668773 itwinai-0.0.1/env-files/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-03 15:31:10.000000 itwinai-0.0.1/env-files/torch/createEnvJSC.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-03 15:31:10.000000 itwinai-0.0.1/env-files/torch/generic_torch.sh
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-03 15:31:10.000000 itwinai-0.0.1/env-files/torch/pytorch-env-cpu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-03 15:31:10.000000 itwinai-0.0.1/env-files/torch/pytorch-env-gpu.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-03 15:31:10.000000 itwinai-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 15:31:15.696772 itwinai-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.652773 itwinai-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.668773 itwinai-0.0.1/src/itwinai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    15404 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/components.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    15681 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.672773 itwinai-0.0.1/src/itwinai/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.672773 itwinai-0.0.1/src/itwinai/tensorflow/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/tensorflow/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/tensorflow/distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.672773 itwinai-0.0.1/src/itwinai/tensorflow/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/tensorflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/tensorflow/models/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/tensorflow/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/tensorflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.672773 itwinai-0.0.1/src/itwinai/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/tests/dummy_components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.672773 itwinai-0.0.1/src/itwinai/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.672773 itwinai-0.0.1/src/itwinai/torch/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30005 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/torch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/torch/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/torch/mlflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.672773 itwinai-0.0.1/src/itwinai/torch/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/torch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/torch/models/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/torch/reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    22212 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/torch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/torch/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-03 15:31:10.000000 itwinai-0.0.1/src/itwinai/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.692772 itwinai-0.0.1/src/itwinai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-03 15:31:15.000000 itwinai-0.0.1/src/itwinai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-05-03 15:31:15.000000 itwinai-0.0.1/src/itwinai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 15:31:15.000000 itwinai-0.0.1/src/itwinai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-03 15:31:15.000000 itwinai-0.0.1/src/itwinai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-03 15:31:15.000000 itwinai-0.0.1/src/itwinai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-03 15:31:15.000000 itwinai-0.0.1/src/itwinai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.672773 itwinai-0.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.676772 itwinai-0.0.1/tests/components/
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-03 15:31:10.000000 itwinai-0.0.1/tests/components/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-03 15:31:10.000000 itwinai-0.0.1/tests/components/test_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-05-03 15:31:10.000000 itwinai-0.0.1/tests/components/test_pipe_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-03 15:31:10.000000 itwinai-0.0.1/tests/components/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-03 15:31:10.000000 itwinai-0.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-03 15:31:10.000000 itwinai-0.0.1/tests/run_on_jsc.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-03 15:31:10.000000 itwinai-0.0.1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.676772 itwinai-0.0.1/tests/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-03 15:31:10.000000 itwinai-0.0.1/tests/torch/distribtued_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-03 15:31:10.000000 itwinai-0.0.1/tests/torch/test_distribtued_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-03 15:31:10.000000 itwinai-0.0.1/tests/torch/torch_dist_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.676772 itwinai-0.0.1/tests/use-cases/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-03 15:31:10.000000 itwinai-0.0.1/tests/use-cases/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-03 15:31:10.000000 itwinai-0.0.1/tests/use-cases/test_3dgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-03 15:31:10.000000 itwinai-0.0.1/tests/use-cases/test_cyclones.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-03 15:31:10.000000 itwinai-0.0.1/tests/use-cases/test_mnist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.656773 itwinai-0.0.1/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.656773 itwinai-0.0.1/tutorials/distributed-ml/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.676772 itwinai-0.0.1/tutorials/distributed-ml/tf-scaling-test-jube/
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/tf-scaling-test-jube/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/tf-scaling-test-jube/bench_plot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/tf-scaling-test-jube/general_jobsys.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/tf-scaling-test-jube/jube_ddp.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/tf-scaling-test-jube/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.676772 itwinai-0.0.1/tutorials/distributed-ml/tf-tutorial-0-basics/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/tf-tutorial-0-basics/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/tf-tutorial-0-basics/tfmirrored_slurm.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/tf-tutorial-0-basics/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.676772 itwinai-0.0.1/tutorials/distributed-ml/tf-tutorial-1-imagenet/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/tf-tutorial-1-imagenet/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/tf-tutorial-1-imagenet/tfmirrored_slurm.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/tf-tutorial-1-imagenet/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.680772 itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.680772 itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/config/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/config/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/config/ddp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/config/deepspeed.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/config/horovod.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     9930 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/ddp_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/deepspeed_trainer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12145 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/horovod_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.680772 itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/img/
--rw-r--r--   0 runner    (1001) docker     (127)   198864 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/img/report.png
--rw-r--r--   0 runner    (1001) docker     (127)    12256 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/itwinai_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/runall.sh
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/scaling-test.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/slurm.sh
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.680772 itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-0-basics/
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-0-basics/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-0-basics/runall.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-0-basics/slurm.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-0-basics/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.684772 itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-1-mnist/
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-1-mnist/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-1-mnist/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-1-mnist/runall.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-1-mnist/slurm.sh
--rw-r--r--   0 runner    (1001) docker     (127)    15210 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-1-mnist/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.684772 itwinai-0.0.1/tutorials/ml-workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/ml-workflows/basic_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/ml-workflows/tutorial_0_basic_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/ml-workflows/tutorial_1_intermediate_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-03 15:31:10.000000 itwinai-0.0.1/tutorials/ml-workflows/tutorial_2_advanced_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.684772 itwinai-0.0.1/use-cases/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.684772 itwinai-0.0.1/use-cases/3dgan/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/3dgan/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/3dgan/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/3dgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/3dgan/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/3dgan/create_inference_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/3dgan/dataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.684772 itwinai-0.0.1/use-cases/3dgan/interLink/
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/3dgan/interLink/3dgan-inference-cpu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/3dgan/interLink/3dgan-inference.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/3dgan/interLink/3dgan-train.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/3dgan/interLink/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    30221 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/3dgan/model.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/3dgan/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/3dgan/saver.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/3dgan/startscript
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/3dgan/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.688773 itwinai-0.0.1/use-cases/cyclones/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/cyclones/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/cyclones/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    21746 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/cyclones/cyclones_vgg.py
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/cyclones/dataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.688773 itwinai-0.0.1/use-cases/cyclones/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/cyclones/lib/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/cyclones/lib/macros.py
--rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/cyclones/lib/scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/cyclones/lib/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.688773 itwinai-0.0.1/use-cases/cyclones/lib/tfrecords/
--rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/cyclones/lib/tfrecords/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/cyclones/lib/tfrecords/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/cyclones/lib/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/cyclones/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/cyclones/pipeline.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/cyclones/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/cyclones/startscript
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/cyclones/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/cyclones/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.656773 itwinai-0.0.1/use-cases/mnist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.688773 itwinai-0.0.1/use-cases/mnist/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/tensorflow/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/tensorflow/pipeline.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/tensorflow/startscript
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.692772 itwinai-0.0.1/use-cases/mnist/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/torch/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/torch/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/torch/create_inference_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/torch/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/torch/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/torch/runall.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/torch/saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/torch/slurm.sh
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/torch/startscript
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 15:31:15.692772 itwinai-0.0.1/use-cases/mnist/torch-lightning/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/torch-lightning/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/torch-lightning/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/torch-lightning/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/torch-lightning/startscript
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-03 15:31:10.000000 itwinai-0.0.1/use-cases/mnist/torch-lightning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.919058 itwinai-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-31 14:41:45.000000 itwinai-0.0.2/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.883058 itwinai-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-31 14:41:45.000000 itwinai-0.0.2/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.883058 itwinai-0.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-31 14:41:45.000000 itwinai-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-31 14:41:45.000000 itwinai-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-31 14:41:45.000000 itwinai-0.0.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-31 14:41:45.000000 itwinai-0.0.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-31 14:41:45.000000 itwinai-0.0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.883058 itwinai-0.0.2/.github/linters/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-31 14:41:45.000000 itwinai-0.0.2/.github/linters/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 14:41:45.000000 itwinai-0.0.2/.github/linters/.jscpd.json
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-31 14:41:45.000000 itwinai-0.0.2/.github/linters/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-31 14:41:45.000000 itwinai-0.0.2/.github/linters/mlc_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.887058 itwinai-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-31 14:41:45.000000 itwinai-0.0.2/.github/workflows/check-links.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-31 14:41:45.000000 itwinai-0.0.2/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-31 14:41:45.000000 itwinai-0.0.2/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-31 14:41:45.000000 itwinai-0.0.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-31 14:41:45.000000 itwinai-0.0.2/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-31 14:41:45.000000 itwinai-0.0.2/.github/workflows/sqaaas.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-31 14:41:45.000000 itwinai-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 14:41:45.000000 itwinai-0.0.2/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-31 14:41:45.000000 itwinai-0.0.2/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.887058 itwinai-0.0.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-31 14:41:45.000000 itwinai-0.0.2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-31 14:41:45.000000 itwinai-0.0.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-31 14:41:45.000000 itwinai-0.0.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-31 14:41:45.000000 itwinai-0.0.2/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 14:41:45.000000 itwinai-0.0.2/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-31 14:41:45.000000 itwinai-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-31 14:41:45.000000 itwinai-0.0.2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-31 14:41:45.000000 itwinai-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-05-31 14:41:45.000000 itwinai-0.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-05-31 14:41:50.919058 itwinai-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-31 14:41:45.000000 itwinai-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.891058 itwinai-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/3dgan_doc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/advanced_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/basic_comp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/basic_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/cyclones_doc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/ddp_why.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/getting_started_with_itwinai.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/intermediate_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/itwinai.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/itwinai.components.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/itwinai.distributed.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/itwinai.loggers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/itwinai.parser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/itwinai.pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/itwinai.serialization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/itwinai.tf.modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/itwinai.torch.modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/itwinai.type.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/itwinai.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/mnist_doc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.891058 itwinai-0.0.2/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    52973 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/notebooks/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/tf_scaling_test.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/tf_tutorial_0_basics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/tf_tutorial_1_imagenet.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/torch_scaling_test.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/torch_tutorial_0_basics.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/torch_tutorial_1_mnist.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/use_cases.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-31 14:41:45.000000 itwinai-0.0.2/docs/virgo_doc.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.875058 itwinai-0.0.2/env-files/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.891058 itwinai-0.0.2/env-files/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-31 14:41:45.000000 itwinai-0.0.2/env-files/tensorflow/createEnvJSCTF.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-31 14:41:45.000000 itwinai-0.0.2/env-files/tensorflow/generic_tf.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-31 14:41:45.000000 itwinai-0.0.2/env-files/tensorflow/tensorflow-2.10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 14:41:45.000000 itwinai-0.0.2/env-files/tensorflow/tensorflow-2.11.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-31 14:41:45.000000 itwinai-0.0.2/env-files/tensorflow/tensorflow-2.13-cpu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 14:41:45.000000 itwinai-0.0.2/env-files/tensorflow/tensorflow-2.13.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.895058 itwinai-0.0.2/env-files/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-31 14:41:45.000000 itwinai-0.0.2/env-files/torch/createEnvJSC.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-31 14:41:45.000000 itwinai-0.0.2/env-files/torch/generic_torch.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-31 14:41:45.000000 itwinai-0.0.2/env-files/torch/pytorch-env-cpu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-31 14:41:45.000000 itwinai-0.0.2/env-files/torch/pytorch-env-gpu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-31 14:41:45.000000 itwinai-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:41:50.919058 itwinai-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.875058 itwinai-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.895058 itwinai-0.0.2/src/itwinai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15722 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25930 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.899058 itwinai-0.0.2/src/itwinai/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.899058 itwinai-0.0.2/src/itwinai/tensorflow/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/tensorflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/tensorflow/distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.899058 itwinai-0.0.2/src/itwinai/tensorflow/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/tensorflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/tensorflow/models/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8425 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/tensorflow/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/tensorflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.899058 itwinai-0.0.2/src/itwinai/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/tests/dummy_components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.899058 itwinai-0.0.2/src/itwinai/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/torch/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.899058 itwinai-0.0.2/src/itwinai/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34310 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/torch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/torch/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/torch/mlflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.899058 itwinai-0.0.2/src/itwinai/torch/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/torch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/torch/models/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/torch/reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25538 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/torch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/torch/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-31 14:41:45.000000 itwinai-0.0.2/src/itwinai/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.919058 itwinai-0.0.2/src/itwinai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7653 2024-05-31 14:41:50.000000 itwinai-0.0.2/src/itwinai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-05-31 14:41:50.000000 itwinai-0.0.2/src/itwinai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:41:50.000000 itwinai-0.0.2/src/itwinai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 14:41:50.000000 itwinai-0.0.2/src/itwinai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-31 14:41:50.000000 itwinai-0.0.2/src/itwinai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 14:41:50.000000 itwinai-0.0.2/src/itwinai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.899058 itwinai-0.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.899058 itwinai-0.0.2/tests/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-31 14:41:45.000000 itwinai-0.0.2/tests/components/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-05-31 14:41:45.000000 itwinai-0.0.2/tests/components/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-05-31 14:41:45.000000 itwinai-0.0.2/tests/components/test_pipe_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-31 14:41:45.000000 itwinai-0.0.2/tests/components/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-31 14:41:45.000000 itwinai-0.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-31 14:41:45.000000 itwinai-0.0.2/tests/run_on_jsc.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-05-31 14:41:45.000000 itwinai-0.0.2/tests/test_loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-31 14:41:45.000000 itwinai-0.0.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.903058 itwinai-0.0.2/tests/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-31 14:41:45.000000 itwinai-0.0.2/tests/torch/distribtued_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-31 14:41:45.000000 itwinai-0.0.2/tests/torch/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-31 14:41:45.000000 itwinai-0.0.2/tests/torch/test_distribtued_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-31 14:41:45.000000 itwinai-0.0.2/tests/torch/torch_dist_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.903058 itwinai-0.0.2/tests/use-cases/
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-31 14:41:45.000000 itwinai-0.0.2/tests/use-cases/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-31 14:41:45.000000 itwinai-0.0.2/tests/use-cases/test_3dgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-31 14:41:45.000000 itwinai-0.0.2/tests/use-cases/test_cyclones.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-31 14:41:45.000000 itwinai-0.0.2/tests/use-cases/test_mnist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.879058 itwinai-0.0.2/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.879058 itwinai-0.0.2/tutorials/distributed-ml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.903058 itwinai-0.0.2/tutorials/distributed-ml/tf-scaling-test-jube/
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/tf-scaling-test-jube/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/tf-scaling-test-jube/bench_plot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/tf-scaling-test-jube/general_jobsys.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/tf-scaling-test-jube/jube_ddp.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/tf-scaling-test-jube/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.903058 itwinai-0.0.2/tutorials/distributed-ml/tf-tutorial-0-basics/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/tf-tutorial-0-basics/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/tf-tutorial-0-basics/tfmirrored_slurm.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/tf-tutorial-0-basics/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.903058 itwinai-0.0.2/tutorials/distributed-ml/tf-tutorial-1-imagenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/tf-tutorial-1-imagenet/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/tf-tutorial-1-imagenet/tfmirrored_slurm.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/tf-tutorial-1-imagenet/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.907058 itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.907058 itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/config/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/config/ddp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/config/deepspeed.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/config/horovod.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9930 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/ddp_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/deepspeed_trainer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12145 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/horovod_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.907058 itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   198864 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/img/report.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12256 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/itwinai_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/runall.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/scaling-test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/slurm.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.907058 itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-0-basics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-0-basics/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-0-basics/runall.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-0-basics/slurm.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-0-basics/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.907058 itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-1-mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-1-mnist/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-1-mnist/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-1-mnist/runall.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-1-mnist/slurm.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    15210 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-1-mnist/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.907058 itwinai-0.0.2/tutorials/ml-workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/ml-workflows/basic_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/ml-workflows/tutorial_0_basic_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/ml-workflows/tutorial_1_intermediate_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-31 14:41:45.000000 itwinai-0.0.2/tutorials/ml-workflows/tutorial_2_advanced_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.907058 itwinai-0.0.2/use-cases/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.911058 itwinai-0.0.2/use-cases/3dgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/3dgan/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/3dgan/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/3dgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/3dgan/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/3dgan/create_inference_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/3dgan/dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.911058 itwinai-0.0.2/use-cases/3dgan/interLink/
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/3dgan/interLink/3dgan-inference-cpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/3dgan/interLink/3dgan-inference.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/3dgan/interLink/3dgan-train.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/3dgan/interLink/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    30221 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/3dgan/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/3dgan/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/3dgan/saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/3dgan/startscript
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/3dgan/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.911058 itwinai-0.0.2/use-cases/cyclones/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/cyclones/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/cyclones/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    21746 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/cyclones/cyclones_vgg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/cyclones/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/cyclones/pipeline.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/cyclones/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.915058 itwinai-0.0.2/use-cases/cyclones/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/cyclones/src/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/cyclones/src/macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/cyclones/src/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/cyclones/src/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.915058 itwinai-0.0.2/use-cases/cyclones/src/tfrecords/
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/cyclones/src/tfrecords/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/cyclones/src/tfrecords/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/cyclones/src/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/cyclones/src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/cyclones/startscript.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/cyclones/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/cyclones/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.879058 itwinai-0.0.2/use-cases/mnist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.915058 itwinai-0.0.2/use-cases/mnist/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/tensorflow/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/tensorflow/pipeline.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/tensorflow/startscript.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.915058 itwinai-0.0.2/use-cases/mnist/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/torch/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/torch/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/torch/create_inference_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/torch/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/torch/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/torch/runall.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/torch/saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/torch/slurm.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/torch/startscript.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.915058 itwinai-0.0.2/use-cases/mnist/torch-lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/torch-lightning/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/torch-lightning/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/torch-lightning/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/torch-lightning/startscript
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/mnist/torch-lightning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.919058 itwinai-0.0.2/use-cases/virgo/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/virgo/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/virgo/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/virgo/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/virgo/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/virgo/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/virgo/runall.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/virgo/slurm.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:41:50.919058 itwinai-0.0.2/use-cases/virgo/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    14181 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/virgo/src/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14416 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/virgo/src/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/virgo/src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/virgo/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-31 14:41:45.000000 itwinai-0.0.2/use-cases/virgo/trainer.py
```

### Comparing `itwinai-0.0.1/.dockerignore` & `itwinai-0.0.2/.dockerignore`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/.github/CODE_OF_CONDUCT.md` & `itwinai-0.0.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `itwinai-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `itwinai-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/.github/ISSUE_TEMPLATE.md` & `itwinai-0.0.2/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/.github/workflows/check-links.yml` & `itwinai-0.0.2/.github/workflows/check-links.yml`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/.github/workflows/lint.yml` & `itwinai-0.0.2/.github/workflows/lint.yml`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
           # Make sure the actual branch is checked out when running on PR
           # ref: ${{ github.event.pull_request.head.sha }}
           # Full git history needed to get proper list of changed files
           fetch-depth: 0
 
       # Runs the Super-Linter action
       - name: Run Super-Linter on new changes
-        uses: super-linter/super-linter/slim@v6.3.0
+        uses: github/super-linter/slim@v6
         env:
           DEFAULT_BRANCH: main
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           MARKDOWN_CONFIG_FILE: .markdownlint.json
           PYTHON_FLAKE8_CONFIG_FILE: .flake8
           JSCPD_CONFIG_FILE: .jscpd.json
           VALIDATE_PYTHON_BLACK: false
@@ -42,14 +42,15 @@
           VALIDATE_PYTHON_MYPY: false
           VALIDATE_PYTHON_PYLINT: false
           VALIDATE_HTML: false
           VALIDATE_GITLEAKS: false
           VALIDATE_BASH_EXEC: false
           VALIDATE_CHECKOV: false # activate to lint k8s pods
           VALIDATE_SHELL_SHFMT: false
+          VALIDATE_JSCPD: false
 
           # Only check new or edited files
           VALIDATE_ALL_CODEBASE: false
           # Fail on errors
           DISABLE_ERRORS: false
           # Skip linting of docs
           FILTER_REGEX_EXCLUDE: .*docs/index.md|.*docs/docs/.*|.*ISSUE_TEMPLATE/.*|use-cases/.*|experimental/.*
```

### Comparing `itwinai-0.0.1/.github/workflows/pages.yml` & `itwinai-0.0.2/.github/workflows/pages.yml`

 * *Files 4% similar despite different names*

```diff
@@ -41,30 +41,30 @@
         with:
           ruby-version: '3.1' # Not needed with a .ruby-version file
           bundler-cache: true # runs 'bundle install' and caches installed gems automatically
           cache-version: 0 # Increment this number if you need to re-download cached gems
           working-directory: '${{ github.workspace }}/docs'
       - name: Setup Pages
         id: pages
-        uses: actions/configure-pages@v3
+        uses: actions/configure-pages@v5
       - name: Build with Jekyll
         # Outputs to the './_site' directory by default
         run: bundle exec jekyll build --baseurl "${{ steps.pages.outputs.base_path }}"
         env:
           JEKYLL_ENV: production
       - name: Upload artifact
         # Automatically uploads an artifact from the './_site' directory by default
-        uses: actions/upload-pages-artifact@v2
+        uses: actions/upload-pages-artifact@v3
         with:
           path: "docs/_site/"
 
   # Deployment job
   deploy:
     environment:
       name: github-pages
       url: ${{ steps.deployment.outputs.page_url }}
     runs-on: ubuntu-latest
     needs: build
     steps:
       - name: Deploy to GitHub Pages
         id: deployment
-        uses: actions/deploy-pages@v2
+        uses: actions/deploy-pages@v4
```

### Comparing `itwinai-0.0.1/.github/workflows/pypi.yml` & `itwinai-0.0.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/.github/workflows/pytest.yml` & `itwinai-0.0.2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/.github/workflows/sqaaas.yml` & `itwinai-0.0.2/.github/workflows/sqaaas.yml`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/.gitignore` & `itwinai-0.0.2/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 *-data/
 *.tar.gz
 *.pth
 *.csv
 *tar.gz
 0
 *.tar
+*.sif
 
 # Use cases files
 MNIST
 3dgan-generated-data/
 mnist-sample-data/
 exp_data/
```

### Comparing `itwinai-0.0.1/.readthedocs.yaml` & `itwinai-0.0.2/.readthedocs.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,19 @@
   os: ubuntu-22.04
   tools:
     python: "3.10"
     # You can also specify other tool versions:
     # nodejs: "19"
     # rust: "1.64"
     # golang: "1.19"
+  apt_packages:
+    - gcc-11
+    - g++-11
+    - cmake
+    - pandoc
 
 # Build documentation in the "docs/" directory with Sphinx
 sphinx:
   configuration: docs/conf.py
 
 # Optionally build your docs in additional formats such as PDF and ePub
 # formats:
@@ -25,8 +30,9 @@
 #    - epub
 
 # Optional but recommended, declare the Python requirements required
 # to build your documentation
 # See https://docs.readthedocs.io/en/stable/guides/reproducible-builds.html
 python:
    install:
+  #  - wheel
    - requirements: docs/requirements.txt
```

### Comparing `itwinai-0.0.1/.vscode/settings.json` & `itwinai-0.0.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/CONTRIBUTING.md` & `itwinai-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/LICENSE` & `itwinai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/Makefile` & `itwinai-0.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/PKG-INFO` & `itwinai-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: itwinai
-Version: 0.0.1
+Version: 0.0.2
 Summary: AI and ML workflows module for scientific digital twins.
-Author-email: Matteo Bunino <matteo.bunino@cern.ch>, Alexander Zoechbauer <alexander.zoechbauer@cern.ch>, Rakesh Sarma <r.sarma@fz-juelich.de>, Mario Ruettgers <m.ruettgers@fz-juelich.de>, Eric Wulff <eric.wulff@cern.ch>
-Maintainer-email: Matteo Bunino <matteo.bunino@cern.ch>, Alexander Zoechbauer <alexander.zoechbauer@cern.ch>, Rakesh Sarma <r.sarma@fz-juelich.de>, Mario Ruettgers <m.ruettgers@fz-juelich.de>
+Author-email: Matteo Bunino <matteo.bunino@cern.ch>, Rakesh Sarma <r.sarma@fz-juelich.de>, Mario Ruettgers <m.ruettgers@fz-juelich.de>, Kalliopi Tsolaki <kalliopi.tsolaki@cern.ch>
+Maintainer-email: Matteo Bunino <matteo.bunino@cern.ch>, Rakesh Sarma <r.sarma@fz-juelich.de>, Mario Ruettgers <m.ruettgers@fz-juelich.de>, Kalliopi Tsolaki <kalliopi.tsolaki@cern.ch>
 License: MIT License
         
         Copyright (c) 2023 interTwin Community
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -28,43 +28,45 @@
         
 Project-URL: Homepage, https://www.intertwin.eu/
 Project-URL: Documentation, https://itwinai.readthedocs.io/
 Project-URL: Repository, https://github.com/interTwin-eu/itwinai
 Keywords: ml,ai,hpc
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: wandb
 Requires-Dist: mlflow
 Requires-Dist: jsonargparse[signatures]
 Requires-Dist: pyyaml
 Requires-Dist: omegaconf
 Requires-Dist: rich>=13.5.3
 Requires-Dist: typer>=0.9.0
 Requires-Dist: wheel
+Requires-Dist: pydantic
 Provides-Extra: torch
 Requires-Dist: lightning; extra == "torch"
 Requires-Dist: torchmetrics; extra == "torch"
 Provides-Extra: dev
 Requires-Dist: pytest>=7.4.2; extra == "dev"
 Requires-Dist: pytest-mock>=3.11.1; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
+Requires-Dist: tensorflow==2.15; extra == "dev"
 
 # itwinai
 
 [![GitHub Super-Linter](https://github.com/interTwin-eu/T6.5-AI-and-ML/actions/workflows/lint.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)
 [![GitHub Super-Linter](https://github.com/interTwin-eu/T6.5-AI-and-ML/actions/workflows/check-links.yml/badge.svg)](https://github.com/marketplace/actions/markdown-link-check)
  [![SQAaaS source code](https://github.com/EOSC-synergy/itwinai.assess.sqaaas/raw/dev/.badge/status_shields.svg)](https://sqaaas.eosc-synergy.eu/#/full-assessment/report/https://raw.githubusercontent.com/eosc-synergy/itwinai.assess.sqaaas/dev/.report/assessment_output.json)
 
-See the latest version of our [docs](https://intertwin-eu.github.io/itwinai/)
+See the latest version of our [docs](https://itwinai.readthedocs.io/)
 for a quick overview of this platform for advanced AI/ML workflows in digital twin applications.
 
 ## Installation
 
 Requirements:
 
 - Linux environment. Windows and macOS were never tested.
```

### Comparing `itwinai-0.0.1/README.md` & `itwinai-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # itwinai
 
 [![GitHub Super-Linter](https://github.com/interTwin-eu/T6.5-AI-and-ML/actions/workflows/lint.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)
 [![GitHub Super-Linter](https://github.com/interTwin-eu/T6.5-AI-and-ML/actions/workflows/check-links.yml/badge.svg)](https://github.com/marketplace/actions/markdown-link-check)
  [![SQAaaS source code](https://github.com/EOSC-synergy/itwinai.assess.sqaaas/raw/dev/.badge/status_shields.svg)](https://sqaaas.eosc-synergy.eu/#/full-assessment/report/https://raw.githubusercontent.com/eosc-synergy/itwinai.assess.sqaaas/dev/.report/assessment_output.json)
 
-See the latest version of our [docs](https://intertwin-eu.github.io/itwinai/)
+See the latest version of our [docs](https://itwinai.readthedocs.io/)
 for a quick overview of this platform for advanced AI/ML workflows in digital twin applications.
 
 ## Installation
 
 Requirements:
 
 - Linux environment. Windows and macOS were never tested.
```

### Comparing `itwinai-0.0.1/docs/Makefile` & `itwinai-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/docs/conf.py` & `itwinai-0.0.2/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,36 +6,47 @@
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 import os
 import sys
 import subprocess
 
-sys.path.insert(0, os.path.abspath('../use-cases/'))
-sys.path.insert(0, os.path.abspath('../use-cases/3dgan/'))
-sys.path.insert(0, os.path.abspath('../use-cases/mnist/torch-lightning/'))
-sys.path.insert(0, os.path.abspath('../use-cases/mnist/torch/'))
+exclude_patterns = 'requirements.txt'
+
+# sys.path.insert(0, os.path.abspath('../use-cases/'))
+# sys.path.insert(0, os.path.abspath('../use-cases/3dgan/'))
+# sys.path.insert(0, os.path.abspath('../use-cases/mnist/torch-lightning/'))
+# sys.path.insert(0, os.path.abspath('../use-cases/mnist/torch/'))
 sys.path.insert(0, os.path.abspath('../tutorials/ml-workflows/'))
-sys.path.insert(0, os.path.abspath('../src/itwinai'))
-sys.path.insert(0, os.path.abspath('../src/itwinai/tensorflow'))
-sys.path.insert(0, os.path.abspath('../src/itwinai/torch'))
-sys.path.insert(0, os.path.abspath('../'))
+# sys.path.insert(0, os.path.abspath('../tutorials/distributed-ml/'))
+# sys.path.insert(0, os.path.abspath('../src/itwinai'))
+# sys.path.insert(0, os.path.abspath('../src/itwinai/tensorflow'))
+# sys.path.insert(0, os.path.abspath('../src/itwinai/torch'))
+sys.path.insert(0, os.path.abspath('../src'))
+# sys.path.insert(0, os.path.abspath('../...'))
 
 project = 'itwinai'
-copyright = ('2024, Matteo Bunino, Alexander Zoechbauer, '
-             'Kalliopi Tsolaki, Rakesh Sarma on behalf of CERN & JSC')
-author = 'Matteo Bunino, Alexander Zoechbauer, Kalliopi Tsolaki'
-# version = '0.0'  # short version
-# release = '0.0.2'  # full version
+copyright = ('2024, Matteo Bunino, Kalliopi Tsolaki,'
+             'Rakesh Sarma, Mario Ruettgers on behalf of CERN & JSC')
+author = 'Matteo Bunino, Kalliopi Tsolaki, Rakesh Sarma, Mario Ruettgers'
+version = '0.0'  # short version
+release = '0.0.2'  # full version
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.doctest',
-              'sphinx.ext.viewcode']  # 'myst_parser'
+              'sphinx.ext.viewcode', 'myst_parser', 'nbsphinx']
+
+source_suffix = {
+    '.rst': 'restructuredtext',
+    '.txt': 'markdown',
+    '.md': 'markdown'  # ,
+    # '.ipynb': 'nbsphinx'
+}
 
 templates_path = ['_templates']
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 autodoc_mock_imports = ["mlflow"]
 
 # -- Options for HTML output -------------------------------------------------
```

### Comparing `itwinai-0.0.1/docs/getting_started_with_itwinai.rst` & `itwinai-0.0.2/docs/getting_started_with_itwinai.rst`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/docs/index.rst` & `itwinai-0.0.2/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 .. itwinai documentation master file, created by
    sphinx-quickstart on Fri Feb  9 13:58:30 2024.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
-🚧 UNDER CONSTRUCTION 🚧
-=========================
-
 Welcome to itwinai's documentation!
 ===================================
 
 ``itwinai`` is a framework for advanced AI/ML workflows in Digital Twins (DTs).
 
 This platform is intended to support general-purpose MLOps for Digital Twin use cases in the `interTwin <https://www.intertwin.eu/>`_ project.
 
@@ -33,38 +30,52 @@
    :caption: 💡 Installation
 
    getting_started_with_itwinai
 
 .. toctree::
    :maxdepth: 2
    :hidden:
-   :caption: 🪄 itwinai Modules
+   :caption: 🪄 Itwinai how it works
 
-   modules
+   ddp_why
 
 .. toctree::
    :maxdepth: 2
    :hidden:
-   :caption: 📚 Integrated Use-cases
+   :caption: 📚 Integrated Use Cases
 
    use_cases
 
 .. toctree::
    :maxdepth: 2
    :hidden:
    :caption: 🚀 Tutorials
 
    tutorials
 
-   
+.. toctree::
+   :maxdepth: 2
+   :hidden:
+   :caption: ⚡ Python API reference
+
+   modules
+
+.. .. toctree::
+..    :maxdepth: 2
+..    :hidden:
+..    :caption: Additional resources
+
+..    notebooks/example
+
+
 `interTwin Demo: itwinai integration with other DTE modules <https://www.youtube.com/watch?v=NoVCfSxwtX0>`_
 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 
 
 Indices and tables
-==================
+++++++++++++++++++
 
 * :ref:`genindex`
 * :ref:`modindex`
 
 .. * :ref:`search`
```

### Comparing `itwinai-0.0.1/docs/make.bat` & `itwinai-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/env-files/tensorflow/createEnvJSCTF.sh` & `itwinai-0.0.2/env-files/tensorflow/createEnvJSCTF.sh`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 cDir=$PWD
 sysN="$(uname -n | cut -f2- -d.)"
 echo "system:${sysN}"
 echo
 
 cont1=false
 if [ "$sysN" = 'hdfml' ] ; then
-  ml Stages/2024 GCC/12.3.0 OpenMPI CUDA/12 MPI-settings/CUDA Python HDF5 PnetCDF libaio mpi4py CMake cuDNN/8.9.5.29-CUDA-12
+  ml Stages/2024 GCC/12.3.0 OpenMPI CUDA/12 MPI-settings/CUDA Python/3.11 HDF5 PnetCDF libaio mpi4py CMake cuDNN/8.9.5.29-CUDA-12
   cont1=true
 else
   echo
   echo 'unknown system detected'
   echo 'canceling'
   echo
 fi
```

### Comparing `itwinai-0.0.1/env-files/tensorflow/generic_tf.sh` & `itwinai-0.0.2/env-files/tensorflow/generic_tf.sh`

 * *Files 10% similar despite different names*

```diff
@@ -41,20 +41,19 @@
 pip3 install --no-cache-dir wheel
 
 # install TF 
 if [ -f "${cDir}/$ENV_NAME/bin/tensorboard" ]; then
   echo 'TF already installed'
   echo
 else
-  # export TMPDIR=${cDir}
   if [ -z "$NO_CUDA" ]; then
-    pip3 install --upgrade tensorflow[and-cuda]==2.13.* --no-cache-dir
+    pip3 install tensorflow[and-cuda]==2.15 --no-cache-dir
   else
     # CPU only installation
-    pip3 install --upgrade tensorflow==2.13.* --no-cache-dir
+    pip3 install tensorflow==2.15 --no-cache-dir
   fi
 fi
 
 # CURRENTLY, horovod is not used with TF. Skipped.
 # # install horovod
 # if [ -f "${cDir}/$ENV_NAME/bin/horovodrun" ]; then
 #   echo 'Horovod already installed'
```

### Comparing `itwinai-0.0.1/env-files/torch/createEnvJSC.sh` & `itwinai-0.0.2/env-files/torch/createEnvJSC.sh`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/env-files/torch/generic_torch.sh` & `itwinai-0.0.2/env-files/torch/generic_torch.sh`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/pyproject.toml` & `itwinai-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,32 +4,31 @@
 
 [build-system]
 requires = ["setuptools", "setuptools-scm", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "itwinai"
-version = "0.0.1"
+version = "0.0.2"
 description = "AI and ML workflows module for scientific digital twins."
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.10"
 license = { file = "LICENSE" }
 keywords = ["ml", "ai", "hpc"]
 authors = [
     { name = "Matteo Bunino", email = "matteo.bunino@cern.ch" },
-    { name = "Alexander Zoechbauer", email = "alexander.zoechbauer@cern.ch" },
     { name = "Rakesh Sarma", email = "r.sarma@fz-juelich.de" },
     { name = "Mario Ruettgers", email = "m.ruettgers@fz-juelich.de" },
-    { name = "Eric Wulff", email = "eric.wulff@cern.ch" },
+    { name = "Kalliopi Tsolaki", email = "kalliopi.tsolaki@cern.ch" },
 ]
 maintainers = [
     { name = "Matteo Bunino", email = "matteo.bunino@cern.ch" },
-    { name = "Alexander Zoechbauer", email = "alexander.zoechbauer@cern.ch" },
     { name = "Rakesh Sarma", email = "r.sarma@fz-juelich.de" },
     { name = "Mario Ruettgers", email = "m.ruettgers@fz-juelich.de" },
+    { name = "Kalliopi Tsolaki", email = "kalliopi.tsolaki@cern.ch" },
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python",
 ]
 
 dependencies = [
@@ -37,14 +36,15 @@
     "mlflow",
     "jsonargparse[signatures]",
     "pyyaml",
     "omegaconf",
     "rich>=13.5.3",
     "typer>=0.9.0",
     "wheel",
+    "pydantic",
 ]
 
 # dynamic = ["version", "description"]
 
 [project.optional-dependencies]
 torch = ["lightning", "torchmetrics"]
 # torch-cpu = [
@@ -57,14 +57,15 @@
 # ]
 dev = [
     "pytest>=7.4.2",
     "pytest-mock>=3.11.1",
     "pytest-cov>=4.1.0",
     "ipykernel",
     "ipython",
+    "tensorflow==2.15",    # needed by tests on tensorboard
 ]
 
 [project.urls]
 Homepage = "https://www.intertwin.eu/"
 Documentation = "https://itwinai.readthedocs.io/"
 Repository = "https://github.com/interTwin-eu/itwinai"
 # Changelog = "https://github.com/me/spam/blob/master/CHANGELOG.md"
```

### Comparing `itwinai-0.0.1/src/itwinai/cli.py` & `itwinai-0.0.2/src/itwinai/cli.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/src/itwinai/components.py` & `itwinai-0.0.2/src/itwinai/components.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,28 +87,37 @@
 from typing import Any, Optional, Tuple, Union, Callable, Dict, List
 from abc import ABC, abstractmethod
 import time
 import functools
 # import logging
 # from logging import Logger as PythonLogger
 
-from .types import MLModel, MLDataset, MLArtifact
+from .type import MLModel, MLDataset, MLArtifact
 from .serialization import ModelLoader, Serializable
+from .distributed import (
+    detect_distributed_environment,
+    distributed_patch_print
+)
 
 
 def monitor_exec(method: Callable) -> Callable:
     """Decorator for execute method of a component class.
     Computes execution time and gives some information about
     the execution of the component.
 
     Args:
         func (Callable): class method.
     """
     @functools.wraps(method)
     def monitored_method(self: BaseComponent, *args, **kwargs) -> Any:
+        # Disable print in workers different from the main one,
+        # when in distributed environments.
+        dist_grank = detect_distributed_environment().global_rank
+        distributed_patch_print(is_main=dist_grank == 0)
+
         msg = f"Starting execution of '{self.name}'..."
         self._printout(msg)
         start_t = time.time()
         try:
             # print(f'ARGS: {args}')
             # print(f'KWARGS: {kwargs}')
             result = method(self, *args, **kwargs)
@@ -239,19 +248,19 @@
         model: Optional[MLModel] = None
     ) -> MLDataset:
         """Applies a machine learning model on a dataset of samples.
 
         Args:
             predict_dataset (MLDataset): dataset for inference.
             model (Optional[MLModel], optional): overrides the internal model,
-                if given. Defaults to None.
+            if given. Defaults to None.
 
         Returns:
             MLDataset: predictions with the same cardinality of the
-                input dataset.
+            input dataset.
         """
 
 
 class DataGetter(BaseComponent):
     """Retrieves a dataset."""
 
     @abstractmethod
@@ -260,15 +269,15 @@
         """Retrieves a dataset.
 
         Returns:
             MLDataset: retrieved dataset.
         """
 
 
-class DataPreproc(BaseComponent):
+class DataProcessor(BaseComponent):
     """Performs dataset pre-processing."""
 
     @abstractmethod
     @monitor_exec
     def execute(
         self,
         train_dataset: MLDataset,
```

### Comparing `itwinai-0.0.1/src/itwinai/parser.py` & `itwinai-0.0.2/src/itwinai/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     config: Dict,
     key_chain: str,
     value: Any
 ) -> None:
     """Replace or add (if not present) a field in a dictionary, following a
     path of dot-separated keys. Adding is not supported for list items.
     Inplace operation.
+
     Args:
         config (Dict): dictionary to be modified.
         key_chain (str): path of nested (dot-separated) keys to specify the
         location
         of the new value (e.g., 'foo.bar.line' adds/overwrites the value
         located at config['foo']['bar']['line']).
         value (Any): the value to insert.
@@ -57,20 +58,24 @@
 
 
 class ConfigParser:
     """
     Parses a pipeline from a configuration file.
     It also provides functionalities for dynamic override
     of fields by means of nested key notation.
+
     Args:
         config (Union[str, Dict]): path to YAML configuration file
         or dict storing a configuration.
         override_keys (Optional[Dict[str, Any]], optional): dict mapping
         nested keys to the value to override. Defaults to None.
+
     Example:
+
+
     >>> # pipeline.yaml file
     >>> pipeline:
     >>>   class_path: itwinai.pipeline.Pipeline
     >>>   init_args:
     >>>     steps:
     >>>       - class_path: dataloader.MNISTDataModuleTorch
     >>>         init_args:
@@ -92,14 +97,15 @@
     >>> pipeline = parser.parse_pipeline()
     >>> print(pipeline)
     >>> print(pipeline.steps)
     >>>
     >>> dataloader = parser.parse_step(0)
     >>> print(dataloader)
     >>> print(dataloader.save_path)
+
     """
 
     config: Dict
     pipeline: Pipeline
 
     def __init__(
         self,
@@ -127,20 +133,22 @@
 
     def parse_pipeline(
         self,
         pipeline_nested_key: str = "pipeline",
         verbose: bool = False
     ) -> Pipeline:
         """Merges steps into pipeline and parses it.
+
         Args:
             pipeline_nested_key (str, optional): nested key in the
             configuration file identifying the pipeline object.
             Defaults to "pipeline".
             verbose (bool): if True, prints the assembled pipeline
             to console formatted as JSON.
+
         Returns:
             Pipeline: instantiated pipeline.
         """
         pipe_parser = JAPArgumentParser()
         pipe_parser.add_subclass_arguments(Pipeline, "pipeline")
 
         pipe_dict = self.config
@@ -237,7 +245,9 @@
             dump_header=dump_header, default_config_files=default_config_files,
             default_env=default_env,
             default_meta=default_meta, **kwargs)
         self.add_argument(
             "-c", "--config", action=ActionConfigFile,
             help="Path to a configuration file in json or yaml format."
         )
+
+# type: ignore
```

### Comparing `itwinai-0.0.1/src/itwinai/pipeline.py` & `itwinai-0.0.2/src/itwinai/pipeline.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/src/itwinai/serialization.py` & `itwinai-0.0.2/src/itwinai/serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict, Any, Union
 import abc
 import json
 import yaml
 from pathlib import Path
 import inspect
 
-from .types import MLModel
+from .type import MLModel
 from .utils import SignatureInspector
 
 
 def is_jsonable(x):
     try:
         json.dumps(x)
         return True
```

### Comparing `itwinai-0.0.1/src/itwinai/tensorflow/distributed.py` & `itwinai-0.0.2/src/itwinai/tensorflow/distributed.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,39 @@
+"""
+TensorFlow distributed strategies.
+"""
+
+from typing import Tuple
 import os
 import tensorflow as tf
 import tensorflow.distribute as dist
 
 
-def get_strategy():
-    """Strategy for distributed TensorFlow training"""
-    if not os.environ.get('SLURM_JOB_ID'):
-        # TODO: improve
-        print('not in SLURM env!')
-        tf_dist_strategy = dist.MirroredStrategy()
-        return tf_dist_strategy, tf_dist_strategy.num_replicas_in_sync
+def get_strategy() -> Tuple[tf.distribute.Strategy, int]:
+    """Strategy for distributed TensorFlow training. It will automatically
+    detect if you are running in a multi-node environment, returning the
+    correct TensorFlow distributed strategy for data parallel distributed
+    training.
+
+    Returns:
+        Tuple[tf.distribute.Strategy, int]: strategy and number of parallel
+        workers. See:
+        https://stackoverflow.com/questions/66005641/why-we-are-using-strategy-num-replicas-in-sync).
+    """
+
+    slurm_jobid = os.environ.get('SLURM_JOB_ID')
+    slurm_nnodes = int(os.environ.get('SLURM_NNODES', 0))
+    if not slurm_jobid or slurm_nnodes < 2:
+        # Single-node environment
+        print('Not in SLURM env! Assuming that you '
+              'are running on a single node')
+        mirrored_strategy = dist.MirroredStrategy()
+        return mirrored_strategy, mirrored_strategy.num_replicas_in_sync
+
+    # Multi-node environment in SLURM
     cluster_resolver = dist.cluster_resolver.SlurmClusterResolver(
         port_base=12345)
     implementation = dist.experimental.CommunicationImplementation.NCCL
     communication_options = dist.experimental.CommunicationOptions(
         implementation=implementation)
 
     # declare distribution strategy
```

### Comparing `itwinai-0.0.1/src/itwinai/tensorflow/models/mnist.py` & `itwinai-0.0.2/src/itwinai/tensorflow/models/mnist.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/src/itwinai/tensorflow/trainer.py` & `itwinai-0.0.2/src/itwinai/tensorflow/trainer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,241 +1,213 @@
 """Base TensorFlow trainer module."""
-from typing import Dict, Any
+from typing import Dict, Any, Optional, List, Union
 
 from jsonargparse import ArgumentParser
 import tensorflow as tf
+from tensorflow.data import Dataset
+from keras.callbacks import Callback
 
 from ..components import Trainer, monitor_exec
 from itwinai.tensorflow.distributed import get_strategy
 
 
 def import_class(name):
     components = name.split('.')
     mod = __import__(components[0])
     for comp in components[1:]:
         mod = getattr(mod, comp)
     return mod
 
 
-def instance_from_dict(obj_dict: Any) -> Any:
+def instance_from_dict(obj_dict: Dict, fail_untyped: bool = True) -> Any:
     if isinstance(obj_dict, dict) and obj_dict.get('class_path') is not None:
         # obj_dict is a dictionary with a structure compliant with
         # jsonargparse
         obj_class = import_class(obj_dict["class_path"])
         parser = ArgumentParser()
-        parser.add_subclass_arguments(obj_class, "object")
+        parser.add_subclass_arguments(
+            obj_class, "object", fail_untyped=fail_untyped)
         obj_dict = {"object": obj_dict}
         return parser.instantiate_classes(obj_dict).object
-    return obj_dict
 
-
-# TODO: the TF trainer is incomplete:
-#   - strategy is not received from constructor argument: if not needed,
-#     remove it
-#   - dataset is not distributed
-#   - much commented code that has to be removed or included
+    raise ValueError(
+        "Unable to instantiate object with this "
+        f"dict configuration: {obj_dict}.\nIt should have "
+        "valid 'class_path' and 'init_args' fields"
+    )
 
 
 class TensorflowTrainer(Trainer):
+    """Trains a Keras model.
+
+        Args:
+            epochs (int): number of training epochs.
+            micro_batch_size (int): per-worker batch size. Equals macro batch
+            size when not running distributed.
+            shuffle_buffer (Optional[int], optional): if given, shuffles
+            dataset using a buffer of given size. See
+            ``tf.data.Dataset.shuffle``. Defaults to None.
+            callbacks (Optional[List], optional): list fo Keras callbacks.
+            Can be a list of dictionary configurations. Defaults to None.
+            model_config (Optional[Dict], optional): model configuration. If
+            given, a model is instantiated from this configuration.
+            Defaults to None.
+            model_compile_config (Optional[Dict], optional): configuration for
+            ``keras.Model.compile``. Defaults to None.
+            rnd_seed (Optional[int], optional): random seed. Defaults to None.
+            verbose (Union[str, int], optional): verbosity level for
+            ``keras.Model.fit``. Defaults to 'auto'.
+    """
+
+    strategy: tf.distribute.Strategy
+    num_workers: int
+    callbacks: Optional[List] = None
+    epochs: int
+    shuffle_buffer: Optional[int]
+    micro_batch_size: int
+    macro_batch_size: int
+    rnd_seed: Optional[int]
+
     def __init__(
-            self,
-            epochs,
-            # train_dataset,
-            # validation_dataset,
-            batch_size,
-            callbacks,
-            model_dict: Dict,
-            compile_conf,
-            strategy
+        self,
+        epochs: int,
+        micro_batch_size: int,
+        shuffle_buffer: Optional[int] = None,
+        callbacks: Optional[List[Union[Dict, Callback]]] = None,
+        model_config: Optional[Dict] = None,
+        model_compile_config: Optional[Dict] = None,
+        rnd_seed: Optional[int] = None,
+        verbose: Union[str, int] = 'auto'
     ):
         super().__init__()
         self.save_parameters(**self.locals2params(locals()))
-        self.strategy = strategy
         self.epochs = epochs
-        self.batch_size = batch_size
-        self.callbacks = callbacks
+        self.micro_batch_size = micro_batch_size
+        self.shuffle_buffer = shuffle_buffer
+        self.rnd_seed = rnd_seed
+        self.verbose = verbose
+        if callbacks is not None:
+            self.callbacks = self.instantiate_callbacks(callbacks)
+        else:
+            self.callbacks = []
 
-        # # Handle the parsing
-        # model_class = import_class(model_dict["class_path"])
-        # parser = ArgumentParser()
-        # parser.add_subclass_arguments(model_class, "model")
-        # model_dict = {"model": model_dict}
-
-        # from itwinai.models.tensorflow.mnist import MNIST_Model
-
-        # Create distributed TF vars
-        if self.strategy:
-            tf_dist_strategy, n_devices = get_strategy()
-            # get total number of workers
-            print("Number of devices: {}".format(n_devices))
-            # distribute datasets among MirroredStrategy's replicas
-            # dist_train_dataset = (
-            #     tf_dist_strategy.experimental_distribute_dataset(
-            #         train_dataset
-            #     ))
-            # dist_validation_dataset = (
-            #     tf_dist_strategy.experimental_distribute_dataset(
-            #         validation_dataset
-            #     ))
-            with self.strategy.scope():
-                # TODO: move loss, optimizer and metrics instantiation under
-                # here
-                # Ref:
-                # https://www.tensorflow.org/guide/distributed_training#use_tfdistributestrategy_with_keras_modelfit
-                # self.model: tf.keras.Model = parser.instantiate_classes(
-                #     model_dict).model
-                # TODO: add dataloaders and model instances
-                self.model: tf.keras.Model = instance_from_dict(model_dict)
-                compile_conf = self.instantiate_compile_conf(compile_conf)
-                self.model.compile(**compile_conf)
-                # print(self.model)
-                # self.model.compile(**compile_conf)
-
-                # self.model = tf.keras.Sequential([
-                #     tf.keras.layers.Conv2D(
-                #         32, 3, activation='relu', input_shape=(28, 28, 1)),
-                #     tf.keras.layers.MaxPooling2D(),
-                #     tf.keras.layers.Flatten(),
-                #     tf.keras.layers.Dense(64, activation='relu'),
-                #     tf.keras.layers.Dense(10)
-                # ])
-                # self.model = MNIST_Model()
-                # self.model.compile(loss='mse', optimizer='sgd')
-                # self.model.compile(loss=tf.keras.losses.CategoricalCrossentropy(from_logits=False),
-                #                    optimizer=tf.keras.optimizers.Adam(
-                #     learning_rate=0.001),
-                #     metrics=['accuracy'])
+        # Distributed strategy
+        self.strategy, self.num_workers = get_strategy()
+        print(
+            f"Distributed strategy is working with: {self.num_workers} devices"
+        )
+        self.macro_batch_size = self.micro_batch_size * self.num_workers
 
+        # Compile model from configuration, if given
+        if model_config is not None and model_compile_config is not None:
+            with self.strategy.scope():
+                self.model: tf.keras.Model = instance_from_dict(model_config)
+                model_compile_config = self.instantiate_compile_conf(
+                    model_compile_config
+                )
+                self.model.compile(**model_compile_config)
         else:
-            self.model: tf.keras.Model = instance_from_dict(model_dict)
-            compile_conf = self.instantiate_compile_conf(compile_conf)
-            self.model.compile(**compile_conf)
-
-        self.num_devices = (
-            self.strategy.num_replicas_in_sync if self.strategy else 1)
-        print(f"Strategy is working with: {self.num_devices} devices")
+            print(
+                "Either model_config or model_compile_config were not given. "
+                "Skipping automatic model compilation."
+            )
 
     @staticmethod
     def instantiate_compile_conf(conf: Dict) -> Dict:
+        final_conf = {}
         for item_name, item in conf.items():
-            conf[item_name] = instance_from_dict(item)
-        return conf
+            if isinstance(item, dict):
+                item = instance_from_dict(item)
+            final_conf[item_name] = item
+        return final_conf
 
-    @monitor_exec
-    def execute(self, train_dataset, validation_dataset) -> Any:
-        # Set batch size to the dataset
-        # train = train.batch(self.batch_size, drop_remainder=True)
-        # test = test.batch(self.batch_size, drop_remainder=True)
-
-        # Number of samples
-        # n_train = train.cardinality().numpy()
-        # n_test = test.cardinality().numpy()
-        print(
-            f"TRAIN CARD: {train_dataset.cardinality().numpy()} - "
-            f"LEN: {len(train_dataset)}")
-        print(next(iter(train_dataset)))
-        print(type(train_dataset))
-        # n_train = len(train) // self.batch_size
-        # n_test = len(test) // self.batch_size
-
-        # TODO: read
-        # https://github.com/tensorflow/tensorflow/issues/56773#issuecomment-1188693881
-        # https://www.tensorflow.org/guide/distributed_training#use_tfdistributestrategy_with_keras_modelfit
-
-        # # Distribute dataset
-        # if self.strategy:
-        #     train = self.strategy.experimental_distribute_dataset(train)
-        #     test = self.strategy.experimental_distribute_dataset(test)
-
-        assert isinstance(train_dataset, tf.data.Dataset)
-
-        # train the model
-        history = self.model.fit(
-            train_dataset.batch(self.batch_size),
-            validation_data=validation_dataset.batch(self.batch_size),
-            # steps_per_epoch=int(n_train // self.num_devices),
-            # validation_steps=int(n_test // self.num_devices),
-            epochs=self.epochs,
-            callbacks=self.callbacks,
-            # batch_size=self.batch_size
-        )
+    @staticmethod
+    def instantiate_callbacks(callbacks: List) -> List:
+        final_callbacks = []
+        for item in callbacks:
+            if isinstance(item, dict):
+                # Not all constructor args in keras callbacks
+                # are typed!
+                item = instance_from_dict(item, fail_untyped=False)
+            final_callbacks.append(item)
+        return final_callbacks
 
-        print("Model trained")
-        return history
+    @monitor_exec
+    def execute(
+        self,
+        train_dataset: Dataset,
+        validation_dataset: Dataset,
+        test_dataset: Optional[Dataset] = None
+    ) -> Any:
+
+        print(f"len(train_dataset): {len(train_dataset)}")
+        print(f"len(validation_dataset): {len(validation_dataset)}")
+        print("micro_batch_size: ", self.micro_batch_size, flush=True)
+        print("macro_batch_size: ", self.macro_batch_size, flush=True)
+
+        # Shuffle dataset
+        if self.shuffle_buffer:
+            train_ds = train_dataset.shuffle(
+                self.shuffle_buffer, seed=self.rnd_seed)
+            valid_ds = validation_dataset.shuffle(
+                self.shuffle_buffer, seed=self.rnd_seed)
+        else:
+            train_ds = train_dataset
+            valid_ds = validation_dataset
 
+        # Set batch size to the dataset and repeat
+        train_ds = train_ds.batch(
+            self.macro_batch_size, drop_remainder=True,
+            num_parallel_calls=tf.data.AUTOTUNE
+        ).repeat(self.epochs)
+        valid_ds = valid_ds.batch(
+            self.macro_batch_size, drop_remainder=True,
+            num_parallel_calls=tf.data.AUTOTUNE
+        ).repeat(self.epochs)
+
+        print(f"len(train_ds): {len(train_ds)}")
+        print(f"len(valid_ds): {len(valid_ds)}")
+
+        # Distribute datasets among strategy's replica
+        dist_train_dataset = self.strategy.experimental_distribute_dataset(
+            train_ds
+        )
+        dist_valid_dataset = self.strategy.experimental_distribute_dataset(
+            valid_ds
+        )
 
-# class TensorflowTrainer2(Trainer):
-#     def __init__(
-#             self,
-#             epochs,
-#             batch_size,
-#             callbacks,
-#             model_dict: Dict,
-#             compile_conf,
-#             strategy
-#     ):
-#         super().__init__()
-#         self.strategy = strategy
-#         self.epochs = epochs
-#         self.batch_size = batch_size
-#         self.callbacks = callbacks
-
-#         # Handle the parsing
-#         model_class = import_class(model_dict["class_path"])
-#         parser = ArgumentParser()
-#         parser.add_subclass_arguments(model_class, "model")
-#         model_dict = {"model": model_dict}
-
-#         # Create distributed TF vars
-#         if self.strategy:
-#             with self.strategy.scope():
-#                 self.model = parser.instantiate_classes(model_dict).model
-#                 print(self.model)
-#                 self.model.compile(**compile_conf)
-#                 # TODO: move loss, optimizer and metrics instantiation under
-#                 # here
-#                 # Ref:
-#                 # https://www.tensorflow.org/guide/distributed_training\
-#                   #use_tfdistributestrategy_with_keras_modelfit
-#         else:
-#             self.model = parser.instantiate_classes(model_dict).model
-#             self.model.compile(**compile_conf)
-
-#         self.num_devices = (
-#             self.strategy.num_replicas_in_sync if self.strategy else 1)
-#         print(f"Strategy is working with: {self.num_devices} devices")
-
-#     def train(self, train_dataset, validation_dataset):
-#         # TODO: FIX Steps sizes in model.fit
-#         train, test = train_dataset, validation_dataset
-
-#         # Set batch size to the dataset
-#         train = train.batch(self.batch_size, drop_remainder=True)
-#         test = test.batch(self.batch_size, drop_remainder=True)
-
-#         # Number of samples
-#         n_train = train.cardinality().numpy()
-#         n_test = test.cardinality().numpy()
-
-#         # TODO: read
-#         # https://github.com/tensorflow/tensorflow/issues/56773\
-#           #issuecomment-1188693881
-#         # https://www.tensorflow.org/guide/distributed_training\
-#           #use_tfdistributestrategy_with_keras_modelfit
-
-#         # Distribute dataset
-#         if self.strategy:
-#             train = self.strategy.experimental_distribute_dataset(train)
-#             test = self.strategy.experimental_distribute_dataset(test)
-
-#         # train the model
-#         history = self.model.fit(
-#             train,
-#             validation_data=test,
-#             steps_per_epoch=int(n_train // self.num_devices),
-#             validation_steps=int(n_test // self.num_devices),
-#             epochs=self.epochs,
-#             callbacks=self.callbacks,
-#         )
+        print(f"len(dist_train_dataset): {len(train_ds)}")
+        print(f"len(dist_train_dataset): {len(valid_ds)}")
 
-#         print("Model trained")
-#         return history
+        # Compute the steps per epoch for train and valid
+        steps_per_epoch = len(train_dataset) // self.macro_batch_size
+        validation_steps = len(validation_dataset) // self.macro_batch_size
+
+        print(f"steps_per_epoch: {steps_per_epoch}")
+        print(f"validation_steps: {validation_steps}")
+
+        #####################################################################
+        # Instantiate here model, optimizer, loss under the strategy scope, #
+        # if not done previously through `model_compile_config` and         #
+        # `model_config` !                                                  #
+        # Always remember that they should be instantiated under the        #
+        # distributed strategy scope: ``with self.strategy.scope():``       #
+        #                                                                   #
+        # Example:                                                          #
+        # with self.strategy.scope():                                       #
+        #   model = tf.keras.Sequential(...)                                #
+        #   optimizer = rf.keras.optimizers.Adam(...)                       #
+        #   loss = tf.keras.losses.BinaryCrossentropy(...)                  #
+        #####################################################################
+
+        # Train the model
+        self.model.fit(
+            dist_train_dataset,
+            validation_data=dist_valid_dataset,
+            steps_per_epoch=steps_per_epoch,
+            validation_steps=validation_steps,
+            epochs=self.epochs,
+            callbacks=self.callbacks,
+            verbose=self.verbose
+        )
+        print("Training completed")
+        return train_dataset, validation_dataset, test_dataset, self.model
```

### Comparing `itwinai-0.0.1/src/itwinai/tests/dummy_components.py` & `itwinai-0.0.2/src/itwinai/tests/dummy_components.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/src/itwinai/torch/distributed.py` & `itwinai-0.0.2/src/itwinai/torch/distributed.py`

 * *Files 12% similar despite different names*

```diff
@@ -109,14 +109,20 @@
             str: torch device in the form 'cuda:N'.
         """
         if not self.is_initialized:
             raise UninitializedStrategyError(
                 "Strategy has not been initialized. Use the init method.")
         return f"cuda:{self.local_rank()}"
 
+    def set_device(self):
+        """Set local device."""
+        torch.cuda.device(self.local_rank())
+        # Needed by torch.distributed.gather_object
+        torch.cuda.set_device(self.local_rank())
+
     def create_dataloader(
         self, dataset: Dataset[T_co], batch_size: Optional[int] = 1,
         shuffle: Optional[bool] = None,
         sampler: Union[Sampler, Iterable, None] = None,
         batch_sampler: Union[Sampler[List], Iterable[List], None] = None,
         num_workers: int = 0, collate_fn: Optional[_collate_fn_t] = None,
         pin_memory: bool = False, drop_last: bool = False,
@@ -203,17 +209,18 @@
             pin_memory_device (str, optional): the device to
                 :attr:`pin_memory` to if ``pin_memory`` is ``True``.
 
 
         .. warning:: If the ``spawn`` start method is used,
                     :attr:`worker_init_fn`
                     cannot be an unpicklable object, e.g., a lambda function.
-                    See :ref:`multiprocessing-best-practices` on more
+                    See `Multiprocessing best practices`_ on more
                     details related to multiprocessing in PyTorch.
 
+
         .. warning:: ``len(dataloader)`` heuristic is based on the length of
                     the sampler used.
                     When :attr:`dataset` is an
                     :class:`~torch.utils.data.IterableDataset`,
                     it instead returns an estimate based on
                     ``len(dataset) / batch_size``, with proper
                     rounding depending on :attr:`drop_last`, regardless
@@ -234,21 +241,36 @@
                     PyTorch can not detect such cases in general.
 
                     See `Dataset Types`_ for more details on these two
                     types of datasets and how
                     :class:`~torch.utils.data.IterableDataset` interacts with
                     `Multi-process data loading`_.
 
-        .. warning:: See :ref:`reproducibility`, and
-                    :ref:`dataloader-workers-random-seed`, and
-                    :ref:`data-loading-randomness` notes for random
-                    seed related questions.
+
+        .. warning:: See `Reproducibility`_, and
+                    `My data loader workers return identical random numbers`_,
+                    and
+                    `Randomness in multi-process data loading`_ notes for
+                    random seed related questions.
+
 
         .. _multiprocessing context:
             https://docs.python.org/3/library/multiprocessing.html#contexts-and-start-methods
+        .. _Multiprocessing best practices:
+            https://pytorch.org/docs/stable/notes/multiprocessing.html#multiprocessing-best-practices
+        .. _Reproducibility:
+            https://pytorch.org/docs/stable/notes/randomness.html#reproducibility
+        .. _My data loader workers return identical random numbers:
+            https://pytorch.org/docs/stable/notes/faq.html#dataloader-workers-random-seed
+        .. _Randomness in multi-process data loading:
+            https://pytorch.org/docs/stable/data.html#data-loading-randomness
+        .. _Multi-process data loading:
+            https://pytorch.org/docs/stable/data.html#multi-process-data-loading
+        .. _Dataset Types:
+            https://pytorch.org/docs/stable/data.html#dataset-types
     """
         if not self.is_initialized:
             raise UninitializedStrategyError(
                 "Strategy has not been initialized. Use the init method.")
 
         if self.is_distributed:
             if sampler is not None:
@@ -273,24 +295,39 @@
         )
 
     @abc.abstractmethod
     def clean_up(self) -> None:
         """Cleans up resources allocated by distributed strategy."""
 
     @abc.abstractmethod
-    def par_allgather_obj(self, obj: Any) -> List[Any]:
-        """Gathers any object from the whole group in a list (to all workers).
+    def allgather_obj(self, obj: Any) -> List[Any]:
+        """All-gathers any object from the whole group in a list
+        (to all workers).
 
         Args:
             obj (Any): object to gather from all workers.
 
         Returns:
             List[Any]: list of objects gathered from all workers.
         """
 
+    @abc.abstractmethod
+    def gather_obj(self, obj: Any, dst_rank: int = 0) -> List[Any]:
+        """Gathers any object from the whole group in a list
+        (to all workers).
+
+        Args:
+            obj (Any): object to gather from all workers.
+            dst_rank (int): rank of the worker on which the objects list
+            are gathered.
+
+        Returns:
+            List[Any]: list of objects gathered from all workers.
+        """
+
 
 class TorchDDPStrategy(TorchDistributedStrategy):
     """PyTorch ``DistributedDataParallel`` distributed strategy class.
 
     Args:
         backend (str): Name of the communication backend to employ.
     """
@@ -314,15 +351,15 @@
             raise RuntimeError(
                 "Trying to run distributed on insufficient resources.")
         if self.is_initialized:
             raise DistributedStrategyError("Strategy was already initialized")
         dist.init_process_group(backend=self.backend)
         self.is_initialized = True
 
-        torch.cuda.device(self.local_rank())
+        self.set_device()
 
     # def distributed_engine(
     #     self, model: nn.Module, optimizer: Optimizer,
     #     lr_scheduler: Optional[LRScheduler] = None,
     #     mixed_precision: bool = False
     # ) -> ModelEngine:
     #     """Build a distributed model engine."""
@@ -417,31 +454,56 @@
         if not self.is_initialized:
             raise UninitializedStrategyError(
                 "Strategy has not been initialized. Use the init method.")
         if torch.cuda.is_available():
             dist.barrier()
             dist.destroy_process_group()
 
-    def par_allgather_obj(self, obj: Any) -> List[Any]:
-        """Gathers any object from the whole group
+    def allgather_obj(self, obj: Any) -> List[Any]:
+        """All-gathers any object from the whole group
         in a list (to all workers).
 
         Args:
             obj (Any): Object to gather from all workers.
 
         Returns:
             List[Any]: List of gathered objects.
         """
+        # https://pytorch.org/docs/stable/distributed.html#collective-functions
         if not self.is_initialized:
             raise UninitializedStrategyError(
                 "Strategy has not been initialized. Use the init method.")
         res = [None] * self.global_world_size()
         dist.all_gather_object(res, obj)
         return res
 
+    def gather_obj(self, obj: Any, dst_rank: int = 0) -> Optional[List[Any]]:
+        """Gathers any object from the whole group in a list
+        (to all workers).
+
+        Args:
+            obj (Any): object to gather from all workers.
+            dst_rank (int): rank of the worker on which the objects list
+            are gathered.
+
+        Returns:
+            Optional[List[Any]]: list of objects gathered from all workers
+            or ``None`` on non-destination ranks.
+        """
+        # https://pytorch.org/docs/stable/distributed.html#collective-functions
+        if not self.is_initialized:
+            raise UninitializedStrategyError(
+                "Strategy has not been initialized. Use the init method.")
+        if self.global_rank() == dst_rank:
+            res = [None] * self.global_world_size()
+            dist.gather_object(obj, res, dst=dst_rank)
+            return res
+
+        dist.gather_object(obj, dst=dst_rank)
+
 
 class DeepSpeedStrategy(TorchDistributedStrategy):
     """DeepSpeed distributed strategy class.
 
     Args:
         backend (str): Name of the communication backend to employ.
         config (Union[dict, Path, str]): DeepSpeed config. Either a
@@ -487,15 +549,15 @@
         os.environ['OMPI_COMM_WORLD_LOCAL_RANK'] = os.environ.get(
             'LOCAL_RANK', ompi_lrank)
 
         # https://deepspeed.readthedocs.io/en/latest/initialize.html#training-initialization
         deepspeed.init_distributed(dist_backend=self.backend)
         self.is_initialized = True
 
-        torch.cuda.device(self.local_rank())
+        self.set_device()
 
     def distributed(
         self, model: nn.Module, optimizer: Optional[Optimizer] = None,
         lr_scheduler: Optional[LRScheduler] = None,
         model_parameters: Optional[Any] = None,
         **init_kwargs
     ) -> Tuple[nn.Module, Optimizer, Optional[LRScheduler]]:
@@ -565,33 +627,58 @@
         return dist.get_rank() % torch.cuda.device_count()
 
     def clean_up(self) -> None:
         """Destroys the current process group."""
         if not self.is_initialized:
             raise UninitializedStrategyError(
                 "Strategy has not been initialized. Use the init method.")
-        deepspeed.sys.exit()
+        # deepspeed.sys.exit() # disabled as it kills the execution
 
-    def par_allgather_obj(self, obj: Any) -> list[Any]:
-        """Gathers any object from the whole group
+    def allgather_obj(self, obj: Any) -> List[Any]:
+        """All-gathers any object from the whole group
         in a list (to all workers).
 
         Args:
             obj (Any): Object to gather from all workers.
 
         Returns:
             List[Any]: List of gathered objects.
         """
+        # https://pytorch.org/docs/stable/distributed.html#collective-functions
         if not self.is_initialized:
             raise UninitializedStrategyError(
                 "Strategy has not been initialized. Use the init method.")
         res = [None] * self.global_world_size()
         dist.all_gather_object(res, obj)
         return res
 
+    def gather_obj(self, obj: Any, dst_rank: int = 0) -> Optional[List[Any]]:
+        """Gathers any object from the whole group in a list
+        (to all workers).
+
+        Args:
+            obj (Any): object to gather from all workers.
+            dst_rank (int): rank of the worker on which the objects list
+            are gathered.
+
+        Returns:
+            Optional[List[Any]]: list of objects gathered from all workers
+            or ``None`` on non-destination ranks.
+        """
+        # https://pytorch.org/docs/stable/distributed.html#collective-functions
+        if not self.is_initialized:
+            raise UninitializedStrategyError(
+                "Strategy has not been initialized. Use the init method.")
+        if self.global_rank() == dst_rank:
+            res = [None] * self.global_world_size()
+            dist.gather_object(obj, res, dst=dst_rank)
+            return res
+
+        dist.gather_object(obj, dst=dst_rank)
+
 
 class HorovodStrategy(TorchDistributedStrategy):
     """Horovod distributed strategy class."""
 
     def init(self) -> None:
         """Initializes the Horovod distributed backend.
 
@@ -604,15 +691,15 @@
             raise RuntimeError(
                 "Trying to run distributed on insufficient resources.")
         if self.is_initialized:
             raise DistributedStrategyError("Strategy was already initialized")
         hvd.init()
         self.is_initialized = True
 
-        torch.cuda.device(self.local_rank())
+        self.set_device()
 
     def distributed(
         self, model: nn.Module, optimizer: Optional[Optimizer] = None,
         lr_scheduler: Optional[LRScheduler] = None,
         **optim_kwargs
     ) -> Tuple[nn.Module, Optimizer, Optional[LRScheduler]]:
         """Setup model, optimizer and scheduler for distributed."""
@@ -704,29 +791,45 @@
     def clean_up(self) -> None:
         """Shuts Horovod down."""
         if not self.is_initialized:
             raise UninitializedStrategyError(
                 "Strategy has not been initialized. Use the init method.")
         hvd.shutdown()
 
-    def par_allgather_obj(self, obj: Any) -> list[Any]:
-        """Gathers scalar objects across all workers to a
+    def allgather_obj(self, obj: Any) -> list[Any]:
+        """All-gathers scalar objects across all workers to a
         list with size(#worker), uses horovod communicator
 
         Args:
             obj (Any): object in a worker.
 
         Returns:
             list: gathered list with size(#worker).
         """
         if not self.is_initialized:
             raise UninitializedStrategyError(
                 "Strategy has not been initialized. Use the init method.")
         return hvd.allgather_object(obj)
 
+    def gather_obj(self, obj: Any, dst_rank: int = 0) -> list[Any]:
+        """The same as ``allgather_obj``, as gather is not supported
+        by Horovod.
+
+        Args:
+            obj (Any): object in a worker.
+            dst_rank (int): ignored.
+
+        Returns:
+            list: gathered list with size(#worker).
+        """
+        if not self.is_initialized:
+            raise UninitializedStrategyError(
+                "Strategy has not been initialized. Use the init method.")
+        return self.allgather_obj(obj)
+
 
 class NonDistributedStrategy(TorchDistributedStrategy):
     """Dummy class for non-distributed environments."""
 
     is_distributed: bool = False
 
     def init(self) -> None:
@@ -735,15 +838,15 @@
         Raises:
             DistributedStrategyError: when trying to initialize a strategy
             already initialized.
         """
         if self.is_initialized:
             raise DistributedStrategyError("Strategy was already initialized")
         if torch.cuda.is_available():
-            torch.cuda.device(self.local_rank())
+            self.set_device()
         self.is_initialized = True
 
     def device(self) -> str:
         """Device used by local worker.
 
         Returns:
             str: cpu device if CUDA is not available.
@@ -801,16 +904,29 @@
             int: local rank.
         """
         return 0
 
     def clean_up(self) -> None:
         """Do nothing."""
 
-    def par_allgather_obj(self, obj: Any) -> list[Any]:
-        """Raise error as this operation is not available.
+    def allgather_obj(self, obj: Any) -> list[Any]:
+        """Wraps ``obj`` into a List object.
 
         Args:
             obj (Any): object in a worker.
+
+        Returns:
+            list[Any]: input object wrapped in a list.
         """
-        raise RuntimeError(
-            f"{self.__class__.__name__} does not support this operation."
-        )
+        return [obj]
+
+    def gather_obj(self, obj: Any, dst_rank: int = 0) -> list[Any]:
+        """Wraps ``obj`` into a List object.
+
+        Args:
+            obj (Any): object in a worker.
+            dst_rank (int): ignored.
+
+        Returns:
+            list[Any]: input object wrapped in a list.
+        """
+        return [obj]
```

### Comparing `itwinai-0.0.1/src/itwinai/torch/inference.py` & `itwinai-0.0.2/src/itwinai/torch/inference.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/src/itwinai/torch/mlflow.py` & `itwinai-0.0.2/src/itwinai/torch/mlflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     run and attaches it to the mlflow auto-logger.
 
     Args:
         pl_config (Dict): pytorch lightning configuration loaded in memory.
         default_experiment_name (str, optional): used as experiment name
         if it is not given in the lightning conf. Defaults to 'Default'.
         tmp_dir (str): where to temporarily store some artifacts.
-        **autolog_kwargs (kwargs): args for mlflow.pytorch.autolog(...).
+        autolog_kwargs (kwargs): args for mlflow.pytorch.autolog(...).
     """
     mlflow_conf: Optional[Dict] = _get_mlflow_logger_conf(pl_config)
     if not mlflow_conf:
         return
 
     tracking_uri = mlflow_conf.get('tracking_uri')
     if not tracking_uri:
```

### Comparing `itwinai-0.0.1/src/itwinai/torch/models/mnist.py` & `itwinai-0.0.2/src/itwinai/torch/models/mnist.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/src/itwinai/torch/reproducibility.py` & `itwinai-0.0.2/src/itwinai/torch/reproducibility.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/src/itwinai/torch/trainer.py` & `itwinai-0.0.2/src/itwinai/torch/trainer.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,20 +34,15 @@
     distributed_resources_available
 )
 from ..utils import load_yaml
 from .mlflow import (
     init_lightning_mlflow,
     teardown_lightning_mlflow
 )
-
-
-class Config:
-    def __init__(self, my_dict: Optional[Dict] = None):
-        my_dict = my_dict if my_dict is not None else {}
-        self.__dict__.update(my_dict)
+from .config import TrainingConfiguration
 
 
 class TorchTrainer(Trainer, LogMixin):
     """Trainer class for torch training algorithms.
 
     Args:
         config (Dict): training configuration containing hyperparameters.
@@ -65,14 +60,18 @@
         reproducibility. If None, the seed is not set. Defaults to None.
         logger (Optional[Logger], optional): logger for ML tracking.
         Defaults to None.
         log_all_workers (bool, optional): if True, the ``log`` method is
         called on all workers in the distributed context. Defaults to False.
         metrics (Optional[Dict[str, Metric]], optional): map of torchmetrics
         metrics. Defaults to None.
+        checkpoints_location (str): path to checkpoints directory.
+        Defaults to "checkpoints".
+        checkpoint_every (Optional[int]): save a checkpoint every
+        ``checkpoint_every`` epochs. Disabled if None. Defaults to None.
         name (Optional[str], optional): trainer custom name. Defaults to None.
     """
     # TODO:
     #   - add checkpointing.
     #   - extract BaseTorchTrainer and extend it creating a set of trainer
     #     templates (e.g.. GAN, Classifier, Transformer) allowing scientists
     #     to reuse ML algos.
@@ -104,32 +103,37 @@
         strategy: Literal["ddp", "deepspeed", "horovod"] = 'ddp',
         validation_every: Optional[int] = 1,
         test_every: Optional[int] = None,
         random_seed: Optional[int] = None,
         logger: Optional[Logger] = None,
         log_all_workers: bool = False,
         metrics: Optional[Dict[str, Metric]] = None,
+        checkpoints_location: str = "checkpoints",
+        checkpoint_every: Optional[int] = None,
         name: Optional[str] = None
     ) -> None:
         super().__init__(name)
         self.save_parameters(**self.locals2params(locals()))
 
         # config is mean to store all hyperparameters, which can very from use
         # case to use case
         # and include learning_rate, batch_size....
-        self.config = Config(config)
+        self.config = TrainingConfiguration(**config)
         self.epochs = epochs
         self.model = model
         self.strategy = strategy
         self.validation_every = validation_every
         self.test_every = test_every
         self.random_seed = random_seed
         self.logger = logger
         self.log_all_workers = log_all_workers
         self.metrics = metrics if metrics is not None else {}
+        self.checkpoints_location = checkpoints_location
+        os.makedirs(self.checkpoints_location, exist_ok=True)
+        self.checkpoint_every = checkpoint_every
 
     @property
     def strategy(self) -> TorchDistributedStrategy:
         return self._strategy
 
     @strategy.setter
     def strategy(self, strategy: Union[str, TorchDistributedStrategy]) -> None:
@@ -303,20 +307,20 @@
         self.create_dataloaders(
             train_dataset=train_dataset,
             validation_dataset=validation_dataset,
             test_dataset=test_dataset
         )
         self.create_model_loss_optimizer()
 
-        if self.strategy.is_main_worker:
+        if self.strategy.is_main_worker and self.logger:
             self.logger.create_logger_context()
 
         self.train()
 
-        if self.strategy.is_main_worker:
+        if self.strategy.is_main_worker and self.logger:
             self.logger.destroy_logger_context()
         self.strategy.clean_up()
         return train_dataset, validation_dataset, test_dataset, self.model
 
     def _set_epoch_dataloaders(self, epoch: int):
         """
         Sets epoch in the distributed sampler of a dataloader when using it.
@@ -333,61 +337,130 @@
         item: Union[Any, List[Any]],
         identifier: Union[str, List[str]],
         kind: str = 'metric',
         step: Optional[int] = None,
         batch_idx: Optional[int] = None,
         **kwargs
     ) -> None:
+        """Log ``item`` with ``identifier`` name of ``kind`` type at ``step``
+        time step.
+
+        Args:
+            item (Union[Any, List[Any]]): element to be logged (e.g., metric).
+            identifier (Union[str, List[str]]): unique identifier for the
+            element to log(e.g., name of a metric).
+            kind (str, optional): type of the item to be logged. Must be one
+            among the list of self.supported_types. Defaults to 'metric'.
+            step (Optional[int], optional): logging step. Defaults to None.
+            batch_idx (Optional[int], optional): DataLoader batch counter
+            (i.e., batch idx), if available. Defaults to None.
+        """
         if self.logger and (
                 self.strategy.is_main_worker or self.log_all_workers):
             self.logger.log(
                 item=item,
                 identifier=identifier,
                 kind=kind,
                 step=step,
                 batch_idx=batch_idx,
                 **kwargs
             )
 
+    def save_checkpoint(
+            self, name: str, epoch: int, loss: Optional[torch.Tensor] = None
+    ) -> None:
+        """Save training checkpoint.
+
+        Args:
+            name (str): name of the checkpoint.
+            epoch (int): current training epoch.
+            loss (Optional[torch.Tensor]): current loss (if available).
+        """
+        state = dict(
+            epoch=epoch,
+            loss=loss,
+            optimizer=self.optimizer.state_dict(),
+            model=self.model.state_dict(),
+            lr_scheduler=self.lr_scheduler
+        )
+        ckpt_path = os.path.join(self.checkpoints_location, name)
+        torch.save(state, ckpt_path)
+        print(f"Saved '{name}' checkpoint at {ckpt_path}")
+
+        # Save checkpoint to logger
+        self.log(ckpt_path, name, kind='artifact')
+
+    def load_checkpoint(self, name: str) -> None:
+        """Load state from a checkpoint.
+
+        Args:
+            name (str): name of the checkpoint to load, assuming it
+            is under ``self.checkpoints_location`` location.
+        """
+        ckpt_path = os.path.join(self.checkpoints_location, name)
+        state = torch.load(ckpt_path, map_location=self.device)
+        self.model.load_state_dict(state['model'])
+        self.optimizer.load_state_dict(state['optimizer'])
+        self.lr_scheduler = state['lr_scheduler']
+
     def train(self):
         """Trains a machine learning model.
         Main training loop/logic.
 
         Args:
             train_dataset (Dataset): training dataset.
             validation_dataset (Dataset): validation dataset.
             test_dataset (Dataset): test dataset.
 
         Returns:
             Tuple[Dataset, Dataset, Dataset, Any]: training dataset,
             validation dataset, test dataset, trained model.
         """
-        # start_time = time.perf_counter()
+        best_loss = float('inf')
         for epoch in range(self.epochs):
             epoch_n = epoch + 1
             self._set_epoch_dataloaders(epoch)
             self.train_epoch()
-            if self.validation_every and self.validation_every % epoch_n == 0:
-                self.validation_epoch()
-            if self.test_every and self.test_every % epoch_n == 0:
+            if self.validation_every and epoch_n % self.validation_every == 0:
+                val_loss = self.validation_epoch()
+
+                # Checkpointing current best model
+                worker_val_losses = self.strategy.gather_obj(
+                    val_loss, dst_rank=0)
+                if self.strategy.global_rank() == 0:
+                    avg_loss = torch.mean(
+                        torch.stack(worker_val_losses)
+                    ).detach().cpu()
+                    if avg_loss < best_loss:
+                        ckpt_name = "best_model.pth"
+                        self.save_checkpoint(
+                            name=ckpt_name, epoch=epoch, loss=avg_loss)
+
+            if self.test_every and epoch_n % self.test_every == 0:
                 self.test_epoch()
 
+            # Periodic checkpointing
+            if (self.strategy.is_main_worker and self.checkpoint_every
+                    and epoch_n % self.checkpoint_every == 0):
+                ckpt_name = f"epoch_{epoch}.pth"
+                self.save_checkpoint(name=ckpt_name, epoch=epoch)
+
     def compute_metrics(
         self,
         true: Batch,
         pred: Batch,
         logger_step: int,
         batch_idx: Optional[int],
         stage: str = 'train'
     ) -> Dict[str, Any]:
         """Compute and log metrics.
 
         Args:
             metrics (Dict[str, Metric]): metrics dict. Can be
-                ``self.train_metrics`` or ``self.validation_metrics``.
+            ``self.train_metrics`` or ``self.validation_metrics``.
             true (Batch): true values.
             pred (Batch): predicted values.
             logger_step (int): global step to pass to the logger.
             stage (str): 'train', 'validation'...
 
         Returns:
             Dict[str, Any]: metric values.
```

### Comparing `itwinai-0.0.1/src/itwinai/torch/types.py` & `itwinai-0.0.2/src/itwinai/torch/types.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/src/itwinai/utils.py` & `itwinai-0.0.2/src/itwinai/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 ) -> MutableMapping:
     """Flatten dictionary
 
     Args:
         d (MutableMapping): nested dictionary to flatten
         parent_key (str, optional): prefix for all keys. Defaults to ''.
         sep (str, optional): separator for nested key concatenation.
-            Defaults to '.'.
+        Defaults to '.'.
 
     Returns:
         MutableMapping: flattened dictionary with new keys.
     """
     items = []
     for k, v in d.items():
         new_key = parent_key + sep + k if parent_key else k
```

### Comparing `itwinai-0.0.1/src/itwinai.egg-info/PKG-INFO` & `itwinai-0.0.2/src/itwinai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: itwinai
-Version: 0.0.1
+Version: 0.0.2
 Summary: AI and ML workflows module for scientific digital twins.
-Author-email: Matteo Bunino <matteo.bunino@cern.ch>, Alexander Zoechbauer <alexander.zoechbauer@cern.ch>, Rakesh Sarma <r.sarma@fz-juelich.de>, Mario Ruettgers <m.ruettgers@fz-juelich.de>, Eric Wulff <eric.wulff@cern.ch>
-Maintainer-email: Matteo Bunino <matteo.bunino@cern.ch>, Alexander Zoechbauer <alexander.zoechbauer@cern.ch>, Rakesh Sarma <r.sarma@fz-juelich.de>, Mario Ruettgers <m.ruettgers@fz-juelich.de>
+Author-email: Matteo Bunino <matteo.bunino@cern.ch>, Rakesh Sarma <r.sarma@fz-juelich.de>, Mario Ruettgers <m.ruettgers@fz-juelich.de>, Kalliopi Tsolaki <kalliopi.tsolaki@cern.ch>
+Maintainer-email: Matteo Bunino <matteo.bunino@cern.ch>, Rakesh Sarma <r.sarma@fz-juelich.de>, Mario Ruettgers <m.ruettgers@fz-juelich.de>, Kalliopi Tsolaki <kalliopi.tsolaki@cern.ch>
 License: MIT License
         
         Copyright (c) 2023 interTwin Community
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -28,43 +28,45 @@
         
 Project-URL: Homepage, https://www.intertwin.eu/
 Project-URL: Documentation, https://itwinai.readthedocs.io/
 Project-URL: Repository, https://github.com/interTwin-eu/itwinai
 Keywords: ml,ai,hpc
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: wandb
 Requires-Dist: mlflow
 Requires-Dist: jsonargparse[signatures]
 Requires-Dist: pyyaml
 Requires-Dist: omegaconf
 Requires-Dist: rich>=13.5.3
 Requires-Dist: typer>=0.9.0
 Requires-Dist: wheel
+Requires-Dist: pydantic
 Provides-Extra: torch
 Requires-Dist: lightning; extra == "torch"
 Requires-Dist: torchmetrics; extra == "torch"
 Provides-Extra: dev
 Requires-Dist: pytest>=7.4.2; extra == "dev"
 Requires-Dist: pytest-mock>=3.11.1; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
+Requires-Dist: tensorflow==2.15; extra == "dev"
 
 # itwinai
 
 [![GitHub Super-Linter](https://github.com/interTwin-eu/T6.5-AI-and-ML/actions/workflows/lint.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)
 [![GitHub Super-Linter](https://github.com/interTwin-eu/T6.5-AI-and-ML/actions/workflows/check-links.yml/badge.svg)](https://github.com/marketplace/actions/markdown-link-check)
  [![SQAaaS source code](https://github.com/EOSC-synergy/itwinai.assess.sqaaas/raw/dev/.badge/status_shields.svg)](https://sqaaas.eosc-synergy.eu/#/full-assessment/report/https://raw.githubusercontent.com/eosc-synergy/itwinai.assess.sqaaas/dev/.report/assessment_output.json)
 
-See the latest version of our [docs](https://intertwin-eu.github.io/itwinai/)
+See the latest version of our [docs](https://itwinai.readthedocs.io/)
 for a quick overview of this platform for advanced AI/ML workflows in digital twin applications.
 
 ## Installation
 
 Requirements:
 
 - Linux environment. Windows and macOS were never tested.
```

### Comparing `itwinai-0.0.1/src/itwinai.egg-info/SOURCES.txt` & `itwinai-0.0.2/src/itwinai.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -31,36 +31,44 @@
 .vscode/settings.json
 docs/3dgan_doc.rst
 docs/Makefile
 docs/advanced_workflow.rst
 docs/basic_comp.rst
 docs/basic_workflow.rst
 docs/conf.py
+docs/cyclones_doc.rst
+docs/ddp_why.rst
 docs/getting_started_with_itwinai.rst
-docs/hpc_setup.rst
 docs/index.rst
 docs/intermediate_workflow.rst
 docs/itwinai.cli.rst
-docs/itwinai.cluster.rst
 docs/itwinai.components.rst
+docs/itwinai.distributed.rst
 docs/itwinai.loggers.rst
 docs/itwinai.parser.rst
 docs/itwinai.pipeline.rst
 docs/itwinai.serialization.rst
 docs/itwinai.tf.modules.rst
 docs/itwinai.torch.modules.rst
-docs/itwinai.types.rst
+docs/itwinai.type.rst
 docs/itwinai.utils.rst
-docs/local_setup.rst
 docs/make.bat
 docs/mnist_doc.rst
 docs/modules.rst
 docs/requirements.txt
+docs/tf_scaling_test.rst
+docs/tf_tutorial_0_basics.rst
+docs/tf_tutorial_1_imagenet.rst
+docs/torch_scaling_test.rst
+docs/torch_tutorial_0_basics.rst
+docs/torch_tutorial_1_mnist.rst
 docs/tutorials.rst
 docs/use_cases.rst
+docs/virgo_doc.rst
+docs/notebooks/example.ipynb
 env-files/tensorflow/createEnvJSCTF.sh
 env-files/tensorflow/generic_tf.sh
 env-files/tensorflow/tensorflow-2.10.yml
 env-files/tensorflow/tensorflow-2.11.yml
 env-files/tensorflow/tensorflow-2.13-cpu.yml
 env-files/tensorflow/tensorflow-2.13.yml
 env-files/torch/createEnvJSC.sh
@@ -71,15 +79,15 @@
 src/itwinai/cli.py
 src/itwinai/components.py
 src/itwinai/distributed.py
 src/itwinai/loggers.py
 src/itwinai/parser.py
 src/itwinai/pipeline.py
 src/itwinai/serialization.py
-src/itwinai/types.py
+src/itwinai/type.py
 src/itwinai/utils.py
 src/itwinai.egg-info/PKG-INFO
 src/itwinai.egg-info/SOURCES.txt
 src/itwinai.egg-info/dependency_links.txt
 src/itwinai.egg-info/entry_points.txt
 src/itwinai.egg-info/requires.txt
 src/itwinai.egg-info/top_level.txt
@@ -89,31 +97,34 @@
 src/itwinai/tensorflow/utils.py
 src/itwinai/tensorflow/data/__init__.py
 src/itwinai/tensorflow/models/__init__.py
 src/itwinai/tensorflow/models/mnist.py
 src/itwinai/tests/__init__.py
 src/itwinai/tests/dummy_components.py
 src/itwinai/torch/__init__.py
+src/itwinai/torch/config.py
 src/itwinai/torch/distributed.py
 src/itwinai/torch/inference.py
 src/itwinai/torch/mlflow.py
 src/itwinai/torch/reproducibility.py
 src/itwinai/torch/trainer.py
 src/itwinai/torch/types.py
 src/itwinai/torch/data/__init__.py
 src/itwinai/torch/models/__init__.py
 src/itwinai/torch/models/mnist.py
 tests/conftest.py
 tests/run_on_jsc.sh
+tests/test_loggers.py
 tests/test_utils.py
 tests/components/conftest.py
 tests/components/test_components.py
 tests/components/test_pipe_parser.py
 tests/components/test_pipeline.py
 tests/torch/distribtued_decorator.py
+tests/torch/test_config.py
 tests/torch/test_distribtued_training.py
 tests/torch/torch_dist_trainer.py
 tests/use-cases/conftest.py
 tests/use-cases/test_3dgan.py
 tests/use-cases/test_cyclones.py
 tests/use-cases/test_mnist.py
 tutorials/distributed-ml/tf-scaling-test-jube/README.md
@@ -172,37 +183,48 @@
 use-cases/3dgan/interLink/README.md
 use-cases/cyclones/.gitignore
 use-cases/cyclones/README.md
 use-cases/cyclones/cyclones_vgg.py
 use-cases/cyclones/dataloader.py
 use-cases/cyclones/pipeline.yaml
 use-cases/cyclones/requirements.txt
-use-cases/cyclones/startscript
+use-cases/cyclones/startscript.sh
 use-cases/cyclones/train.py
 use-cases/cyclones/trainer.py
-use-cases/cyclones/lib/callbacks.py
-use-cases/cyclones/lib/macros.py
-use-cases/cyclones/lib/scaling.py
-use-cases/cyclones/lib/strategy.py
-use-cases/cyclones/lib/transform.py
-use-cases/cyclones/lib/utils.py
-use-cases/cyclones/lib/tfrecords/dataset.py
-use-cases/cyclones/lib/tfrecords/functions.py
+use-cases/cyclones/src/callbacks.py
+use-cases/cyclones/src/macros.py
+use-cases/cyclones/src/scaling.py
+use-cases/cyclones/src/strategy.py
+use-cases/cyclones/src/transform.py
+use-cases/cyclones/src/utils.py
+use-cases/cyclones/src/tfrecords/dataset.py
+use-cases/cyclones/src/tfrecords/functions.py
 use-cases/mnist/tensorflow/dataloader.py
 use-cases/mnist/tensorflow/pipeline.yaml
-use-cases/mnist/tensorflow/startscript
-use-cases/mnist/tensorflow/trainer.py
+use-cases/mnist/tensorflow/startscript.sh
 use-cases/mnist/torch/Dockerfile
 use-cases/mnist/torch/README.md
 use-cases/mnist/torch/config.yaml
 use-cases/mnist/torch/create_inference_sample.py
 use-cases/mnist/torch/dataloader.py
 use-cases/mnist/torch/model.py
 use-cases/mnist/torch/runall.sh
 use-cases/mnist/torch/saver.py
 use-cases/mnist/torch/slurm.sh
-use-cases/mnist/torch/startscript
+use-cases/mnist/torch/startscript.sh
 use-cases/mnist/torch-lightning/README.md
 use-cases/mnist/torch-lightning/config.yaml
 use-cases/mnist/torch-lightning/dataloader.py
 use-cases/mnist/torch-lightning/startscript
-use-cases/mnist/torch-lightning/utils.py
+use-cases/mnist/torch-lightning/utils.py
+use-cases/virgo/.gitignore
+use-cases/virgo/README.md
+use-cases/virgo/config.yaml
+use-cases/virgo/data.py
+use-cases/virgo/requirements.txt
+use-cases/virgo/runall.sh
+use-cases/virgo/slurm.sh
+use-cases/virgo/train.py
+use-cases/virgo/trainer.py
+use-cases/virgo/src/dataset.py
+use-cases/virgo/src/model.py
+use-cases/virgo/src/utils.py
```

### Comparing `itwinai-0.0.1/tests/components/conftest.py` & `itwinai-0.0.2/tests/components/conftest.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tests/components/test_components.py` & `itwinai-0.0.2/tests/components/test_components.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tests/components/test_pipe_parser.py` & `itwinai-0.0.2/tests/components/test_pipe_parser.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tests/components/test_pipeline.py` & `itwinai-0.0.2/tests/components/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tests/conftest.py` & `itwinai-0.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tests/run_on_jsc.sh` & `itwinai-0.0.2/tests/run_on_jsc.sh`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tests/test_utils.py` & `itwinai-0.0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tests/torch/distribtued_decorator.py` & `itwinai-0.0.2/tests/torch/distribtued_decorator.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tests/torch/test_distribtued_training.py` & `itwinai-0.0.2/tests/torch/test_distribtued_training.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tests/torch/torch_dist_trainer.py` & `itwinai-0.0.2/tests/torch/torch_dist_trainer.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tests/use-cases/conftest.py` & `itwinai-0.0.2/tests/use-cases/conftest.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tests/use-cases/test_3dgan.py` & `itwinai-0.0.2/tests/use-cases/test_3dgan.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tests/use-cases/test_cyclones.py` & `itwinai-0.0.2/tests/use-cases/test_cyclones.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tests/use-cases/test_mnist.py` & `itwinai-0.0.2/tests/use-cases/test_mnist.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/tf-scaling-test-jube/README.md` & `itwinai-0.0.2/tutorials/distributed-ml/tf-scaling-test-jube/README.md`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/tf-scaling-test-jube/bench_plot.ipynb` & `itwinai-0.0.2/tutorials/distributed-ml/tf-scaling-test-jube/bench_plot.ipynb`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/tf-scaling-test-jube/general_jobsys.xml` & `itwinai-0.0.2/tutorials/distributed-ml/tf-scaling-test-jube/general_jobsys.xml`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/tf-scaling-test-jube/jube_ddp.sh` & `itwinai-0.0.2/tutorials/distributed-ml/tf-scaling-test-jube/jube_ddp.sh`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/tf-scaling-test-jube/train.py` & `itwinai-0.0.2/tutorials/distributed-ml/tf-scaling-test-jube/train.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/tf-tutorial-0-basics/README.md` & `itwinai-0.0.2/tutorials/distributed-ml/tf-tutorial-0-basics/README.md`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/tf-tutorial-0-basics/tfmirrored_slurm.sh` & `itwinai-0.0.2/tutorials/distributed-ml/tf-tutorial-0-basics/tfmirrored_slurm.sh`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/tf-tutorial-0-basics/train.py` & `itwinai-0.0.2/tutorials/distributed-ml/tf-tutorial-0-basics/train.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/tf-tutorial-1-imagenet/README.md` & `itwinai-0.0.2/tutorials/distributed-ml/tf-tutorial-1-imagenet/README.md`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/tf-tutorial-1-imagenet/tfmirrored_slurm.sh` & `itwinai-0.0.2/tutorials/distributed-ml/tf-tutorial-1-imagenet/tfmirrored_slurm.sh`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/tf-tutorial-1-imagenet/train.py` & `itwinai-0.0.2/tutorials/distributed-ml/tf-tutorial-1-imagenet/train.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/README.md` & `itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/README.md`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/ddp_trainer.py` & `itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/ddp_trainer.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/deepspeed_trainer.py` & `itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/deepspeed_trainer.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/horovod_trainer.py` & `itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/horovod_trainer.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/img/report.png` & `itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/img/report.png`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/itwinai_trainer.py` & `itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/itwinai_trainer.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/runall.sh` & `itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/runall.sh`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/slurm.sh` & `itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/slurm.sh`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/torch-scaling-test/utils.py` & `itwinai-0.0.2/tutorials/distributed-ml/torch-scaling-test/utils.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-0-basics/README.md` & `itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-1-mnist/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Tutorial: distributed strategies for PyTorch
+# Tutorial: distributed strategies for PyTorch model trained on MNIST dataset
 
 In this tutorial we show how to use torch `DistributedDataParallel` (DDP), Horovod and
 DeepSpeed from the same client code.
 Note that the environment is tested on the HDFML system at JSC. For other systems,
 the module versions might need change accordingly.
 
 ## Setup
@@ -11,53 +11,63 @@
 pytorch, horovod and deepspeed. You can *try* with:
 
 ```bash
 # Creates a Python venv called envAI_hdfml
 make torch-gpu-jsc
 ```
 
+Before launching training, since on JSC's compute nodes there is not internet connection,
+you need to download the dataset before while on the login lode:
+
+```bash
+source ../../../envAI_hdfml/bin/activate
+python train.py --download-only
+```
+
+This command creates a local folder called "MNIST" with the dataset.
+
 ## Distributed training
 
 Each distributed strategy has its own SLURM job script, which
 should be used to run it:
 
 If you want to distribute the code in `train.py` with **torch DDP**, run from terminal:
   
 ```bash
 export DIST_MODE="ddp"
 export RUN_NAME="ddp-itwinai"
-export TRAINING_CMD="train.py -s ddp"
+export TRAINING_CMD="train.py -s ddp -c config.yaml"
 export PYTHON_VENV="../../../envAI_hdfml"
 sbatch --export=ALL,DIST_MODE="$DIST_MODE",RUN_NAME="$RUN_NAME",TRAINING_CMD="$TRAINING_CMD",PYTHON_VENV="$PYTHON_VENV" \
     --job-name="$RUN_NAME-n$N" \
     --output="logs_slurm/job-$RUN_NAME-n$N.out" \
     --error="logs_slurm/job-$RUN_NAME-n$N.err" \
     slurm.sh
 ```
 
 If you want to distribute the code in `train.py` with **DeepSpeed**, run from terminal:
   
 ```bash
 export DIST_MODE="deepspeed"
 export RUN_NAME="deepspeed-itwinai"
-export TRAINING_CMD="train.py -s deepspeed"
+export TRAINING_CMD="train.py -s deepspeed -c config.yaml"
 export PYTHON_VENV="../../../envAI_hdfml"
 sbatch --export=ALL,DIST_MODE="$DIST_MODE",RUN_NAME="$RUN_NAME",TRAINING_CMD="$TRAINING_CMD",PYTHON_VENV="$PYTHON_VENV" \
     --job-name="$RUN_NAME-n$N" \
     --output="logs_slurm/job-$RUN_NAME-n$N.out" \
     --error="logs_slurm/job-$RUN_NAME-n$N.err" \
     slurm.sh
 ```
 
 If you want to distribute the code in `train.py` with **Horovod**, run from terminal:
   
 ```bash
-export DIST_MODE="deepspeed"
-export RUN_NAME="deepspeed-itwinai"
-export TRAINING_CMD="train.py -s deepspeed"
+export DIST_MODE="horovod"
+export RUN_NAME="horovod-itwinai"
+export TRAINING_CMD="train.py -s horovod -c config.yaml"
 export PYTHON_VENV="../../../envAI_hdfml"
 sbatch --export=ALL,DIST_MODE="$DIST_MODE",RUN_NAME="$RUN_NAME",TRAINING_CMD="$TRAINING_CMD",PYTHON_VENV="$PYTHON_VENV" \
     --job-name="$RUN_NAME-n$N" \
     --output="logs_slurm/job-$RUN_NAME-n$N.out" \
     --error="logs_slurm/job-$RUN_NAME-n$N.err" \
     slurm.sh
 ```
```

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-0-basics/runall.sh` & `itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-0-basics/runall.sh`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-0-basics/slurm.sh` & `itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-0-basics/slurm.sh`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-0-basics/train.py` & `itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-0-basics/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             loss = loss_fn(y_pred, y)
             loss.backward()
 
             optim.step()
 
             if strategy.is_main_worker:
                 print(f"Loss [epoch={epoch}]: {loss.item()}")
-            print(f"NNLoss [epoch={epoch}]: {loss.item()}")
+            # print(f"NNLoss [epoch={epoch}]: {loss.item()}")
 
         # Update scheduler
         if lr_sched:
             lr_sched.step()
 
     time.sleep(1)
     print(f"<Global rank: {strategy.global_rank()}> - TRAINING FINISHED")
```

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-1-mnist/README.md` & `itwinai-0.0.2/docs/torch_tutorial_1_mnist.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,119 @@
-# Tutorial: distributed strategies for PyTorch model trained on MNIST dataset
+PyTorch MNIST example
+=====================
 
-In this tutorial we show how to use torch `DistributedDataParallel` (DDP), Horovod and
+Tutorial: distributed strategies for PyTorch model trained on MNIST dataset
+---------------------------------------------------------------------------
+
+In this tutorial we show how to use torch ``DistributedDataParallel`` (DDP), Horovod and
 DeepSpeed from the same client code.
 Note that the environment is tested on the HDFML system at JSC. For other systems,
 the module versions might need change accordingly.
 
-## Setup
+Setup
++++++
 
 First, from the root of this repository, build the environment containing
 pytorch, horovod and deepspeed. You can *try* with:
 
-```bash
-# Creates a Python venv called envAI_hdfml
-make torch-gpu-jsc
-```
+.. code-block:: bash
+
+    # Creates a Python venv called envAI_hdfml
+    make torch-gpu-jsc
+
 
 Before launching training, since on JSC's compute nodes there is not internet connection,
 you need to download the dataset before while on the login lode:
 
-```bash
-source ../../../envAI_hdfml/bin/activate
-python train.py --download-only
-```
+.. code-block:: bash
+
+    source ../../../envAI_hdfml/bin/activate
+    python train.py --download-only
+
 
 This command creates a local folder called "MNIST" with the dataset.
 
-## Distributed training
+Distributed training
+++++++++++++++++++++
 
 Each distributed strategy has its own SLURM job script, which
 should be used to run it:
 
-If you want to distribute the code in `train.py` with **torch DDP**, run from terminal:
+If you want to distribute the code in ``train.py`` with **torch DDP**, run from terminal:
   
-```bash
-export DIST_MODE="ddp"
-export RUN_NAME="ddp-itwinai"
-export TRAINING_CMD="train.py -s ddp -c config.yaml"
-export PYTHON_VENV="../../../envAI_hdfml"
-sbatch --export=ALL,DIST_MODE="$DIST_MODE",RUN_NAME="$RUN_NAME",TRAINING_CMD="$TRAINING_CMD",PYTHON_VENV="$PYTHON_VENV" \
-    --job-name="$RUN_NAME-n$N" \
-    --output="logs_slurm/job-$RUN_NAME-n$N.out" \
-    --error="logs_slurm/job-$RUN_NAME-n$N.err" \
-    slurm.sh
-```
+.. code-block:: bash
+
+    export DIST_MODE="ddp"
+    export RUN_NAME="ddp-itwinai"
+    export TRAINING_CMD="train.py -s ddp -c config.yaml"
+    export PYTHON_VENV="../../../envAI_hdfml"
+    sbatch --export=ALL,DIST_MODE="$DIST_MODE",RUN_NAME="$RUN_NAME",TRAINING_CMD="$TRAINING_CMD",PYTHON_VENV="$PYTHON_VENV" \
+        --job-name="$RUN_NAME-n$N" \
+        --output="logs_slurm/job-$RUN_NAME-n$N.out" \
+        --error="logs_slurm/job-$RUN_NAME-n$N.err" \
+        slurm.sh
+
 
-If you want to distribute the code in `train.py` with **DeepSpeed**, run from terminal:
+If you want to distribute the code in ``train.py`` with **DeepSpeed**, run from terminal:
   
-```bash
-export DIST_MODE="deepspeed"
-export RUN_NAME="deepspeed-itwinai"
-export TRAINING_CMD="train.py -s deepspeed -c config.yaml"
-export PYTHON_VENV="../../../envAI_hdfml"
-sbatch --export=ALL,DIST_MODE="$DIST_MODE",RUN_NAME="$RUN_NAME",TRAINING_CMD="$TRAINING_CMD",PYTHON_VENV="$PYTHON_VENV" \
-    --job-name="$RUN_NAME-n$N" \
-    --output="logs_slurm/job-$RUN_NAME-n$N.out" \
-    --error="logs_slurm/job-$RUN_NAME-n$N.err" \
-    slurm.sh
-```
+.. code-block:: bash
 
-If you want to distribute the code in `train.py` with **Horovod**, run from terminal:
+    export DIST_MODE="deepspeed"
+    export RUN_NAME="deepspeed-itwinai"
+    export TRAINING_CMD="train.py -s deepspeed -c config.yaml"
+    export PYTHON_VENV="../../../envAI_hdfml"
+    sbatch --export=ALL,DIST_MODE="$DIST_MODE",RUN_NAME="$RUN_NAME",TRAINING_CMD="$TRAINING_CMD",PYTHON_VENV="$PYTHON_VENV" \
+        --job-name="$RUN_NAME-n$N" \
+        --output="logs_slurm/job-$RUN_NAME-n$N.out" \
+        --error="logs_slurm/job-$RUN_NAME-n$N.err" \
+        slurm.sh
+
+
+If you want to distribute the code in ``train.py`` with **Horovod**, run from terminal:
   
-```bash
-export DIST_MODE="horovod"
-export RUN_NAME="horovod-itwinai"
-export TRAINING_CMD="train.py -s horovod -c config.yaml"
-export PYTHON_VENV="../../../envAI_hdfml"
-sbatch --export=ALL,DIST_MODE="$DIST_MODE",RUN_NAME="$RUN_NAME",TRAINING_CMD="$TRAINING_CMD",PYTHON_VENV="$PYTHON_VENV" \
-    --job-name="$RUN_NAME-n$N" \
-    --output="logs_slurm/job-$RUN_NAME-n$N.out" \
-    --error="logs_slurm/job-$RUN_NAME-n$N.err" \
-    slurm.sh
-```
-
-You can run all of them with:
-
-```bash
-bash runall.sh
-```
+.. code-block:: bash
+
+    export DIST_MODE="horovod"
+    export RUN_NAME="horovod-itwinai"
+    export TRAINING_CMD="train.py -s horovod -c config.yaml"
+    export PYTHON_VENV="../../../envAI_hdfml"
+    sbatch --export=ALL,DIST_MODE="$DIST_MODE",RUN_NAME="$RUN_NAME",TRAINING_CMD="$TRAINING_CMD",PYTHON_VENV="$PYTHON_VENV" \
+        --job-name="$RUN_NAME-n$N" \
+        --output="logs_slurm/job-$RUN_NAME-n$N.out" \
+        --error="logs_slurm/job-$RUN_NAME-n$N.err" \
+        slurm.sh
+
+
+**You can run all of them with:**
+
+.. code-block:: bash
+
+    bash runall.sh
+
+
+config.yaml
++++++++++++
+
+.. literalinclude:: ../tutorials/distributed-ml/torch-tutorial-1-mnist/config.yaml
+   :language: yaml
+
+
+runall.sh
++++++++++
+
+.. literalinclude:: ../tutorials/distributed-ml/torch-tutorial-1-mnist/runall.sh
+   :language: bash
+
+
+slurm.sh
+++++++++
+
+.. literalinclude:: ../tutorials/distributed-ml/torch-tutorial-1-mnist/slurm.sh
+   :language: bash
+
+
+train.py
+++++++++
+
+.. literalinclude:: ../tutorials/distributed-ml/torch-tutorial-1-mnist/train.py
+   :language: python
+
```

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-1-mnist/runall.sh` & `itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-1-mnist/runall.sh`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-1-mnist/slurm.sh` & `itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-1-mnist/slurm.sh`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/distributed-ml/torch-tutorial-1-mnist/train.py` & `itwinai-0.0.2/tutorials/distributed-ml/torch-tutorial-1-mnist/train.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/ml-workflows/basic_components.py` & `itwinai-0.0.2/tutorials/ml-workflows/basic_components.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/ml-workflows/tutorial_0_basic_workflow.py` & `itwinai-0.0.2/tutorials/ml-workflows/tutorial_0_basic_workflow.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/ml-workflows/tutorial_1_intermediate_workflow.py` & `itwinai-0.0.2/tutorials/ml-workflows/tutorial_1_intermediate_workflow.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/tutorials/ml-workflows/tutorial_2_advanced_workflow.py` & `itwinai-0.0.2/tutorials/ml-workflows/tutorial_2_advanced_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """
 In the first two tutorials we saw how to define simple sequential workflows by
 means of the Pipeline object, which feds the outputs of the previous component
 as inputs of the following one.
-
 In this tutorial we show how to create more complex workflows, with
 non-sequential data flows. Here, components can be arranges as an directed
 acyclic graph (DAG). Under the DAG assumption, outputs of each block can be fed
 as input potentially to any other component, granting great flexibility to the
 experimenter.
-
 The trade-off for improved flexibility is a change in the way we define
 configuration files. From now on, it will only be possible to configure the
 parameters used by the training script, but not its structure through the
 Pipeline.
 
 itwinai provides a wrapper of jsonarparse's ArgumentParser which supports
 configuration files by default.
@@ -20,28 +18,31 @@
 To run as usual:
 >>> python my_script.py -d 20 --train-prop 0.7 --val-prop 0.2 --lr 1e-5
 
 To reuse the parameters saved in a configuration file and override some
 parameter (e.g., learning rate):
 >>> python my_script.py --config advanced_tutorial_conf.yaml --lr 2e-3
 
+
 """
 from typing import Any
 from itwinai.parser import ArgumentParser
 from itwinai.components import Predictor, monitor_exec
 
 from basic_components import (
     MyDataGetter, MyDatasetSplitter, MyTrainer, MySaver
 )
 
 
 class MyEnsemblePredictor(Predictor):
     @monitor_exec
     def execute(self, dataset, model_ensemble) -> Any:
-        # do some predictions with model on dataset...
+        """
+        do some predictions with model on dataset...
+        """
         return dataset
 
 
 if __name__ == "__main__":
     parser = ArgumentParser(description="itwinai advanced workflows tutorial")
     parser.add_argument(
         "--data-size", "-d", type=int, required=True,
```

### Comparing `itwinai-0.0.1/use-cases/3dgan/Dockerfile` & `itwinai-0.0.2/use-cases/3dgan/Dockerfile`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/3dgan/README.md` & `itwinai-0.0.2/use-cases/3dgan/README.md`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/3dgan/config.yaml` & `itwinai-0.0.2/use-cases/3dgan/config.yaml`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/3dgan/create_inference_sample.py` & `itwinai-0.0.2/use-cases/3dgan/create_inference_sample.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/3dgan/dataloader.py` & `itwinai-0.0.2/use-cases/3dgan/dataloader.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/3dgan/interLink/3dgan-inference-cpu.yaml` & `itwinai-0.0.2/use-cases/3dgan/interLink/3dgan-inference-cpu.yaml`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/3dgan/interLink/3dgan-inference.yaml` & `itwinai-0.0.2/use-cases/3dgan/interLink/3dgan-inference.yaml`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/3dgan/interLink/3dgan-train.yaml` & `itwinai-0.0.2/use-cases/3dgan/interLink/3dgan-train.yaml`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/3dgan/interLink/README.md` & `itwinai-0.0.2/use-cases/3dgan/interLink/README.md`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/3dgan/model.py` & `itwinai-0.0.2/use-cases/3dgan/model.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/3dgan/saver.py` & `itwinai-0.0.2/use-cases/3dgan/saver.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/3dgan/startscript` & `itwinai-0.0.2/use-cases/3dgan/startscript`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/3dgan/trainer.py` & `itwinai-0.0.2/use-cases/3dgan/trainer.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/README.md` & `itwinai-0.0.2/use-cases/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# itwinai use cases
+# interTwin use cases integrated into itwinai
 
-Show how `itwinai` can be used. Each use case folder contains:
+Show how `itwinai` can be used to support scientific use cases. Each use case folder contains:
 
-- `pipeline.yaml`: textual description of the ML workflow for that use case
-- `train.py`: entry point of training workflow.
-- `startscript`: file to execute the training workflow on a SLURM-based cluster.
+- A YAML configuration file describing the ML workflows for that use case.
+- A SLURM job script, used to execute the ML workflows on a SLURM-based cluster.
 - `requirements.txt`: (optional) use case-specific requirements. can be installed with:
   
   ```bash
   cd use/case/folder
   # After activating the correct environment...
   pip install -r requirements.txt
   ```
@@ -24,19 +23,11 @@
 ```
 
 Alternatively, you can use the use case Docker image, if available.
 
 Then, go to the use case's directory:
 
 ```bash
-cd /use/case/path
+cd use/case/path
 ```
 
-From here you can run the use case (having activated the correct Python env):
-
-```bash
-# Locally
-python train.py [OPTIONS...]
-
-# With SLURM: stdout and stderr will be saved to job.out and job.err files
-sbatch startscript
-```
+From there you can run the use case following the instruction provided in the use case's folder.
```

### Comparing `itwinai-0.0.1/use-cases/cyclones/cyclones_vgg.py` & `itwinai-0.0.2/use-cases/cyclones/cyclones_vgg.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/cyclones/dataloader.py` & `itwinai-0.0.2/use-cases/cyclones/dataloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,67 @@
+from typing import List, Dict, Optional
 from os import listdir
 from os.path import join, exists
-from itwinai.components import DataGetter, monitor_exec
-from typing import List, Dict
-from lib.macros import (
-    PatchType,
-    LabelNoCyclone,
-    AugmentationType,
-)
 
 import gdown
 import numpy as np
 
+from itwinai.components import DataGetter, monitor_exec
 
-from lib.tfrecords.functions import read_tfrecord_as_tensor
-from lib.scaling import save_tf_minmax
-from lib.tfrecords.dataset import eFlowsTFRecordDataset
-from lib.transform import (
+from src.macros import (
+    PatchType,
+    LabelNoCyclone,
+    AugmentationType,
+)
+from src.tfrecords.functions import read_tfrecord_as_tensor
+from src.scaling import save_tf_minmax
+from src.tfrecords.dataset import eFlowsTFRecordDataset
+from src.transform import (
     coo_left_right,
     coo_up_down,
     coo_rot180,
     msk_left_right,
     msk_up_down,
     msk_rot180,
 )
 
 
-class TensorflowDataGetter(DataGetter):
+class CyclonesDataGetter(DataGetter):
     def __init__(
         self,
-        data_url: str,
+        dataset_url: str,
         patch_type: PatchType,
         shuffle: bool,
         split_ratio: List[float],
-        batch_size: int,
         augment: bool,
         epochs: int,
         target_scale: bool,
         label_no_cyclone: LabelNoCyclone,
         aug_type: AugmentationType,
         experiment: Dict,
         global_config: Dict,
-        shuffle_buffer: int = None,
-        data_path: str = "tmp_data",
-        local_dataset_path: str = "trainval"
+        shuffle_buffer: Optional[int] = None,
+        dataset_root: str = "tmp_data",
+        tfrecords_dir: str = "trainval"
     ):
         super().__init__()
         self.save_parameters(**self.locals2params(locals()))
-        self.data_url = data_url
-        self.batch_size = batch_size
+        self.dataset_url = dataset_url
         self.split_ratio = split_ratio
         self.epochs = epochs
         self.target_scale = target_scale
         self.label_no_cyclone = label_no_cyclone.value
         self.shuffle_buffer = shuffle_buffer
         self.aug_type = aug_type.value
         self.patch_type = patch_type.value
         self.augment = augment
         self.global_config = global_config
         self.shuffle = shuffle
-        self.data_path = data_path
-        self.local_dataset_path = local_dataset_path
+        self.dataset_root = dataset_root
+        self.tfrecords_dir = tfrecords_dir
         self.drv_vars, self.coo_vars = (
             experiment["DRV_VARS_1"],
             experiment["COO_VARS_1"],
         )
         self.msk_var = (
             None if experiment["MSK_VAR_1"] == "None"
             else experiment["MSK_VAR_!"]
@@ -92,14 +90,68 @@
                 }
         else:
             self.aug_fns = {}
 
         # Parse global config
         self.setup_config(self.global_config)
 
+    def setup_config(self, config: Dict) -> None:
+        self.shape = config["shape"]
+        root_dir = config["root_dir"]
+
+        # Download data
+        if not exists(self.dataset_root):
+            gdown.download_folder(
+                url=self.dataset_url, quiet=False,
+                # verify=False,
+                output=self.dataset_root
+            )
+
+        # Scalar fields
+        self.root_dir = root_dir
+        self.tfrecords_path = join(self.dataset_root,
+                                   self.tfrecords_dir)
+        self.scaler_file = join(config["scaler_dir"], "minmax.tfrecord")
+
+        # get records filenames
+        self.cyclone_files = sorted(
+            [
+                join(self.tfrecords_path, f)
+                for f in listdir(self.tfrecords_path)
+                if f.endswith(".tfrecord") and f.startswith(
+                    PatchType.CYCLONE.value)
+            ]
+        )
+        if self.patch_type == PatchType.NEAREST.value:
+            self.adj_files = sorted(
+                [
+                    join(self.tfrecords_path, f)
+                    for f in listdir(self.tfrecords_path)
+                    if f.endswith(".tfrecord") and f.startswith(
+                        PatchType.NEAREST.value)
+                ]
+            )
+        elif self.patch_type == PatchType.ALLADJACENT.value:
+            self.adj_files = sorted(
+                [
+                    join(self.tfrecords_path, f)
+                    for f in listdir(self.tfrecords_path)
+                    if f.endswith(".tfrecord")
+                    and f.startswith(PatchType.ALLADJACENT.value)
+                ]
+            )
+        self.random_files = sorted(
+            [
+                join(self.tfrecords_path, f)
+                for f in listdir(self.tfrecords_path)
+                if f.endswith(".tfrecord") and f.startswith(
+                    PatchType.RANDOM.value)
+            ]
+        )
+
     def split_files(self, files, ratio):
         n = len(files)
         return (
             files[0: int(ratio[0] * n)],
             files[int(ratio[0] * n): int((ratio[0] + ratio[1]) * n)],
         )
 
@@ -134,15 +186,14 @@
 
         # instantiate training, validation and test sets
         # Contains: (dataset, n_count)
         train_dataset = eFlowsTFRecordDataset(
             cyc_fnames=train_c_fs,
             adj_fnames=train_a_fs,
             rnd_fnames=train_r_fs,
-            batch_size=self.batch_size,
             epochs=self.epochs,
             scalers=scalers,
             target_scale=self.target_scale,
             shape=self.shape,
             label_no_cyclone=self.label_no_cyclone,
             drv_vars=self.drv_vars,
             coo_vars=self.coo_vars,
@@ -152,76 +203,21 @@
             patch_type=self.patch_type,
             aug_type=self.aug_type,
         )
         valid_dataset = eFlowsTFRecordDataset(
             cyc_fnames=valid_c_fs,
             adj_fnames=valid_a_fs,
             rnd_fnames=valid_r_fs,
-            batch_size=self.batch_size,
             epochs=self.epochs,
             scalers=scalers,
             target_scale=self.target_scale,
             shape=self.shape,
             label_no_cyclone=self.label_no_cyclone,
             drv_vars=self.drv_vars,
             coo_vars=self.coo_vars,
             msk_var=self.msk_var,
             shuffle_buffer=self.shuffle_buffer,
             aug_fns=self.aug_fns,
             patch_type=self.patch_type,
             aug_type=self.aug_type,
         )
         return train_dataset, valid_dataset, self.channels
-
-    def setup_config(self, config: Dict) -> None:
-        self.shape = config["shape"]
-        root_dir = config["root_dir"]
-
-        # Download data
-        if not exists(self.data_path):
-            gdown.download_folder(
-                url=self.data_url, quiet=False,
-                # verify=False,
-                output=self.data_path
-            )
-
-        # Scalar fields
-        self.root_dir = root_dir
-        self.dataset_dir = join(self.data_path,
-                                self.local_dataset_path)
-        self.scaler_file = join(config["scaler_dir"], "minmax.tfrecord")
-
-        # get records filenames
-        self.cyclone_files = sorted(
-            [
-                join(self.dataset_dir, f)
-                for f in listdir(self.dataset_dir)
-                if f.endswith(".tfrecord") and f.startswith(
-                    PatchType.CYCLONE.value)
-            ]
-        )
-        if self.patch_type == PatchType.NEAREST.value:
-            self.adj_files = sorted(
-                [
-                    join(self.dataset_dir, f)
-                    for f in listdir(self.dataset_dir)
-                    if f.endswith(".tfrecord") and f.startswith(
-                        PatchType.NEAREST.value)
-                ]
-            )
-        elif self.patch_type == PatchType.ALLADJACENT.value:
-            self.adj_files = sorted(
-                [
-                    join(self.dataset_dir, f)
-                    for f in listdir(self.dataset_dir)
-                    if f.endswith(".tfrecord")
-                    and f.startswith(PatchType.ALLADJACENT.value)
-                ]
-            )
-        self.random_files = sorted(
-            [
-                join(self.dataset_dir, f)
-                for f in listdir(self.dataset_dir)
-                if f.endswith(".tfrecord") and f.startswith(
-                    PatchType.RANDOM.value)
-            ]
-        )
```

### Comparing `itwinai-0.0.1/use-cases/cyclones/lib/callbacks.py` & `itwinai-0.0.2/use-cases/cyclones/src/callbacks.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/cyclones/lib/macros.py` & `itwinai-0.0.2/use-cases/cyclones/src/macros.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/cyclones/lib/scaling.py` & `itwinai-0.0.2/use-cases/cyclones/src/scaling.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/cyclones/lib/strategy.py` & `itwinai-0.0.2/use-cases/cyclones/src/strategy.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/cyclones/lib/tfrecords/functions.py` & `itwinai-0.0.2/use-cases/cyclones/src/tfrecords/functions.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/cyclones/lib/transform.py` & `itwinai-0.0.2/use-cases/cyclones/src/transform.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/cyclones/lib/utils.py` & `itwinai-0.0.2/use-cases/cyclones/src/utils.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/cyclones/startscript` & `itwinai-0.0.2/use-cases/mnist/torch/startscript.sh`

 * *Files 13% similar despite different names*

```diff
@@ -25,11 +25,10 @@
 ml --force purge
 ml Stages/2023 StdEnv/2023 NVHPC/23.1 OpenMPI/4.1.4 cuDNN/8.6.0.163-CUDA-11.7 Python/3.10.4 HDF5 libaio/0.3.112 GCC/11.3.0
 
 # shellcheck source=/dev/null
 source ~/.bashrc
 
 # ON LOGIN NODE download datasets:
-# ../../.venv-tf/bin/python train.py -p pipeline.yaml --download-only
-
-source ../../.venv-tf/bin/activate
-srun python train.py -p pipeline.yaml
+# ../../../.venv-pytorch/bin/itwinai exec-pipeline --config config.yaml --pipe-key training_pipeline --steps dataloading_step
+source ../../../.venv-pytorch/bin/activate
+srun itwinai exec-pipeline --config config.yaml --pipe-key training_pipeline
```

### Comparing `itwinai-0.0.1/use-cases/cyclones/train.py` & `itwinai-0.0.2/use-cases/cyclones/train.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,20 +14,29 @@
 from typing import Dict
 import argparse
 import logging
 from os.path import join
 from os import makedirs
 from datetime import datetime
 
+# # the mock-0.3.1 dir contains testcase.py, testutils.py & mock.py
 from itwinai.parser import ConfigParser, ArgumentParser
 
-from lib.macros import PATCH_SIZE, SHAPE
+from src.macros import PATCH_SIZE, SHAPE
 
 
-def setup_config(args) -> Dict:
+def dynamic_config(args) -> Dict:
+    """Generates a configuration with values computed at runtime.
+
+    Args:
+        args (argparse.Namespace): arguments parsed from command line.
+
+    Returns:
+        Dict: configuration.
+    """
     config = {}
 
     # Paths, Folders
     FORMATTED_DATETIME = str(datetime.now().strftime("%Y-%m-%d_%H-%M-%S"))
     MODEL_BACKUP_DIR = join(args.root_dir, "models/")
     EXPERIMENTS_DIR = join(args.root_dir, "experiments")
     RUN_DIR = join(EXPERIMENTS_DIR, args.run_name +
@@ -77,39 +86,35 @@
         "-p", "--pipeline", type=str, required=True,
         help='Configuration file to the pipeline to execute.'
     )
     parser.add_argument("-r", "--root_dir", type=str, default='./data')
     parser.add_argument("--data_path", type=str,
                         default='./data/data_path')
     parser.add_argument("-n", "--run_name", default="noname", type=str)
-    parser.add_argument("-e", "--epochs", default=1, type=int)
-    parser.add_argument("-b", "--batch_size", default=32, type=int)
     parser.add_argument(
         '-d', '--download-only',
         action=argparse.BooleanOptionalAction,
         default=False,
         help=('Whether to download only the dataset and exit execution '
               '(suggested on login nodes of HPC systems)')
     )
+
     args = parser.parse_args()
-    global_config = setup_config(args)
+    global_config = dynamic_config(args)
 
     # Create parser for the pipeline
-    downloader_params = "pipeline.init_args.steps.download-step.init_args."
-    trainer_params = "pipeline.init_args.steps.training-step.init_args."
     pipe_parser = ConfigParser(
         config=args.pipeline,
         override_keys={
-            downloader_params + "epochs": args.epochs,
-            downloader_params + "batch_size": args.batch_size,
-            downloader_params + "data_path": args.data_path,
-            downloader_params + "global_config": global_config,
-            trainer_params + "global_config": global_config
+            "dataset_root": args.data_path,
+            "global_config": global_config
         }
     )
-    pipeline = pipe_parser.parse_pipeline()
+    pipeline = pipe_parser.parse_pipeline(
+        pipeline_nested_key='training_pipeline'
+    )
 
     if args.download_only:
         print('Downloading datasets and exiting...')
         pipeline = pipeline[:1]
 
     pipeline.execute()
```

### Comparing `itwinai-0.0.1/use-cases/mnist/tensorflow/dataloader.py` & `itwinai-0.0.2/use-cases/mnist/tensorflow/dataloader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 from typing import Tuple
 import tensorflow.keras as keras
 import tensorflow as tf
 
-from itwinai.components import DataGetter, DataPreproc, monitor_exec
+from itwinai.components import DataGetter, DataProcessor, monitor_exec
 
 
 class MNISTDataGetter(DataGetter):
     def __init__(self):
         super().__init__()
         self.save_parameters(**self.locals2params(locals()))
 
     @monitor_exec
     def execute(self) -> Tuple:
         train, test = keras.datasets.mnist.load_data()
         return train, test
 
 
-class MNISTDataPreproc(DataPreproc):
+class MNISTDataPreproc(DataProcessor):
     def __init__(self, classes: int):
         super().__init__()
         self.save_parameters(**self.locals2params(locals()))
         self.classes = classes
 
     @monitor_exec
     def execute(
         self,
         *datasets,
     ) -> Tuple:
         options = tf.data.Options()
         options.experimental_distribute.auto_shard_policy = (
-            tf.data.experimental.AutoShardPolicy.FILE)
+            tf.data.experimental.AutoShardPolicy.DATA)
         preprocessed = []
         for dataset in datasets:
             x, y = dataset
             y = keras.utils.to_categorical(y, self.classes)
             sliced = tf.data.Dataset.from_tensor_slices((x, y))
             sliced = sliced.with_options(options)
             preprocessed.append(sliced)
```

### Comparing `itwinai-0.0.1/use-cases/mnist/tensorflow/pipeline.yaml` & `itwinai-0.0.2/use-cases/virgo/config.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-pipeline:
+# General configuration
+data_root: data
+epochs: 2
+batch_size: 20
+strategy: ddp
+checkpoint_path: checkpoints/epoch_{}.pth
+
+training_pipeline:
   class_path: itwinai.pipeline.Pipeline
   init_args:
     steps:
-      - class_path: dataloader.MNISTDataGetter
-
-      - class_path: dataloader.MNISTDataPreproc
+      - class_path: data.TimeSeriesDatasetGenerator
         init_args:
-          classes: 10
-
-      - class_path: trainer.MNISTTrainer
+          data_root: ${data_root}
+      - class_path: data.TimeSeriesDatasetSplitter
         init_args:
-          epochs: 10
-          batch_size: 17
-
-          loss:
-            class_path: tensorflow.keras.losses.CategoricalCrossentropy
-            init_args:
-              from_logits: False
-
-          optimizer: 
-            class_path: tensorflow.keras.optimizers.Adam
-            init_args: 
-                learning_rate: 0.001
-
-          model:
-            class_path: itwinai.tensorflow.models.mnist.MNIST_Model
+          train_proportion: 0.9
+          rnd_seed: 42
+          images_dataset: data/Image_dataset_synthetic_64x64.pkl
+      - class_path: data.TimeSeriesProcessor
+      - class_path: trainer.NoiseGeneratorTrainer
+        init_args:
+          generator: unet
+          batch_size: ${batch_size}
+          num_epochs: ${epochs}
+          strategy: ${strategy}
+          checkpoint_path: ${checkpoint_path}
+          logger:
+            class_path: itwinai.loggers.LoggersCollection
             init_args:
-              input_shape: [ 28, 28, 1 ]
-              output_shape: 10
-
-          strategy:
-            class_path: tensorflow.python.distribute.mirrored_strategy.MirroredStrategy
-
-          # logger: 
-          #   - class_path: itwinai.loggers.ConsoleLogger
-          #   - class_path: itwinai.loggers.MLFlowLogger
-          #     init_args:
-          #       experiment_name: MNIST classifier
-          #       log_freq: batch 
+              loggers:
+                - class_path: itwinai.loggers.ConsoleLogger
+                  init_args:
+                    log_freq: 100
+                - class_path: itwinai.loggers.MLFlowLogger
+                  init_args:
+                    experiment_name: Noise simulator (Virgo)
+                    log_freq: batch 
+
```

### Comparing `itwinai-0.0.1/use-cases/mnist/tensorflow/startscript` & `itwinai-0.0.2/use-cases/mnist/tensorflow/startscript.sh`

 * *Files 12% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 #SBATCH --mail-type=ALL
 #SBATCH --output=job.out
 #SBATCH --error=job.err
 #SBATCH --time=00:30:00
 
 # configure node and process count on the CM
 #SBATCH --partition=batch
-#SBATCH --nodes=1
+#SBATCH --nodes=2
 #SBATCH --ntasks-per-node=1
 #SBATCH --cpus-per-task=4
 #SBATCH --gpus-per-node=4
 
 #SBATCH --exclusive
 
 # gres options have to be disabled for deepv
 #SBATCH --gres=gpu:4
 
 # load modules
 ml --force purge
-ml Stages/2023 StdEnv/2023 NVHPC/23.1 OpenMPI/4.1.4 cuDNN/8.6.0.163-CUDA-11.7 Python/3.10.4 HDF5 libaio/0.3.112 GCC/11.3.0
+ml Stages/2024 GCC/12.3.0 OpenMPI CUDA/12 MPI-settings/CUDA Python/3.11 HDF5 PnetCDF libaio mpi4py CMake cuDNN/8.9.5.29-CUDA-12
 
 # shellcheck source=/dev/null
 source ~/.bashrc
 
 # ON LOGIN NODE download datasets:
-# ../../.venv-tf/bin/itwinai exec-pipeline --config pipeline.yaml --steps 0
-source ../../.venv-tf/bin/activate
-srun itwinai exec-pipeline --config pipeline.yaml
+# ../../../.venv-tf/bin/itwinai exec-pipeline --config pipeline.yaml --pipe-key pipeline --steps 0
+source ../../../envAItf_hdfml/bin/activate
+srun itwinai exec-pipeline --config pipeline.yaml --pipe-key pipeline -o verbose=2
```

### Comparing `itwinai-0.0.1/use-cases/mnist/torch/README.md` & `itwinai-0.0.2/use-cases/mnist/torch/README.md`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/mnist/torch/config.yaml` & `itwinai-0.0.2/use-cases/mnist/torch/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 epochs: 2
 strategy: ddp
 test_data_path: mnist-sample-data
 inference_model_mlflow_uri: mnist-pre-trained.pth
 predictions_dir: mnist-predictions
 predictions_file: predictions.csv
 class_labels: null
+checkpoints_location: checkpoints
+checkpoint_every: 1
 
 # Workflows configuration
 training_pipeline:
   class_path: itwinai.pipeline.Pipeline
   init_args:
     steps:
       dataloading_step:
@@ -64,20 +66,17 @@
                   init_args:
                     log_freq: 10000
                 - class_path: itwinai.loggers.MLFlowLogger
                   init_args:
                     experiment_name: MNIST classifier
                     log_freq: batch 
           strategy: ${strategy}
-          # checkpoint_every: 1
-          # cluster:
-          #   class_path: itwinai.torch.cluster.LocalCluster
-          #   init_args:
-          #     gpus: '0,1,2'
-          #     backend: nccl
+          checkpoint_every: ${checkpoint_every}
+          checkpoints_location: ${checkpoints_location}
+
 
 inference_pipeline:
   class_path: itwinai.pipeline.Pipeline
   init_args:
     steps:
       - class_path: dataloader.MNISTPredictLoader
         init_args:
```

### Comparing `itwinai-0.0.1/use-cases/mnist/torch/create_inference_sample.py` & `itwinai-0.0.2/use-cases/mnist/torch/create_inference_sample.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/mnist/torch/dataloader.py` & `itwinai-0.0.2/use-cases/mnist/torch/dataloader.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/mnist/torch/model.py` & `itwinai-0.0.2/use-cases/mnist/torch/model.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/mnist/torch/runall.sh` & `itwinai-0.0.2/use-cases/mnist/torch/runall.sh`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 #!/bin/bash
 
 # Python virtual environment (no conda/micromamba)
 PYTHON_VENV="../../../envAI_hdfml"
 
 # Clear SLURM logs (*.out and *.err files)
-rm -rf logs_slurm
+rm -rf logs_slurm checkpoints* mllogs*
 mkdir logs_slurm
 rm -rf logs_torchrun
 
 # DDP itwinai
 DIST_MODE="ddp"
 RUN_NAME="ddp-itwinai"
-TRAINING_CMD="$PYTHON_VENV/bin/itwinai exec-pipeline --config config.yaml --pipe-key training_pipeline -o strategy=ddp"
+TRAINING_CMD="$PYTHON_VENV/bin/itwinai exec-pipeline --config config.yaml --pipe-key training_pipeline -o strategy=ddp -o checkpoints_location=checkpoints_ddp"
 sbatch --export=ALL,DIST_MODE="$DIST_MODE",RUN_NAME="$RUN_NAME",TRAINING_CMD="$TRAINING_CMD",PYTHON_VENV="$PYTHON_VENV" \
     --job-name="$RUN_NAME-n$N" \
     --output="logs_slurm/job-$RUN_NAME-n$N.out" \
     --error="logs_slurm/job-$RUN_NAME-n$N.err" \
     slurm.sh
 
 # DeepSpeed itwinai
 DIST_MODE="deepspeed"
 RUN_NAME="deepspeed-itwinai"
-TRAINING_CMD="$PYTHON_VENV/bin/itwinai exec-pipeline --config config.yaml --pipe-key training_pipeline -o strategy=deepspeed"
+TRAINING_CMD="$PYTHON_VENV/bin/itwinai exec-pipeline --config config.yaml --pipe-key training_pipeline -o strategy=deepspeed -o checkpoints_location=checkpoints_deepspeed"
 sbatch --export=ALL,DIST_MODE="$DIST_MODE",RUN_NAME="$RUN_NAME",TRAINING_CMD="$TRAINING_CMD",PYTHON_VENV="$PYTHON_VENV" \
     --job-name="$RUN_NAME-n$N" \
     --output="logs_slurm/job-$RUN_NAME-n$N.out" \
     --error="logs_slurm/job-$RUN_NAME-n$N.err" \
     slurm.sh
 
 # Horovod itwinai
 DIST_MODE="horovod"
 RUN_NAME="horovod-itwinai"
-TRAINING_CMD="$PYTHON_VENV/bin/itwinai exec-pipeline --config config.yaml --pipe-key training_pipeline -o strategy=horovod"
+TRAINING_CMD="$PYTHON_VENV/bin/itwinai exec-pipeline --config config.yaml --pipe-key training_pipeline -o strategy=horovod -o checkpoints_location=checkpoints_hvd"
 sbatch --export=ALL,DIST_MODE="$DIST_MODE",RUN_NAME="$RUN_NAME",TRAINING_CMD="$TRAINING_CMD",PYTHON_VENV="$PYTHON_VENV" \
     --job-name="$RUN_NAME-n$N" \
     --output="logs_slurm/job-$RUN_NAME-n$N.out" \
     --error="logs_slurm/job-$RUN_NAME-n$N.err" \
     slurm.sh
```

### Comparing `itwinai-0.0.1/use-cases/mnist/torch/saver.py` & `itwinai-0.0.2/use-cases/mnist/torch/saver.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/mnist/torch/slurm.sh` & `itwinai-0.0.2/use-cases/mnist/torch/slurm.sh`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/mnist/torch/startscript` & `itwinai-0.0.2/use-cases/mnist/torch-lightning/startscript`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/mnist/torch-lightning/config.yaml` & `itwinai-0.0.2/use-cases/mnist/torch-lightning/config.yaml`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/mnist/torch-lightning/dataloader.py` & `itwinai-0.0.2/use-cases/mnist/torch-lightning/dataloader.py`

 * *Files identical despite different names*

### Comparing `itwinai-0.0.1/use-cases/mnist/torch-lightning/utils.py` & `itwinai-0.0.2/use-cases/mnist/torch-lightning/utils.py`

 * *Files identical despite different names*

