# Comparing `tmp/vyper-0.4.0rc5.tar.gz` & `tmp/vyper-0.4.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vyper-0.4.0rc5.tar", last modified: Thu May 16 14:28:43 2024, max compression
+gzip compressed data, was "vyper-0.4.0rc6.tar", last modified: Thu May 30 22:54:27 2024, max compression
```

## Comparing `vyper-0.4.0rc5.tar` & `vyper-0.4.0rc6.tar`

### file list

```diff
@@ -1,607 +1,615 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.639678 vyper-0.4.0rc5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.563677 vyper-0.4.0rc5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.563677 vyper-0.4.0rc5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/.github/ISSUE_TEMPLATE/vip.md
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.567677 vyper-0.4.0rc5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/.github/workflows/era-tester.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/.github/workflows/ghcr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/.github/workflows/pull-request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/.github/workflows/release-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-16 14:28:43.639678 vyper-0.4.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.571677 vyper-0.4.0rc5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.571677 vyper-0.4.0rc5/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/_templates/versions.html
--rw-r--r--   0 runner    (1001) docker     (127)    39020 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/built-in-functions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/compiler-exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15623 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/compiling-a-contract.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/constants-and-vars.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/control-structures.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/deploying-contracts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/event-logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/installing-vyper.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/interfaces.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/natspec.rst
--rw-r--r--   0 runner    (1001) docker     (127)    64067 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/scoping-and-declarations.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/statements.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/structure-of-a-contract.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15593 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/style-guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/testing-contracts-brownie.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/testing-contracts-ethtester.rst
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/testing-contracts.rst
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/toctree.rst
--rw-r--r--   0 runner    (1001) docker     (127)    23266 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/types.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/versioning.rst
--rw-r--r--   0 runner    (1001) docker     (127)    29097 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/docs/vyper-by-example.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.571677 vyper-0.4.0rc5/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.571677 vyper-0.4.0rc5/examples/auctions/
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/examples/auctions/blind_auction.vy
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/examples/auctions/simple_open_auction.vy
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/examples/crowdfund.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.571677 vyper-0.4.0rc5/examples/factory/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/examples/factory/Exchange.vy
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/examples/factory/Factory.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.571677 vyper-0.4.0rc5/examples/market_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/examples/market_maker/on_chain_market_maker.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.571677 vyper-0.4.0rc5/examples/name_registry/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/examples/name_registry/name_registry.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.571677 vyper-0.4.0rc5/examples/safe_remote_purchase/
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/examples/safe_remote_purchase/safe_remote_purchase.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.571677 vyper-0.4.0rc5/examples/stock/
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/examples/stock/company.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.571677 vyper-0.4.0rc5/examples/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/examples/storage/advanced_storage.vy
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/examples/storage/storage.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.571677 vyper-0.4.0rc5/examples/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)    15365 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/examples/tokens/ERC1155ownable.vy
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/examples/tokens/ERC20.vy
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/examples/tokens/ERC4626.vy
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/examples/tokens/ERC721.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.571677 vyper-0.4.0rc5/examples/voting/
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/examples/voting/ballot.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.571677 vyper-0.4.0rc5/examples/wallet/
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/examples/wallet/wallet.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.575677 vyper-0.4.0rc5/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      265 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/hooks/build
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/make.cmd
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      207 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/quicktest.sh
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-16 14:28:43.639678 vyper-0.4.0rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.575677 vyper-0.4.0rc5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.575677 vyper-0.4.0rc5/tests/evm_backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/evm_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/evm_backends/abi.py
--rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/evm_backends/abi_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/evm_backends/base_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/evm_backends/pyevm_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/evm_backends/revm_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.575677 vyper-0.4.0rc5/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.559677 vyper-0.4.0rc5/tests/functional/builtins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.579677 vyper-0.4.0rc5/tests/functional/builtins/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13889 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_abi_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_abi_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_addmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_blobhash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)    20237 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    19256 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_create_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_ec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_ecrecover.py
--rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_extract32.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_floor.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_is_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_method_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_minmax_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_mulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)    16628 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_raw_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_send.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_uint2str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_unary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/codegen/test_unsafe_math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.579677 vyper-0.4.0rc5/tests/functional/builtins/folding/
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/folding/test_abs.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/folding/test_addmod_mulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/folding/test_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/folding/test_epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/folding/test_floor_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/folding/test_fold_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/folding/test_keccak_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/folding/test_len.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/folding/test_min_max.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/builtins/folding/test_powmod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.583677 vyper-0.4.0rc5/tests/functional/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.583677 vyper-0.4.0rc5/tests/functional/codegen/calling_convention/
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/calling_convention/test_default_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/calling_convention/test_default_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/calling_convention/test_erc20_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)    57029 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/calling_convention/test_external_contract_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/calling_convention/test_return.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/calling_convention/test_self_call_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.583677 vyper-0.4.0rc5/tests/functional/codegen/environment_variables/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/environment_variables/test_blobbasefee.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/environment_variables/test_block_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/environment_variables/test_blockhash.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/environment_variables/test_tx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.587677 vyper-0.4.0rc5/tests/functional/codegen/features/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.587677 vyper-0.4.0rc5/tests/functional/codegen/features/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/decorators/test_nonreentrant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/decorators/test_payable.py
--rw-r--r--   0 runner    (1001) docker     (127)    13982 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/decorators/test_private.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/decorators/test_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/decorators/test_pure.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/decorators/test_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.587677 vyper-0.4.0rc5/tests/functional/codegen/features/iteration/
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/iteration/test_break.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/iteration/test_continue.py
--rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/iteration/test_for_in_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    11326 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/iteration/test_for_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/iteration/test_range_in.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_address_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_assert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_assert_unreachable.py
--rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_bytes_map_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    15767 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_clampers.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_conditionals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_gas.py
--rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_immutable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    15018 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_internal_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    29735 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_logging_bytes_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_logging_from_call.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_memory_alloc.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_memory_dealloc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_reverting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_short_circuiting.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_string_map_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_ternary.py
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/features/test_transient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.587677 vyper-0.4.0rc5/tests/functional/codegen/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/integration/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/integration/test_crowdfund.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/integration/test_escrow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.591677 vyper-0.4.0rc5/tests/functional/codegen/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/modules/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/modules/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/modules/test_flag_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/modules/test_interface_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/modules/test_module_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/modules/test_module_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/modules/test_nonreentrant.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/modules/test_stateless_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.591677 vyper-0.4.0rc5/tests/functional/codegen/storage_variables/
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/storage_variables/test_getters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/storage_variables/test_setters.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/storage_variables/test_storage_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/test_call_graph_stability.py
--rw-r--r--   0 runner    (1001) docker     (127)    15992 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    14744 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/test_selector_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/test_selector_table_stability.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.591677 vyper-0.4.0rc5/tests/functional/codegen/types/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.595677 vyper-0.4.0rc5/tests/functional/codegen/types/numbers/
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_decimals.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_division.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_exponents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_isqrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_modulo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_signed_ints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_sqrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_unsigned_ints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/test_array_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/test_bytes_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/test_bytes_zero_padding.py
--rw-r--r--   0 runner    (1001) docker     (127)    48925 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/test_dynamic_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/test_identifier_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)    23216 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/test_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/test_node_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/test_string_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/codegen/types/test_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.559677 vyper-0.4.0rc5/tests/functional/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.595677 vyper-0.4.0rc5/tests/functional/examples/auctions/
--rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/examples/auctions/test_blind_auction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/examples/auctions/test_simple_open_auction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.595677 vyper-0.4.0rc5/tests/functional/examples/company/
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/examples/company/test_company.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.595677 vyper-0.4.0rc5/tests/functional/examples/crowdfund/
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/examples/crowdfund/test_crowdfund_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.595677 vyper-0.4.0rc5/tests/functional/examples/factory/
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/examples/factory/test_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.595677 vyper-0.4.0rc5/tests/functional/examples/market_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/examples/market_maker/test_on_chain_market_maker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.595677 vyper-0.4.0rc5/tests/functional/examples/name_registry/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/examples/name_registry/test_name_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.595677 vyper-0.4.0rc5/tests/functional/examples/safe_remote_purchase/
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.595677 vyper-0.4.0rc5/tests/functional/examples/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/examples/storage/test_advanced_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/examples/storage/test_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.595677 vyper-0.4.0rc5/tests/functional/examples/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)    13340 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/examples/tokens/test_erc1155.py
--rw-r--r--   0 runner    (1001) docker     (127)    13167 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/examples/tokens/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/examples/tokens/test_erc4626.py
--rw-r--r--   0 runner    (1001) docker     (127)    10201 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/examples/tokens/test_erc721.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.595677 vyper-0.4.0rc5/tests/functional/examples/voting/
--rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/examples/voting/test_ballot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.595677 vyper-0.4.0rc5/tests/functional/examples/wallet/
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/examples/wallet/test_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.595677 vyper-0.4.0rc5/tests/functional/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/grammar/test_grammar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.603677 vyper-0.4.0rc5/tests/functional/syntax/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.607677 vyper-0.4.0rc5/tests/functional/syntax/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_argument_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_call_violation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_constancy_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_function_declaration_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_instantiation_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_invalid_literal_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_invalid_payable.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_invalid_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_invalid_type_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_namespace_collision.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_overflow_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_structure_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_syntax_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_type_mismatch_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_undeclared_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_variable_declaration_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_vyper_exception_pos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.607677 vyper-0.4.0rc5/tests/functional/syntax/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/modules/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/modules/test_deploy_visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/modules/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/modules/test_implements.py
--rw-r--r--   0 runner    (1001) docker     (127)    28823 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/modules/test_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.607677 vyper-0.4.0rc5/tests/functional/syntax/names/
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/names/test_event_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/names/test_function_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/names/test_variable_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.607677 vyper-0.4.0rc5/tests/functional/syntax/signatures/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/signatures/test_invalid_function_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/signatures/test_method_id_conflicts.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_abi_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_abi_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_abs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_addmulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_address_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_ann_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_as_uint256.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_blockscope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_bool_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_chainid.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_code_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_codehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_conditionals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_create_with_code_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_dynamic_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_external_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_extract32.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_floor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_for_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_functions_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_immutables.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_invalids.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_len.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_method_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_minmax_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_msg_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_nested_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_no_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_powmod.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_print.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_raw_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_return_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_self_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_selfdestruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_send.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_ternary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_tuple_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_uint2str.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_unary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/functional/syntax/test_unbalanced_return.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.607677 vyper-0.4.0rc5/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.607677 vyper-0.4.0rc5/tests/unit/abi_types/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/abi_types/test_invalid_abi_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.611677 vyper-0.4.0rc5/tests/unit/ast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.611677 vyper-0.4.0rc5/tests/unit/ast/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/nodes/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/nodes/test_compare_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/nodes/test_fold_binop_decimal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/nodes/test_fold_binop_int.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/nodes/test_fold_boolop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/nodes/test_fold_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/nodes/test_fold_subscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/nodes/test_fold_unaryop.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/nodes/test_from_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/nodes/test_get_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/nodes/test_get_descendants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/nodes/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/test_annotate_and_optimize_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)    68091 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/test_ast_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/test_metadata_journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/test_natspec.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/test_pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/ast/test_source_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.559677 vyper-0.4.0rc5/tests/unit/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.611677 vyper-0.4.0rc5/tests/unit/cli/storage_layout/
--rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/cli/storage_layout/test_storage_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/cli/storage_layout/test_storage_layout_overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.611677 vyper-0.4.0rc5/tests/unit/cli/vyper_compile/
--rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/cli/vyper_compile/test_compile_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/cli/vyper_compile/test_parse_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.615677 vyper-0.4.0rc5/tests/unit/cli/vyper_json/
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/cli/vyper_json/test_compile_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/cli/vyper_json/test_get_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/cli/vyper_json/test_get_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/cli/vyper_json/test_output_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.615677 vyper-0.4.0rc5/tests/unit/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.615677 vyper-0.4.0rc5/tests/unit/compiler/asm/
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/asm/test_asm_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.615677 vyper-0.4.0rc5/tests/unit/compiler/ir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/ir/test_calldatacopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/ir/test_compile_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/ir/test_optimize_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/ir/test_repeat.py
--rw-r--r--   0 runner    (1001) docker     (127)    13843 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/ir/test_with.py
--rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/test_bytecode_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    24877 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/test_compile_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/test_default_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/test_input_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/test_opcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/test_pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/test_sha3_32.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/test_source_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.619677 vyper-0.4.0rc5/tests/unit/compiler/venom/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/venom/test_convert_basicblock_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/venom/test_dominator_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/venom/test_duplicate_operands.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/venom/test_liveness_simple_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/venom/test_make_ssa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/venom/test_multi_entry_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/venom/test_sccp.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/venom/test_stack_at_external_return.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/compiler/venom/test_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.619677 vyper-0.4.0rc5/tests/unit/semantics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.619677 vyper-0.4.0rc5/tests/unit/semantics/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/semantics/analysis/test_array_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/semantics/analysis/test_cyclic_function_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/semantics/analysis/test_for_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/semantics/analysis/test_potential_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/semantics/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/semantics/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/semantics/test_storage_slots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.619677 vyper-0.4.0rc5/tests/unit/semantics/types/
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/semantics/types/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/semantics/types/test_pure_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/semantics/types/test_size_in_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/semantics/types/test_type_from_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/semantics/types/test_type_from_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.619677 vyper-0.4.0rc5/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/unit/utils/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.619677 vyper-0.4.0rc5/vyper/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/abi_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.623677 vyper-0.4.0rc5/vyper/ast/
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ast/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ast/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ast/grammar.lark
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ast/grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ast/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ast/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ast/natspec.py
--rw-r--r--   0 runner    (1001) docker     (127)    45908 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ast/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ast/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ast/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ast/pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ast/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ast/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.623677 vyper-0.4.0rc5/vyper/builtins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/builtins/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/builtins/_signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/builtins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    91509 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/builtins/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.623677 vyper-0.4.0rc5/vyper/builtins/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/builtins/interfaces/IERC165.vyi
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/builtins/interfaces/IERC20.vyi
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/builtins/interfaces/IERC20Detailed.vyi
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/builtins/interfaces/IERC4626.vyi
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/builtins/interfaces/IERC721.vyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.627678 vyper-0.4.0rc5/vyper/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/cli/compile_archive.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13322 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/cli/vyper_compile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/cli/vyper_ir.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15875 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/cli/vyper_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.627678 vyper-0.4.0rc5/vyper/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/abi_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13045 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    42566 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    30724 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/expr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/external_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.627678 vyper-0.4.0rc5/vyper/codegen/function_definitions/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/function_definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/function_definitions/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7802 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/function_definitions/external_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/function_definitions/internal_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/ir_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/jumptable_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/keccak256_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/memory_allocator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21180 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/return_.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/self_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/codegen/stmt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.631677 vyper-0.4.0rc5/vyper/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/compiler/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/compiler/input_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/compiler/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/compiler/output_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)    12134 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/compiler/phases.py
--rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/compiler/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/compiler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.631677 vyper-0.4.0rc5/vyper/evm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/evm/address_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/evm/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.631677 vyper-0.4.0rc5/vyper/ir/
--rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45899 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ir/compile_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)    24821 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ir/optimizer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/ir/s_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.631677 vyper-0.4.0rc5/vyper/semantics/
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.635677 vyper-0.4.0rc5/vyper/semantics/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/analysis/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/analysis/constant_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/analysis/data_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/analysis/getters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/analysis/global_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/analysis/import_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/analysis/levenshtein_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    37249 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/analysis/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    37057 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/analysis/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    23690 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/analysis/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/data_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.635677 vyper-0.4.0rc5/vyper/semantics/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/types/bytestrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    31063 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/types/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    18935 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/types/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/types/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/types/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/types/subscriptable.py
--rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/types/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/semantics/types/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    16938 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.635677 vyper-0.4.0rc5/vyper/venom/
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.639678 vyper-0.4.0rc5/vyper/venom/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/analysis/cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/analysis/dfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/analysis/dominators.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/analysis/dup_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/analysis/liveness.py
--rw-r--r--   0 runner    (1001) docker     (127)    16451 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/basicblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    19028 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/ir_node_to_venom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.639678 vyper-0.4.0rc5/vyper/venom/passes/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/passes/base_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/passes/dft.py
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/passes/make_ssa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/passes/mem2var.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/passes/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/passes/remove_unused_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.639678 vyper-0.4.0rc5/vyper/venom/passes/sccp/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/passes/sccp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/passes/sccp/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/passes/sccp/sccp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/passes/simplify_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/passes/stack_reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/passes/store_elimination.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/stack_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20025 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/venom/venom_to_assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-16 14:28:43.000000 vyper-0.4.0rc5/vyper/version.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 14:28:40.000000 vyper-0.4.0rc5/vyper/vyper_git_commithash.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-16 14:28:32.000000 vyper-0.4.0rc5/vyper/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:28:43.623677 vyper-0.4.0rc5/vyper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-16 14:28:43.000000 vyper-0.4.0rc5/vyper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21056 2024-05-16 14:28:43.000000 vyper-0.4.0rc5/vyper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:28:43.000000 vyper-0.4.0rc5/vyper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-16 14:28:43.000000 vyper-0.4.0rc5/vyper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-16 14:28:43.000000 vyper-0.4.0rc5/vyper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 14:28:43.000000 vyper-0.4.0rc5/vyper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.233980 vyper-0.4.0rc6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.157980 vyper-0.4.0rc6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.157980 vyper-0.4.0rc6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/.github/ISSUE_TEMPLATE/vip.md
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.157980 vyper-0.4.0rc6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/.github/workflows/era-tester.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/.github/workflows/ghcr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/.github/workflows/pull-request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/.github/workflows/release-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-30 22:54:27.233980 vyper-0.4.0rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.161980 vyper-0.4.0rc6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.161980 vyper-0.4.0rc6/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/_templates/versions.html
+-rw-r--r--   0 runner    (1001) docker     (127)    39020 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/built-in-functions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/compiler-exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18285 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/compiling-a-contract.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/constants-and-vars.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14436 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/control-structures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/deploying-contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/event-logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/installing-vyper.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/interfaces.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/natspec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    64067 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/scoping-and-declarations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/statements.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/structure-of-a-contract.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/style-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/testing-contracts-brownie.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/testing-contracts-titanoboa.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/testing-contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/toctree.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    23356 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/using-modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/versioning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    29097 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/docs/vyper-by-example.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.161980 vyper-0.4.0rc6/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.161980 vyper-0.4.0rc6/examples/auctions/
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/examples/auctions/blind_auction.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/examples/auctions/simple_open_auction.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/examples/crowdfund.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.161980 vyper-0.4.0rc6/examples/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/examples/factory/Exchange.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/examples/factory/Factory.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.161980 vyper-0.4.0rc6/examples/market_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/examples/market_maker/on_chain_market_maker.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.165980 vyper-0.4.0rc6/examples/name_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/examples/name_registry/name_registry.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.165980 vyper-0.4.0rc6/examples/safe_remote_purchase/
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/examples/safe_remote_purchase/safe_remote_purchase.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.165980 vyper-0.4.0rc6/examples/stock/
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/examples/stock/company.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.165980 vyper-0.4.0rc6/examples/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/examples/storage/advanced_storage.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/examples/storage/storage.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.165980 vyper-0.4.0rc6/examples/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)    15365 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/examples/tokens/ERC1155ownable.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/examples/tokens/ERC20.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/examples/tokens/ERC4626.vy
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/examples/tokens/ERC721.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.165980 vyper-0.4.0rc6/examples/voting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/examples/voting/ballot.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.165980 vyper-0.4.0rc6/examples/wallet/
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/examples/wallet/wallet.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.165980 vyper-0.4.0rc6/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      265 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/hooks/build
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/make.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      207 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/quicktest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-30 22:54:27.233980 vyper-0.4.0rc6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.165980 vyper-0.4.0rc6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.165980 vyper-0.4.0rc6/tests/evm_backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/evm_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/evm_backends/abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/evm_backends/abi_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/evm_backends/base_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/evm_backends/pyevm_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/evm_backends/revm_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.165980 vyper-0.4.0rc6/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.149980 vyper-0.4.0rc6/tests/functional/builtins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.169980 vyper-0.4.0rc6/tests/functional/builtins/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32698 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_abi_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12027 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_abi_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_addmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_blobhash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20237 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20204 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_create_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_ec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_ecrecover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15885 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_extract32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_floor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_is_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_method_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_minmax_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_mulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16628 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_raw_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_uint2str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_unary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/codegen/test_unsafe_math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.173980 vyper-0.4.0rc6/tests/functional/builtins/folding/
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/folding/test_abs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/folding/test_addmod_mulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/folding/test_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/folding/test_epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/folding/test_floor_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/folding/test_fold_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/folding/test_keccak_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/folding/test_len.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/folding/test_min_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/builtins/folding/test_powmod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.173980 vyper-0.4.0rc6/tests/functional/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.173980 vyper-0.4.0rc6/tests/functional/codegen/calling_convention/
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/calling_convention/test_default_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/calling_convention/test_default_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/calling_convention/test_erc20_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58155 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/calling_convention/test_external_contract_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15850 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/calling_convention/test_internal_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/calling_convention/test_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/calling_convention/test_self_call_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.173980 vyper-0.4.0rc6/tests/functional/codegen/environment_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/environment_variables/test_blobbasefee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/environment_variables/test_block_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/environment_variables/test_blockhash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/environment_variables/test_tx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.177980 vyper-0.4.0rc6/tests/functional/codegen/features/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.181980 vyper-0.4.0rc6/tests/functional/codegen/features/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/decorators/test_nonreentrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/decorators/test_payable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13982 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/decorators/test_private.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/decorators/test_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/decorators/test_pure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/decorators/test_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.181980 vyper-0.4.0rc6/tests/functional/codegen/features/iteration/
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/iteration/test_break.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/iteration/test_continue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/iteration/test_for_in_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/iteration/test_for_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/iteration/test_range_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_address_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_assert_unreachable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_bytes_map_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15767 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_clampers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_immutable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29735 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_logging_bytes_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_logging_from_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_memory_alloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_memory_dealloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_reverting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_short_circuiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_string_map_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6650 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/features/test_transient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.181980 vyper-0.4.0rc6/tests/functional/codegen/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/integration/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/integration/test_crowdfund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/integration/test_escrow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.181980 vyper-0.4.0rc6/tests/functional/codegen/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/modules/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/modules/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/modules/test_flag_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/modules/test_interface_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/modules/test_module_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/modules/test_module_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/modules/test_nonreentrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/modules/test_stateless_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.181980 vyper-0.4.0rc6/tests/functional/codegen/storage_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/storage_variables/test_getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/storage_variables/test_setters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/storage_variables/test_storage_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/test_call_graph_stability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15992 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14744 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/test_selector_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/test_selector_table_stability.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.185979 vyper-0.4.0rc6/tests/functional/codegen/types/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.185979 vyper-0.4.0rc6/tests/functional/codegen/types/numbers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_decimals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_division.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_exponents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_isqrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_modulo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10757 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_signed_ints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_sqrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_unsigned_ints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/test_array_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/test_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/test_bytes_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/test_bytes_zero_padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49454 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/test_dynamic_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/test_identifier_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23216 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/test_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/test_node_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/test_string_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/codegen/types/test_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.149980 vyper-0.4.0rc6/tests/functional/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.185979 vyper-0.4.0rc6/tests/functional/examples/auctions/
+-rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/examples/auctions/test_blind_auction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/examples/auctions/test_simple_open_auction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.185979 vyper-0.4.0rc6/tests/functional/examples/company/
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/examples/company/test_company.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.185979 vyper-0.4.0rc6/tests/functional/examples/crowdfund/
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/examples/crowdfund/test_crowdfund_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.185979 vyper-0.4.0rc6/tests/functional/examples/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/examples/factory/test_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.185979 vyper-0.4.0rc6/tests/functional/examples/market_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/examples/market_maker/test_on_chain_market_maker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.185979 vyper-0.4.0rc6/tests/functional/examples/name_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/examples/name_registry/test_name_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.185979 vyper-0.4.0rc6/tests/functional/examples/safe_remote_purchase/
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.189980 vyper-0.4.0rc6/tests/functional/examples/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/examples/storage/test_advanced_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/examples/storage/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.189980 vyper-0.4.0rc6/tests/functional/examples/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)    13340 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/examples/tokens/test_erc1155.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13167 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/examples/tokens/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/examples/tokens/test_erc4626.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10201 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/examples/tokens/test_erc721.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.189980 vyper-0.4.0rc6/tests/functional/examples/voting/
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/examples/voting/test_ballot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.189980 vyper-0.4.0rc6/tests/functional/examples/wallet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/examples/wallet/test_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.189980 vyper-0.4.0rc6/tests/functional/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/grammar/test_grammar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.197980 vyper-0.4.0rc6/tests/functional/syntax/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.201979 vyper-0.4.0rc6/tests/functional/syntax/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_argument_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_call_violation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_constancy_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_function_declaration_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_instantiation_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_invalid_literal_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_invalid_payable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_invalid_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_invalid_type_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_namespace_collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_overflow_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_structure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_syntax_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_type_mismatch_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_undeclared_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_variable_declaration_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_vyper_exception_pos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.201979 vyper-0.4.0rc6/tests/functional/syntax/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/modules/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/modules/test_deploy_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/modules/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/modules/test_implements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28823 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/modules/test_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.201979 vyper-0.4.0rc6/tests/functional/syntax/names/
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/names/test_event_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/names/test_function_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/names/test_variable_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.201979 vyper-0.4.0rc6/tests/functional/syntax/signatures/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/signatures/test_invalid_function_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/signatures/test_method_id_conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_abi_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_abi_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_abs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_addmulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_address_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_ann_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_as_uint256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_blockscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_bool_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_chainid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_code_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_codehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_create_with_code_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_dynamic_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_external_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_extract32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_floor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_for_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_functions_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_immutables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_invalids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_len.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_method_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_minmax_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_msg_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_nested_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_no_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_powmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_raw_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_return_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_self_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_selfdestruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_tuple_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_uint2str.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_unary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/functional/syntax/test_unbalanced_return.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.201979 vyper-0.4.0rc6/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.201979 vyper-0.4.0rc6/tests/unit/abi_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/abi_types/test_invalid_abi_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.201979 vyper-0.4.0rc6/tests/unit/ast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.205979 vyper-0.4.0rc6/tests/unit/ast/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/nodes/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/nodes/test_compare_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/nodes/test_fold_binop_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/nodes/test_fold_binop_int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/nodes/test_fold_boolop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/nodes/test_fold_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/nodes/test_fold_subscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/nodes/test_fold_unaryop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/nodes/test_from_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/nodes/test_get_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/nodes/test_get_descendants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/nodes/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/test_annotate_and_optimize_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68091 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/test_ast_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/test_metadata_journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/test_natspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/test_pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/ast/test_source_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.149980 vyper-0.4.0rc6/tests/unit/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.205979 vyper-0.4.0rc6/tests/unit/cli/storage_layout/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/cli/storage_layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/cli/storage_layout/test_storage_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10728 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/cli/storage_layout/test_storage_layout_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/cli/storage_layout/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.205979 vyper-0.4.0rc6/tests/unit/cli/vyper_compile/
+-rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/cli/vyper_compile/test_compile_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/cli/vyper_compile/test_parse_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.205979 vyper-0.4.0rc6/tests/unit/cli/vyper_json/
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/cli/vyper_json/test_compile_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/cli/vyper_json/test_get_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/cli/vyper_json/test_get_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/cli/vyper_json/test_output_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.209980 vyper-0.4.0rc6/tests/unit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.209980 vyper-0.4.0rc6/tests/unit/compiler/asm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/asm/test_asm_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.209980 vyper-0.4.0rc6/tests/unit/compiler/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/ir/test_calldatacopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/ir/test_compile_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/ir/test_optimize_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/ir/test_repeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13843 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/ir/test_with.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14979 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/test_bytecode_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/test_compile_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/test_default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/test_input_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/test_opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/test_pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/test_sha3_32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/test_source_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.209980 vyper-0.4.0rc6/tests/unit/compiler/venom/
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/venom/test_algebraic_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/venom/test_branch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/venom/test_convert_basicblock_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/venom/test_dominator_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/venom/test_duplicate_operands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/venom/test_liveness_simple_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/venom/test_make_ssa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/venom/test_multi_entry_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/venom/test_sccp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/venom/test_stack_at_external_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/compiler/venom/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.209980 vyper-0.4.0rc6/tests/unit/semantics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.213980 vyper-0.4.0rc6/tests/unit/semantics/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/semantics/analysis/test_array_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/semantics/analysis/test_cyclic_function_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/semantics/analysis/test_for_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/semantics/analysis/test_potential_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/semantics/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/semantics/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/semantics/test_storage_slots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.213980 vyper-0.4.0rc6/tests/unit/semantics/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/semantics/types/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/semantics/types/test_pure_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/semantics/types/test_size_in_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/semantics/types/test_type_from_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/semantics/types/test_type_from_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.213980 vyper-0.4.0rc6/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/unit/utils/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.213980 vyper-0.4.0rc6/vyper/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/abi_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.217980 vyper-0.4.0rc6/vyper/ast/
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ast/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ast/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ast/grammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ast/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ast/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ast/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ast/natspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45908 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ast/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ast/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ast/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ast/pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ast/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ast/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.217980 vyper-0.4.0rc6/vyper/builtins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/builtins/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/builtins/_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/builtins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92093 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/builtins/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.217980 vyper-0.4.0rc6/vyper/builtins/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/builtins/interfaces/IERC165.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/builtins/interfaces/IERC20.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/builtins/interfaces/IERC20Detailed.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/builtins/interfaces/IERC4626.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/builtins/interfaces/IERC721.vyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.217980 vyper-0.4.0rc6/vyper/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/cli/compile_archive.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13424 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/cli/vyper_compile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/cli/vyper_ir.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15875 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/cli/vyper_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.221979 vyper-0.4.0rc6/vyper/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/abi_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13045 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46924 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31279 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/external_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.221979 vyper-0.4.0rc6/vyper/codegen/function_definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/function_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/function_definitions/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7802 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/function_definitions/external_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/function_definitions/internal_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24048 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/ir_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/jumptable_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/keccak256_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/memory_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21180 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/return_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/self_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13789 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/codegen/stmt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.221979 vyper-0.4.0rc6/vyper/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/compiler/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/compiler/input_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14667 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/compiler/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/compiler/output_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/compiler/phases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/compiler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/compiler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.225979 vyper-0.4.0rc6/vyper/evm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/evm/address_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/evm/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.225979 vyper-0.4.0rc6/vyper/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45925 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ir/compile_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24821 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ir/optimizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/ir/s_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.225979 vyper-0.4.0rc6/vyper/semantics/
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.225979 vyper-0.4.0rc6/vyper/semantics/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10414 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/analysis/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/analysis/constant_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14613 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/analysis/data_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/analysis/getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/analysis/global_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/analysis/import_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/analysis/levenshtein_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37249 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/analysis/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36843 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/analysis/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23690 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/analysis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/data_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.229979 vyper-0.4.0rc6/vyper/semantics/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/types/bytestrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30717 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/types/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18935 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/types/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12480 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/types/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/types/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/types/subscriptable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/semantics/types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17097 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.229979 vyper-0.4.0rc6/vyper/venom/
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.229979 vyper-0.4.0rc6/vyper/venom/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/analysis/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/analysis/dfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/analysis/dominators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/analysis/dup_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/analysis/liveness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16885 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/basicblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8914 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19028 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/ir_node_to_venom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.233980 vyper-0.4.0rc6/vyper/venom/passes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/passes/algebraic_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/passes/base_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/passes/branch_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/passes/dft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/passes/make_ssa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/passes/mem2var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/passes/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/passes/remove_unused_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.233980 vyper-0.4.0rc6/vyper/venom/passes/sccp/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/passes/sccp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/passes/sccp/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/passes/sccp/sccp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/passes/simplify_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/passes/stack_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/passes/store_elimination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/stack_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20800 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/venom/venom_to_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-30 22:54:26.000000 vyper-0.4.0rc6/vyper/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 22:54:24.000000 vyper-0.4.0rc6/vyper/vyper_git_commithash.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-30 22:54:16.000000 vyper-0.4.0rc6/vyper/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:54:27.213980 vyper-0.4.0rc6/vyper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-30 22:54:27.000000 vyper-0.4.0rc6/vyper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21374 2024-05-30 22:54:27.000000 vyper-0.4.0rc6/vyper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 22:54:27.000000 vyper-0.4.0rc6/vyper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-30 22:54:27.000000 vyper-0.4.0rc6/vyper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-30 22:54:27.000000 vyper-0.4.0rc6/vyper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-30 22:54:27.000000 vyper-0.4.0rc6/vyper.egg-info/top_level.txt
```

### Comparing `vyper-0.4.0rc5/.github/ISSUE_TEMPLATE/bug.md` & `vyper-0.4.0rc6/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/.github/ISSUE_TEMPLATE/vip.md` & `vyper-0.4.0rc6/.github/ISSUE_TEMPLATE/vip.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/.github/workflows/build.yml` & `vyper-0.4.0rc6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/.github/workflows/codeql.yml` & `vyper-0.4.0rc6/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/.github/workflows/era-tester.yml` & `vyper-0.4.0rc6/.github/workflows/era-tester.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/.github/workflows/ghcr.yml` & `vyper-0.4.0rc6/.github/workflows/ghcr.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/.github/workflows/pull-request.yaml` & `vyper-0.4.0rc6/.github/workflows/pull-request.yaml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/.github/workflows/release-pypi.yml` & `vyper-0.4.0rc6/.github/workflows/release-pypi.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/.github/workflows/test.yml` & `vyper-0.4.0rc6/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,20 @@
         # https://docs.github.com/en/actions/using-jobs/using-a-matrix-for-your-jobs#expanding-or-adding-matrix-configurations
         include:
           # test default settings with 3.11 across all supported evm versions
           - evm-version: london
           - evm-version: paris
           - evm-version: shanghai
 
+          # test pre-cancun with opt-codesize and opt-none
+          - evm-version: shanghai
+            opt-mode: none
+          - evm-version: shanghai
+            opt-mode: codesize
+
           # test py-evm
           - evm-backend: py-evm
             evm-version: shanghai
 
           - evm-backend: py-evm
             evm-version: cancun
```

### Comparing `vyper-0.4.0rc5/.pre-commit-config.yaml` & `vyper-0.4.0rc6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/Dockerfile` & `vyper-0.4.0rc6/Dockerfile`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/LICENSE` & `vyper-0.4.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/Makefile` & `vyper-0.4.0rc6/Makefile`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/PKG-INFO` & `vyper-0.4.0rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vyper
-Version: 0.4.0rc5
+Version: 0.4.0rc6
 Summary: Vyper: the Pythonic Programming Language for the EVM
 Home-page: https://github.com/vyperlang/vyper
 Author: Vyper Team
 Author-email: 
 License: Apache License 2.0
 Keywords: ethereum evm smart contract language
 Classifier: Intended Audience :: Developers
```

### Comparing `vyper-0.4.0rc5/README.md` & `vyper-0.4.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/SECURITY.md` & `vyper-0.4.0rc6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/docs/Makefile` & `vyper-0.4.0rc6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/docs/_templates/versions.html` & `vyper-0.4.0rc6/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/docs/built-in-functions.rst` & `vyper-0.4.0rc6/docs/built-in-functions.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/docs/compiler-exceptions.rst` & `vyper-0.4.0rc6/docs/compiler-exceptions.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/docs/compiling-a-contract.rst` & `vyper-0.4.0rc6/docs/compiling-a-contract.rst`

 * *Files 12% similar despite different names*

```diff
@@ -2,38 +2,40 @@
 ********************
 
 Command-Line Compiler Tools
 ===========================
 
 Vyper includes the following command-line scripts for compiling contracts:
 
-* ``vyper``: Compiles vyper contract files into ``IR`` or bytecode
+* ``vyper``: Compiles vyper contract or archive files
 * ``vyper-json``: Provides a JSON interface to the compiler
 
 .. note::
 
     The ``--help`` flag gives verbose explanations of how to use each of these scripts.
 
+.. _vyper-cli-command:
+
 vyper
 -----
 
-``vyper`` provides command-line access to the compiler. It can generate various outputs including simple binaries, ASTs, interfaces and source mappings.
+``vyper`` provides CLI access to the compiler. It can generate various outputs including simple binaries, ASTs, interfaces and source mappings.
 
 To compile a contract:
 
 .. code:: shell
 
     $ vyper yourFileName.vy
 
 
 Include the ``-f`` flag to specify which output formats to return. Use ``vyper --help`` for a full list of output options.
 
 .. code:: shell
 
-    $ vyper -f abi,abi_python,bytecode,bytecode_runtime,interface,external_interface,ast,annotated_ast,ir,ir_json,ir_runtime,hex-ir,asm,opcodes,opcodes_runtime,source_map,method_identifiers,userdoc,devdoc,metadata,combined_json,layout yourFileName.vy
+    $ vyper -f abi,abi_python,bytecode,bytecode_runtime,blueprint_bytecode,interface,external_interface,ast,annotated_ast,integrity,ir,ir_json,ir_runtime,asm,opcodes,opcodes_runtime,source_map,source_map_runtime,archive,solc_json,method_identifiers,userdoc,devdoc,metadata,combined_json,layout yourFileName.vy
 
 .. note::
     The ``opcodes`` and ``opcodes_runtime`` output of the compiler has been returning incorrect opcodes since ``0.2.0`` due to a lack of 0 padding (patched via `PR 3735 <https://github.com/vyperlang/vyper/pull/3735>`_). If you rely on these functions for debugging, please use the latest patched versions.
 
 The ``-p`` flag allows you to set a root path that is used when searching for interface files to import.  If none is given, it will default to the current working directory. See :ref:`searching_for_imports` for more information.
 
 .. code:: shell
@@ -91,15 +93,14 @@
 Importing Interfaces
 ~~~~~~~~~~~~~~~~~~~~
 
 ``vyper-json`` searches for imported interfaces in the following sequence:
 
 1. Interfaces defined in the ``interfaces`` field of the input JSON.
 2. Derived interfaces generated from contracts in the ``sources`` field of the input JSON.
-3. (Optional) The local filesystem, if a root path was explicitly declared via the ``-p`` flag.
 
 See :ref:`searching_for_imports` for more information on Vyper's import system.
 
 Online Compilers
 ================
 
 Try VyperLang!
@@ -117,15 +118,15 @@
    While the Vyper version of the Remix IDE compiler is updated on a regular basis, it might be a bit behind the latest version found in the master branch of the repository. Make sure the byte code matches the output from your local compiler.
 
 .. _optimization-mode:
 
 Compiler Optimization Modes
 ===========================
 
-The vyper CLI tool accepts an optimization mode ``"none"``, ``"codesize"``, or ``"gas"`` (default). It can be set using the ``--optimize`` flag. For example, invoking ``vyper --optimize codesize MyContract.vy`` will compile the contract, optimizing for code size. As a rough summary of the differences between gas and codesize mode, in gas optimized mode, the compiler will try to generate bytecode which minimizes gas (up to a point), including:
+The Vyper CLI tool accepts an optimization mode ``"none"``, ``"codesize"``, or ``"gas"`` (default). It can be set using the ``--optimize`` flag. For example, invoking ``vyper --optimize codesize MyContract.vy`` will compile the contract, optimizing for code size. As a rough summary of the differences between gas and codesize mode, in gas optimized mode, the compiler will try to generate bytecode which minimizes gas (up to a point), including:
 
 * using a sparse selector table which optimizes for gas over codesize
 * inlining some constants, and
 * trying to unroll some loops, especially for data copies.
 
 In codesize optimized mode, the compiler will try hard to minimize codesize by
 
@@ -188,28 +189,67 @@
 
 .. py:attribute:: cancun (default)
 
    - The ``transient`` keyword allows declaration of variables which live in transient storage
    - Functions marked with ``@nonreentrant`` are protected with TLOAD/TSTORE instead of SLOAD/SSTORE
    - The ``MCOPY`` opcode will be generated automatically by the compiler for most memory operations.
 
+.. _integrity-hash:
+
+Integrity Hash
+==============
+
+To help tooling detect whether two builds are the same, Vyper provides the ``-f integrity`` output, which outputs the integrity hash of a contract. The integrity hash is recursively defined as the sha256 of the source code with the integrity hashes of its dependencies (imports).
+
+.. _vyper-archives:
+
+Vyper Archives
+==============
+
+A Vyper archive is a compileable bundle of input sources and settings. Technically, it is a `ZIP file <https://en.wikipedia.org/wiki/ZIP_(file_format)>`_, with a special structure to make it useable as input to the compiler. It can use any suffix, but the convention is to use a ``.zip`` suffix or ``.vyz`` suffix. It must contain a ``MANIFEST/`` folder, with the following directory structure.
+
+::
+
+    MANIFEST
+    ├── cli_settings.txt
+    ├── compilation_targets
+    ├── compiler_version
+    ├── integrity
+    ├── searchpaths
+    └── settings.json
+
+* ``cli_settings.txt`` is a text representation of the settings that were used on the compilation run that generated this archive.
+* ``compilation_targets`` is a newline separated list of compilation targets. Currently only one compilation is supported
+* ``compiler_version`` is a text representation of the compiler version used to generate this archive
+* ``integrity`` is the :ref:`integrity hash <integrity-hash>` of the input contract
+* ``searchpaths`` is a newline-separated list of the search paths used on this compilation run
+* ``settings.json`` is a json representation of the settings used on this compilation run. It is 1:1 with ``cli_settings.txt``, but both are provided as they are convenient for different workflows (typically, manually vs automated).
+
+A Vyper archive file can be produced by requesting the ``-f archive`` output format. The compiler can also produce the archive in base64 encoded form using the ``--base64`` flag. The Vyper compiler can accept both ``.vyz`` and base64-encoded Vyper archives directly as input.
+
+.. code-block:: bash
+
+    $ vyper -f archive my_contract.vy -o my_contract.vyz  # write the archive to my_contract.vyz
+    $ vyper -f archive my_contract.vy --base64 > my_contract.vyz.b64  # write the archive, as base64-encoded text
+    $ vyper my_contract.vyz  # compile my_contract.vyz
+    $ vyper my_contract.vyz.b64  # compile my_contract.vyz.b64
 
 Compiler Input and Output JSON Description
 ==========================================
 
-Especially when dealing with complex or automated setups, the recommended way to compile is to use :ref:`vyper-json` and the JSON-input-output interface.
+JSON input/output is provided for compatibility with solidity, however, the recommended way is to use the aforementioned :ref:`Vyper archives <vyper-archives>`. So-called "standard json" input can be generated from a contract using the ``vyper -f solc_json`` output format.
 
 Where possible, the Vyper JSON compiler formats follow those of `Solidity <https://solidity.readthedocs.io/en/latest/using-the-compiler.html#compiler-input-and-output-json-description>`_.
 
 .. _vyper-json-input:
 
 Input JSON Description
 ----------------------
 
-The following example describes the expected input format of ``vyper-json``. Comments are of course not permitted and used here *only for explanatory purposes*.
+The following example describes the expected input format of ``vyper-json``. (Comments are not normally permitted in JSON and are used here for explanatory purposes).
 
 .. code-block:: json
 
     {
         // Required: Source code language. Must be set to "Vyper".
         "language": "Vyper",
         // Required
@@ -219,18 +259,18 @@
                 // Optional: keccak256 hash of the source file
                 "keccak256": "0x234...",
                 // Required: literal contents of the source file
                 "content": "@external\ndef foo() -> bool:\n    return True"
             }
         },
         // Optional
-        // Interfaces given here are made available for import by the sources
+        // Sources given here are made available for import by the contracts
         // that are compiled. If the suffix is ".vy", the compiler will expect
-        // a contract-as-interface using proper Vyper syntax. If the suffix is
-        // "abi" the compiler will expect an ABI object.
+        // Vyper syntax. If the suffix is "abi" the compiler will expect an
+        // ABI object.
         "interfaces": {
             "contracts/bar.vy": {
                 "content": ""
             },
             "contracts/baz.json": {
                 "abi": []
             }
@@ -241,14 +281,19 @@
             // optional, optimization mode
             // defaults to "gas". can be one of "gas", "codesize", "none",
             // false  and true (the last two are for backwards compatibility).
             "optimize": "gas",
             // optional, whether or not the bytecode should include Vyper's signature
             // defaults to true
             "bytecodeMetadata": true,
+            // optional, whether to use the experimental venom pipeline
+            // defaults to false
+            "experimentalCodegen": false,
+            // the search paths to use for resolving imports
+            "search_paths": [],
             // The following is used to select desired outputs based on file names.
             // File names are given as keys, a star as a file name matches all files.
             // Outputs can also follow the Solidity format where second level keys
             // denoting contract names - all 2nd level outputs are applied to the file.
             //
             // To select all possible compiler outputs: "outputSelection: { '*': ["*"] }"
             // Note that this might slow down the compilation process needlessly.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vyper-0.4.0rc5/docs/conf.py` & `vyper-0.4.0rc6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/docs/constants-and-vars.rst` & `vyper-0.4.0rc6/docs/constants-and-vars.rst`

 * *Files 2% similar despite different names*

```diff
@@ -97,10 +97,10 @@
 Custom constants can be defined at a global level in Vyper. To define a constant, make use of the ``constant`` keyword.
 
 .. code-block:: vyper
 
     TOTAL_SUPPLY: constant(uint256) = 10000000
     total_supply: public(uint256)
 
-    @external
+    @deploy
     def __init__():
         self.total_supply = TOTAL_SUPPLY
```

### Comparing `vyper-0.4.0rc5/docs/contributing.rst` & `vyper-0.4.0rc6/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/docs/control-structures.rst` & `vyper-0.4.0rc6/docs/control-structures.rst`

 * *Files 5% similar despite different names*

```diff
@@ -14,20 +14,25 @@
 
     @external
     def bid():
         ...
 
 Functions may be called internally or externally depending on their :ref:`visibility <function-visibility>`. Functions may accept input arguments and return variables in order to pass values between them.
 
-.. _function-visibility:
-
 Visibility
 ----------
 
-All functions must include exactly one visibility decorator.
+.. _function-visibility:
+
+You can optionally declare a function's visibility by using a :ref:`decorator <function-decorators>`. There are three visibility levels in Vyper:
+
+    * ``@external``: exposed in the selector table, can be called by an external call into this contract
+    * ``@internal`` (default): can be invoked only from within this contract. Not available to external callers
+    * ``@deploy``: constructor code. This is code which is invoked once in the lifetime of a contract, upon its deploy. It is not available at runtime to either external callers or internal call invocations. At this time, only the :ref:`__init__() function <init-function>` may be marked as ``@deploy``.
+
 
 External Functions
 ******************
 
 External functions (marked with the ``@external`` decorator) are a part of the contract interface and may only be called via transactions or from other contracts.
 
 .. code-block:: vyper
@@ -46,40 +51,70 @@
     For external functions with default arguments like ``def my_function(x: uint256, b: uint256 = 1)`` the Vyper compiler will generate ``N+1`` overloaded function selectors based on ``N`` default arguments.
 
 .. _structure-functions-internal:
 
 Internal Functions
 ******************
 
-Internal functions (marked with the ``@internal`` decorator) are only accessible from other functions within the same contract. They are called via the :ref:`self<constants-self>` object:
+Internal functions (optionally marked with the ``@internal`` decorator) are only accessible from other functions within the same contract. They are invoked via the :ref:`self<constants-self>` object:
 
 .. code-block:: vyper
 
-    @internal
-    def _times_two(amount: uint256, two: uint256 = 2) -> uint256:
-        return amount * two
+    def _times_two(amount: uint256) -> uint256:
+        return amount * 2
 
     @external
     def calculate(amount: uint256) -> uint256:
         return self._times_two(amount)
 
+Or for internal functions which are defined in :ref:`imported modules <modules>`, they are invoked by prefixing the name of the module to the function name:
+
+.. code-block:: vyper
+    import calculator_library
+
+    @external
+    def calculate(amount: uint256) -> uint256:
+        return calculator_library._times_two(amount)
+
+.. note::
+   As of v0.4.0, the ``@internal`` decorator is optional. That is, functions with no visibility decorator default to being ``internal``.
+
 .. note::
-    Since calling an ``internal`` function is realized by jumping to its entry label, the internal function dispatcher ensures the correctness of the jumps. Please note that for ``internal`` functions which use more than one default parameter, Vyper versions ``>=0.3.8`` are strongly recommended due to the security advisory `GHSA-ph9x-4vc9-m39g <https://github.com/vyperlang/vyper/security/advisories/GHSA-ph9x-4vc9-m39g>`_.
+    Please note that for ``internal`` functions which use more than one default parameter, Vyper versions ``>=0.3.8`` are recommended due to the security advisory `GHSA-ph9x-4vc9-m39g <https://github.com/vyperlang/vyper/security/advisories/GHSA-ph9x-4vc9-m39g>`_.
+
+
+The ``__init__`` Function
+-------------------------
+
+.. _init-function:
+
+The ``__init__()`` function, also known as the constructor, is a special initialization function that is only called at the time of deploying a contract. It can be used to set initial values for storage or immutable variables. It must be declared with the ``@deploy`` decorator. A common use case is to set an ``owner`` variable with the creator of the contract:
+
+.. code-block:: vyper
+
+    owner: address
+
+    @deploy
+    def __init__():
+        self.owner = msg.sender
+
+Additionally, :ref:`immutable variables <immutable-variables>` may only be set within the constructor.
+
 
 Mutability
 ----------
 
 .. _function-mutability:
 
 You can optionally declare a function's mutability by using a :ref:`decorator <function-decorators>`. There are four mutability levels:
 
-    * **Pure**: does not read from the contract state or any environment variables.
-    * **View**: may read from the contract state, but does not alter it.
-    * **Nonpayable**: may read from and write to the contract state, but cannot receive Ether.
-    * **Payable**: may read from and write to the contract state, and can receive Ether.
+    * ``@pure``: does not read from the contract state or any environment variables.
+    * ``@view``: may read from the contract state, but does not alter it.
+    * ``@nonpayable`` (default): may read from and write to the contract state, but cannot receive Ether.
+    * ``@payable``: may read from and write to the contract state, and can receive Ether.
 
 .. code-block:: vyper
 
     @view
     @external
     def readonly():
         # this function cannot write to state
@@ -147,15 +182,15 @@
     @payable
     def __default__():
         log Payment(msg.value, msg.sender)
 
 Considerations
 **************
 
-Just as in Solidity, Vyper generates a default function if one isn't found, in the form of a ``REVERT`` call. Note that this still `generates an exception <https://github.com/ethereum/wiki/wiki/Subtleties>`_ and thus will not succeed in receiving funds.
+Just as in Solidity, Vyper generates a default function if one isn't found, in the form of a ``REVERT`` call. Note that this rolls back state changes, and thus will not succeed in receiving funds.
 
 Ethereum specifies that the operations will be rolled back if the contract runs out of gas in execution. ``send`` calls to the contract come with a free stipend of 2300 gas, which does not leave much room to perform other operations except basic logging. **However**, if the sender includes a higher gas amount through a ``call`` instead of ``send``, then more complex functionality can be run.
 
 It is considered a best practice to ensure your payable default function is compatible with this stipend. The following operations will consume more than 2300 gas:
 
     * Writing to storage
     * Creating a contract
@@ -164,41 +199,25 @@
 
 Lastly, although the default function receives no arguments, it can still access the ``msg`` object, including:
 
     * the address of who is interacting with the contract (``msg.sender``)
     * the amount of ETH sent (``msg.value``)
     * the gas provided (``msg.gas``).
 
-The ``__init__`` Function
--------------------------
-
-``__init__`` is a special initialization function that may only be called at the time of deploying a contract. It can be used to set initial values for storage variables. A common use case is to set an ``owner`` variable with the creator the contract:
-
-.. code-block:: vyper
-
-    owner: address
-
-    @external
-    def __init__():
-        self.owner = msg.sender
-
-You cannot call to other contract functions from the initialization function.
-
 .. _function-decorators:
 
 Decorators Reference
 --------------------
 
-All functions must include one :ref:`visibility <function-visibility>` decorator (``@external`` or ``@internal``). The remaining decorators are optional.
-
 =============================== ===========================================================
 Decorator                       Description
 =============================== ===========================================================
-``@external``                   Function can only be called externally
+``@external``                   Function can only be called externally, it is part of the runtime selector table
 ``@internal``                   Function can only be called within current contract
+``@deploy``                     Function is called only at deploy time
 ``@pure``                       Function does not read contract state or environment variables
 ``@view``                       Function does not alter contract state
 ``@payable``                    Function is able to receive Ether
 ``@nonreentrant``               Function cannot be called back into during an external call
 =============================== ===========================================================
 
 ``if`` statements
@@ -229,73 +248,73 @@
 ``for`` loops
 =============
 
 The ``for`` statement is a control flow construct used to iterate over a value:
 
 .. code-block:: vyper
 
-    for i in <ITERABLE>:
+    for i: <TYPE> in <ITERABLE>:
         ...
 
 The iterated value can be a static array, a dynamic array, or generated from the built-in ``range`` function.
 
 Array Iteration
 ---------------
 
 You can use ``for`` to iterate through the values of any array variable:
 
 .. code-block:: vyper
 
     foo: int128[3] = [4, 23, 42]
-    for i in foo:
+    for i: int128 in foo:
         ...
 
 In the above, example, the loop executes three times with ``i`` assigned the values of ``4``, ``23``, and then ``42``.
 
-You can also iterate over a literal array, as long as a common type can be determined for each item in the array:
+You can also iterate over a literal array, as long as the annotated type is valid for each item in the array:
 
 .. code-block:: vyper
 
-    for i in [4, 23, 42]:
+    for i: int128 in [4, 23, 42]:
         ...
 
 Some restrictions:
 
 * You cannot iterate over a multi-dimensional array.  ``i`` must always be a base type.
 * You cannot modify a value in an array while it is being iterated, or call to a function that might modify the array being iterated.
 
 Range Iteration
 ---------------
 
 Ranges are created using the ``range`` function. The following examples are valid uses of ``range``:
 
 .. code-block:: vyper
 
-    for i in range(STOP):
+    for i: uint256 in range(STOP):
         ...
 
-``STOP`` is a literal integer greater than zero. ``i`` begins as zero and increments by one until it is equal to ``STOP``.
+``STOP`` is a literal integer greater than zero. ``i`` begins as zero and increments by one until it is equal to ``STOP``. ``i`` must be of the same type as ``STOP``.
 
 .. code-block:: vyper
 
-    for i in range(stop, bound=N):
+    for i: uint256 in range(stop, bound=N):
         ...
 
-Here, ``stop`` can be a variable with integer type, greater than zero. ``N`` must be a compile-time constant. ``i`` begins as zero and increments by one until it is equal to ``stop``. If ``stop`` is larger than ``N``, execution will revert at runtime. In certain cases, you may not have a guarantee that ``stop`` is less than ``N``, but still want to avoid the possibility of runtime reversion. To accomplish this, use the ``bound=`` keyword in combination with ``min(stop, N)`` as the argument to ``range``, like ``range(min(stop, N), bound=N)``. This is helpful for use cases like chunking up operations on larger arrays across multiple transactions.
+Here, ``stop`` can be a variable with integer type, greater than zero. ``N`` must be a compile-time constant. ``i`` begins as zero and increments by one until it is equal to ``stop``. If ``stop`` is larger than ``N``, execution will revert at runtime. In certain cases, you may not have a guarantee that ``stop`` is less than ``N``, but still want to avoid the possibility of runtime reversion. To accomplish this, use the ``bound=`` keyword in combination with ``min(stop, N)`` as the argument to ``range``, like ``range(min(stop, N), bound=N)``. This is helpful for use cases like chunking up operations on larger arrays across multiple transactions. ``i``, ``stop`` and ``N`` must be of the same type.
 
 Another use of range can be with ``START`` and ``STOP`` bounds.
 
 .. code-block:: vyper
 
-    for i in range(START, STOP):
+    for i: uint256 in range(START, STOP):
         ...
 
-Here, ``START`` and ``STOP`` are literal integers, with ``STOP`` being a greater value than ``START``. ``i`` begins as ``START`` and increments by one until it is equal to ``STOP``.
+Here, ``START`` and ``STOP`` are literal integers, with ``STOP`` being a greater value than ``START``. ``i`` begins as ``START`` and increments by one until it is equal to ``STOP``. ``i``, ``START`` and ``STOP`` must be of the same type.
 
 Finally, it is possible to use ``range`` with runtime `start` and `stop` values as long as a constant `bound` value is provided.
 In this case, Vyper checks at runtime that `end - start <= bound`.
-``N`` must be a compile-time constant.
+``N`` must be a compile-time constant. ``i``, ``stop`` and ``N`` must be of the same type.
 
 .. code-block:: vyper
 
-    for i in range(start, end, bound=N):
+    for i: uint256 in range(start, end, bound=N):
         ...
```

### Comparing `vyper-0.4.0rc5/docs/event-logging.rst` & `vyper-0.4.0rc6/docs/event-logging.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/docs/index.rst` & `vyper-0.4.0rc6/docs/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -19,21 +19,19 @@
 
 * **Bounds and overflow checking**: On array accesses and arithmetic.
 * **Support for signed integers and decimal fixed point numbers**
 * **Decidability**: It is possible to compute a precise upper bound for the gas consumption of any Vyper function call.
 * **Strong typing**
 * **Clean and understandable compiler code**
 * **Support for pure functions**: Anything marked ``pure`` is not allowed to change the state.
-* **Code reuse through composition**: Vyper supports code reuse through composition, and to help auditors, requires syntactic marking of dependencies which potentially modify state.
+* **Code reuse through composition**: Vyper supports code reuse through composition, and requires syntactic marking of dependencies which potentially modify state.
 
 Following the principles and goals, Vyper **does not** provide the following features:
 
 * **Modifiers**: For example in Solidity you can define a ``function foo() mod1 { ... }``, where ``mod1`` can be defined elsewhere in the code to include a check that is done before execution, a check that is done after execution, some state changes, or possibly other things. Vyper does not have this, because it makes it too easy to write misleading code. ``mod1`` just looks too innocuous for something that could add arbitrary pre-conditions, post-conditions or state changes. Also, it encourages people to write code where the execution jumps around the file, harming auditability. The usual use case for a modifier is something that performs a single check before execution of a program; our recommendation is to simply inline these checks as asserts.
 * **Class inheritance**: Class inheritance requires readers to jump between multiple files to understand what a program is doing, and requires readers to understand the rules of precedence in case of conflicts ("Which class's function ``X`` is the one that's actually used?").
 * **Inline assembly**: Adding inline assembly would make it no longer possible to search for a variable name in order to find all instances where that variable is read or modified.
 * **Function overloading**: This can cause lots of confusion on which function is called at any given time. Thus it's easier to write misleading code (``foo("hello")`` logs "hello" but ``foo("hello", "world")`` steals your funds). Another problem with function overloading is that it makes the code much harder to search through as you have to keep track on which call refers to which function.
 * **Operator overloading**: Operator overloading makes writing misleading code possible. For example ``+`` could be overloaded so that it executes commands that are not visible at a first glance, such as sending funds the user did not want to send.
 * **Recursive calling**: Recursive calling makes it impossible to set an upper bound on gas limits, opening the door for gas limit attacks.
 * **Infinite-length loops**: Similar to recursive calling, infinite-length loops make it impossible to set an upper bound on gas limits, opening the door for gas limit attacks.
 * **Binary fixed point**: Decimal fixed point is better, because any decimal fixed point value written as a literal in code has an exact representation, whereas with binary fixed point approximations are often required (e.g. (0.2)\ :sub:`10` = (0.001100110011...)\ :sub:`2`, which needs to be truncated), leading to unintuitive results, e.g. in Python 0.3 + 0.3 + 0.3 + 0.1 != 1.
-
-Vyper **does not** strive to be a 100% replacement for everything that can be done in Solidity; it will deliberately forbid things or make things harder if it deems fit to do so for the goal of increasing security.
```

### Comparing `vyper-0.4.0rc5/docs/installing-vyper.rst` & `vyper-0.4.0rc6/docs/installing-vyper.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/docs/interfaces.rst` & `vyper-0.4.0rc6/docs/interfaces.rst`

 * *Files 10% similar despite different names*

```diff
@@ -20,46 +20,56 @@
 
 The defined interface can then be used to make external calls, given a contract address:
 
 .. code-block:: vyper
 
     @external
     def test(foobar: FooBar):
-        foobar.calculate()
+        extcall foobar.test1()
+
+    @external
+    def test2(foobar: FooBar) -> uint256:
+        return staticcall foobar.calculate()
 
 The interface name can also be used as a type annotation for storage variables. You then assign an address value to the variable to access that interface. Note that casting an address to an interface is possible, e.g. ``FooBar(<address_var>)``:
 
 .. code-block:: vyper
 
     foobar_contract: FooBar
 
-    @external
+    @deploy
     def __init__(foobar_address: address):
         self.foobar_contract = FooBar(foobar_address)
 
     @external
     def test():
-        self.foobar_contract.calculate()
+        extcall self.foobar_contract.test1()
 
-Specifying ``payable`` or ``nonpayable`` annotation indicates that the call made to the external contract will be able to alter storage, whereas the ``view`` ``pure`` call will use a ``STATICCALL`` ensuring no storage can be altered during execution. Additionally, ``payable`` allows non-zero value to be sent along with the call.
+Specifying ``payable`` or ``nonpayable`` annotation in the interface indicates that the call made to the external contract will be able to alter storage, whereas ``view`` and ``pure`` calls will use a ``STATICCALL`` ensuring no storage can be altered during execution. Additionally, ``payable`` allows non-zero value to be sent along with the call.
+
+Either the ``extcall`` or ``staticcall`` keyword is required to precede the external call to distinguish it from internal calls. The keyword must match the visibility of the function, ``staticcall`` for ``pure`` and ``view`` functions, and ``extcall`` for ``payable`` and ``nonpayable`` functions. Additionally, the output of a ``staticcall`` must be assigned to a result.
+
+.. warning::
+
+    If the signature in an interface does not match the actual signature of the called contract, you can get runtime errors or undefined behavior. For instance, if you accidentally mark a ``nonpayable`` function as ``view``, calling that function may result in the EVM reverting execution in the called contract.
 
 .. code-block:: vyper
 
     interface FooBar:
         def calculate() -> uint256: pure
         def query() -> uint256: view
         def update(): nonpayable
         def pay(): payable
 
     @external
     def test(foobar: FooBar):
-        foobar.calculate()  # cannot change storage
-        foobar.query()  # cannot change storage, but reads itself
-        foobar.update()  # storage can be altered
-        foobar.pay(value=1)  # storage can be altered, and value can be sent
+        s: uint256 = staticcall foobar.calculate()  # cannot change storage
+        s = staticcall foobar.query()  # cannot change storage, but reads itself
+        extcall foobar.update()  # storage can be altered
+        extcall foobar.pay(value=1)  # storage can be altered, and value can be sent
 
 Vyper offers the option to set the following additional keyword arguments when making external calls:
 
 =============================== ===========================================================
 Keyword                         Description
 =============================== ===========================================================
 ``gas``                         Specify gas value for the call
@@ -68,103 +78,25 @@
 ``default_return_value``        Specify a default return value if no value is returned
 =============================== ===========================================================
 
 The ``default_return_value`` parameter can be used to handle ERC20 tokens affected by the missing return value bug in a way similar to OpenZeppelin's ``safeTransfer`` for Solidity:
 
 .. code-block:: vyper
 
-    IERC20(USDT).transfer(msg.sender, 1, default_return_value=True) # returns True
-    IERC20(USDT).transfer(msg.sender, 1) # reverts because nothing returned
+    extcall IERC20(USDT).transfer(msg.sender, 1, default_return_value=True) # returns True
+    extcall IERC20(USDT).transfer(msg.sender, 1) # reverts because nothing returned
 
 .. warning::
 
    When ``skip_contract_check=True`` is used and the called function returns data (ex.: ``x: uint256 = SomeContract.foo(skip_contract_check=True)``, no guarantees are provided by the compiler as to the validity of the returned value. In other words, it is undefined behavior what happens if the called contract did not exist. In particular, the returned value might point to garbage memory. It is therefore recommended to only use ``skip_contract_check=True`` to call contracts which have been manually ensured to exist at the time of the call.
 
-Importing Interfaces
-====================
-
-Interfaces are imported with ``import`` or ``from ... import`` statements.
-
-Imported interfaces are written using standard Vyper syntax. The body of each function is ignored when the interface is imported. If you are defining a standalone interface, it is normally specified by using a ``pass`` statement:
-
-.. code-block:: vyper
-
-    @external
-    def test1():
-        pass
-
-    @external
-    def calculate() -> uint256:
-        pass
-
-You can also import a fully implemented contract and Vyper will automatically convert it to an interface. It is even possible for a contract to import itself to gain access to its own interface.
-
-.. code-block:: vyper
-
-    import greeter as Greeter
-
-    name: public(String[10])
-
-    @external
-    def __init__(_name: String[10]):
-        self.name = _name
-
-    @view
-    @external
-    def greet() -> String[16]:
-        return concat("Hello ", Greeter(msg.sender).name())
-
-Imports via ``import``
-----------------------
-
-With absolute ``import`` statements, you **must** include an alias as a name for the imported package. In the following example, failing to include ``as Foo`` will raise a compile error:
-
-.. code-block:: vyper
-
-    import contract.foo as Foo
-
-Imports via ``from ... import``
--------------------------------
-
-Using ``from`` you can perform both absolute and relative imports. You may optionally include an alias - if you do not, the name of the interface will be the same as the file.
-
-.. code-block:: vyper
-
-    # without an alias
-    from contract import foo
-
-    # with an alias
-    from contract import foo as Foo
-
-Relative imports are possible by prepending dots to the contract name. A single leading dot indicates a relative import starting with the current package. Two leading dots indicate a relative import from the parent of the current package:
-
-.. code-block:: vyper
-
-    from . import foo
-    from ..interfaces import baz
-
-.. _searching_for_imports:
-
-Searching For Interface Files
------------------------------
-
-When looking for a file to import, Vyper will first search relative to the same folder as the contract being compiled. For absolute imports, it also searches relative to the root path for the project. Vyper checks for the file name with a ``.vy`` suffix first, then ``.json``.
-
-When using the command line compiler, the root path defaults to the current working directory. You can change it with the ``-p`` flag:
-
-::
-
-    $ vyper my_project/contracts/my_contract.vy -p my_project
-
-In the above example, the ``my_project`` folder is set as the root path. A contract cannot perform a relative import that goes beyond the top-level folder.
-
 Built-in Interfaces
 ===================
 
-Vyper includes common built-in interfaces such as `ERC20 <https://eips.ethereum.org/EIPS/eip-20>`_ and `ERC721 <https://eips.ethereum.org/EIPS/eip-721>`_. These are imported from ``ethereum.ercs``:
+Vyper includes common built-in interfaces such as `IERC20 <https://eips.ethereum.org/EIPS/eip-20>`_ and `IERC721 <https://eips.ethereum.org/EIPS/eip-721>`_. These are imported from ``ethereum.ercs``:
 
 .. code-block:: vyper
 
     from ethereum.ercs import IERC20
 
     implements: IERC20
 
@@ -178,46 +110,66 @@
 .. code-block:: vyper
 
     import an_interface as FooBarInterface
 
     implements: FooBarInterface
 
 
-This imports the defined interface from the vyper file at ``an_interface.vy`` (or ``an_interface.json`` if using ABI json interface type) and ensures your current contract implements all the necessary external functions. If any interface functions are not included in the contract, it will fail to compile. This is especially useful when developing contracts around well-defined standards such as ERC20.
+This imports the defined interface from the vyper file at ``an_interface.vyi`` (or ``an_interface.json`` if using ABI json interface type) and ensures your current contract implements all the necessary external functions. If any interface functions are not included in the contract, it will fail to compile. This is especially useful when developing contracts around well-defined standards such as ERC20.
 
 .. note::
 
   Interfaces that implement functions with return values that require an upper bound (e.g. ``Bytes``, ``DynArray``, or ``String``), the upper bound defined in the interface represents the lower bound of the implementation. Assuming a function ``my_func`` returns a value ``String[1]`` in the interface, this would mean for the implementation function of ``my_func`` that the return value must have **at least** length 1. This behavior might change in the future.
 
+.. note::
+
+  Prior to v0.4.0, ``implements`` required that events defined in an interface were re-defined in the "implementing" contract. As of v0.4.0, this is no longer required because events can be used just by importing them. Any events used in a contract will automatically be exported in the ABI output.
+
+Standalone Interfaces
+=====================
+
+Standalone interfaces are written using a variant of standard Vyper syntax. The body of each function must be an ellipsis (``...``). Interface files must have a ``.vyi`` suffix in order to be found by an import statement.
+
+.. code-block:: vyper
+    # ISomeInterface.vyi
+
+    @external
+    def test1():
+        ...
+
+    @external
+    def calculate() -> uint256:
+        ...
+
 Extracting Interfaces
 =====================
 
-Vyper has a built-in format option to allow you to make your own Vyper interfaces easily.
+Vyper has a built-in format option to allow you to easily export a Vyper interface from a pre-existing contract.
 
 ::
 
     $ vyper -f interface examples/voting/ballot.vy
 
     # Functions
 
     @view
     @external
     def delegated(addr: address) -> bool:
-        pass
+        ...
 
     # ...
 
-If you want to do an external call to another contract, Vyper provides an external interface extract utility as well.
+If you want to export it as an inline interface, Vyper provides a utility to extract that as well.
 
 ::
 
     $ vyper -f external_interface examples/voting/ballot.vy
 
     # External Contracts
     interface Ballot:
         def delegated(addr: address) -> bool: view
         def directlyVoted(addr: address) -> bool: view
         def giveRightToVote(voter: address): nonpayable
         def forwardWeight(delegate_with_weight_to_forward: address): nonpayable
         # ...
 
-The output can then easily be copy-pasted to be consumed.
+The output can then easily be copy-pasted directly in a regular vyper file.
```

### Comparing `vyper-0.4.0rc5/docs/logo.svg` & `vyper-0.4.0rc6/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/docs/make.bat` & `vyper-0.4.0rc6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/docs/natspec.rst` & `vyper-0.4.0rc6/docs/natspec.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/docs/release-notes.rst` & `vyper-0.4.0rc6/docs/release-notes.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/docs/resources.rst` & `vyper-0.4.0rc6/docs/resources.rst`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 - `Vyper Hub for development <https://github.com/zcor/vyper-dev>`_
 - `Vyper greatest hits smart contract examples <https://github.com/pynchmeister/vyper-greatest-hits/tree/main/contracts>`_
 - `A curated list of Vyper resources, libraries, tools, and more <https://github.com/stars/pcaversaccio/lists/vyper>`_
 
 Frameworks and tooling
 ----------------------
 
-- `Titanoboa – An experimental Vyper interpreter with pretty tracebacks, forking, debugging features and more <https://github.com/vyperlang/titanoboa/>`_
+- `Titanoboa – A Vyper interpreter with pretty tracebacks, forking, debugging features and more <https://github.com/vyperlang/titanoboa/>`_
 - `ApeWorX – The Ethereum development framework for Python Developers, Data Scientists, and Security Professionals <https://www.apeworx.io/>`_
 - `VyperDeployer – A helper smart contract to compile and test Vyper contracts in Foundry <https://github.com/pcaversaccio/snekmate/blob/main/lib/utils/VyperDeployer.sol>`_
 - `🐍 snekmate – Vyper smart contract building blocks <https://github.com/pcaversaccio/snekmate>`_
 - `Serpentor – A set of smart contracts tools for governance <https://github.com/yearn/serpentor>`_
 - `Smart contract development frameworks and tools for Vyper on Ethereum.org <https://ethereum.org/en/developers/docs/programming-languages/python/>`_
 - `Vyper Online Compiler - an online platform for compiling and deploying Vyper smart contracts <https://github.com/0x0077/vyper-online-compiler>`_
```

### Comparing `vyper-0.4.0rc5/docs/scoping-and-declarations.rst` & `vyper-0.4.0rc6/docs/scoping-and-declarations.rst`

 * *Files 6% similar despite different names*

```diff
@@ -29,24 +29,26 @@
 
     data: public(int128)
 
 The compiler automatically creates getter functions for all public storage variables. For the example above, the compiler will generate a function called ``data`` that does not take any arguments and returns an ``int128``, the value of the state variable data.
 
 For public arrays, you can only retrieve a single element via the generated getter. This mechanism exists to avoid high gas costs when returning an entire array. The getter will accept an argument to specify which element to return, for example ``data(0)``.
 
+.. _immutable-variables:
+
 Declaring Immutable Variables
 -----------------------------
 
 Variables can be marked as ``immutable`` during declaration:
 
 .. code-block:: vyper
 
     DATA: immutable(uint256)
 
-    @external
+    @deploy
     def __init__(_data: uint256):
         DATA = _data
 
 Variables declared as immutable are similar to constants, except they are assigned a value in the constructor of the contract. Immutable values must be assigned a value at construction and cannot be assigned a value after construction.
 
 The contract creation code generated by the compiler will modify the contract’s runtime code before it is returned by appending all values assigned to immutables to the runtime code returned by the constructor. This is important if you are comparing the runtime code generated by the compiler with the one actually stored in the blockchain.
 
@@ -119,16 +121,14 @@
 .. _scoping-module:
 
 Module Scope
 ------------
 
 Variables and other items declared outside of a code block (functions, constants, event and struct definitions, ...), are visible even before they were declared. This means you can use module-scoped items before they are declared.
 
-An exception to this rule is that you can only call functions that have already been declared.
-
 Accessing Module Scope from Functions
 *************************************
 
 Values that are declared in the module scope of a contract, such as storage variables and functions, are accessed via the ``self`` object:
 
 .. code-block:: vyper
 
@@ -157,17 +157,18 @@
         # memory variable cannot have the same name as a constant or immutable variable
         a: bool = False
         return a
 .. code-block:: vyper
 
     a: immutable(bool)
 
-    @external
+    @deploy
     def __init__():
         a = True
+
     @external
     def foo(a:bool) -> bool:
         # input argument cannot have the same name as a constant or immutable variable
         return a
 
 Function Scope
 --------------
@@ -226,20 +227,20 @@
 
 In a ``for`` statement, the target variable exists within the scope of the loop. For example, the following contract is valid because ``i`` is no longer available upon exiting the loop:
 
 .. code-block:: vyper
 
     @external
     def foo(a: bool) -> int128:
-        for i in [1, 2, 3]:
+        for i: int128 in [1, 2, 3]:
             pass
         i: bool = False
 
 The following contract fails to compile because ``a`` has not been declared outside of the loop.
 
 .. code-block:: vyper
 
     @external
     def foo(a: bool) -> int128:
-        for i in [1, 2, 3]:
+        for i: int128 in [1, 2, 3]:
             a: int128 = i
         a += 3
```

### Comparing `vyper-0.4.0rc5/docs/statements.rst` & `vyper-0.4.0rc6/docs/statements.rst`

 * *Files 5% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 break
 -----
 
 The ``break`` statement terminates the nearest enclosing ``for`` loop.
 
 .. code-block:: vyper
 
-    for i in [1, 2, 3, 4, 5]:
+    for i: uint256 in [1, 2, 3, 4, 5]:
         if i == a:
             break
 
 In the above example, the ``for`` loop terminates if ``i == a``.
 
 continue
 --------
 
 The ``continue`` statement begins the next cycle of the nearest enclosing ``for`` loop.
 
 .. code-block:: vyper
 
-    for i in [1, 2, 3, 4, 5]:
+    for i: uint256 in [1, 2, 3, 4, 5]:
         if i != a:
             continue
         ...
 
 In the above example, the ``for`` loop begins the next cycle immediately whenever ``i != a``.
 
 pass
```

### Comparing `vyper-0.4.0rc5/docs/style-guide.rst` & `vyper-0.4.0rc6/docs/style-guide.rst`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     * All publicly exposed classes and methods **should** include `PEP 484 <https://www.python.org/dev/peps/pep-0484/>`_ annotations for all arguments and return values.
     * Type annotations **should** be included directly in the source. `Stub files <https://www.python.org/dev/peps/pep-0484/#stub-files>`_ **may** be used where there is a valid reason. Source files using stubs **must** still be annotated to aid readability.
     * Internal methods **should** include type annotations.
 
 Tests
 =====
 
-We use the `pytest <https://docs.pytest.org/en/latest/>`_ framework for testing, and :ref:`eth-tester<testing-contracts-ethtester>` for our local development chain.
+We use the `pytest <https://docs.pytest.org/en/latest/>`_ framework for testing.
 
 Best Practices
 --------------
 
     * ``pytest`` functionality **should not** be imported with ``from ...`` style syntax, particularly :func:`pytest.raises<pytest.raises>`. Importing the library itself aids readability.
     * Tests **must not** be interdependent. We use ``xdist`` to execute tests in parallel. You **cannot** rely on which order tests will execute in, or that two tests will execute in the same process.
     * Test cases **should** be designed with a minimalistic approach. Each test should verify a single behavior. A good test is one with few assertions, and where it is immediately obvious exactly what is being tested.
```

### Comparing `vyper-0.4.0rc5/docs/testing-contracts-brownie.rst` & `vyper-0.4.0rc6/docs/testing-contracts-brownie.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/docs/toctree.rst` & `vyper-0.4.0rc6/docs/toctree.rst`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     structure-of-a-contract.rst
     types.rst
     constants-and-vars.rst
     statements.rst
     control-structures.rst
     scoping-and-declarations.rst
     built-in-functions.rst
+    using-modules.rst
     interfaces.rst
     event-logging.rst
     natspec.rst
 
 .. toctree::
     :caption: Using the Compiler
     :maxdepth: 2
```

### Comparing `vyper-0.4.0rc5/docs/types.rst` & `vyper-0.4.0rc6/docs/types.rst`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,16 @@
 
 
 Decimals
 --------
 
 **Keyword:** ``decimal``
 
-A decimal is a type to store a decimal fixed point value.
+A decimal is a type to store a decimal fixed point value. As of v0.4.0, decimals must be enabled with the CLI flag ``--enable-decimals``.
+
 
 Values
 ******
 
 A value with a precision of 10 decimal places between -18707220957835557353007165858768422651595.9365500928 (-2\ :sup:`167` / 10\ :sup:`10`) and 18707220957835557353007165858768422651595.9365500927 ((2\ :sup:`167` - 1) / 10\ :sup:`10`).
 
 In order for a literal to be interpreted as ``decimal`` it must include a decimal point.
@@ -558,15 +559,15 @@
     Attempting to access data past the runtime length of an array, ``pop()`` an empty array or ``append()`` to a full array will result in a runtime ``REVERT``. Attempting to pass an array in calldata which is larger than the array bound will result in a runtime ``REVERT``.
 
 .. note::
     To keep code easy to reason about, modifying an array while using it as an iterator is disallowed by the language. For instance, the following usage is not allowed:
 
     .. code-block:: vyper
 
-        for item in self.my_array:
+        for item: uint256 in self.my_array:
             self.my_array[0] = item
 
 In the ABI, they are represented as ``_Type[]``. For instance, ``DynArray[int128, 3]`` gets represented as ``int128[]``, and ``DynArray[DynArray[int128, 3], 3]`` gets represented as ``int128[][]``.
 
 .. note::
     Defining a dynamic array in storage whose size is significantly larger than ``2**64`` can result in security vulnerabilities due to risk of overflow.
```

### Comparing `vyper-0.4.0rc5/docs/versioning.rst` & `vyper-0.4.0rc6/docs/versioning.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/docs/vyper-by-example.rst` & `vyper-0.4.0rc6/docs/vyper-by-example.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/examples/auctions/blind_auction.vy` & `vyper-0.4.0rc6/examples/auctions/blind_auction.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/examples/auctions/simple_open_auction.vy` & `vyper-0.4.0rc6/examples/auctions/simple_open_auction.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/examples/crowdfund.vy` & `vyper-0.4.0rc6/examples/crowdfund.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/examples/factory/Exchange.vy` & `vyper-0.4.0rc6/examples/factory/Exchange.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/examples/factory/Factory.vy` & `vyper-0.4.0rc6/examples/factory/Factory.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/examples/market_maker/on_chain_market_maker.vy` & `vyper-0.4.0rc6/examples/market_maker/on_chain_market_maker.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/examples/safe_remote_purchase/safe_remote_purchase.vy` & `vyper-0.4.0rc6/examples/safe_remote_purchase/safe_remote_purchase.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/examples/stock/company.vy` & `vyper-0.4.0rc6/examples/stock/company.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/examples/tokens/ERC1155ownable.vy` & `vyper-0.4.0rc6/examples/tokens/ERC1155ownable.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/examples/tokens/ERC20.vy` & `vyper-0.4.0rc6/examples/tokens/ERC20.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/examples/tokens/ERC4626.vy` & `vyper-0.4.0rc6/examples/tokens/ERC4626.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/examples/tokens/ERC721.vy` & `vyper-0.4.0rc6/examples/tokens/ERC721.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/examples/voting/ballot.vy` & `vyper-0.4.0rc6/examples/voting/ballot.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/examples/wallet/wallet.vy` & `vyper-0.4.0rc6/examples/wallet/wallet.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/make.cmd` & `vyper-0.4.0rc6/make.cmd`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/setup.cfg` & `vyper-0.4.0rc6/setup.cfg`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/setup.py` & `vyper-0.4.0rc6/setup.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/conftest.py` & `vyper-0.4.0rc6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/evm_backends/abi.py` & `vyper-0.4.0rc6/tests/evm_backends/abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/evm_backends/abi_contract.py` & `vyper-0.4.0rc6/tests/evm_backends/abi_contract.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/evm_backends/base_env.py` & `vyper-0.4.0rc6/tests/evm_backends/base_env.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/evm_backends/pyevm_env.py` & `vyper-0.4.0rc6/tests/evm_backends/pyevm_env.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/evm_backends/revm_env.py` & `vyper-0.4.0rc6/tests/evm_backends/revm_env.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_abi_decode.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_abi_encode.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,150 +1,168 @@
 import pytest
 from eth.codecs import abi
 
-from tests.evm_backends.base_env import EvmError, ExecutionReverted
 from tests.utils import decimal_to_int
-from vyper.exceptions import ArgumentException, StructureException
 
-TEST_ADDR = "0x" + b"".join(chr(i).encode("utf-8") for i in range(20)).hex()
 
-
-def test_abi_decode_complex(get_contract):
-    contract = """
+# @pytest.mark.parametrize("string", ["a", "abc", "abcde", "potato"])
+def test_abi_encode(get_contract):
+    code = """
 struct Animal:
   name: String[5]
   address_: address
   id_: int128
   is_furry: bool
   price: decimal
   data: uint256[3]
   metadata: bytes32
 
 struct Human:
   name: String[64]
   pet: Animal
 
 @external
-def abi_decode(x: Bytes[160]) -> (address, int128, bool, decimal, bytes32):
-    a: address = empty(address)
-    b: int128 = 0
-    c: bool = False
-    d: decimal = 0.0
-    e: bytes32 = 0x0000000000000000000000000000000000000000000000000000000000000000
-    a, b, c, d, e = _abi_decode(x, (address, int128, bool, decimal, bytes32))
-    return a, b, c, d, e
-
-@external
-def abi_decode_struct(x: Bytes[544]) -> Human:
+# TODO accept struct input once the functionality is available
+def abi_encode(
+    name: String[64],
+    pet_name: String[5],
+    pet_address: address,
+    pet_id: int128,
+    pet_is_furry: bool,
+    pet_price: decimal,
+    pet_data: uint256[3],
+    pet_metadata: bytes32,
+    ensure_tuple: bool,
+    include_method_id: bool
+) -> Bytes[548]:
     human: Human = Human(
-        name="",
-        pet=Animal(
-            name="",
-            address_=empty(address),
-            id_=0,
-            is_furry=False,
-            price=0.0,
-            data=[0, 0, 0],
-            metadata=0x0000000000000000000000000000000000000000000000000000000000000000
-        )
+      name=name,
+      pet=Animal(
+        name=pet_name,
+        address_=pet_address,
+        id_=pet_id,
+        is_furry=pet_is_furry,
+        price=pet_price,
+        data=pet_data,
+        metadata=pet_metadata
+      ),
     )
-    human = _abi_decode(x, Human)
-    return human
+    if ensure_tuple:
+        if not include_method_id:
+            return _abi_encode(human) # default ensure_tuple=True
+        return _abi_encode(human, method_id=0xdeadbeef)
+    else:
+        if not include_method_id:
+            return _abi_encode(human, ensure_tuple=False)
+        return _abi_encode(human, ensure_tuple=False, method_id=0xdeadbeef)
+
+@external
+def abi_encode2(name: String[32], ensure_tuple: bool, include_method_id: bool) -> Bytes[100]:
+    if ensure_tuple:
+        if not include_method_id:
+            return _abi_encode(name) # default ensure_tuple=True
+        return _abi_encode(name, method_id=0xdeadbeef)
+    else:
+        if not include_method_id:
+            return _abi_encode(name, ensure_tuple=False)
+        return _abi_encode(name, ensure_tuple=False, method_id=0xdeadbeef)
+
+@external
+def abi_encode3(x: uint256, ensure_tuple: bool, include_method_id: bool) -> Bytes[36]:
+
+    if ensure_tuple:
+        if not include_method_id:
+            return _abi_encode(x) # default ensure_tuple=True
+
+        return _abi_encode(x, method_id=0xdeadbeef)
+
+    else:
+        if not include_method_id:
+            return _abi_encode(x, ensure_tuple=False)
+
+        return _abi_encode(x, ensure_tuple=False, method_id=0xdeadbeef)
     """
+    c = get_contract(code)
 
-    c = get_contract(contract)
+    method_id = 0xDEADBEEF.to_bytes(4, "big")
 
-    test_bytes32 = b"".join(chr(i).encode("utf-8") for i in range(32))
-    args = (TEST_ADDR, -1, True, decimal_to_int("-123.4"), test_bytes32)
-    encoding = "(address,int128,bool,int168,bytes32)"
-    encoded = abi.encode(encoding, args)
-    assert tuple(c.abi_decode(encoded)) == (
-        TEST_ADDR,
-        -1,
-        True,
-        decimal_to_int("-123.4"),
-        test_bytes32,
+    # test each method once each with ensure_tuple set to True and False
+
+    arg = 123
+    assert c.abi_encode3(arg, False, False).hex() == abi.encode("uint256", arg).hex()
+    assert c.abi_encode3(arg, True, False).hex() == abi.encode("(uint256)", (arg,)).hex()
+    assert c.abi_encode3(arg, False, True).hex() == (method_id + abi.encode("uint256", arg)).hex()
+    assert (
+        c.abi_encode3(arg, True, True).hex() == (method_id + abi.encode("(uint256)", (arg,))).hex()
     )
 
+    arg = "some string"
+    assert c.abi_encode2(arg, False, False).hex() == abi.encode("string", arg).hex()
+    assert c.abi_encode2(arg, True, False).hex() == abi.encode("(string)", (arg,)).hex()
+    assert c.abi_encode2(arg, False, True).hex() == (method_id + abi.encode("string", arg)).hex()
+    assert (
+        c.abi_encode2(arg, True, True).hex() == (method_id + abi.encode("(string)", (arg,))).hex()
+    )
+
+    test_addr = "0x" + b"".join(chr(i).encode("utf-8") for i in range(20)).hex()
     test_bytes32 = b"".join(chr(i).encode("utf-8") for i in range(32))
     human_tuple = (
         "foobar",
-        ("vyper", TEST_ADDR, 123, True, decimal_to_int("123.4"), [123, 456, 789], test_bytes32),
+        ("vyper", test_addr, 123, True, decimal_to_int("123.4"), [123, 456, 789], test_bytes32),
     )
+    args = tuple([human_tuple[0]] + list(human_tuple[1]))
+    human_t = "(string,(string,address,int128,bool,int168,uint256[3],bytes32))"
+    human_encoded = abi.encode(human_t, human_tuple)
+    assert c.abi_encode(*args, False, False).hex() == human_encoded.hex()
+    assert c.abi_encode(*args, False, True).hex() == (method_id + human_encoded).hex()
+
+    human_encoded = abi.encode(f"({human_t})", (human_tuple,))
+    assert c.abi_encode(*args, True, False).hex() == human_encoded.hex()
+    assert c.abi_encode(*args, True, True).hex() == (method_id + human_encoded).hex()
 
-    human_t = "((string,(string,address,int128,bool,int168,uint256[3],bytes32)))"
-    human_encoded = abi.encode(human_t, (human_tuple,))
-    assert c.abi_decode_struct(human_encoded) == (
-        "foobar",
-        ("vyper", TEST_ADDR, 123, True, decimal_to_int("123.4"), [123, 456, 789], test_bytes32),
-    )
 
+@pytest.mark.parametrize("type,value", [("Bytes", b"hello"), ("String", "hello")])
+def test_abi_encode_length_failing(get_contract, assert_compile_failed, type, value):
+    code = f"""
+struct WrappedBytes:
+    bs: {type}[6]
 
-@pytest.mark.parametrize(
-    "expected,input_len,output_typ,abi_typ,unwrap_tuple",
-    [
-        (123, 32, "uint256", "uint256", False),
-        (123, 32, "uint256", "(uint256)", True),
-        ("vyper", 64, "String[5]", "string", False),
-        ("vyper", 96, "String[5]", "(string)", True),
-        ([123, 456, 789], 96, "uint256[3]", "uint256[3]", False),
-        ([123, 456, 789], 96, "uint256[3]", "(uint256[3])", True),
-        ([123, 456, 789], 128, "DynArray[uint256, 3]", "uint256[]", False),
-        ([123, 456, 789], 160, "DynArray[uint256, 3]", "(uint256[])", True),
-    ],
-)
-def test_abi_decode_single(get_contract, expected, input_len, output_typ, abi_typ, unwrap_tuple):
-    contract = f"""
-@external
-def foo(x: Bytes[{input_len}]) -> {output_typ}:
-    a: {output_typ} = _abi_decode(x, {output_typ}, unwrap_tuple={unwrap_tuple})
-    return a
+@internal
+def foo():
+    x: WrappedBytes = WrappedBytes(bs={value})
+    y: {type}[96] = _abi_encode(x, ensure_tuple=True) # should be Bytes[128]
     """
-    c = get_contract(contract)
 
-    encode_arg = expected
-    if unwrap_tuple is True:
-        encode_arg = (expected,)
+    assert_compile_failed(lambda: get_contract(code))
 
-    encoded = abi.encode(abi_typ, encode_arg)
-    assert c.foo(encoded) == expected
 
+def test_abi_encode_dynarray(get_contract):
+    code = """
+@external
+def abi_encode(d: DynArray[uint256, 3], ensure_tuple: bool, include_method_id: bool) -> Bytes[164]:
+    if ensure_tuple:
+        if not include_method_id:
+            return _abi_encode(d) # default ensure_tuple=True
+        return _abi_encode(d, method_id=0xdeadbeef)
+    else:
+        if not include_method_id:
+            return _abi_encode(d, ensure_tuple=False)
+        return _abi_encode(d, ensure_tuple=False, method_id=0xdeadbeef)
+    """
+    c = get_contract(code)
 
-@pytest.mark.parametrize(
-    "arg,expected,input_len,output_typ1,output_typ2,abi_typ",
-    [
-        ((123, 456), (123, 456), 64, "uint256", "uint256", "(uint256,uint256)"),
-        ((TEST_ADDR, 123), (TEST_ADDR, 123), 64, "address", "int128", "(address,int128)"),
-        (
-            ("vyper", TEST_ADDR),
-            ("vyper", TEST_ADDR),
-            128,
-            "String[5]",
-            "address",
-            "(string,address)",
-        ),
-        ((1, b"234"), (1, b"234"), 128, "uint256", "Bytes[32]", ("(uint256,bytes)")),
-    ],
-)
-@pytest.mark.parametrize("unwrap_tuple", (True, False))
-def test_abi_decode_double(
-    get_contract, arg, expected, input_len, output_typ1, output_typ2, abi_typ, unwrap_tuple
-):
-    contract = f"""
-@external
-def foo(x: Bytes[{input_len}]) -> ({output_typ1}, {output_typ2}):
-    a: {output_typ1} = empty({output_typ1})
-    b: {output_typ2} = empty({output_typ2})
-    a, b = _abi_decode(x, ({output_typ1}, {output_typ2}), unwrap_tuple={unwrap_tuple})
-    return a, b
-    """
-
-    c = get_contract(contract)
-    encoded = abi.encode(abi_typ, arg)
-    assert tuple(c.foo(encoded)) == expected
+    method_id = 0xDEADBEEF.to_bytes(4, "big")
+
+    arg = [123, 456, 789]
+    assert c.abi_encode(arg, False, False).hex() == abi.encode("uint256[]", arg).hex()
+    assert c.abi_encode(arg, True, False).hex() == abi.encode("(uint256[])", (arg,)).hex()
+    assert c.abi_encode(arg, False, True).hex() == (method_id + abi.encode("uint256[]", arg)).hex()
+    assert (
+        c.abi_encode(arg, True, True).hex() == (method_id + abi.encode("(uint256[])", (arg,))).hex()
+    )
 
 
 nested_2d_array_args = [
     [[123, 456, 789], [234, 567, 891], [345, 678, 912]],
     [[], [], []],
     [[123, 456], [234, 567, 891]],
     [[123, 456, 789], [234, 567], [345]],
@@ -155,33 +173,42 @@
     [[], [234, 567, 891], []],
     [[]],
     [[123], [234]],
 ]
 
 
 @pytest.mark.parametrize("args", nested_2d_array_args)
-@pytest.mark.parametrize("unwrap_tuple", (True, False))
-def test_abi_decode_nested_dynarray(get_contract, args, unwrap_tuple):
-    if unwrap_tuple is True:
-        encoded = abi.encode("(uint256[][])", (args,))
-        len = 544
-    else:
-        encoded = abi.encode("uint256[][]", args)
-        len = 512
-
-    code = f"""
+def test_abi_encode_nested_dynarray(get_contract, args):
+    code = """
 @external
-def abi_decode(x: Bytes[{len}]) -> DynArray[DynArray[uint256, 3], 3]:
-    a: DynArray[DynArray[uint256, 3], 3] = []
-    a = _abi_decode(x, DynArray[DynArray[uint256, 3], 3], unwrap_tuple={unwrap_tuple})
-    return a
+def abi_encode(
+    d: DynArray[DynArray[uint256, 3], 3], ensure_tuple: bool, include_method_id: bool
+) -> Bytes[548]:
+    if ensure_tuple:
+        if not include_method_id:
+            return _abi_encode(d) # default ensure_tuple=True
+        return _abi_encode(d, method_id=0xdeadbeef)
+    else:
+        if not include_method_id:
+            return _abi_encode(d, ensure_tuple=False)
+        return _abi_encode(d, ensure_tuple=False, method_id=0xdeadbeef)
     """
-
     c = get_contract(code)
-    assert c.abi_decode(encoded) == args
+
+    method_id = 0xDEADBEEF.to_bytes(4, "big")
+
+    assert c.abi_encode(args, False, False).hex() == abi.encode("uint256[][]", args).hex()
+    assert c.abi_encode(args, True, False).hex() == abi.encode("(uint256[][])", (args,)).hex()
+    assert (
+        c.abi_encode(args, False, True).hex() == (method_id + abi.encode("uint256[][]", args)).hex()
+    )
+    assert (
+        c.abi_encode(args, True, True).hex()
+        == (method_id + abi.encode("(uint256[][])", (args,))).hex()
+    )
 
 
 nested_3d_array_args = [
     [
         [[123, 456, 789], [234, 567, 891], [345, 678, 912]],
         [[234, 567, 891], [345, 678, 912], [123, 456, 789]],
         [[345, 678, 912], [123, 456, 789], [234, 567, 891]],
@@ -195,279 +222,152 @@
     [[[]], [[123]], [[]]],
     [[[123, 456, 789], [234, 567]], [[234]], [[567], [912], [345]]],
     [[[]]],
 ]
 
 
 @pytest.mark.parametrize("args", nested_3d_array_args)
-@pytest.mark.parametrize("unwrap_tuple", (True, False))
-def test_abi_decode_nested_dynarray2(get_contract, args, unwrap_tuple):
-    if unwrap_tuple is True:
-        encoded = abi.encode("(uint256[][][])", (args,))
-        len = 1696
-    else:
-        encoded = abi.encode("uint256[][][]", args)
-        len = 1664
-
-    code = f"""
+def test_abi_encode_nested_dynarray_2(get_contract, args):
+    code = """
 @external
-def abi_decode(x: Bytes[{len}]) -> DynArray[DynArray[DynArray[uint256, 3], 3], 3]:
-    a: DynArray[DynArray[DynArray[uint256, 3], 3], 3] = []
-    a = _abi_decode(
-        x,
-        DynArray[DynArray[DynArray[uint256, 3], 3], 3],
-        unwrap_tuple={unwrap_tuple}
-    )
-    return a
+def abi_encode(
+    d: DynArray[DynArray[DynArray[uint256, 3], 3], 3],
+    ensure_tuple: bool,
+    include_method_id: bool
+) -> Bytes[1700]:
+    if ensure_tuple:
+        if not include_method_id:
+            return _abi_encode(d) # default ensure_tuple=True
+        return _abi_encode(d, method_id=0xdeadbeef)
+    else:
+        if not include_method_id:
+            return _abi_encode(d, ensure_tuple=False)
+        return _abi_encode(d, ensure_tuple=False, method_id=0xdeadbeef)
     """
-
     c = get_contract(code)
-    assert c.abi_decode(encoded) == args
+
+    method_id = 0xDEADBEEF.to_bytes(4, "big")
+
+    assert c.abi_encode(args, False, False).hex() == abi.encode("uint256[][][]", args).hex()
+    assert c.abi_encode(args, True, False).hex() == abi.encode("(uint256[][][])", (args,)).hex()
+    assert (
+        c.abi_encode(args, False, True).hex()
+        == (method_id + abi.encode("uint256[][][]", args)).hex()
+    )
+    assert (
+        c.abi_encode(args, True, True).hex()
+        == (method_id + abi.encode("(uint256[][][])", (args,))).hex()
+    )
 
 
 def test_side_effects_evaluation(get_contract):
     contract_1 = """
 counter: uint256
 
 @deploy
 def __init__():
     self.counter = 0
 
 @external
-def get_counter() -> Bytes[128]:
+def get_counter() -> (uint256, String[6]):
     self.counter += 1
-    return _abi_encode(self.counter, "hello")
+    return (self.counter, "hello")
     """
 
     c = get_contract(contract_1)
 
     contract_2 = """
 interface Foo:
-    def get_counter() -> Bytes[128]: nonpayable
+    def get_counter() -> (uint256, String[6]): nonpayable
 
 @external
-def foo(addr: address) -> (uint256, String[5]):
-    a: uint256 = 0
-    b: String[5] = ""
-    a, b = _abi_decode(extcall Foo(addr).get_counter(), (uint256, String[5]), unwrap_tuple=False)
-    return a, b
+def foo(addr: address) -> Bytes[164]:
+    return _abi_encode(extcall Foo(addr).get_counter(), method_id=0xdeadbeef)
     """
 
     c2 = get_contract(contract_2)
 
-    assert tuple(c2.foo(c.address)) == (1, "hello")
+    method_id = 0xDEADBEEF.to_bytes(4, "big")
 
+    # call to get_counter() should be evaluated only once
+    get_counter_encoded = abi.encode("((uint256,string))", ((1, "hello"),))
+
+    assert c2.foo(c.address).hex() == (method_id + get_counter_encoded).hex()
 
-def test_abi_decode_private_dynarray(get_contract):
-    code = """
-bytez: DynArray[uint256, 3]
 
+# test _abi_encode in private functions to check buffer overruns
+def test_abi_encode_private(get_contract):
+    code = """
+bytez: Bytes[96]
 @internal
-def _foo(bs: Bytes[160]):
-    self.bytez = _abi_decode(bs, DynArray[uint256, 3])
+def _foo(bs: Bytes[32]):
+    self.bytez = _abi_encode(bs)
 
 @external
-def foo(bs: Bytes[160]) -> (uint256, DynArray[uint256, 3]):
+def foo(bs: Bytes[32]) -> (uint256, Bytes[96]):
     dont_clobber_me: uint256 = max_value(uint256)
     self._foo(bs)
     return dont_clobber_me, self.bytez
     """
     c = get_contract(code)
-    bs = [1, 2, 3]
-    encoded = abi.encode("(uint256[])", (bs,))
-    assert c.foo(encoded) == (2**256 - 1, bs)
+    bs = b"\x00" * 32
+    assert c.foo(bs) == (2**256 - 1, abi.encode("(bytes)", (bs,)))
 
 
-def test_abi_decode_private_nested_dynarray(get_contract):
+def test_abi_encode_private_dynarray(get_contract):
     code = """
-bytez: DynArray[DynArray[DynArray[uint256, 3], 3], 3]
+bytez: Bytes[160]
+@internal
+def _foo(bs: DynArray[uint256, 3]):
+    self.bytez = _abi_encode(bs)
+@external
+def foo(bs: DynArray[uint256, 3]) -> (uint256, Bytes[160]):
+    dont_clobber_me: uint256 = max_value(uint256)
+    self._foo(bs)
+    return dont_clobber_me, self.bytez
+    """
+    c = get_contract(code)
+    bs = [1, 2, 3]
+    assert c.foo(bs) == (2**256 - 1, abi.encode("(uint256[])", (bs,)))
+
 
+def test_abi_encode_private_nested_dynarray(get_contract):
+    code = """
+bytez: Bytes[1696]
 @internal
-def _foo(bs: Bytes[1696]):
-    self.bytez = _abi_decode(bs, DynArray[DynArray[DynArray[uint256, 3], 3], 3])
+def _foo(bs: DynArray[DynArray[DynArray[uint256, 3], 3], 3]):
+    self.bytez = _abi_encode(bs)
 
 @external
-def foo(bs: Bytes[1696]) -> (uint256, DynArray[DynArray[DynArray[uint256, 3], 3], 3]):
+def foo(bs: DynArray[DynArray[DynArray[uint256, 3], 3], 3]) -> (uint256, Bytes[1696]):
     dont_clobber_me: uint256 = max_value(uint256)
     self._foo(bs)
     return dont_clobber_me, self.bytez
     """
     c = get_contract(code)
     bs = [
         [[1, 2, 3], [4, 5, 6], [7, 8, 9]],
         [[10, 11, 12], [13, 14, 15], [16, 17, 18]],
         [[19, 20, 21], [22, 23, 24], [25, 26, 27]],
     ]
-    encoded = abi.encode("(uint256[][][])", (bs,))
-    assert c.foo(encoded) == (2**256 - 1, bs)
-
-
-def test_abi_decode_return(get_contract):
-    contract = """
-@external
-def abi_decode(x: Bytes[64]) -> (address, int128):
-    return _abi_decode(x, (address, int128))
-    """
-
-    c = get_contract(contract)
-
-    encoded = abi.encode("(address,int128)", (TEST_ADDR, 123))
-
-    assert tuple(c.abi_decode(encoded)) == (TEST_ADDR, 123)
-
+    assert c.foo(bs) == (2**256 - 1, abi.encode("(uint256[][][])", (bs,)))
 
-def test_abi_decode_annassign(get_contract):
-    contract = """
-@external
-def abi_decode(x: Bytes[32]) -> uint256:
-    a: uint256 = _abi_decode(x, uint256, unwrap_tuple=False)
-    return a
-    """
-    c = get_contract(contract)
-
-    encoded = abi.encode("uint256", 123)
-    assert c.abi_decode(encoded) == 123
-
-
-@pytest.mark.parametrize(
-    "input_",
-    [
-        b"",  # Length of byte array is below minimum size of output type
-        b"\x01" * 96,  # Length of byte array is beyond size bound of output type
-    ],
-)
-def test_clamper(get_contract, tx_failed, input_):
-    contract = """
-@external
-def abi_decode(x: Bytes[96]) -> (uint256, uint256):
-    a: uint256 = empty(uint256)
-    b: uint256 = empty(uint256)
-    a, b = _abi_decode(x, (uint256, uint256))
-    return a, b
-    """
-    c = get_contract(contract)
-    with tx_failed():
-        c.abi_decode(input_)
-
-
-def test_clamper_nested_uint8(get_contract, tx_failed):
-    # check that _abi_decode clamps on word-types even when it is in a nested expression
-    # decode -> validate uint8 -> revert if input >= 256 -> cast back to uint256
-    contract = """
-@external
-def abi_decode(x: uint256) -> uint256:
-    a: uint256 = convert(_abi_decode(slice(msg.data, 4, 32), (uint8)), uint256)
-    return a
-    """
-    c = get_contract(contract)
-    assert c.abi_decode(255) == 255
-    with tx_failed():
-        c.abi_decode(256)
 
-
-def test_clamper_nested_bytes(get_contract, tx_failed):
-    # check that _abi_decode clamps dynamic even when it is in a nested expression
-    # decode -> validate Bytes[20] -> revert if len(input) > 20 -> convert back to -> add 1
-    contract = """
+@pytest.mark.parametrize("empty_literal", ('b""', '""', "empty(Bytes[1])", "empty(String[1])"))
+def test_abi_encode_empty_string(get_contract, empty_literal):
+    code = f"""
 @external
-def abi_decode(x: Bytes[96]) -> Bytes[21]:
-    a: Bytes[21] = concat(b"a", _abi_decode(x, Bytes[20]))
-    return a
+def foo(ensure_tuple: bool) -> Bytes[96]:
+    if ensure_tuple:
+        return _abi_encode({empty_literal}) # default ensure_tuple=True
+    else:
+        return _abi_encode({empty_literal}, ensure_tuple=False)
     """
-    c = get_contract(contract)
-    assert c.abi_decode(abi.encode("(bytes)", (b"bc",))) == b"abc"
-    with tx_failed():
-        c.abi_decode(abi.encode("(bytes)", (b"a" * 22,)))
-
-
-@pytest.mark.parametrize(
-    "output_typ,input_",
-    [
-        ("DynArray[uint256, 3]", b""),
-        ("DynArray[uint256, 3]", b"\x01" * 192),
-        ("Bytes[5]", b""),
-        ("Bytes[5]", b"\x01" * 192),
-    ],
-)
-def test_clamper_dynamic(get_contract, tx_failed, output_typ, input_):
-    contract = f"""
-@external
-def abi_decode(x: Bytes[192]) -> {output_typ}:
-    a: {output_typ} = empty({output_typ})
-    a = _abi_decode(x, {output_typ})
-    return a
-    """
-    c = get_contract(contract)
-    with tx_failed():
-        c.abi_decode(input_)
-
-
-@pytest.mark.parametrize(
-    "arg,encoding,expected", [(123, "(uint256)", 123), ([123, 456, 789], "(uint256[])", 789)]
-)
-def test_abi_decode_conditional(get_contract, arg, encoding, expected):
-    contract = """
-@external
-def abi_decode(x: Bytes[160]) -> uint256:
-    if len(x) == 32:
-        a: uint256 = _abi_decode(x, uint256)
-        return a
-    elif len(x) == 160:
-        b: DynArray[uint256, 3] = _abi_decode(x, DynArray[uint256, 3])
-        return b[2]
-    return 0
-    """
-    c = get_contract(contract)
-    encoded = abi.encode(encoding, (arg,))
-    assert c.abi_decode(encoded) == expected
-
-
-@pytest.mark.parametrize(
-    "output_typ1,output_typ2,input_,error,error_property",
-    [
-        ("DynArray[uint256, 3]", "uint256", b"", ExecutionReverted, ""),
-        ("DynArray[uint256, 3]", "uint256", b"\x01" * 128, EvmError, "OUT_OF_GAS_ERROR"),
-        ("Bytes[5]", "address", b"", ExecutionReverted, ""),
-        ("Bytes[5]", "address", b"\x01" * 128, EvmError, "OUT_OF_GAS_ERROR"),
-    ],
-)
-def test_clamper_dynamic_tuple(
-    get_contract, tx_failed, output_typ1, output_typ2, input_, error, error_property, env
-):
-    contract = f"""
-@external
-def abi_decode(x: Bytes[224]) -> ({output_typ1}, {output_typ2}):
-    a: {output_typ1} = empty({output_typ1})
-    b: {output_typ2} = empty({output_typ2})
-    a, b = _abi_decode(x, ({output_typ1}, {output_typ2}))
-    return a, b
-    """
-    c = get_contract(contract)
-    with tx_failed(error, exc_text=getattr(env, error_property, None)):
-        c.abi_decode(input_)
-
-
-FAIL_LIST = [
-    (
-        """
-@external
-def foo(x: Bytes[32]):
-    a: uint256 = 0
-    b: uint256 = 0
-    a, b = _abi_decode(x, (uint256, uint256))
-    """,
-        StructureException,  # Size of input data is smaller than expected output
-    ),
-    (
-        """
-@external
-def foo(x: Bytes[32]):
-    _abi_decode(x)
-    """,
-        ArgumentException,  # Output types arg is missing
-    ),
-]
 
+    c = get_contract(code)
 
-@pytest.mark.parametrize("bad_code,exception", FAIL_LIST)
-def test_abi_decode_length_mismatch(get_contract, assert_compile_failed, bad_code, exception):
-    assert_compile_failed(lambda: get_contract(bad_code), exception)
+    # eth-abi does not encode zero-length string correctly -
+    # see https://github.com/ethereum/eth-abi/issues/157
+    expected_output = b"\x00" * 32
+    assert c.foo(False) == expected_output
+    expected_output = b"\x00" * 31 + b"\x20" + b"\x00" * 32
+    assert c.foo(True) == expected_output
```

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_addmod.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_addmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_as_wei_value.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_bitwise.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_bitwise.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_blobhash.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_blobhash.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_ceil.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_ceil.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_concat.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_concat.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_convert.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_convert.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_create_functions.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_create_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -661,14 +661,53 @@
     d.test(f.address)
 
     test = FooContract(d.created_address())
     assert env.get_code(test.address) == expected_runtime_code
     assert test.foo() == 12
 
 
+def test_blueprint_evals_once_side_effects(get_contract, deploy_blueprint_for, env):
+    # test msize allocator does not get trampled by salt= kwarg
+    code = """
+foo: public(uint256)
+    """
+
+    deployer_code = """
+created_address: public(address)
+deployed: public(uint256)
+
+@external
+def get() -> Bytes[32]:
+    self.deployed += 1
+    return b''
+
+@external
+def create_(target: address):
+    self.created_address = create_from_blueprint(
+        target,
+        raw_call(self, method_id("get()"), max_outsize=32),
+        raw_args=True, code_offset=3
+    )
+    """
+
+    foo_contract = get_contract(code)
+    expected_runtime_code = env.get_code(foo_contract.address)
+
+    f, FooContract = deploy_blueprint_for(code)
+
+    d = get_contract(deployer_code)
+
+    d.create_(f.address)
+
+    test = FooContract(d.created_address())
+    assert env.get_code(test.address) == expected_runtime_code
+    assert test.foo() == 0
+    assert d.deployed() == 1
+
+
 def test_create_copy_of_complex_kwargs(get_contract, env):
     # test msize allocator does not get trampled by salt= kwarg
     complex_salt = """
 created_address: public(address)
 
 @external
 def test(target: address) -> address:
```

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_ec.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_ec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_ecrecover.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_ecrecover.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_empty.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_empty.py`

 * *Files 2% similar despite different names*

```diff
@@ -615,32 +615,25 @@
     """,
     ],
 )
 def test_clear_typecheck(contract, get_contract, assert_compile_failed):
     assert_compile_failed(lambda: get_contract(contract), TypeMismatch)
 
 
+_33_bytes = b"\x01" * 33
+_65_bytes = b"\x01" * 65
+
+
 @pytest.mark.parametrize(
     "a,b,expected",
     [
-        ("empty(Bytes[65])", "b'hello'", (b"hello", b"")),
-        ("b'hello'", "empty(Bytes[33])", (b"", b"hello")),
-        (
-            "empty(Bytes[65])",
-            "b'thirty three bytes long baby!!!!!'",
-            (b"thirty three bytes long baby!!!!!", b""),
-        ),
-        (
-            "b'thirty three bytes long baby!!!aathirty three bytes long baby!!!a'",
-            "b'thirty three bytes long baby!!!aa'",
-            (
-                b"thirty three bytes long baby!!!aa",
-                b"thirty three bytes long baby!!!aathirty three bytes long baby!!!a",
-            ),
-        ),
+        ("empty(Bytes[65])", b"hello", (b"hello", b"")),
+        (b"hello", "empty(Bytes[33])", (b"", b"hello")),
+        ("empty(Bytes[65])", _33_bytes, (_33_bytes, b"")),
+        (_65_bytes, _33_bytes, (_33_bytes, _65_bytes)),
     ],
 )
 def test_empty_as_func_arg(get_contract, a, b, expected):
     code_a = """
 @view
 @external
 def foo(
```

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_extract32.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_extract32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_floor.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_floor.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_is_contract.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_is_contract.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_keccak256.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_keccak256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_length.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_length.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_method_id.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_method_id.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_minmax.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_minmax.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_minmax_value.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_minmax_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_mulmod.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_mulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_raw_call.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_raw_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_send.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_send.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_sha256.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_sha256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_slice.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_slice.py`

 * *Files 3% similar despite different names*

```diff
@@ -532,7 +532,33 @@
 
 
 @pytest.mark.parametrize("bad_code", oob_fail_list)
 def test_slice_buffer_oob_reverts(bad_code, get_contract, tx_failed):
     c = get_contract(bad_code)
     with tx_failed():
         c.do_slice()
+
+
+# tests all 3 adhoc locations: `msg.data`, `self.code`, `<address>.code`
+@pytest.mark.parametrize("adhoc_loc", ["msg.data", "self.code", "a.code"])
+def test_slice_start_eval_once(get_contract, adhoc_loc):
+    code = f"""
+counter: uint256
+
+@internal
+def bar() -> uint256:
+    self.counter += 1
+    return 1
+
+@external
+def foo(cs: String[64]) -> uint256:
+    s: Bytes[64] = b""
+    # use `a` to exercise the path with `<address>.code`
+    a: address = self
+    s = slice({adhoc_loc}, self.bar(), 3)
+    return self.counter
+    """
+
+    arg = "a" * 64
+    c = get_contract(code)
+    # ensure that counter was incremented only once
+    assert c.foo(arg) == 1
```

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_uint2str.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_uint2str.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_unary.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_unary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/codegen/test_unsafe_math.py` & `vyper-0.4.0rc6/tests/functional/builtins/codegen/test_unsafe_math.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/folding/test_abs.py` & `vyper-0.4.0rc6/tests/functional/builtins/folding/test_abs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/folding/test_addmod_mulmod.py` & `vyper-0.4.0rc6/tests/functional/builtins/folding/test_addmod_mulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/folding/test_bitwise.py` & `vyper-0.4.0rc6/tests/functional/builtins/folding/test_bitwise.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/folding/test_floor_ceil.py` & `vyper-0.4.0rc6/tests/functional/builtins/folding/test_floor_ceil.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/folding/test_fold_as_wei_value.py` & `vyper-0.4.0rc6/tests/functional/builtins/folding/test_fold_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/folding/test_keccak_sha.py` & `vyper-0.4.0rc6/tests/functional/builtins/folding/test_keccak_sha.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/folding/test_len.py` & `vyper-0.4.0rc6/tests/functional/builtins/folding/test_len.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/folding/test_min_max.py` & `vyper-0.4.0rc6/tests/functional/builtins/folding/test_min_max.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/builtins/folding/test_powmod.py` & `vyper-0.4.0rc6/tests/functional/builtins/folding/test_powmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/calling_convention/test_default_function.py` & `vyper-0.4.0rc6/tests/functional/codegen/calling_convention/test_default_function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/calling_convention/test_default_parameters.py` & `vyper-0.4.0rc6/tests/functional/codegen/calling_convention/test_default_parameters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/calling_convention/test_erc20_abi.py` & `vyper-0.4.0rc6/tests/functional/codegen/calling_convention/test_erc20_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/calling_convention/test_external_contract_calls.py` & `vyper-0.4.0rc6/tests/functional/codegen/calling_convention/test_external_contract_calls.py`

 * *Files 2% similar despite different names*

```diff
@@ -2523,7 +2523,62 @@
     malformed = data[:264]
     with tx_failed():
         env.message_call(c1.address, data=malformed)
 
     # Dynamic size is at least minimum (132 bytes * 2 + 2 (for 0x) = 266)
     valid = data[:266]
     env.message_call(c1.address, data=valid)
+
+
+def test_make_setter_external_call(get_contract):
+    # variant of GH #3503
+    code = """
+interface A:
+   def boo() -> uint256:nonpayable
+
+a: DynArray[uint256, 10]
+
+@external
+def foo() -> DynArray[uint256, 10]:
+    self.a = [1, 2, extcall A(self).boo(), 4]
+    return self.a  # returns [11, 12, 3, 4]
+
+@external
+def boo() -> uint256:
+    self.a = [11, 12, 13, 14, 15, 16]
+    self.a = []
+    # it should now be impossible to read any of [11, 12, 13, 14, 15, 16]
+    return 3
+    """
+    c = get_contract(code)
+
+    assert c.foo() == [1, 2, 3, 4]
+
+
+def test_make_setter_external_call2(get_contract):
+    # variant of GH #3503
+    code = """
+interface A:
+   def boo(): nonpayable
+
+a: DynArray[uint256, 10]
+
+@external
+def foo() -> DynArray[uint256, 10]:
+    self.a = [1, 2, self.baz(), 4]
+    return self.a # returns [11, 12, 3, 4]
+
+
+@internal
+def baz() -> uint256:
+    extcall A(self).boo()
+    return 3
+
+@external
+def boo():
+    self.a = [11, 12, 13, 14, 15, 16]
+    self.a = []
+    # it should now be impossible to read any of [11, 12, 13, 14, 15, 16]
+    """
+    c = get_contract(code)
+
+    assert c.foo() == [1, 2, 3, 4]
```

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py` & `vyper-0.4.0rc6/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/calling_convention/test_return.py` & `vyper-0.4.0rc6/tests/functional/codegen/calling_convention/test_return.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/calling_convention/test_self_call_struct.py` & `vyper-0.4.0rc6/tests/functional/codegen/calling_convention/test_self_call_struct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/environment_variables/test_blobbasefee.py` & `vyper-0.4.0rc6/tests/functional/codegen/environment_variables/test_blobbasefee.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/environment_variables/test_blockhash.py` & `vyper-0.4.0rc6/tests/functional/codegen/environment_variables/test_blockhash.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/decorators/test_nonreentrant.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/decorators/test_nonreentrant.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/decorators/test_payable.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/decorators/test_payable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/decorators/test_private.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/decorators/test_private.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/decorators/test_pure.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/decorators/test_pure.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/decorators/test_view.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/decorators/test_view.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/iteration/test_break.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/iteration/test_break.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/iteration/test_continue.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/iteration/test_continue.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/iteration/test_for_in_list.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/iteration/test_for_in_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/iteration/test_for_range.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/iteration/test_for_range.py`

 * *Files 6% similar despite different names*

```diff
@@ -469,7 +469,41 @@
         res.append(i)
     return res
     """
     if not experimental_codegen:
         return
     with pytest.raises(StaticAssertionException):
         get_contract(code)
+
+
+def test_for_range_start_double_eval(get_contract, tx_failed):
+    code = """
+@external
+def foo() -> (uint256, DynArray[uint256, 3]):
+    x:DynArray[uint256, 3] = [3, 1]
+    res: DynArray[uint256, 3] = empty(DynArray[uint256, 3])
+    for i:uint256 in range(x.pop(),x.pop(), bound = 3):
+        res.append(i)
+
+    return len(x), res
+    """
+    c = get_contract(code)
+    length, res = c.foo()
+
+    assert (length, res) == (0, [1, 2])
+
+
+def test_for_range_stop_double_eval(get_contract, tx_failed):
+    code = """
+@external
+def foo() -> (uint256, DynArray[uint256, 3]):
+    x:DynArray[uint256, 3] = [3, 3]
+    res: DynArray[uint256, 3] = empty(DynArray[uint256, 3])
+    for i:uint256 in range(x.pop(), bound = 3):
+        res.append(i)
+
+    return len(x), res
+    """
+    c = get_contract(code)
+    length, res = c.foo()
+
+    assert (length, res) == (1, [0, 1, 2])
```

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/iteration/test_range_in.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/iteration/test_range_in.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_assert.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_assert.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_assert_unreachable.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_assert_unreachable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_assignment.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_assignment.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_bytes_map_keys.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_bytes_map_keys.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_clampers.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_clampers.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_comparison.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_comparison.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_conditionals.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_constructor.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_constructor.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_immutable.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_immutable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_init.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_init.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_internal_call.py` & `vyper-0.4.0rc6/tests/functional/codegen/calling_convention/test_internal_call.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from tests.utils import decimal_to_int
 from vyper.compiler import compile_code
 from vyper.exceptions import ArgumentException, CallViolation
 
 
 def test_selfcall_code(get_contract):
     selfcall_code = """
-@internal
 def _foo() -> int128:
     return 3
 
 @external
 def bar() -> int128:
     return self._foo()
     """
@@ -24,23 +23,21 @@
     assert c.bar() == 3
 
     print("Passed no-argument self-call test")
 
 
 def test_selfcall_code_2(get_contract, keccak):
     selfcall_code_2 = """
-@internal
 def _double(x: int128) -> int128:
     return x * 2
 
 @external
 def returnten() -> int128:
     return self._double(5)
 
-@internal
 def _hashy(x: bytes32) -> bytes32:
     return keccak256(x)
 
 @external
 def return_hash_of_rzpadded_cow() -> bytes32:
     return self._hashy(0x636f770000000000000000000000000000000000000000000000000000000000)
     """
@@ -620,14 +617,57 @@
     """
 
     c = get_contract(contract)
 
     assert c.bar() == b"hello"
 
 
+def test_make_setter_internal_call(get_contract):
+    # cf. GH #3503
+    code = """
+a:DynArray[uint256,2]
+
+@external
+def foo() -> DynArray[uint256,2]:
+    # Initial value
+    self.a = [1, 2]
+    self.a = [self.bar(1), self.bar(0)]
+    return self.a
+
+@internal
+def bar(i: uint256) -> uint256:
+    return self.a[i]
+    """
+    c = get_contract(code)
+
+    assert c.foo() == [2, 1]
+
+
+def test_make_setter_internal_call2(get_contract):
+    # cf. GH #3503
+    code = """
+a: DynArray[uint256, 10]
+
+@external
+def foo() -> DynArray[uint256, 10]:
+    self.a = [1, 2, self.boo(), 4]
+    return self.a # returns [11, 12, 3, 4]
+
+@internal
+def boo() -> uint256:
+    self.a = [11, 12, 13, 14, 15, 16]
+    self.a = []
+    # it should now be impossible to read any of [11, 12, 13, 14, 15, 16]
+    return 3
+    """
+    c = get_contract(code)
+
+    assert c.foo() == [1, 2, 3, 4]
+
+
 def test_dynamically_sized_struct_member_as_arg_2(get_contract):
     contract = """
 struct X:
     x: uint256
     y: String[6]
 
 @internal
```

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_logging.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_logging.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_logging_bytes_extended.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_logging_bytes_extended.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_logging_from_call.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_logging_from_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_memory_dealloc.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_memory_dealloc.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_packing.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_packing.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_reverting.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_reverting.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_short_circuiting.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_short_circuiting.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_string_map_keys.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_string_map_keys.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_ternary.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_ternary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/features/test_transient.py` & `vyper-0.4.0rc6/tests/functional/codegen/features/test_transient.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/integration/test_crowdfund.py` & `vyper-0.4.0rc6/tests/functional/codegen/integration/test_crowdfund.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/integration/test_escrow.py` & `vyper-0.4.0rc6/tests/functional/codegen/integration/test_escrow.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/modules/test_events.py` & `vyper-0.4.0rc6/tests/functional/codegen/modules/test_events.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/modules/test_exports.py` & `vyper-0.4.0rc6/tests/functional/codegen/modules/test_exports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/modules/test_flag_imports.py` & `vyper-0.4.0rc6/tests/functional/codegen/modules/test_flag_imports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/modules/test_interface_imports.py` & `vyper-0.4.0rc6/tests/functional/codegen/modules/test_interface_imports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/modules/test_module_constants.py` & `vyper-0.4.0rc6/tests/functional/codegen/modules/test_module_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/modules/test_module_variables.py` & `vyper-0.4.0rc6/tests/functional/codegen/modules/test_module_variables.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/modules/test_nonreentrant.py` & `vyper-0.4.0rc6/tests/functional/codegen/modules/test_nonreentrant.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/modules/test_stateless_functions.py` & `vyper-0.4.0rc6/tests/functional/codegen/modules/test_stateless_functions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/storage_variables/test_getters.py` & `vyper-0.4.0rc6/tests/functional/codegen/storage_variables/test_getters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/storage_variables/test_setters.py` & `vyper-0.4.0rc6/tests/functional/codegen/storage_variables/test_setters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/storage_variables/test_storage_variable.py` & `vyper-0.4.0rc6/tests/functional/codegen/storage_variables/test_storage_variable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/test_call_graph_stability.py` & `vyper-0.4.0rc6/tests/functional/codegen/test_call_graph_stability.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 
 import vyper.ast as vy_ast
 from vyper.ast.identifiers import RESERVED_KEYWORDS
 from vyper.compiler.phases import CompilerData
 
 
 def _valid_identifier(attr):
+    if attr == "foo":
+        # the entry point to the test is named foo(),
+        # skip it to avoid collision
+        return False
+
     return attr not in RESERVED_KEYWORDS
 
 
 # random names for functions
 @settings(max_examples=20)
 @given(
     st.lists(
```

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/test_interfaces.py` & `vyper-0.4.0rc6/tests/functional/codegen/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/test_selector_table.py` & `vyper-0.4.0rc6/tests/functional/codegen/test_selector_table.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/test_selector_table_stability.py` & `vyper-0.4.0rc6/tests/functional/codegen/test_selector_table_stability.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_constants.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_decimals.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_decimals.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_division.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_division.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_exponents.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_exponents.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_isqrt.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_isqrt.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_modulo.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_modulo.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_signed_ints.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_signed_ints.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_sqrt.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_sqrt.py`

 * *Files 5% similar despite different names*

```diff
@@ -159,7 +159,26 @@
     )
 )
 @hypothesis.example(value=Decimal(SizeLimits.MIN_INT128))
 @hypothesis.example(value=Decimal("-1E10"))
 def test_sqrt_invalid_range(tx_failed, sqrt_contract, value):
     with tx_failed():
         sqrt_contract.test(decimal_to_int(value))
+
+
+def test_sqrt_eval_once(get_contract):
+    code = """
+c: uint256
+
+@internal
+def some_decimal() -> decimal:
+    self.c += 1
+    return 1.0
+
+@external
+def foo() -> uint256:
+    k: decimal = sqrt(self.some_decimal())
+    return self.c
+    """
+
+    c = get_contract(code)
+    assert c.foo() == 1
```

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/numbers/test_unsigned_ints.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/numbers/test_unsigned_ints.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/test_array_indexing.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/test_array_indexing.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/test_bytes.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/test_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/test_bytes_literal.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/test_bytes_literal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/test_bytes_zero_padding.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/test_bytes_zero_padding.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/test_dynamic_array.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/test_dynamic_array.py`

 * *Files 0% similar despite different names*

```diff
@@ -1861,7 +1861,29 @@
 
 @pytest.mark.parametrize("code", dynarray_length_no_clobber_cases)
 def test_dynarray_length_no_clobber(get_contract, tx_failed, code):
     # check that length is not clobbered before dynarray data copy happens
     c = get_contract(code)
     with tx_failed():
         c.should_revert()
+
+
+def test_dynarray_make_setter_overlap(get_contract):
+    # GH 4056, variant of GH 3503
+    code = """
+a: DynArray[DynArray[uint256, 10], 10]
+
+@external
+def foo() -> DynArray[uint256, 10]:
+    self.a.append([1, 2, self.boo(), 4])
+    return self.a[0] # returns [11, 12, 3, 4]
+
+@internal
+def boo() -> uint256:
+    self.a.append([11, 12, 13, 14, 15, 16])
+    self.a.pop()
+    # it should now be impossible to read any of [11, 12, 13, 14, 15, 16]
+    return 3
+    """
+
+    c = get_contract(code)
+    assert c.foo() == [1, 2, 3, 4]
```

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/test_flag.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/test_flag.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/test_identifier_naming.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/test_identifier_naming.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/test_lists.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/test_lists.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/test_node_types.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/test_node_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/test_string.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/test_string.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/test_string_literal.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/test_string_literal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/codegen/types/test_struct.py` & `vyper-0.4.0rc6/tests/functional/codegen/types/test_struct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/examples/auctions/test_blind_auction.py` & `vyper-0.4.0rc6/tests/functional/examples/auctions/test_blind_auction.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/examples/auctions/test_simple_open_auction.py` & `vyper-0.4.0rc6/tests/functional/examples/auctions/test_simple_open_auction.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/examples/company/test_company.py` & `vyper-0.4.0rc6/tests/functional/examples/company/test_company.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/examples/crowdfund/test_crowdfund_example.py` & `vyper-0.4.0rc6/tests/functional/examples/crowdfund/test_crowdfund_example.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/examples/factory/test_factory.py` & `vyper-0.4.0rc6/tests/functional/examples/factory/test_factory.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/examples/market_maker/test_on_chain_market_maker.py` & `vyper-0.4.0rc6/tests/functional/examples/market_maker/test_on_chain_market_maker.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py` & `vyper-0.4.0rc6/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/examples/storage/test_advanced_storage.py` & `vyper-0.4.0rc6/tests/functional/examples/storage/test_advanced_storage.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/examples/storage/test_storage.py` & `vyper-0.4.0rc6/tests/functional/examples/storage/test_storage.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/examples/tokens/test_erc1155.py` & `vyper-0.4.0rc6/tests/functional/examples/tokens/test_erc1155.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/examples/tokens/test_erc20.py` & `vyper-0.4.0rc6/tests/functional/examples/tokens/test_erc20.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/examples/tokens/test_erc4626.py` & `vyper-0.4.0rc6/tests/functional/examples/tokens/test_erc4626.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/examples/tokens/test_erc721.py` & `vyper-0.4.0rc6/tests/functional/examples/tokens/test_erc721.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/examples/voting/test_ballot.py` & `vyper-0.4.0rc6/tests/functional/examples/voting/test_ballot.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/examples/wallet/test_wallet.py` & `vyper-0.4.0rc6/tests/functional/examples/wallet/test_wallet.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/grammar/test_grammar.py` & `vyper-0.4.0rc6/tests/functional/grammar/test_grammar.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_argument_exception.py` & `vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_argument_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_call_violation.py` & `vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_call_violation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_constancy_exception.py` & `vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_constancy_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_function_declaration_exception.py` & `vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_function_declaration_exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,24 +15,14 @@
 x: int128
 @external
 @monkeydoodledoo
 def foo() -> int128:
     pass
     """,
     """
-def foo() -> int128:
-    q: int128 = 111
-    return q
-    """,
-    """
-q: int128
-def foo() -> int128:
-    return self.q
-    """,
-    """
 @external
 def test_func() -> int128:
     return (1, 2)
     """,
     """
 @deploy
 def __init__(a: int128 = 12):
```

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_instantiation_exception.py` & `vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_instantiation_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_invalid_literal_exception.py` & `vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_invalid_literal_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_invalid_payable.py` & `vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_invalid_payable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_invalid_reference.py` & `vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_invalid_reference.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_invalid_type_exception.py` & `vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_invalid_type_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_namespace_collision.py` & `vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_namespace_collision.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_overflow_exception.py` & `vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_overflow_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_structure_exception.py` & `vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_structure_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_syntax_exception.py` & `vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_syntax_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_type_mismatch_exception.py` & `vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_type_mismatch_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_undeclared_definition.py` & `vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_undeclared_definition.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_variable_declaration_exception.py` & `vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_variable_declaration_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/exceptions/test_vyper_exception_pos.py` & `vyper-0.4.0rc6/tests/functional/syntax/exceptions/test_vyper_exception_pos.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/modules/test_deploy_visibility.py` & `vyper-0.4.0rc6/tests/functional/syntax/modules/test_deploy_visibility.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/modules/test_exports.py` & `vyper-0.4.0rc6/tests/functional/syntax/modules/test_exports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/modules/test_implements.py` & `vyper-0.4.0rc6/tests/functional/syntax/modules/test_implements.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/modules/test_initializers.py` & `vyper-0.4.0rc6/tests/functional/syntax/modules/test_initializers.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/names/test_event_names.py` & `vyper-0.4.0rc6/tests/functional/syntax/names/test_event_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/names/test_function_names.py` & `vyper-0.4.0rc6/tests/functional/syntax/names/test_function_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/names/test_variable_names.py` & `vyper-0.4.0rc6/tests/functional/syntax/names/test_variable_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/signatures/test_invalid_function_decorators.py` & `vyper-0.4.0rc6/tests/functional/syntax/signatures/test_invalid_function_decorators.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/signatures/test_method_id_conflicts.py` & `vyper-0.4.0rc6/tests/functional/syntax/signatures/test_method_id_conflicts.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_abi_decode.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_abi_decode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_abi_encode.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_abi_encode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_abs.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_abs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_addmulmod.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_addmulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_address_code.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_address_code.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_ann_assign.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_ann_assign.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_as_uint256.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_as_uint256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_as_wei_value.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_block.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_block.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_blockscope.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_blockscope.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_bool.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_bool.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_bool_ops.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_bool_ops.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_bytes.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_chainid.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_chainid.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_code_size.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_code_size.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_codehash.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_codehash.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_concat.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_concat.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_constants.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_create_with_code_of.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_create_with_code_of.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_dynamic_array.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_dynamic_array.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_external_calls.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_external_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_extract32.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_extract32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_flag.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_flag.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_for_range.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_for_range.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_functions_call.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_functions_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_immutables.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_immutables.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_init.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_init.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_interfaces.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_invalids.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_invalids.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_keccak256.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_keccak256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_len.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_len.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_list.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_logging.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_logging.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_method_id.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_method_id.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_minmax.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_minmax.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_minmax_value.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_minmax_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_msg_data.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_msg_data.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_nested_list.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_nested_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_no_none.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_no_none.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_powmod.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_powmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_print.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_print.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_public.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_public.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_raw_call.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_raw_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_return_tuple.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_return_tuple.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_self_balance.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_self_balance.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_selfdestruct.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_selfdestruct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_send.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_send.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_slice.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_slice.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_string.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_string.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_structs.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_structs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_ternary.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_ternary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_tuple_assign.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_tuple_assign.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/functional/syntax/test_unbalanced_return.py` & `vyper-0.4.0rc6/tests/functional/syntax/test_unbalanced_return.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/abi_types/test_invalid_abi_types.py` & `vyper-0.4.0rc6/tests/unit/abi_types/test_invalid_abi_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/nodes/test_compare_nodes.py` & `vyper-0.4.0rc6/tests/unit/ast/nodes/test_compare_nodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/nodes/test_fold_binop_decimal.py` & `vyper-0.4.0rc6/tests/unit/ast/nodes/test_fold_binop_decimal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/nodes/test_fold_binop_int.py` & `vyper-0.4.0rc6/tests/unit/ast/nodes/test_fold_binop_int.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/nodes/test_fold_boolop.py` & `vyper-0.4.0rc6/tests/unit/ast/nodes/test_fold_boolop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/nodes/test_fold_compare.py` & `vyper-0.4.0rc6/tests/unit/ast/nodes/test_fold_compare.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/nodes/test_fold_subscript.py` & `vyper-0.4.0rc6/tests/unit/ast/nodes/test_fold_subscript.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/nodes/test_fold_unaryop.py` & `vyper-0.4.0rc6/tests/unit/ast/nodes/test_fold_unaryop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/nodes/test_from_node.py` & `vyper-0.4.0rc6/tests/unit/ast/nodes/test_from_node.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/nodes/test_get_children.py` & `vyper-0.4.0rc6/tests/unit/ast/nodes/test_get_children.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/nodes/test_get_descendants.py` & `vyper-0.4.0rc6/tests/unit/ast/nodes/test_get_descendants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/nodes/test_hex.py` & `vyper-0.4.0rc6/tests/unit/ast/nodes/test_hex.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/test_annotate_and_optimize_ast.py` & `vyper-0.4.0rc6/tests/unit/ast/test_annotate_and_optimize_ast.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/test_ast_dict.py` & `vyper-0.4.0rc6/tests/unit/ast/test_ast_dict.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/test_metadata_journal.py` & `vyper-0.4.0rc6/tests/unit/ast/test_metadata_journal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/test_natspec.py` & `vyper-0.4.0rc6/tests/unit/ast/test_natspec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/test_parser.py` & `vyper-0.4.0rc6/tests/unit/ast/test_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/test_pre_parser.py` & `vyper-0.4.0rc6/tests/unit/ast/test_pre_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/ast/test_source_annotation.py` & `vyper-0.4.0rc6/tests/unit/ast/test_source_annotation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/cli/storage_layout/test_storage_layout.py` & `vyper-0.4.0rc6/tests/unit/cli/storage_layout/test_storage_layout.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,11 @@
 from vyper.compiler import compile_code
 from vyper.evm.opcodes import version_check
 
-
-def _adjust_storage_layout_for_cancun(layout):
-    def _go(layout):
-        for _varname, item in layout.items():
-            if "slot" in item and isinstance(item["slot"], int):
-                item["slot"] -= 1
-            else:
-                # recurse to submodule
-                _go(item)
-
-    if version_check(begin="cancun"):
-        layout["transient_storage_layout"] = {
-            "$.nonreentrant_key": layout["storage_layout"].pop("$.nonreentrant_key")
-        }
-        _go(layout["storage_layout"])
+from .utils import adjust_storage_layout_for_cancun
 
 
 def test_storage_layout():
     code = """
 foo: HashMap[address, uint256]
 
 @external
@@ -51,27 +37,26 @@
 
 @external
 @nonreentrant
 def public_foo3():
     pass
     """
 
-    out = compile_code(code, output_formats=["layout"])
-
     expected = {
         "storage_layout": {
-            "$.nonreentrant_key": {"slot": 0, "type": "nonreentrant lock"},
-            "foo": {"slot": 1, "type": "HashMap[address, uint256]"},
-            "arr": {"slot": 2, "type": "DynArray[uint256, 3]"},
-            "baz": {"slot": 6, "type": "Bytes[65]"},
-            "bar": {"slot": 10, "type": "uint256"},
+            "$.nonreentrant_key": {"slot": 0, "type": "nonreentrant lock", "n_slots": 1},
+            "foo": {"slot": 1, "type": "HashMap[address, uint256]", "n_slots": 1},
+            "arr": {"slot": 2, "type": "DynArray[uint256, 3]", "n_slots": 4},
+            "baz": {"slot": 6, "type": "Bytes[65]", "n_slots": 4},
+            "bar": {"slot": 10, "type": "uint256", "n_slots": 1},
         }
     }
-    _adjust_storage_layout_for_cancun(expected)
+    adjust_storage_layout_for_cancun(expected)
 
+    out = compile_code(code, output_formats=["layout"])
     assert out["layout"] == expected
 
 
 def test_storage_and_immutables_layout():
     code = """
 name: String[32]
 SYMBOL: immutable(String[32])
@@ -84,20 +69,17 @@
     """
 
     expected_layout = {
         "code_layout": {
             "SYMBOL": {"length": 64, "offset": 0, "type": "String[32]"},
             "DECIMALS": {"length": 32, "offset": 64, "type": "uint8"},
         },
-        "storage_layout": {
-            "$.nonreentrant_key": {"slot": 0, "type": "nonreentrant lock"},
-            "name": {"slot": 1, "type": "String[32]"},
-        },
+        "storage_layout": {"name": {"slot": 1, "type": "String[32]", "n_slots": 2}},
     }
-    _adjust_storage_layout_for_cancun(expected_layout)
+    adjust_storage_layout_for_cancun(expected_layout)
 
     out = compile_code(code, output_formats=["layout"])
     assert out["layout"] == expected_layout
 
 
 def test_storage_layout_module(make_input_bundle):
     lib1 = """
@@ -133,21 +115,20 @@
             "some_immutable": {"length": 352, "offset": 0, "type": "DynArray[uint256, 10]"},
             "a_library": {
                 "SYMBOL": {"length": 64, "offset": 352, "type": "String[32]"},
                 "DECIMALS": {"length": 32, "offset": 416, "type": "uint8"},
             },
         },
         "storage_layout": {
-            "$.nonreentrant_key": {"slot": 0, "type": "nonreentrant lock"},
-            "counter": {"slot": 1, "type": "uint256"},
-            "counter2": {"slot": 2, "type": "uint256"},
-            "a_library": {"supply": {"slot": 3, "type": "uint256"}},
+            "counter": {"slot": 1, "type": "uint256", "n_slots": 1},
+            "counter2": {"slot": 2, "type": "uint256", "n_slots": 1},
+            "a_library": {"supply": {"slot": 3, "type": "uint256", "n_slots": 1}},
         },
     }
-    _adjust_storage_layout_for_cancun(expected_layout)
+    adjust_storage_layout_for_cancun(expected_layout)
 
     out = compile_code(code, input_bundle=input_bundle, output_formats=["layout"])
     assert out["layout"] == expected_layout
 
 
 def test_storage_layout_module2(make_input_bundle):
     # test module storage layout, but initializes is in a different order
@@ -183,21 +164,20 @@
             "some_immutable": {"length": 352, "offset": 0, "type": "DynArray[uint256, 10]"},
             "a_library": {
                 "SYMBOL": {"length": 64, "offset": 352, "type": "String[32]"},
                 "DECIMALS": {"length": 32, "offset": 416, "type": "uint8"},
             },
         },
         "storage_layout": {
-            "$.nonreentrant_key": {"slot": 0, "type": "nonreentrant lock"},
-            "counter": {"slot": 1, "type": "uint256"},
-            "a_library": {"supply": {"slot": 2, "type": "uint256"}},
-            "counter2": {"slot": 3, "type": "uint256"},
+            "counter": {"slot": 1, "type": "uint256", "n_slots": 1},
+            "a_library": {"supply": {"slot": 2, "type": "uint256", "n_slots": 1}},
+            "counter2": {"slot": 3, "type": "uint256", "n_slots": 1},
         },
     }
-    _adjust_storage_layout_for_cancun(expected_layout)
+    adjust_storage_layout_for_cancun(expected_layout)
 
     out = compile_code(code, input_bundle=input_bundle, output_formats=["layout"])
     assert out["layout"] == expected_layout
 
 
 def test_storage_layout_module_uses(make_input_bundle):
     # test module storage layout, with initializes/uses and a nonreentrant
@@ -267,22 +247,22 @@
             "lib2": {"immutable_variable": {"length": 32, "offset": 352, "type": "uint256"}},
             "a_library": {
                 "SYMBOL": {"length": 64, "offset": 384, "type": "String[32]"},
                 "DECIMALS": {"length": 32, "offset": 448, "type": "uint8"},
             },
         },
         "storage_layout": {
-            "$.nonreentrant_key": {"slot": 0, "type": "nonreentrant lock"},
-            "counter": {"slot": 1, "type": "uint256"},
-            "lib2": {"storage_variable": {"slot": 2, "type": "uint256"}},
-            "counter2": {"slot": 3, "type": "uint256"},
-            "a_library": {"supply": {"slot": 4, "type": "uint256"}},
+            "$.nonreentrant_key": {"slot": 0, "type": "nonreentrant lock", "n_slots": 1},
+            "counter": {"slot": 1, "type": "uint256", "n_slots": 1},
+            "lib2": {"storage_variable": {"slot": 2, "type": "uint256", "n_slots": 1}},
+            "counter2": {"slot": 3, "type": "uint256", "n_slots": 1},
+            "a_library": {"supply": {"slot": 4, "type": "uint256", "n_slots": 1}},
         },
     }
-    _adjust_storage_layout_for_cancun(expected_layout)
+    adjust_storage_layout_for_cancun(expected_layout)
 
     out = compile_code(code, input_bundle=input_bundle, output_formats=["layout"])
     assert out["layout"] == expected_layout
 
 
 def test_storage_layout_module_nested_initializes(make_input_bundle):
     # test module storage layout, with initializes in an imported module
@@ -347,20 +327,56 @@
                     "SYMBOL": {"length": 64, "offset": 352, "type": "String[32]"},
                     "DECIMALS": {"length": 32, "offset": 416, "type": "uint8"},
                 },
                 "immutable_variable": {"length": 32, "offset": 448, "type": "uint256"},
             },
         },
         "storage_layout": {
-            "$.nonreentrant_key": {"slot": 0, "type": "nonreentrant lock"},
-            "counter": {"slot": 1, "type": "uint256"},
+            "counter": {"slot": 1, "type": "uint256", "n_slots": 1},
             "lib2": {
-                "lib1": {"supply": {"slot": 2, "type": "uint256"}},
-                "storage_variable": {"slot": 3, "type": "uint256"},
+                "lib1": {"supply": {"slot": 2, "type": "uint256", "n_slots": 1}},
+                "storage_variable": {"slot": 3, "type": "uint256", "n_slots": 1},
             },
-            "counter2": {"slot": 4, "type": "uint256"},
+            "counter2": {"slot": 4, "type": "uint256", "n_slots": 1},
         },
     }
-    _adjust_storage_layout_for_cancun(expected_layout)
+    adjust_storage_layout_for_cancun(expected_layout)
 
     out = compile_code(code, input_bundle=input_bundle, output_formats=["layout"])
     assert out["layout"] == expected_layout
+
+
+def test_multiple_compile_codes(make_input_bundle):
+    # test calling compile_code multiple times with the same library allocated
+    # in different locations
+    lib = """
+x: uint256
+    """
+    input_bundle = make_input_bundle({"lib.vy": lib})
+
+    main1 = """
+import lib
+
+initializes: lib
+t: uint256
+    """
+    main2 = """
+import lib
+
+t: uint256
+initializes: lib
+    """
+    out1 = compile_code(main1, input_bundle=input_bundle, output_formats=["layout"])["layout"]
+    out2 = compile_code(main2, input_bundle=input_bundle, output_formats=["layout"])["layout"]
+
+    layout1 = out1["storage_layout"]["lib"]
+    layout2 = out2["storage_layout"]["lib"]
+
+    assert layout1 != layout2  # for clarity
+
+    if version_check(begin="cancun"):
+        start_slot = 0
+    else:
+        start_slot = 1
+
+    assert layout1 == {"x": {"slot": start_slot, "type": "uint256", "n_slots": 1}}
+    assert layout2 == {"x": {"slot": start_slot + 1, "type": "uint256", "n_slots": 1}}
```

### Comparing `vyper-0.4.0rc5/tests/unit/cli/vyper_compile/test_compile_files.py` & `vyper-0.4.0rc6/tests/unit/cli/vyper_compile/test_compile_files.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/cli/vyper_compile/test_parse_args.py` & `vyper-0.4.0rc6/tests/unit/cli/vyper_compile/test_parse_args.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/cli/vyper_json/test_compile_json.py` & `vyper-0.4.0rc6/tests/unit/cli/vyper_json/test_compile_json.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/cli/vyper_json/test_get_inputs.py` & `vyper-0.4.0rc6/tests/unit/cli/vyper_json/test_get_inputs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/cli/vyper_json/test_get_settings.py` & `vyper-0.4.0rc6/tests/unit/cli/vyper_json/test_get_settings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/cli/vyper_json/test_output_selection.py` & `vyper-0.4.0rc6/tests/unit/cli/vyper_json/test_output_selection.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py` & `vyper-0.4.0rc6/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/asm/test_asm_optimizer.py` & `vyper-0.4.0rc6/tests/unit/compiler/asm/test_asm_optimizer.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/ir/test_compile_ir.py` & `vyper-0.4.0rc6/tests/unit/compiler/ir/test_compile_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/ir/test_optimize_ir.py` & `vyper-0.4.0rc6/tests/unit/compiler/ir/test_optimize_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/ir/test_with.py` & `vyper-0.4.0rc6/tests/unit/compiler/ir/test_with.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/test_abi.py` & `vyper-0.4.0rc6/tests/unit/compiler/test_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/test_bytecode_runtime.py` & `vyper-0.4.0rc6/tests/unit/compiler/test_bytecode_runtime.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/test_default_settings.py` & `vyper-0.4.0rc6/tests/unit/compiler/test_default_settings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/test_input_bundle.py` & `vyper-0.4.0rc6/tests/unit/compiler/test_input_bundle.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/test_opcodes.py` & `vyper-0.4.0rc6/tests/unit/compiler/test_opcodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/test_pre_parser.py` & `vyper-0.4.0rc6/tests/unit/compiler/test_pre_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/test_sha3_32.py` & `vyper-0.4.0rc6/tests/unit/compiler/test_sha3_32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/test_source_map.py` & `vyper-0.4.0rc6/tests/unit/compiler/test_source_map.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/venom/test_convert_basicblock_simple.py` & `vyper-0.4.0rc6/tests/unit/compiler/venom/test_convert_basicblock_simple.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/venom/test_dominator_tree.py` & `vyper-0.4.0rc6/tests/unit/compiler/venom/test_dominator_tree.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/venom/test_duplicate_operands.py` & `vyper-0.4.0rc6/tests/unit/compiler/venom/test_duplicate_operands.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/venom/test_make_ssa.py` & `vyper-0.4.0rc6/tests/unit/compiler/venom/test_make_ssa.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/venom/test_multi_entry_block.py` & `vyper-0.4.0rc6/tests/unit/compiler/venom/test_multi_entry_block.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/compiler/venom/test_sccp.py` & `vyper-0.4.0rc6/tests/unit/compiler/venom/test_sccp.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/semantics/analysis/test_array_index.py` & `vyper-0.4.0rc6/tests/unit/semantics/analysis/test_array_index.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/semantics/analysis/test_cyclic_function_calls.py` & `vyper-0.4.0rc6/tests/unit/semantics/analysis/test_cyclic_function_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/semantics/analysis/test_for_loop.py` & `vyper-0.4.0rc6/tests/unit/semantics/analysis/test_for_loop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/semantics/analysis/test_potential_types.py` & `vyper-0.4.0rc6/tests/unit/semantics/analysis/test_potential_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/semantics/conftest.py` & `vyper-0.4.0rc6/tests/unit/semantics/conftest.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/semantics/test_namespace.py` & `vyper-0.4.0rc6/tests/unit/semantics/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/semantics/test_storage_slots.py` & `vyper-0.4.0rc6/tests/unit/semantics/test_storage_slots.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/semantics/types/test_event.py` & `vyper-0.4.0rc6/tests/unit/semantics/types/test_event.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/semantics/types/test_pure_types.py` & `vyper-0.4.0rc6/tests/unit/semantics/types/test_pure_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/semantics/types/test_size_in_bytes.py` & `vyper-0.4.0rc6/tests/unit/semantics/types/test_size_in_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/semantics/types/test_type_from_abi.py` & `vyper-0.4.0rc6/tests/unit/semantics/types/test_type_from_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/unit/semantics/types/test_type_from_annotation.py` & `vyper-0.4.0rc6/tests/unit/semantics/types/test_type_from_annotation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/tests/utils.py` & `vyper-0.4.0rc6/tests/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/__init__.py` & `vyper-0.4.0rc6/vyper/__init__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/__main__.py` & `vyper-0.4.0rc6/vyper/__main__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/abi_types.py` & `vyper-0.4.0rc6/vyper/abi_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/ast/README.md` & `vyper-0.4.0rc6/vyper/ast/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/ast/grammar.lark` & `vyper-0.4.0rc6/vyper/ast/grammar.lark`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/ast/grammar.py` & `vyper-0.4.0rc6/vyper/ast/grammar.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/ast/identifiers.py` & `vyper-0.4.0rc6/vyper/ast/identifiers.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/ast/metadata.py` & `vyper-0.4.0rc6/vyper/ast/metadata.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/ast/natspec.py` & `vyper-0.4.0rc6/vyper/ast/natspec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/ast/nodes.py` & `vyper-0.4.0rc6/vyper/ast/nodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/ast/nodes.pyi` & `vyper-0.4.0rc6/vyper/ast/nodes.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -230,14 +230,15 @@
 class VariableDecl(VyperNode):
     target: Name = ...
     value: VyperNode = ...
     annotation: VyperNode = ...
     is_constant: bool = ...
     is_public: bool = ...
     is_immutable: bool = ...
+    is_transient: bool = ...
     _expanded_getter: FunctionDef = ...
 
 class AugAssign(VyperNode):
     op: VyperNode = ...
     target: ExprNode = ...
     value: ExprNode = ...
```

### Comparing `vyper-0.4.0rc5/vyper/ast/parse.py` & `vyper-0.4.0rc6/vyper/ast/parse.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/ast/pre_parser.py` & `vyper-0.4.0rc6/vyper/ast/pre_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/ast/utils.py` & `vyper-0.4.0rc6/vyper/ast/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/ast/validation.py` & `vyper-0.4.0rc6/vyper/ast/validation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/builtins/_convert.py` & `vyper-0.4.0rc6/vyper/builtins/_convert.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/builtins/_signatures.py` & `vyper-0.4.0rc6/vyper/builtins/_signatures.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/builtins/_utils.py` & `vyper-0.4.0rc6/vyper/builtins/_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/builtins/functions.py` & `vyper-0.4.0rc6/vyper/builtins/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from vyper.codegen.core import (
     LOAD,
     STORE,
     IRnode,
     add_ofst,
     bytes_data_ptr,
     calculate_type_for_external_return,
+    check_buffer_overflow_ir,
     check_external_call,
     clamp,
     clamp2,
     clamp_basetype,
     clamp_nonzero,
     copy_bytes,
     dummy_node_for_type,
@@ -228,72 +229,62 @@
     def build_IR(self, expr, context):
         return convert(expr, context)
 
 
 ADHOC_SLICE_NODE_MACROS = ["~calldata", "~selfcode", "~extcode"]
 
 
-# make sure we don't overrun the source buffer, checking for overflow:
-# valid inputs satisfy:
-#   `assert !(start+length > src_len || start+length < start`
-def _make_slice_bounds_check(start, length, src_len):
-    with start.cache_when_complex("start") as (b1, start):
-        with add_ofst(start, length).cache_when_complex("end") as (b2, end):
-            arithmetic_overflow = ["lt", end, start]
-            buffer_oob = ["gt", end, src_len]
-            ok = ["iszero", ["or", arithmetic_overflow, buffer_oob]]
-            return b1.resolve(b2.resolve(["assert", ok]))
-
-
 def _build_adhoc_slice_node(sub: IRnode, start: IRnode, length: IRnode, context: Context) -> IRnode:
     assert length.is_literal, "typechecker failed"
     assert isinstance(length.value, int)  # mypy hint
 
     dst_typ = BytesT(length.value)
     # allocate a buffer for the return value
     buf = context.new_internal_variable(dst_typ)
 
-    # `msg.data` by `calldatacopy`
-    if sub.value == "~calldata":
-        node = [
-            "seq",
-            _make_slice_bounds_check(start, length, "calldatasize"),
-            ["mstore", buf, length],
-            ["calldatacopy", add_ofst(buf, 32), start, length],
-            buf,
-        ]
-
-    # `self.code` by `codecopy`
-    elif sub.value == "~selfcode":
-        node = [
-            "seq",
-            _make_slice_bounds_check(start, length, "codesize"),
-            ["mstore", buf, length],
-            ["codecopy", add_ofst(buf, 32), start, length],
-            buf,
-        ]
+    with scope_multi((start, length), ("start", "length")) as (b1, (start, length)):
+        # `msg.data` by `calldatacopy`
+        if sub.value == "~calldata":
+            node = [
+                "seq",
+                check_buffer_overflow_ir(start, length, "calldatasize"),
+                ["mstore", buf, length],
+                ["calldatacopy", add_ofst(buf, 32), start, length],
+                buf,
+            ]
 
-    # `<address>.code` by `extcodecopy`
-    else:
-        assert sub.value == "~extcode" and len(sub.args) == 1
-        node = [
-            "with",
-            "_extcode_address",
-            sub.args[0],
-            [
+        # `self.code` by `codecopy`
+        elif sub.value == "~selfcode":
+            node = [
                 "seq",
-                _make_slice_bounds_check(start, length, ["extcodesize", "_extcode_address"]),
+                check_buffer_overflow_ir(start, length, "codesize"),
                 ["mstore", buf, length],
-                ["extcodecopy", "_extcode_address", add_ofst(buf, 32), start, length],
+                ["codecopy", add_ofst(buf, 32), start, length],
                 buf,
-            ],
-        ]
+            ]
 
-    assert isinstance(length.value, int)  # mypy hint
-    return IRnode.from_list(node, typ=BytesT(length.value), location=MEMORY)
+        # `<address>.code` by `extcodecopy`
+        else:
+            assert sub.value == "~extcode" and len(sub.args) == 1
+            node = [
+                "with",
+                "_extcode_address",
+                sub.args[0],
+                [
+                    "seq",
+                    check_buffer_overflow_ir(start, length, ["extcodesize", "_extcode_address"]),
+                    ["mstore", buf, length],
+                    ["extcodecopy", "_extcode_address", add_ofst(buf, 32), start, length],
+                    buf,
+                ],
+            ]
+
+        assert isinstance(length.value, int)  # mypy hint
+        ret = IRnode.from_list(node, typ=BytesT(length.value), location=MEMORY)
+        return b1.resolve(ret)
 
 
 # note: this and a lot of other builtins could be refactored to accept any uint type
 class Slice(BuiltinFunctionT):
     _id = "slice"
     _inputs = [
         ("b", (BYTES32_T, BytesT.any(), StringT.any())),
@@ -450,15 +441,15 @@
                 copy_len = length
                 copy_maxlen = buflen
 
             do_copy = copy_bytes(copy_dst, copy_src, copy_len, copy_maxlen)
 
             ret = [
                 "seq",
-                _make_slice_bounds_check(start, length, src_len),
+                check_buffer_overflow_ir(start, length, src_len),
                 do_copy,
                 ["mstore", dst, length],  # set length
                 dst,  # return pointer to dst
             ]
             ret = IRnode.from_list(ret, typ=dst_typ, location=MEMORY)
             return b1.resolve(b2.resolve(b3.resolve(ret)))
 
@@ -1812,30 +1803,40 @@
 
         ctor_args = [ensure_in_memory(arg, context) for arg in ctor_args]
 
         if raw_args:
             if len(ctor_args) != 1 or not isinstance(ctor_args[0].typ, BytesT):
                 raise StructureException("raw_args must be used with exactly 1 bytes argument")
 
-            argbuf = bytes_data_ptr(ctor_args[0])
-            argslen = get_bytearray_length(ctor_args[0])
-            bufsz = ctor_args[0].typ.maxlen
+            with ctor_args[0].cache_when_complex("arg") as (b1, arg):
+                argbuf = bytes_data_ptr(arg)
+                argslen = get_bytearray_length(arg)
+                bufsz = arg.typ.maxlen
+                return b1.resolve(
+                    self._helper(
+                        argbuf, bufsz, target, value, salt, argslen, code_offset, revert_on_failure
+                    )
+                )
         else:
             # encode the varargs
             to_encode = ir_tuple_from_args(ctor_args)
 
             # pretend we allocated enough memory for the encoder
             # (we didn't, but we are clobbering unused memory so it's safe.)
             bufsz = to_encode.typ.abi_type.size_bound()
             argbuf = context.new_internal_variable(get_type_for_exact_size(bufsz))
 
             # return a complex expression which writes to memory and returns
             # the length of the encoded data
             argslen = abi_encode(argbuf, to_encode, context, bufsz=bufsz, returns_len=True)
+            return self._helper(
+                argbuf, bufsz, target, value, salt, argslen, code_offset, revert_on_failure
+            )
 
+    def _helper(self, argbuf, bufsz, target, value, salt, argslen, code_offset, revert_on_failure):
         # NOTE: we need to invoke the abi encoder before evaluating MSIZE,
         # then copy the abi encoded buffer to past-the-end of the initcode
         # (since the abi encoder could write to fresh memory).
         # it would be good to not require the memory copy, but need
         # to evaluate memory safety.
         with scope_multi(
             (target, value, salt, argslen, code_offset),
@@ -2114,56 +2115,58 @@
     @process_inputs
     def build_IR(self, expr, args, kwargs, context):
         # TODO fix cyclic dependency with codegen/stmt.py
         from ._utils import generate_inline_function
 
         arg = args[0]
         # TODO: reify decimal and integer sqrt paths (see isqrt)
-        sqrt_code = """
+        with arg.cache_when_complex("x") as (b1, arg):
+            sqrt_code = """
 assert x >= 0.0
 z: decimal = 0.0
 
 if x == 0.0:
     z = 0.0
 else:
     z = x / 2.0 + 0.5
     y: decimal = x
 
     for i: uint256 in range(256):
         if z == y:
             break
         y = z
         z = (x / z + z) / 2.0
-        """
+            """
 
-        x_type = DecimalT()
-        placeholder_copy = ["pass"]
-        # Steal current position if variable is already allocated.
-        if arg.value == "mload":
-            new_var_pos = arg.args[0]
-        # Other locations need to be copied.
-        else:
-            new_var_pos = context.new_internal_variable(x_type)
-            placeholder_copy = ["mstore", new_var_pos, arg]
-        # Create input variables.
-        variables = {"x": VariableRecord(name="x", pos=new_var_pos, typ=x_type, mutable=False)}
-        # Dictionary to update new (i.e. typecheck) namespace
-        variables_2 = {"x": VarInfo(DecimalT())}
-        # Generate inline IR.
-        new_ctx, sqrt_ir = generate_inline_function(
-            code=sqrt_code,
-            variables=variables,
-            variables_2=variables_2,
-            memory_allocator=context.memory_allocator,
-        )
-        return IRnode.from_list(
-            ["seq", placeholder_copy, sqrt_ir, new_ctx.vars["z"].pos],  # load x variable
-            typ=DecimalT(),
-            location=MEMORY,
-        )
+            x_type = DecimalT()
+            placeholder_copy = ["pass"]
+            # Steal current position if variable is already allocated.
+            if arg.value == "mload":
+                new_var_pos = arg.args[0]
+            # Other locations need to be copied.
+            else:
+                new_var_pos = context.new_internal_variable(x_type)
+                placeholder_copy = ["mstore", new_var_pos, arg]
+            # Create input variables.
+            variables = {"x": VariableRecord(name="x", pos=new_var_pos, typ=x_type, mutable=False)}
+            # Dictionary to update new (i.e. typecheck) namespace
+            variables_2 = {"x": VarInfo(DecimalT())}
+            # Generate inline IR.
+            new_ctx, sqrt_ir = generate_inline_function(
+                code=sqrt_code,
+                variables=variables,
+                variables_2=variables_2,
+                memory_allocator=context.memory_allocator,
+            )
+            ret = IRnode.from_list(
+                ["seq", placeholder_copy, sqrt_ir, new_ctx.vars["z"].pos],  # load x variable
+                typ=DecimalT(),
+                location=MEMORY,
+            )
+            return b1.resolve(ret)
 
 
 class ISqrt(BuiltinFunctionT):
     _id = "isqrt"
     _inputs = [("d", UINT256_T)]
     _return_type = UINT256_T
 
@@ -2521,15 +2524,19 @@
             # TODO optimization: skip make_setter when we don't need
             # input validation
 
             output_buf = context.new_internal_variable(wrapped_typ)
 
             # sanity check buffer size for wrapped output type will not buffer overflow
             assert wrapped_typ.memory_bytes_required == output_typ.memory_bytes_required
-            ret.append(make_setter(output_buf, to_decode))
+
+            # pass a buffer bound to make_setter so appropriate oob
+            # validation is performed
+            buf_bound = add_ofst(data_ptr, data_len)
+            ret.append(make_setter(output_buf, to_decode, hi=buf_bound))
 
             ret.append(output_buf)
             # finalize. set the type and location for the return buffer.
             # (note: unwraps the tuple type if necessary)
             ret = IRnode.from_list(ret, typ=output_typ, location=MEMORY)
             return b1.resolve(ret)
```

### Comparing `vyper-0.4.0rc5/vyper/builtins/interfaces/IERC20.vyi` & `vyper-0.4.0rc6/vyper/builtins/interfaces/IERC20.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/builtins/interfaces/IERC4626.vyi` & `vyper-0.4.0rc6/vyper/builtins/interfaces/IERC4626.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/builtins/interfaces/IERC721.vyi` & `vyper-0.4.0rc6/vyper/builtins/interfaces/IERC721.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/cli/compile_archive.py` & `vyper-0.4.0rc6/vyper/cli/compile_archive.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/cli/vyper_compile.py` & `vyper-0.4.0rc6/vyper/cli/vyper_compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 external_interface - External interface of a contract, used for outside contract calls
 opcodes            - List of opcodes as a string
 opcodes_runtime    - List of runtime opcodes as a string
 ir                 - Intermediate representation in list format
 ir_json            - Intermediate representation in JSON format
 ir_runtime         - Intermediate representation of runtime bytecode in list format
 asm                - Output the EVM assembly of the deployable bytecode
+integrity          - Output the integrity hash of the source code
 archive            - Output the build as an archive file
 solc_json          - Output the build in solc json format
 """
 
 combined_json_outputs = [
     "bytecode",
     "bytecode_runtime",
@@ -159,27 +160,32 @@
         help="Switch to standard JSON mode. Use `--standard-json -h` for available options.",
         action="store_true",
     )
     parser.add_argument(
         "--hex-ir", help="Represent integers as hex values in the IR", action="store_true"
     )
     parser.add_argument(
-        "--path", "-p", help="Set the root path for contract imports", action="append", dest="paths"
+        "--path",
+        "-p",
+        help="Add a path to the compiler's search path",
+        action="append",
+        dest="paths",
     )
+    parser.add_argument(
+        "--disable-sys-path", help="Disable the use of sys.path", action="store_true"
+    )
+
     parser.add_argument("-o", help="Set the output path", dest="output_path")
     parser.add_argument(
         "--experimental-codegen",
         help="The compiler use the new IR codegen. This is an experimental feature.",
         action="store_true",
         dest="experimental_codegen",
     )
     parser.add_argument("--enable-decimals", help="Enable decimals", action="store_true")
-    parser.add_argument(
-        "--disable-sys-path", help="Disable the use of sys.path", action="store_true"
-    )
 
     args = parser.parse_args(argv)
 
     if args.traceback_limit is not None:
         sys.tracebacklimit = args.traceback_limit
     elif VYPER_TRACEBACK_LIMIT is not None:
         sys.tracebacklimit = VYPER_TRACEBACK_LIMIT
```

### Comparing `vyper-0.4.0rc5/vyper/cli/vyper_ir.py` & `vyper-0.4.0rc6/vyper/cli/vyper_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/cli/vyper_json.py` & `vyper-0.4.0rc6/vyper/cli/vyper_json.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/codegen/abi_encoder.py` & `vyper-0.4.0rc6/vyper/codegen/abi_encoder.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/codegen/arithmetic.py` & `vyper-0.4.0rc6/vyper/codegen/arithmetic.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/codegen/context.py` & `vyper-0.4.0rc6/vyper/codegen/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
             self.pos,
             typ=self.typ,
             annotation=self.name,
             encoding=self.encoding,
             mutable=self.mutable,
             location=self.location,
         )
-        ret._referenced_variables = {self}
         if self.alloca is not None:
             ret.passthrough_metadata["alloca"] = self.alloca
         return ret
 
 
 # compilation context for a function
 class Context:
```

### Comparing `vyper-0.4.0rc5/vyper/codegen/core.py` & `vyper-0.4.0rc6/vyper/codegen/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     CALLDATA,
     DATA,
     IMMUTABLES,
     MEMORY,
     STORAGE,
     TRANSIENT,
     AddrSpace,
+    legal_in_staticcall,
 )
 from vyper.evm.opcodes import version_check
 from vyper.exceptions import CompilerPanic, TypeCheckFailure, TypeMismatch
 from vyper.semantics.data_locations import DataLocation
 from vyper.semantics.types import (
     AddressT,
     BoolT,
@@ -132,34 +133,39 @@
         return DataLocation.CODE
     if s == CALLDATA:
         return DataLocation.CALLDATA
 
     raise CompilerPanic("unreachable!")  # pragma: nocover
 
 
+def writeable(context, ir_node):
+    assert ir_node.is_pointer  # sanity check
+
+    if context.is_constant() and not legal_in_staticcall(ir_node.location):
+        return False
+    return ir_node.mutable
+
+
 # Copy byte array word-for-word (including layout)
 # TODO make this a private function
 def make_byte_array_copier(dst, src):
     assert isinstance(src.typ, _BytestringT)
     assert isinstance(dst.typ, _BytestringT)
 
     _check_assign_bytes(dst, src)
 
     # TODO: remove this branch, copy_bytes and get_bytearray_length should handle
     if src.value == "~empty" or src.typ.maxlen == 0:
         # set length word to 0.
         return STORE(dst, 0)
 
     with src.cache_when_complex("src") as (b1, src):
-        has_storage = STORAGE in (src.location, dst.location)
-        is_memory_copy = dst.location == src.location == MEMORY
-        batch_uses_identity = is_memory_copy and not version_check(begin="cancun")
-        if src.typ.maxlen <= 32 and (has_storage or batch_uses_identity):
+        if src.typ.maxlen <= 32 and not copy_opcode_available(dst, src):
+            # if there is no batch copy opcode available,
             # it's cheaper to run two load/stores instead of copy_bytes
-
             ret = ["seq"]
             # store length word
             len_ = get_bytearray_length(src)
             ret.append(STORE(dst, len_))
 
             # store the single data word.
             dst_data_ptr = bytes_data_ptr(dst)
@@ -184,28 +190,31 @@
 def dynarray_data_ptr(ptr):
     if ptr.location is None:  # pragma: nocover
         raise CompilerPanic("tried to modify non-pointer type")
     assert isinstance(ptr.typ, DArrayT)
     return add_ofst(ptr, ptr.location.word_scale)
 
 
-def _dynarray_make_setter(dst, src):
+def _dynarray_make_setter(dst, src, hi=None):
     assert isinstance(src.typ, DArrayT)
     assert isinstance(dst.typ, DArrayT)
 
     if src.value == "~empty":
         return IRnode.from_list(STORE(dst, 0))
 
     # copy contents of src dynarray to dst.
     # note that in case src and dst refer to the same dynarray,
     # in order for get_element_ptr oob checks on the src dynarray
     # to work, we need to wait until after the data is copied
     # before we clobber the length word.
 
     if src.value == "multi":
+        # validation is only performed on unsafe data, but we are dealing with
+        # a literal here.
+        assert hi is None
         ret = ["seq"]
         # handle literals
 
         # copy each item
         n_items = len(src.args)
 
         for i in range(n_items):
@@ -248,14 +257,15 @@
 
             if should_loop:
                 i = IRnode.from_list(_freshname("copy_darray_ix"), typ=UINT256_T)
 
                 loop_body = make_setter(
                     get_element_ptr(dst, i, array_bounds_check=False),
                     get_element_ptr(src, i, array_bounds_check=False),
+                    hi=hi,
                 )
                 loop_body.annotation = f"{dst}[i] = {src}[i]"
 
                 ret.append(["repeat", i, 0, count, src.typ.count, loop_body])
                 # write the length word after data is copied
                 ret.append(STORE(dst, count))
 
@@ -397,29 +407,30 @@
             # NOTE: typechecks elem_node
             # NOTE skip array bounds check bc we already asserted len two lines up
             ret.append(
                 make_setter(get_element_ptr(darray_node, len_, array_bounds_check=False), elem_node)
             )
 
             # store new length
-            ret.append(STORE(darray_node, ["add", len_, 1]))
+            ret.append(ensure_eval_once("append_dynarray", STORE(darray_node, ["add", len_, 1])))
+
             return IRnode.from_list(b1.resolve(b2.resolve(ret)))
 
 
 def pop_dyn_array(darray_node, return_popped_item):
     assert isinstance(darray_node.typ, DArrayT)
     assert darray_node.encoding == Encoding.VYPER
     ret = ["seq"]
     with darray_node.cache_when_complex("darray") as (b1, darray_node):
         old_len = clamp("gt", get_dyn_array_count(darray_node), 0)
         new_len = IRnode.from_list(["sub", old_len, 1], typ=UINT256_T)
 
         with new_len.cache_when_complex("new_len") as (b2, new_len):
             # store new length
-            ret.append(STORE(darray_node, new_len))
+            ret.append(ensure_eval_once("pop_dynarray", STORE(darray_node, new_len)))
 
             # NOTE skip array bounds check bc we already asserted len two lines up
             if return_popped_item:
                 popped_item = get_element_ptr(darray_node, new_len, array_bounds_check=False)
                 ret.append(popped_item)
                 typ = popped_item.typ
                 location = popped_item.location
@@ -438,53 +449,54 @@
 # shorthand util
 def _mul(x, y):
     ret = ["mul", x, y]
     return IRnode.from_list(ret)
 
 
 # Resolve pointer locations for ABI-encoded data
-def _getelemptr_abi_helper(parent, member_t, ofst, clamp=True):
+def _getelemptr_abi_helper(parent, member_t, ofst):
     member_abi_t = member_t.abi_type
 
     # ABI encoding has length word and then pretends length is not there
     # e.g. [[1,2]] is encoded as 0x01 <len> 0x20 <inner array ofst> <encode(inner array)>
     # note that inner array ofst is 0x20, not 0x40.
     if has_length_word(parent.typ):
         parent = add_ofst(parent, parent.location.word_scale * DYNAMIC_ARRAY_OVERHEAD)
 
     ofst_ir = add_ofst(parent, ofst)
 
     if member_abi_t.is_dynamic():
         # double dereference, according to ABI spec
-        # TODO optimize special case: first dynamic item
-        # offset is statically known.
         ofst_ir = add_ofst(parent, unwrap_location(ofst_ir))
+        if _dirty_read_risk(ofst_ir):
+            # check no arithmetic overflow
+            ofst_ir = ["seq", ["assert", ["ge", ofst_ir, parent]], ofst_ir]
 
     return IRnode.from_list(
         ofst_ir,
         typ=member_t,
         location=parent.location,
         encoding=parent.encoding,
         annotation=f"{parent}{ofst}",
     )
 
 
 # TODO simplify this code, especially the ABI decoding
-def _get_element_ptr_tuplelike(parent, key):
+def _get_element_ptr_tuplelike(parent, key, hi=None):
     typ = parent.typ
     assert is_tuple_like(typ)
 
     if isinstance(typ, StructT):
         assert isinstance(key, str)
         subtype = typ.member_types[key]
         attrs = list(typ.tuple_keys())
         index = attrs.index(key)
         annotation = key
     else:
-        # TupleT
+        assert isinstance(typ, TupleT)
         assert isinstance(key, int)
         subtype = typ.member_types[key]
         attrs = list(typ.tuple_keys())
         index = key
         annotation = None
 
     # generated by empty() + make_setter
@@ -861,18 +873,72 @@
         return any(needs_clamp(m, encoding) for m in t.tuple_members())
     if t._is_prim_word:
         return t not in (INT256_T, UINT256_T, BYTES32_T)
 
     raise CompilerPanic("unreachable")  # pragma: nocover
 
 
+# when abi encoded data is user provided and lives in memory,
+# we risk either reading oob of the buffer or oob of the payload data.
+# in these cases, we need additional validation.
+def _dirty_read_risk(ir_node):
+    return ir_node.encoding == Encoding.ABI and ir_node.location == MEMORY
+
+
+# child elements which have dynamic length, and could overflow the buffer
+# even if the start of the item is in-bounds.
+def _abi_payload_size(ir_node):
+    SCALE = ir_node.location.word_scale
+    assert SCALE == 32  # we must be in some byte-addressable region, like memory
+
+    OFFSET = DYNAMIC_ARRAY_OVERHEAD * SCALE
+
+    if isinstance(ir_node.typ, DArrayT):
+        return ["add", OFFSET, ["mul", get_dyn_array_count(ir_node), SCALE]]
+
+    if isinstance(ir_node.typ, _BytestringT):
+        return ["add", OFFSET, get_bytearray_length(ir_node)]
+
+    raise CompilerPanic("unreachable")  # pragma: nocover
+
+
+def potential_overlap(left, right):
+    """
+    Return true if make_setter(left, right) could potentially trample
+    src or dst during evaluation.
+    """
+    if left.typ._is_prim_word and right.typ._is_prim_word:
+        return False
+
+    if len(left.referenced_variables & right.referenced_variables) > 0:
+        return True
+
+    if len(left.referenced_variables) > 0 and right.contains_risky_call:
+        return True
+
+    if left.contains_risky_call and len(right.referenced_variables) > 0:
+        return True
+
+    return False
+
+
 # Create an x=y statement, where the types may be compound
-def make_setter(left, right):
+def make_setter(left, right, hi=None):
     check_assign(left, right)
 
+    if potential_overlap(left, right):
+        raise CompilerPanic("overlap between src and dst!")
+
+    # we need bounds checks when decoding from memory, otherwise we can
+    # get oob reads.
+    #
+    # the caller is responsible for calculating the bound;
+    # sanity check that there is a bound if there is dirty read risk
+    assert (hi is not None) == _dirty_read_risk(right)
+
     # For types which occupy just one word we can use single load/store
     if left.typ._is_prim_word:
         enc = right.encoding  # unwrap_location butchers encoding
         right = unwrap_location(right)
         # TODO rethink/streamline the clamp_basetype logic
         if needs_clamp(right.typ, enc):
             right = clamp_basetype(right)
@@ -881,43 +947,52 @@
 
     # Byte arrays
     elif isinstance(left.typ, _BytestringT):
         # TODO rethink/streamline the clamp_basetype logic
         if needs_clamp(right.typ, right.encoding):
             with right.cache_when_complex("bs_ptr") as (b, right):
                 copier = make_byte_array_copier(left, right)
-                ret = b.resolve(["seq", clamp_bytestring(right), copier])
+                ret = b.resolve(["seq", clamp_bytestring(right, hi=hi), copier])
         else:
             ret = make_byte_array_copier(left, right)
 
         return IRnode.from_list(ret)
 
     elif isinstance(left.typ, DArrayT):
         # TODO should we enable this?
         # implicit conversion from sarray to darray
         # if isinstance(right.typ, SArrayType):
         #    return _complex_make_setter(left, right)
 
         # TODO rethink/streamline the clamp_basetype logic
         if needs_clamp(right.typ, right.encoding):
             with right.cache_when_complex("arr_ptr") as (b, right):
-                copier = _dynarray_make_setter(left, right)
-                ret = b.resolve(["seq", clamp_dyn_array(right), copier])
+                copier = _dynarray_make_setter(left, right, hi=hi)
+                ret = b.resolve(["seq", clamp_dyn_array(right, hi=hi), copier])
         else:
             ret = _dynarray_make_setter(left, right)
 
         return IRnode.from_list(ret)
 
     # Complex Types
     assert isinstance(left.typ, (SArrayT, TupleT, StructT))
 
-    return _complex_make_setter(left, right)
+    return _complex_make_setter(left, right, hi=hi)
+
 
+# locations with no dedicated copy opcode
+# (i.e. storage and transient storage)
+def copy_opcode_available(left, right):
+    if left.location == MEMORY and right.location == MEMORY:
+        return version_check(begin="cancun")
 
-def _complex_make_setter(left, right):
+    return left.location == MEMORY and right.location.has_copy_opcode
+
+
+def _complex_make_setter(left, right, hi=None):
     if right.value == "~empty" and left.location == MEMORY:
         # optimized memzero
         return mzero(left, left.typ.memory_bytes_required)
 
     ret = ["seq"]
 
     if isinstance(left.typ, SArrayT):
@@ -930,16 +1005,18 @@
 
     if left.is_pointer and right.is_pointer and right.encoding == Encoding.VYPER:
         # both left and right are pointers, see if we want to batch copy
         # instead of unrolling the loop.
         assert left.encoding == Encoding.VYPER
         len_ = left.typ.memory_bytes_required
 
-        has_storage = STORAGE in (left.location, right.location)
-        if has_storage:
+        # special logic for identity precompile (pre-cancun) in the else branch
+        mem2mem = left.location == right.location == MEMORY
+
+        if not copy_opcode_available(left, right) and not mem2mem:
             if _opt_codesize():
                 # assuming PUSH2, a single sstore(dst (sload src)) is 8 bytes,
                 # sstore(add (dst ofst), (sload (add (src ofst)))) is 16 bytes,
                 # whereas loop overhead is 16-17 bytes.
                 base_cost = 3
                 if left._optimized.is_literal:
                     # code size is smaller since add is performed at compile-time
@@ -978,34 +1055,35 @@
                 identity_base_cost = 115  # staticcall 4 gas dst len src len
 
                 n_words = ceil32(len_) // 32
                 should_batch_copy = (
                     base_unroll_cost + (nth_word_cost * (n_words - 1)) >= identity_base_cost
                 )
 
-            # calldata to memory, code to memory, cancun, or codesize -
+            # calldata to memory, code to memory, cancun, or opt-codesize -
             # batch copy is always better.
             else:
                 should_batch_copy = True
 
         if should_batch_copy:
             return copy_bytes(left, right, len_, len_)
 
     # general case, unroll
     with left.cache_when_complex("_L") as (b1, left), right.cache_when_complex("_R") as (b2, right):
         for k in keys:
             l_i = get_element_ptr(left, k, array_bounds_check=False)
             r_i = get_element_ptr(right, k, array_bounds_check=False)
-            ret.append(make_setter(l_i, r_i))
+            ret.append(make_setter(l_i, r_i, hi=hi))
 
         return b1.resolve(b2.resolve(IRnode.from_list(ret)))
 
 
 def ensure_in_memory(ir_var, context):
-    """Ensure a variable is in memory. This is useful for functions
+    """
+    Ensure a variable is in memory. This is useful for functions
     which expect to operate on memory variables.
     """
     if ir_var.location == MEMORY:
         return ir_var
 
     typ = ir_var.typ
     buf = IRnode.from_list(context.new_internal_variable(typ), typ=typ, location=MEMORY)
@@ -1063,27 +1141,55 @@
     return ["shl", bits, x]
 
 
 def sar(bits, x):
     return ["sar", bits, x]
 
 
-def clamp_bytestring(ir_node):
+def clamp_bytestring(ir_node, hi=None):
     t = ir_node.typ
     if not isinstance(t, _BytestringT):  # pragma: nocover
         raise CompilerPanic(f"{t} passed to clamp_bytestring")
-    ret = ["assert", ["le", get_bytearray_length(ir_node), t.maxlen]]
-    return IRnode.from_list(ret, error_msg=f"{ir_node.typ} bounds check")
 
+    # check if byte array length is within type max
+    with get_bytearray_length(ir_node).cache_when_complex("length") as (b1, length):
+        len_check = ["assert", ["le", length, t.maxlen]]
+
+        assert (hi is not None) == _dirty_read_risk(ir_node)
+        if hi is not None:
+            assert t.maxlen < 2**64  # sanity check
+
+            # note: this add does not risk arithmetic overflow because
+            # length is bounded by maxlen.
+            item_end = add_ofst(ir_node, _abi_payload_size(ir_node))
 
-def clamp_dyn_array(ir_node):
+            len_check = ["seq", ["assert", ["le", item_end, hi]], len_check]
+
+        return IRnode.from_list(b1.resolve(len_check), error_msg=f"{ir_node.typ} bounds check")
+
+
+def clamp_dyn_array(ir_node, hi=None):
     t = ir_node.typ
     assert isinstance(t, DArrayT)
-    ret = ["assert", ["le", get_dyn_array_count(ir_node), t.count]]
-    return IRnode.from_list(ret, error_msg=f"{ir_node.typ} bounds check")
+
+    len_check = ["assert", ["le", get_dyn_array_count(ir_node), t.count]]
+
+    assert (hi is not None) == _dirty_read_risk(ir_node)
+
+    # if the subtype is dynamic, the check will be performed in the recursion
+    if hi is not None and not t.abi_type.subtyp.is_dynamic():
+        assert t.count < 2**64  # sanity check
+
+        # note: this add does not risk arithmetic overflow because
+        # length is bounded by count * elemsize.
+        item_end = add_ofst(ir_node, _abi_payload_size(ir_node))
+
+        len_check = ["seq", ["assert", ["le", item_end, hi]], len_check]
+
+    return IRnode.from_list(len_check, error_msg=f"{ir_node.typ} bounds check")
 
 
 # clampers for basetype
 def clamp_basetype(ir_node):
     t = ir_node.typ
     if not t._is_prim_word:  # pragma: nocover
         raise CompilerPanic(f"{t} passed to clamp_basetype")
@@ -1189,7 +1295,19 @@
 
 def clamp2(lo, arg, hi, signed):
     with IRnode.from_list(arg).cache_when_complex("clamp2_arg") as (b1, arg):
         GE = "sge" if signed else "ge"
         LE = "sle" if signed else "le"
         ret = ["seq", ["assert", ["and", [GE, arg, lo], [LE, arg, hi]]], arg]
         return IRnode.from_list(b1.resolve(ret), typ=arg.typ)
+
+
+# make sure we don't overrun the source buffer, checking for overflow:
+# valid inputs satisfy:
+#   `assert !(start+length > src_len || start+length < start)`
+def check_buffer_overflow_ir(start, length, src_len):
+    with start.cache_when_complex("start") as (b1, start):
+        with add_ofst(start, length).cache_when_complex("end") as (b2, end):
+            arithmetic_overflow = ["lt", end, start]
+            buffer_oob = ["gt", end, src_len]
+            ok = ["iszero", ["or", arithmetic_overflow, buffer_oob]]
+            return b1.resolve(b2.resolve(["assert", ok]))
```

### Comparing `vyper-0.4.0rc5/vyper/codegen/events.py` & `vyper-0.4.0rc6/vyper/codegen/events.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/codegen/expr.py` & `vyper-0.4.0rc6/vyper/codegen/expr.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,17 @@
     get_dyn_array_count,
     get_element_ptr,
     is_array_like,
     is_bytes_m_type,
     is_flag_type,
     is_numeric_type,
     is_tuple_like,
+    make_setter,
     pop_dyn_array,
+    potential_overlap,
     sar,
     shl,
     shr,
     unwrap_location,
 )
 from vyper.codegen.ir_node import IRnode
 from vyper.codegen.keccak256_helper import keccak256_helper
@@ -161,41 +163,50 @@
     def parse_NameConstant(self):
         assert isinstance(self.expr.value, bool)
         val = int(self.expr.value)
         return IRnode.from_list(val, typ=BoolT())
 
     # Variable names
     def parse_Name(self):
-        if self.expr.id == "self":
+        varname = self.expr.id
+
+        if varname == "self":
             return IRnode.from_list(["address"], typ=AddressT())
-        elif self.expr.id in self.context.vars:
-            return self.context.lookup_var(self.expr.id).as_ir_node()
 
-        elif (varinfo := self.expr._expr_info.var_info) is not None:
-            if varinfo.is_constant:
-                return Expr.parse_value_expr(varinfo.decl_node.value, self.context)
+        varinfo = self.expr._expr_info.var_info
+        assert varinfo is not None
+
+        # local variable
+        if varname in self.context.vars:
+            ret = self.context.lookup_var(varname).as_ir_node()
+            ret._referenced_variables = {varinfo}
+            return ret
 
-            assert varinfo.is_immutable, "not an immutable!"
+        if varinfo.is_constant:
+            return Expr.parse_value_expr(varinfo.decl_node.value, self.context)
 
+        if varinfo.is_immutable:
             mutable = self.context.is_ctor_context
 
             location = data_location_to_address_space(
                 varinfo.location, self.context.is_ctor_context
             )
 
             ret = IRnode.from_list(
                 varinfo.position.position,
                 typ=varinfo.typ,
                 location=location,
-                annotation=self.expr.id,
+                annotation=varname,
                 mutable=mutable,
             )
             ret._referenced_variables = {varinfo}
             return ret
 
+        raise CompilerPanic("unreachable")  # pragma: nocover
+
     # x.y or x[5]
     def parse_Attribute(self):
         typ = self.expr._metadata["type"]
 
         # check if we have a flag constant, e.g.
         # [lib1].MyFlag.FOO
         if isinstance(typ, FlagT) and is_type_t(self.expr.value._metadata["type"], FlagT):
@@ -687,18 +698,28 @@
                 return_item = not self.is_stmt
                 return pop_dyn_array(darray, return_popped_item=return_item)
             elif self.expr.func.attr == "append":
                 (arg,) = args
                 check_assign(
                     dummy_node_for_type(darray.typ.value_type), dummy_node_for_type(arg.typ)
                 )
-                return append_dyn_array(darray, arg)
+
+                ret = ["seq"]
+                if potential_overlap(darray, arg):
+                    tmp = self.context.new_internal_variable(arg.typ)
+                    tmp = IRnode.from_list(tmp, typ=arg.typ, location=MEMORY)
+                    ret.append(make_setter(tmp, arg))
+                    arg = tmp
+
+                ret.append(append_dyn_array(darray, arg))
+                return IRnode.from_list(ret)
 
         assert isinstance(func_t, ContractFunctionT)
         assert func_t.is_internal or func_t.is_constructor
+
         return self_call.ir_for_self_call(self.expr, self.context)
 
     @classmethod
     def handle_external_call(cls, expr, context):
         # TODO fix cyclic import
         from vyper.builtins._signatures import BuiltinFunctionT
```

### Comparing `vyper-0.4.0rc5/vyper/codegen/external_call.py` & `vyper-0.4.0rc6/vyper/codegen/external_call.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,15 +115,22 @@
     assert isinstance(wrapped_return_t, TupleT)
 
     # unpack strictly
     if needs_clamp(wrapped_return_t, encoding):
         return_buf = context.new_internal_variable(wrapped_return_t)
 
         # note: make_setter does ABI decoding and clamps
-        unpacker.append(make_setter(return_buf, buf))
+
+        payload_bound = IRnode.from_list(
+            ["select", ["lt", ret_len, "returndatasize"], ret_len, "returndatasize"]
+        )
+        with payload_bound.cache_when_complex("payload_bound") as (b1, payload_bound):
+            unpacker.append(
+                b1.resolve(make_setter(return_buf, buf, hi=add_ofst(buf, payload_bound)))
+            )
     else:
         return_buf = buf
 
     if call_kwargs.default_return_value is not None:
         # if returndatasize == 0:
         #    copy return override to buf
         # else:
```

### Comparing `vyper-0.4.0rc5/vyper/codegen/function_definitions/common.py` & `vyper-0.4.0rc6/vyper/codegen/function_definitions/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 
 @dataclass
 class _FuncIRInfo:
     func_t: ContractFunctionT
     gas_estimate: Optional[int] = None
     frame_info: Optional[FrameInfo] = None
+    func_ir: Optional["InternalFuncIR"] = None
 
     @property
     def visibility(self):
         return "internal" if self.func_t.is_internal else "external"
 
     @property
     def exit_sequence_label(self) -> str:
@@ -52,14 +53,18 @@
     def set_frame_info(self, frame_info: FrameInfo) -> None:
         # XXX: when can this happen?
         if self.frame_info is not None:
             assert frame_info == self.frame_info
         else:
             self.frame_info = frame_info
 
+    def set_func_ir(self, func_ir: "InternalFuncIR") -> None:
+        assert self.func_t.is_internal or self.func_t.is_deploy
+        self.func_ir = func_ir
+
     @property
     # common entry point for external function with kwargs
     def external_function_base_entry_label(self) -> str:
         assert not self.func_t.is_internal, "uh oh, should be external"
         return self.ir_identifier + "_common"
 
     def internal_function_label(self, is_ctor_context: bool = False) -> str:
```

### Comparing `vyper-0.4.0rc5/vyper/codegen/function_definitions/external_function.py` & `vyper-0.4.0rc6/vyper/codegen/function_definitions/external_function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/codegen/function_definitions/internal_function.py` & `vyper-0.4.0rc6/vyper/codegen/function_definitions/internal_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,8 +78,11 @@
 
     ir_node = IRnode.from_list(["seq", body, cleanup_routine])
 
     # tag gas estimate and frame info
     func_t._ir_info.gas_estimate = ir_node.gas
     tag_frame_info(func_t, context)
 
-    return InternalFuncIR(ir_node)
+    ret = InternalFuncIR(ir_node)
+    func_t._ir_info.func_ir = ret
+
+    return ret
```

### Comparing `vyper-0.4.0rc5/vyper/codegen/ir_node.py` & `vyper-0.4.0rc6/vyper/codegen/ir_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,19 +452,33 @@
         # TODO this could really be moved into optimizer.py
         should_inline = not self._optimized.is_complex_ir
 
         return _WithBuilder(self, name, should_inline)
 
     @cached_property
     def referenced_variables(self):
-        ret = set()
+        ret = getattr(self, "_referenced_variables", set())
+
         for arg in self.args:
             ret |= arg.referenced_variables
 
-        ret |= getattr(self, "_referenced_variables", set())
+        if getattr(self, "is_self_call", False):
+            ret |= self.invoked_function_ir.func_ir.referenced_variables
+
+        return ret
+
+    @cached_property
+    def contains_risky_call(self):
+        ret = self.value in ("call", "delegatecall", "create", "create2")
+
+        for arg in self.args:
+            ret |= arg.contains_risky_call
+
+        if getattr(self, "is_self_call", False):
+            ret |= self.invoked_function_ir.func_ir.contains_risky_call
 
         return ret
 
     @cached_property
     def contains_self_call(self):
         return getattr(self, "is_self_call", False) or any(x.contains_self_call for x in self.args)
```

### Comparing `vyper-0.4.0rc5/vyper/codegen/jumptable_utils.py` & `vyper-0.4.0rc6/vyper/codegen/jumptable_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/codegen/keccak256_helper.py` & `vyper-0.4.0rc6/vyper/codegen/keccak256_helper.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/codegen/memory_allocator.py` & `vyper-0.4.0rc6/vyper/codegen/memory_allocator.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/codegen/module.py` & `vyper-0.4.0rc6/vyper/codegen/module.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/codegen/return_.py` & `vyper-0.4.0rc6/vyper/codegen/return_.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/codegen/self_call.py` & `vyper-0.4.0rc6/vyper/codegen/self_call.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,8 +106,9 @@
         call_sequence,
         typ=func_t.return_type,
         location=MEMORY,
         annotation=stmt_expr.get("node_source_code"),
         add_gas_estimate=func_t._ir_info.gas_estimate,
     )
     o.is_self_call = True
+    o.invoked_function_ir = func_t._ir_info.func_ir
     return o
```

### Comparing `vyper-0.4.0rc5/vyper/codegen/stmt.py` & `vyper-0.4.0rc6/vyper/codegen/stmt.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,21 @@
     IRnode,
     add_ofst,
     clamp_le,
     get_dyn_array_count,
     get_element_ptr,
     get_type_for_exact_size,
     make_setter,
+    potential_overlap,
     wrap_value_for_external_return,
+    writeable,
 )
 from vyper.codegen.expr import Expr
 from vyper.codegen.return_ import make_return_stmt
-from vyper.evm.address_space import MEMORY, STORAGE
+from vyper.evm.address_space import MEMORY
 from vyper.exceptions import CodegenPanic, StructureException, TypeCheckFailure, tag_exceptions
 from vyper.semantics.types import DArrayT
 from vyper.semantics.types.shortcuts import UINT256_T
 
 
 class Stmt:
     def __init__(self, node: vy_ast.VyperNode, context: Context) -> None:
@@ -65,16 +67,15 @@
 
     def parse_Assign(self):
         # Assignment (e.g. x[4] = y)
         src = Expr(self.stmt.value, self.context).ir_node
         dst = self._get_target(self.stmt.target)
 
         ret = ["seq"]
-        overlap = len(dst.referenced_variables & src.referenced_variables) > 0
-        if overlap and not dst.typ._is_prim_word:
+        if potential_overlap(dst, src):
             # there is overlap between the lhs and rhs, and the type is
             # complex - i.e., it spans multiple words. for safety, we
             # copy to a temporary buffer before copying to the destination.
             tmp = self.context.new_internal_variable(src.typ)
             tmp = IRnode.from_list(tmp, typ=src.typ, location=MEMORY)
             ret.append(make_setter(tmp, src))
             src = tmp
@@ -195,52 +196,51 @@
             kwargs = {
                 s.arg: Expr.parse_value_expr(s.value, self.context) for s in range_call.keywords
             }
 
         # sanity check that the following `end - start` is a valid operation
         assert start.typ == end.typ == target_type
 
-        if "bound" in kwargs:
-            with end.cache_when_complex("end") as (b1, end):
-                # note: the check for rounds<=rounds_bound happens in asm
-                # generation for `repeat`.
-                clamped_start = clamp_le(start, end, target_type.is_signed)
-                rounds = b1.resolve(IRnode.from_list(["sub", end, clamped_start]))
-            rounds_bound = kwargs.pop("bound").int_value()
-        else:
-            rounds = end.int_value() - start.int_value()
-            rounds_bound = rounds
-
-        assert len(kwargs) == 0  # sanity check stray keywords
-
-        if rounds_bound < 1:  # pragma: nocover
-            raise TypeCheckFailure("unreachable: unchecked 0 bound")
-
-        varname = self.stmt.target.target.id
-        i = IRnode.from_list(self.context.fresh_varname("range_ix"), typ=target_type)
-        iptr = self.context.new_variable(varname, target_type)
+        with start.cache_when_complex("start") as (b1, start):
+            if "bound" in kwargs:
+                with end.cache_when_complex("end") as (b2, end):
+                    # note: the check for rounds<=rounds_bound happens in asm
+                    # generation for `repeat`.
+                    clamped_start = clamp_le(start, end, target_type.is_signed)
+                    rounds = b2.resolve(IRnode.from_list(["sub", end, clamped_start]))
+                rounds_bound = kwargs.pop("bound").int_value()
+            else:
+                rounds = end.int_value() - start.int_value()
+                rounds_bound = rounds
 
-        self.context.forvars[varname] = True
+            assert len(kwargs) == 0  # sanity check stray keywords
 
-        loop_body = ["seq"]
-        # store the current value of i so it is accessible to userland
-        loop_body.append(["mstore", iptr, i])
-        loop_body.append(parse_body(self.stmt.body, self.context))
-
-        # NOTE: codegen for `repeat` inserts an assertion that
-        # (gt rounds_bound rounds). note this also covers the case where
-        # rounds < 0.
-        # if we ever want to remove that, we need to manually add the assertion
-        # where it makes sense.
-        ir_node = IRnode.from_list(
-            ["repeat", i, start, rounds, rounds_bound, loop_body], error_msg="range() bounds check"
-        )
-        del self.context.forvars[varname]
+            if rounds_bound < 1:  # pragma: nocover
+                raise TypeCheckFailure("unreachable: unchecked 0 bound")
 
-        return ir_node
+            varname = self.stmt.target.target.id
+            i = IRnode.from_list(self.context.fresh_varname("range_ix"), typ=target_type)
+            iptr = self.context.new_variable(varname, target_type)
+
+            self.context.forvars[varname] = True
+
+            loop_body = ["seq"]
+            # store the current value of i so it is accessible to userland
+            loop_body.append(["mstore", iptr, i])
+            loop_body.append(parse_body(self.stmt.body, self.context))
+
+            del self.context.forvars[varname]
+
+            # NOTE: codegen for `repeat` inserts an assertion that
+            # (gt rounds_bound rounds). note this also covers the case where
+            # rounds < 0.
+            # if we ever want to remove that, we need to manually add the assertion
+            # where it makes sense.
+            loop = ["repeat", i, start, rounds, rounds_bound, loop_body]
+            return b1.resolve(IRnode.from_list(loop, error_msg="range() bounds check"))
 
     def _parse_For_list(self):
         with self.context.range_scope():
             iter_list = Expr(self.stmt.iter, self.context).ir_node
 
         target_type = self.stmt.target.target._metadata["type"]
         assert target_type == iter_list.typ.value_type
@@ -308,26 +308,26 @@
         if self.stmt.value is not None:
             ir_val = Expr(self.stmt.value, self.context).ir_node
         return make_return_stmt(ir_val, self.stmt, self.context)
 
     def _get_target(self, target):
         _dbg_expr = target
 
-        if isinstance(target, vy_ast.Name) and target.id in self.context.forvars:
+        if isinstance(target, vy_ast.Name) and target.id in self.context.forvars:  # pragma: nocover
             raise TypeCheckFailure(f"Failed constancy check\n{_dbg_expr}")
 
         if isinstance(target, vy_ast.Tuple):
             target = Expr(target, self.context).ir_node
-            for node in target.args:
-                if (node.location == STORAGE and self.context.is_constant()) or not node.mutable:
-                    raise TypeCheckFailure(f"Failed constancy check\n{_dbg_expr}")
+            items = target.args
+            if any(not writeable(self.context, item) for item in items):  # pragma: nocover
+                raise TypeCheckFailure(f"Failed constancy check\n{_dbg_expr}")
             return target
 
         target = Expr.parse_pointer_expr(target, self.context)
-        if (target.location == STORAGE and self.context.is_constant()) or not target.mutable:
+        if not writeable(self.context, target):  # pragma: nocover
             raise TypeCheckFailure(f"Failed constancy check\n{_dbg_expr}")
         return target
 
 
 # Parse a statement (usually one line of code but not always)
 def parse_stmt(stmt, context):
     return Stmt(stmt, context).ir_node
```

### Comparing `vyper-0.4.0rc5/vyper/compiler/README.md` & `vyper-0.4.0rc6/vyper/compiler/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/compiler/__init__.py` & `vyper-0.4.0rc6/vyper/compiler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
     """
     settings = settings or get_global_settings() or Settings()
 
     if output_formats is None:
         output_formats = ("bytecode",)
 
     # make IR output the same between runs
+    # TODO: move this to CompilerData.__init__()
     codegen.reset_names()
 
     compiler_data = CompilerData(
         file_input,
         input_bundle,
         settings=settings,
         integrity_sum=integrity_sum,
```

### Comparing `vyper-0.4.0rc5/vyper/compiler/input_bundle.py` & `vyper-0.4.0rc6/vyper/compiler/input_bundle.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/compiler/output.py` & `vyper-0.4.0rc6/vyper/compiler/output.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/compiler/output_bundle.py` & `vyper-0.4.0rc6/vyper/compiler/output_bundle.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/compiler/phases.py` & `vyper-0.4.0rc6/vyper/compiler/phases.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from vyper.ast import natspec
 from vyper.codegen import module
 from vyper.codegen.ir_node import IRnode
 from vyper.compiler.input_bundle import FileInput, FilesystemInputBundle, InputBundle
 from vyper.compiler.settings import OptimizationLevel, Settings, anchor_settings, merge_settings
 from vyper.ir import compile_ir, optimizer
 from vyper.semantics import analyze_module, set_data_positions, validate_compilation_target
+from vyper.semantics.analysis.data_positions import generate_layout_export
 from vyper.semantics.types.function import ContractFunctionT
 from vyper.semantics.types.module import ModuleT
 from vyper.typing import StorageLayout
 from vyper.utils import ERC5202_PREFIX, vyper_warn
 from vyper.venom import generate_assembly_experimental, generate_ir
 
 DEFAULT_CONTRACT_PATH = PurePath("VyperContract.vy")
@@ -89,14 +90,17 @@
         self.storage_layout_override = storage_layout
         self.show_gas_estimates = show_gas_estimates
         self.no_bytecode_metadata = no_bytecode_metadata
         self.original_settings = settings
         self.input_bundle = input_bundle or FilesystemInputBundle([Path(".")])
         self.expected_integrity_sum = integrity_sum
 
+        # ast cache, hitchhike onto the input_bundle object
+        self.input_bundle._cache._ast_of: dict[int, vy_ast.Module] = {}  # type: ignore
+
     @cached_property
     def source_code(self):
         return self.file_input.source_code
 
     @cached_property
     def source_id(self):
         return self.file_input.source_id
@@ -176,15 +180,17 @@
 
         validate_compilation_target(module_t)
         return self.annotated_vyper_module
 
     @cached_property
     def storage_layout(self) -> StorageLayout:
         module_ast = self.compilation_target
-        return set_data_positions(module_ast, self.storage_layout_override)
+        set_data_positions(module_ast, self.storage_layout_override)
+
+        return generate_layout_export(module_ast)
 
     @property
     def global_ctx(self) -> ModuleT:
         # ensure storage layout is computed
         _ = self.storage_layout
         # ensure natspec is computed
         _ = self.natspec
```

### Comparing `vyper-0.4.0rc5/vyper/compiler/settings.py` & `vyper-0.4.0rc6/vyper/compiler/settings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/compiler/utils.py` & `vyper-0.4.0rc6/vyper/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/evm/address_space.py` & `vyper-0.4.0rc6/vyper/evm/address_space.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,39 +16,50 @@
         name: human-readable nickname for the address space
         word_scale: a constant which helps calculate offsets in a given
             address space. 1 for word-addressable locations (storage),
             32 for byte-addressable locations (memory, calldata, code)
         load_op: the opcode for loading a word from this address space
         store_op: the opcode for storing a word to this address space
             (an address space is read-only if store_op is None)
+        copy_op: the opcode for batch-copying from this address space
+            to memory
     """
 
     name: str
     word_scale: int
     load_op: str
     # TODO maybe make positional instead of defaulting to None
     store_op: Optional[str] = None
+    copy_op: Optional[str] = None
 
     @property
     def word_addressable(self) -> bool:
         return self.word_scale == 1
 
+    @property
+    def has_copy_opcode(self):
+        return self.copy_op is not None
+
 
 # alternative:
 # class Memory(AddrSpace):
 #   @property
 #   def word_scale(self):
 #     return 32
 # # implement more properties...
 #
 # MEMORY = Memory()
 
-MEMORY = AddrSpace("memory", 32, "mload", "mstore")
+MEMORY = AddrSpace("memory", 32, "mload", "mstore", "mcopy")
 STORAGE = AddrSpace("storage", 1, "sload", "sstore")
 TRANSIENT = AddrSpace("transient", 1, "tload", "tstore")
-CALLDATA = AddrSpace("calldata", 32, "calldataload")
+CALLDATA = AddrSpace("calldata", 32, "calldataload", None, "calldatacopy")
 # immutables address space: "immutables" section of memory
 # which is read-write in deploy code but then gets turned into
 # the "data" section of the runtime code
 IMMUTABLES = AddrSpace("immutables", 32, "iload", "istore")
 # data addrspace: "data" section of runtime code, read-only.
-DATA = AddrSpace("data", 32, "dload")
+DATA = AddrSpace("data", 32, "dload", None, "dloadbytes")
+
+
+def legal_in_staticcall(location: AddrSpace):
+    return location not in (STORAGE, TRANSIENT)
```

### Comparing `vyper-0.4.0rc5/vyper/evm/opcodes.py` & `vyper-0.4.0rc6/vyper/evm/opcodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/exceptions.py` & `vyper-0.4.0rc6/vyper/exceptions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/ir/README.md` & `vyper-0.4.0rc6/vyper/ir/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/ir/compile_ir.py` & `vyper-0.4.0rc6/vyper/ir/compile_ir.py`

 * *Files 0% similar despite different names*

```diff
@@ -576,15 +576,17 @@
                 "SHA3",
             ]
         )
         return o
     # SHA3 a 64 byte value
     elif code.value == "sha3_64":
         o = _compile_to_assembly(code.args[0], withargs, existing_labels, break_dest, height)
-        o.extend(_compile_to_assembly(code.args[1], withargs, existing_labels, break_dest, height))
+        o.extend(
+            _compile_to_assembly(code.args[1], withargs, existing_labels, break_dest, height + 1)
+        )
         o.extend(
             [
                 *PUSH(MemoryPositions.FREE_VAR_SPACE2),
                 "MSTORE",
                 *PUSH(MemoryPositions.FREE_VAR_SPACE),
                 "MSTORE",
                 *PUSH(64),
```

### Comparing `vyper-0.4.0rc5/vyper/ir/optimizer.py` & `vyper-0.4.0rc6/vyper/ir/optimizer.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/ir/s_expressions.py` & `vyper-0.4.0rc6/vyper/ir/s_expressions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/README.md` & `vyper-0.4.0rc6/vyper/semantics/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/analysis/base.py` & `vyper-0.4.0rc6/vyper/semantics/analysis/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,28 +190,32 @@
         assert self.decl_node is not None  # help mypy
         ret = self.decl_node._expanded_getter
         assert (ret is not None) == self.is_public, self
         return ret
 
     def set_position(self, position: VarOffset) -> None:
         if self.position is not None:
-            raise CompilerPanic("Position was already assigned")
+            raise CompilerPanic(f"Position was already assigned: {self}")
         assert isinstance(position, VarOffset)  # sanity check
         self.position = position
 
     def is_state_variable(self):
         non_state_locations = (DataLocation.UNSET, DataLocation.MEMORY, DataLocation.CALLDATA)
         # `self` gets a VarInfo, but it is not considered a state
         # variable (it is magic), so we ignore it here.
         return self.location not in non_state_locations and not isinstance(self.typ, SelfT)
 
     def get_size(self) -> int:
         return self.typ.get_size_in(self.location)
 
     @property
+    def is_storage(self):
+        return self.location == DataLocation.STORAGE
+
+    @property
     def is_transient(self):
         return self.location == DataLocation.TRANSIENT
 
     @property
     def is_immutable(self):
         return self.location == DataLocation.CODE
```

### Comparing `vyper-0.4.0rc5/vyper/semantics/analysis/common.py` & `vyper-0.4.0rc6/vyper/semantics/analysis/common.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/analysis/constant_folding.py` & `vyper-0.4.0rc6/vyper/semantics/analysis/constant_folding.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/analysis/data_positions.py` & `vyper-0.4.0rc6/vyper/semantics/analysis/data_positions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,45 @@
+import json
 from collections import defaultdict
-from typing import Generic, TypeVar
+from typing import Generic, Optional, TypeVar
 
 from vyper import ast as vy_ast
 from vyper.evm.opcodes import version_check
 from vyper.exceptions import CompilerPanic, StorageLayoutException
 from vyper.semantics.analysis.base import VarOffset
 from vyper.semantics.data_locations import DataLocation
 from vyper.typing import StorageLayout
 
 
 def set_data_positions(
     vyper_module: vy_ast.Module, storage_layout_overrides: StorageLayout = None
-) -> StorageLayout:
+) -> None:
     """
     Parse the annotated Vyper AST, determine data positions for all variables,
     and annotate the AST nodes with the position data.
 
     Arguments
     ---------
     vyper_module : vy_ast.Module
         Top-level Vyper AST node that has already been annotated with type data.
     """
     if storage_layout_overrides is not None:
-        # extract code layout with no overrides
-        code_offsets = _allocate_layout_r(vyper_module, immutables_only=True)["code_layout"]
-        storage_slots = set_storage_slots_with_overrides(vyper_module, storage_layout_overrides)
-        return {"storage_layout": storage_slots, "code_layout": code_offsets}
-
-    ret = _allocate_layout_r(vyper_module)
-    assert isinstance(ret, defaultdict)
-    return dict(ret)  # convert back to dict
+        # allocate code layout with no overrides
+        _allocate_layout_r(vyper_module, no_storage=True)
+        _allocate_with_overrides(vyper_module, storage_layout_overrides)
+
+        # sanity check that generated layout file is the same as the input.
+        roundtrip = generate_layout_export(vyper_module).get(_LAYOUT_KEYS[DataLocation.STORAGE], {})
+        if roundtrip != storage_layout_overrides:
+            msg = "Computed storage layout does not match override file!\n"
+            msg += f"expected: {json.dumps(storage_layout_overrides)}\n\n"
+            msg += f"got:\n{json.dumps(roundtrip)}"
+            raise CompilerPanic(msg)
+    else:
+        _allocate_layout_r(vyper_module)
 
 
 _T = TypeVar("_T")
 _K = TypeVar("_K")
 
 
 class InsertableOnceDict(Generic[_T, _K], dict[_T, _K]):
@@ -41,37 +47,38 @@
         if k in self:
             raise ValueError(f"{k} is already in dict!")
         super().__setitem__(k, v)
 
 
 # some name that the user cannot assign to a variable
 GLOBAL_NONREENTRANT_KEY = "$.nonreentrant_key"
+NONREENTRANT_KEY_SIZE = 1
 
 
 class SimpleAllocator:
     def __init__(self, max_slot: int = 2**256, starting_slot: int = 0):
         # Allocate storage slots from 0
         # note storage is word-addressable, not byte-addressable
         self._starting_slot = starting_slot
         self._slot = starting_slot
         self._max_slot = max_slot
 
-    def allocate_slot(self, n, var_name, node=None):
+    def allocate_slot(self, n, node=None):
         ret = self._slot
         if self._slot + n >= self._max_slot:
             raise StorageLayoutException(
                 f"Invalid storage slot, tried to allocate"
                 f" slots {self._slot} through {self._slot + n}",
                 node,
             )
         self._slot += n
         return ret
 
     def allocate_global_nonreentrancy_slot(self):
-        slot = self.allocate_slot(1, GLOBAL_NONREENTRANT_KEY)
+        slot = self.allocate_slot(NONREENTRANT_KEY_SIZE)
         assert slot == self._starting_slot
         return slot
 
 
 class Allocators:
     storage_allocator: SimpleAllocator
     transient_storage_allocator: SimpleAllocator
@@ -137,82 +144,113 @@
             raise StorageLayoutException(
                 f"Storage collision! Tried to assign '{var_name}' to slot {slot} but it has "
                 f"already been reserved by '{collided_var}'"
             )
         self.occupied_slots[slot] = var_name
 
 
-def set_storage_slots_with_overrides(
-    vyper_module: vy_ast.Module, storage_layout_overrides: StorageLayout
-) -> StorageLayout:
+def _fetch_path(path: list[str], layout: StorageLayout, node: vy_ast.VyperNode):
+    tmp = layout
+    qualified_path = ".".join(path)
+
+    for segment in path:
+        if segment not in tmp:
+            raise StorageLayoutException(
+                f"Could not find storage slot for {qualified_path}. "
+                "Have you used the correct storage layout file?",
+                node,
+            )
+        tmp = tmp[segment]
+
+    try:
+        ret = tmp["slot"]
+    except KeyError as e:
+        raise StorageLayoutException(f"no storage slot for {qualified_path}", node) from e
+
+    return ret
+
+
+def _allocate_with_overrides(vyper_module: vy_ast.Module, layout: StorageLayout):
     """
     Set storage layout given a layout override file.
-    Returns the layout as a dict of variable name -> variable info
-    (Doesn't handle modules, or transient storage)
     """
-    ret: InsertableOnceDict[str, dict] = InsertableOnceDict()
-    reserved_slots = OverridingStorageAllocator()
+    allocator = OverridingStorageAllocator()
 
+    nonreentrant_slot = None
+    if GLOBAL_NONREENTRANT_KEY in layout:
+        nonreentrant_slot = layout[GLOBAL_NONREENTRANT_KEY]["slot"]
+
+    _allocate_with_overrides_r(vyper_module, layout, allocator, nonreentrant_slot, [])
+
+
+def _allocate_with_overrides_r(
+    vyper_module: vy_ast.Module,
+    layout: StorageLayout,
+    allocator: OverridingStorageAllocator,
+    global_nonreentrant_slot: Optional[int],
+    path: list[str],
+):
     # Search through function definitions to find non-reentrant functions
     for node in vyper_module.get_children(vy_ast.FunctionDef):
-        type_ = node._metadata["func_type"]
+        fn_t = node._metadata["func_type"]
 
         # Ignore functions without non-reentrant
-        if not type_.nonreentrant:
+        if not fn_t.nonreentrant:
             continue
 
-        variable_name = GLOBAL_NONREENTRANT_KEY
-
-        # re-entrant key was already identified
-        if variable_name in ret:
+        # if reentrancy keys get allocated in transient storage, we don't
+        # override them
+        if get_reentrancy_key_location() == DataLocation.TRANSIENT:
             continue
 
         # Expect to find this variable within the storage layout override
-        if variable_name in storage_layout_overrides:
-            reentrant_slot = storage_layout_overrides[variable_name]["slot"]
-            # Ensure that this slot has not been used, and prevents other storage variables
-            # from using the same slot
-            reserved_slots.reserve_slot_range(reentrant_slot, 1, variable_name)
-
-            type_.set_reentrancy_key_position(VarOffset(reentrant_slot))
-
-            ret[variable_name] = {"type": "nonreentrant lock", "slot": reentrant_slot}
-        else:
+        if global_nonreentrant_slot is None:
             raise StorageLayoutException(
-                f"Could not find storage_slot for {variable_name}. "
+                f"Could not find storage slot for {GLOBAL_NONREENTRANT_KEY}. "
                 "Have you used the correct storage layout file?",
                 node,
             )
 
-    # Iterate through variables
-    for node in vyper_module.get_children(vy_ast.VariableDecl):
-        # Ignore immutable parameters
-        if node.get("annotation.func.id") == "immutable":
-            continue
+        # prevent other storage variables from using the same slot
+        if allocator.occupied_slots.get(global_nonreentrant_slot) != GLOBAL_NONREENTRANT_KEY:
+            allocator.reserve_slot_range(
+                global_nonreentrant_slot, NONREENTRANT_KEY_SIZE, GLOBAL_NONREENTRANT_KEY
+            )
 
-        varinfo = node.target._metadata["varinfo"]
+        fn_t.set_reentrancy_key_position(VarOffset(global_nonreentrant_slot))
 
-        # Expect to find this variable within the storage layout overrides
-        if node.target.id in storage_layout_overrides:
-            var_slot = storage_layout_overrides[node.target.id]["slot"]
-            storage_length = varinfo.typ.storage_size_in_words
-            # Ensure that all required storage slots are reserved, and prevents other variables
-            # from using these slots
-            reserved_slots.reserve_slot_range(var_slot, storage_length, node.target.id)
-            varinfo.set_position(VarOffset(var_slot))
+    for node in _get_allocatable(vyper_module):
+        if isinstance(node, vy_ast.InitializesDecl):
+            module_info = node._metadata["initializes_info"].module_info
 
-            ret[node.target.id] = {"type": str(varinfo.typ), "slot": var_slot}
-        else:
-            raise StorageLayoutException(
-                f"Could not find storage_slot for {node.target.id}. "
-                "Have you used the correct storage layout file?",
-                node,
+            sub_path = [*path, module_info.alias]
+            _allocate_with_overrides_r(
+                module_info.module_node, layout, allocator, global_nonreentrant_slot, sub_path
             )
+            continue
 
-    return ret
+        # Iterate through variables
+        # Ignore immutables and transient variables
+        varinfo = node.target._metadata["varinfo"]
+
+        if not varinfo.is_storage:
+            continue
+
+        # Expect to find this variable within the storage layout overrides
+        varname = node.target.id
+        varpath = [*path, varname]
+        qualified_varname = ".".join(varpath)
+
+        var_slot = _fetch_path(varpath, layout, node)
+
+        storage_length = varinfo.typ.storage_size_in_words
+        # Ensure that all required storage slots are reserved, and
+        # prevent other variables from using these slots
+        allocator.reserve_slot_range(var_slot, storage_length, qualified_varname)
+        varinfo.set_position(VarOffset(var_slot))
 
 
 def _get_allocatable(vyper_module: vy_ast.Module) -> list[vy_ast.VyperNode]:
     allocable = (vy_ast.InitializesDecl, vy_ast.VariableDecl)
     return [node for node in vyper_module.body if isinstance(node, allocable)]
 
 
@@ -225,92 +263,135 @@
 _LAYOUT_KEYS = {
     DataLocation.CODE: "code_layout",
     DataLocation.TRANSIENT: "transient_storage_layout",
     DataLocation.STORAGE: "storage_layout",
 }
 
 
-def _allocate_nonreentrant_keys(vyper_module, allocators):
+def _set_nonreentrant_keys(vyper_module, allocators):
     SLOT = allocators.get_global_nonreentrant_key_slot()
 
     for node in vyper_module.get_children(vy_ast.FunctionDef):
         type_ = node._metadata["func_type"]
         if not type_.nonreentrant:
             continue
 
         # a nonreentrant key can appear many times in a module but it
         # only takes one slot. after the first time we see it, do not
         # increment the storage slot.
         type_.set_reentrancy_key_position(VarOffset(SLOT))
 
 
 def _allocate_layout_r(
-    vyper_module: vy_ast.Module, allocators: Allocators = None, immutables_only=False
-) -> StorageLayout:
+    vyper_module: vy_ast.Module, allocators: Allocators = None, no_storage=False
+):
     """
     Parse module-level Vyper AST to calculate the layout of storage variables.
     Returns the layout as a dict of variable name -> variable info
     """
-    global_ = False
     if allocators is None:
-        global_ = True
         allocators = Allocators()
         # always allocate nonreentrancy slot, so that adding or removing
         # reentrancy protection from a contract does not change its layout
         allocators.allocate_global_nonreentrancy_slot()
 
-    ret: defaultdict[str, InsertableOnceDict[str, dict]] = defaultdict(InsertableOnceDict)
-
     # tag functions with the global nonreentrant key
-    if not immutables_only:
-        _allocate_nonreentrant_keys(vyper_module, allocators)
-
-        layout_key = _LAYOUT_KEYS[get_reentrancy_key_location()]
-        # TODO this could have better typing but leave it untyped until
-        # we nail down the format better
-        if global_ and GLOBAL_NONREENTRANT_KEY not in ret[layout_key]:
-            slot = allocators.get_global_nonreentrant_key_slot()
-            ret[layout_key][GLOBAL_NONREENTRANT_KEY] = {"type": "nonreentrant lock", "slot": slot}
+    if not no_storage or get_reentrancy_key_location() == DataLocation.TRANSIENT:
+        _set_nonreentrant_keys(vyper_module, allocators)
 
     for node in _get_allocatable(vyper_module):
         if isinstance(node, vy_ast.InitializesDecl):
             module_info = node._metadata["initializes_info"].module_info
-            module_layout = _allocate_layout_r(module_info.module_node, allocators)
-            module_alias = module_info.alias
-            for layout_key in module_layout.keys():
-                assert layout_key in _LAYOUT_KEYS.values()
-                ret[layout_key][module_alias] = module_layout[layout_key]
+            _allocate_layout_r(module_info.module_node, allocators, no_storage)
             continue
 
         assert isinstance(node, vy_ast.VariableDecl)
-        # skip non-state variables
         varinfo = node.target._metadata["varinfo"]
+
+        # skip things we don't need to allocate, like constants
         if not varinfo.is_state_variable():
             continue
-        location = varinfo.location
 
-        if immutables_only and location != DataLocation.CODE:
+        if no_storage and varinfo.is_storage:
             continue
 
-        allocator = allocators.get_allocator(location)
+        allocator = allocators.get_allocator(varinfo.location)
         size = varinfo.get_size()
 
         # CMC 2021-07-23 note that HashMaps get assigned a slot here
         # using the same allocator (even though there is not really
         # any risk of physical overlap)
-        offset = allocator.allocate_slot(size, node.target.id, node)
-
+        offset = allocator.allocate_slot(size, node)
         varinfo.set_position(VarOffset(offset))
 
+
+# get the layout for export
+def generate_layout_export(vyper_module: vy_ast.Module):
+    return _generate_layout_export_r(vyper_module)
+
+
+def _generate_layout_export_r(vyper_module):
+    ret: defaultdict[str, InsertableOnceDict[str, dict]] = defaultdict(InsertableOnceDict)
+
+    for node in _get_allocatable(vyper_module):
+        if isinstance(node, vy_ast.InitializesDecl):
+            module_info = node._metadata["initializes_info"].module_info
+            module_layout = _generate_layout_export_r(module_info.module_node)
+            module_alias = module_info.alias
+            for layout_key in module_layout.keys():
+                assert layout_key in _LAYOUT_KEYS.values()
+
+                # lift the nonreentrancy key (if any) into the outer dict
+                # note that lifting can leave the inner dict empty, which
+                # should be filtered (below) for cleanliness
+                nonreentrant = module_layout[layout_key].pop(GLOBAL_NONREENTRANT_KEY, None)
+                if nonreentrant is not None and GLOBAL_NONREENTRANT_KEY not in ret[layout_key]:
+                    ret[layout_key][GLOBAL_NONREENTRANT_KEY] = nonreentrant
+
+                # add the module as a nested dict, but only if it is non-empty
+                if len(module_layout[layout_key]) != 0:
+                    ret[layout_key][module_alias] = module_layout[layout_key]
+
+            continue
+
+        assert isinstance(node, vy_ast.VariableDecl)
+        varinfo = node.target._metadata["varinfo"]
+        # skip non-state variables
+        if not varinfo.is_state_variable():
+            continue
+
+        location = varinfo.location
         layout_key = _LAYOUT_KEYS[location]
         type_ = varinfo.typ
+        size = varinfo.get_size()
+        offset = varinfo.position.position
+
         # this could have better typing but leave it untyped until
         # we understand the use case better
         if location == DataLocation.CODE:
             item = {"type": str(type_), "length": size, "offset": offset}
         elif location in (DataLocation.STORAGE, DataLocation.TRANSIENT):
-            item = {"type": str(type_), "slot": offset}
+            item = {"type": str(type_), "n_slots": size, "slot": offset}
         else:  # pragma: nocover
             raise CompilerPanic("unreachable")
         ret[layout_key][node.target.id] = item
 
+    for fn in vyper_module.get_children(vy_ast.FunctionDef):
+        fn_t = fn._metadata["func_type"]
+        if not fn_t.nonreentrant:
+            continue
+
+        location = get_reentrancy_key_location()
+        layout_key = _LAYOUT_KEYS[location]
+
+        if GLOBAL_NONREENTRANT_KEY in ret[layout_key]:
+            break
+
+        slot = fn_t.reentrancy_key_position.position
+        ret[layout_key][GLOBAL_NONREENTRANT_KEY] = {
+            "type": "nonreentrant lock",
+            "slot": slot,
+            "n_slots": NONREENTRANT_KEY_SIZE,
+        }
+        break
+
     return ret
```

### Comparing `vyper-0.4.0rc5/vyper/semantics/analysis/getters.py` & `vyper-0.4.0rc6/vyper/semantics/analysis/getters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/analysis/global_.py` & `vyper-0.4.0rc6/vyper/semantics/analysis/global_.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/analysis/import_graph.py` & `vyper-0.4.0rc6/vyper/semantics/analysis/import_graph.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/analysis/levenshtein_utils.py` & `vyper-0.4.0rc6/vyper/semantics/analysis/levenshtein_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/analysis/local.py` & `vyper-0.4.0rc6/vyper/semantics/analysis/local.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/analysis/module.py` & `vyper-0.4.0rc6/vyper/semantics/analysis/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,18 +195,14 @@
         # keep track of exported functions to prevent duplicate exports
         self._exposed_functions: dict[ContractFunctionT, vy_ast.VyperNode] = {}
 
         self._events: list[EventT] = []
 
         self.module_t: Optional[ModuleT] = None
 
-        # ast cache, hitchhike onto the input_bundle object
-        if not hasattr(self.input_bundle._cache, "_ast_of"):
-            self.input_bundle._cache._ast_of: dict[int, vy_ast.Module] = {}  # type: ignore
-
     def analyze_module_body(self):
         # generate a `ModuleT` from the top-level node
         # note: also validates unique method ids
 
         assert "type" not in self.ast._metadata
 
         self._to_visit = self.ast.body.copy()
@@ -617,21 +613,14 @@
         self._exposed_functions[func_t] = node
 
     def visit_VariableDecl(self, node):
         # postcondition of VariableDecl.validate
         assert isinstance(node.target, vy_ast.Name)
         name = node.target.id
 
-        if node.is_public:
-            # generate function type and add to metadata
-            # we need this when building the public getter
-            func_t = ContractFunctionT.getter_from_VariableDecl(node)
-            node._metadata["getter_type"] = func_t
-            self._add_exposed_function(func_t, node)
-
         # TODO: move this check to local analysis
         if node.is_immutable:
             # mutability is checked automatically preventing assignment
             # outside of the constructor, here we just check a value is assigned,
             # not necessarily where
             assignments = self.ast.get_descendants(
                 vy_ast.Assign, filters={"target.id": node.target.id}
@@ -644,15 +633,15 @@
                 message = (
                     "Immutable variables must be accessed without 'self'"
                     if len(wrong_self_attribute) > 0
                     else "Immutable definition requires an assignment in the constructor"
                 )
                 raise ImmutableViolation(message, node)
 
-        data_loc = (
+        location = (
             DataLocation.CODE
             if node.is_immutable
             else DataLocation.UNSET
             if node.is_constant
             else DataLocation.TRANSIENT
             if node.is_transient
             else DataLocation.STORAGE
@@ -662,29 +651,36 @@
             Modifiability.RUNTIME_CONSTANT
             if node.is_immutable
             else Modifiability.CONSTANT
             if node.is_constant
             else Modifiability.MODIFIABLE
         )
 
-        type_ = type_from_annotation(node.annotation, data_loc)
+        type_ = type_from_annotation(node.annotation, location)
 
         if node.is_transient and not version_check(begin="cancun"):
             raise EvmVersionException("`transient` is not available pre-cancun", node.annotation)
 
         var_info = VarInfo(
             type_,
             decl_node=node,
-            location=data_loc,
+            location=location,
             modifiability=modifiability,
             is_public=node.is_public,
         )
         node.target._metadata["varinfo"] = var_info  # TODO maybe put this in the global namespace
         node._metadata["type"] = type_
 
+        if node.is_public:
+            # generate function type and add to metadata
+            # we need this when building the public getter
+            func_t = ContractFunctionT.getter_from_VariableDecl(node)
+            node._metadata["getter_type"] = func_t
+            self._add_exposed_function(func_t, node)
+
         def _finalize():
             # add the variable name to `self` namespace if the variable is either
             # 1. a public constant or immutable; or
             # 2. a storage variable, whether private or public
             if (node.is_constant or node.is_immutable) and not node.is_public:
                 return
```

### Comparing `vyper-0.4.0rc5/vyper/semantics/analysis/utils.py` & `vyper-0.4.0rc6/vyper/semantics/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/environment.py` & `vyper-0.4.0rc6/vyper/semantics/environment.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/namespace.py` & `vyper-0.4.0rc6/vyper/semantics/namespace.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/types/__init__.py` & `vyper-0.4.0rc6/vyper/semantics/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/types/base.py` & `vyper-0.4.0rc6/vyper/semantics/types/base.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/types/bytestrings.py` & `vyper-0.4.0rc6/vyper/semantics/types/bytestrings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/types/function.py` & `vyper-0.4.0rc6/vyper/semantics/types/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,16 +345,14 @@
         return_type = _parse_return_type(funcdef)
 
         if len(funcdef.body) != 1 or not isinstance(funcdef.body[0].get("value"), vy_ast.Ellipsis):
             raise FunctionDeclarationException(
                 "function body in an interface can only be `...`!", funcdef
             )
 
-        assert function_visibility is not None  # mypy hint
-
         return cls(
             funcdef.name,
             positional_args,
             keyword_args,
             return_type,
             function_visibility,
             state_mutability,
@@ -401,31 +399,27 @@
         if funcdef.name == "__init__":
             if state_mutability in (StateMutability.PURE, StateMutability.VIEW):
                 raise FunctionDeclarationException(
                     "Constructor cannot be marked as `@pure` or `@view`", funcdef
                 )
             if function_visibility != FunctionVisibility.DEPLOY:
                 raise FunctionDeclarationException(
-                    f"Constructor must be marked as `@deploy`, not `@{function_visibility}`",
-                    funcdef,
+                    "Constructor must be marked as `@deploy`", funcdef
                 )
             if return_type is not None:
                 raise FunctionDeclarationException(
                     "Constructor may not have a return type", funcdef.returns
                 )
 
             # call arguments
             if funcdef.args.defaults:
                 raise FunctionDeclarationException(
                     "Constructor may not use default arguments", funcdef.args.defaults[0]
                 )
 
-        # sanity check
-        assert function_visibility is not None
-
         return cls(
             funcdef.name,
             positional_args,
             keyword_args,
             return_type,
             function_visibility,
             state_mutability,
@@ -456,15 +450,18 @@
 
         Returns
         -------
         ContractFunctionT
         """
         if not node.is_public:
             raise CompilerPanic("getter generated for non-public function")
-        type_ = type_from_annotation(node.annotation, DataLocation.STORAGE)
+
+        # calculated by caller (ModuleAnalyzer.visit_VariableDecl)
+        type_ = node.target._metadata["varinfo"].typ
+
         arguments, return_type = type_.getter_signature
         args = []
         for i, item in enumerate(arguments):
             args.append(PositionalArg(f"arg{i}", item))
 
         return cls(
             node.target.id,
@@ -695,15 +692,15 @@
         return None
     # note: consider, for cleanliness, adding DataLocation.RETURN_VALUE
     return type_from_annotation(funcdef.returns, DataLocation.MEMORY)
 
 
 def _parse_decorators(
     funcdef: vy_ast.FunctionDef,
-) -> tuple[Optional[FunctionVisibility], StateMutability, bool]:
+) -> tuple[FunctionVisibility, StateMutability, bool]:
     function_visibility = None
     state_mutability = None
     nonreentrant_node = None
 
     for decorator in funcdef.decorator_list:
         if isinstance(decorator, vy_ast.Call):
             msg = "Decorator is not callable"
@@ -751,27 +748,23 @@
                     )
                 raise FunctionDeclarationException(f"Unknown decorator: {decorator.id}", decorator)
 
         else:
             raise StructureException("Bad decorator syntax", decorator)
 
     if function_visibility is None:
-        raise FunctionDeclarationException(
-            f"Visibility must be set to one of: {', '.join(FunctionVisibility.values())}", funcdef
-        )
+        function_visibility = FunctionVisibility.INTERNAL
 
     if state_mutability is None:
         # default to nonpayable
         state_mutability = StateMutability.NONPAYABLE
 
     if state_mutability == StateMutability.PURE and nonreentrant_node is not None:
         raise StructureException("Cannot use reentrancy guard on pure functions", nonreentrant_node)
 
-    # assert function_visibility is not None  # mypy
-    # assert state_mutability is not None  # mypy
     nonreentrant = nonreentrant_node is not None
     return function_visibility, state_mutability, nonreentrant
 
 
 def _parse_args(
     funcdef: vy_ast.FunctionDef, is_interface: bool = False
 ) -> tuple[list[PositionalArg], list[KeywordArg]]:
```

### Comparing `vyper-0.4.0rc5/vyper/semantics/types/module.py` & `vyper-0.4.0rc6/vyper/semantics/types/module.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/types/primitives.py` & `vyper-0.4.0rc6/vyper/semantics/types/primitives.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/types/subscriptable.py` & `vyper-0.4.0rc6/vyper/semantics/types/subscriptable.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 class HashMapT(_SubscriptableT):
     typeclass = "hashmap"
     _id = "HashMap"  # CMC 2024-03-03 maybe this would be better as repr(self)
 
     _equality_attrs = ("key_type", "value_type")
 
-    # disallow everything but storage
+    # disallow everything but storage or transient
     _invalid_locations = (
         DataLocation.UNSET,
         DataLocation.CALLDATA,
         DataLocation.CODE,
         DataLocation.MEMORY,
     )
 
@@ -80,18 +80,19 @@
                     "HashMap must be defined with a key type and a value type, "
                     "e.g. my_hashmap: HashMap[k, v]"
                 ),
                 node,
             )
 
         k_ast, v_ast = node.slice.elements
-        key_type = type_from_annotation(k_ast, DataLocation.STORAGE)
+        key_type = type_from_annotation(k_ast)
         if not key_type._as_hashmap_key:
             raise InvalidType("can only use primitive types as HashMap key!", k_ast)
 
+        # TODO: thread through actual location - might also be TRANSIENT
         value_type = type_from_annotation(v_ast, DataLocation.STORAGE)
 
         return cls(key_type, value_type)
 
 
 class _SequenceT(_SubscriptableT):
     """
```

### Comparing `vyper-0.4.0rc5/vyper/semantics/types/user.py` & `vyper-0.4.0rc6/vyper/semantics/types/user.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/semantics/types/utils.py` & `vyper-0.4.0rc6/vyper/semantics/types/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/utils.py` & `vyper-0.4.0rc6/vyper/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,24 @@
 
     def __len__(self):
         return len(self._data)
 
     def first(self):
         return next(iter(self))
 
+    def pop(self):
+        return self._data.popitem()[0]
+
     def add(self, item: _T) -> None:
         self._data[item] = None
 
+    def addmany(self, iterable):
+        for item in iterable:
+            self._data[item] = None
+
     def remove(self, item: _T) -> None:
         del self._data[item]
 
     def drop(self, item: _T):
         # friendly version of remove
         self._data.pop(item, None)
```

### Comparing `vyper-0.4.0rc5/vyper/venom/README.md` & `vyper-0.4.0rc6/vyper/venom/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/venom/__init__.py` & `vyper-0.4.0rc6/vyper/venom/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 # (can have an `__init__.py` which exposes the API).
 
 from typing import Optional
 
 from vyper.codegen.ir_node import IRnode
 from vyper.compiler.settings import OptimizationLevel
 from vyper.venom.analysis.analysis import IRAnalysesCache
-from vyper.venom.analysis.liveness import LivenessAnalysis
 from vyper.venom.context import IRContext
 from vyper.venom.function import IRFunction
 from vyper.venom.ir_node_to_venom import ir_node_to_venom
+from vyper.venom.passes.algebraic_optimization import AlgebraicOptimizationPass
+from vyper.venom.passes.branch_optimization import BranchOptimizationPass
 from vyper.venom.passes.dft import DFTPass
 from vyper.venom.passes.make_ssa import MakeSSA
 from vyper.venom.passes.mem2var import Mem2Var
 from vyper.venom.passes.remove_unused_variables import RemoveUnusedVariablesPass
 from vyper.venom.passes.sccp import SCCP
 from vyper.venom.passes.simplify_cfg import SimplifyCFGPass
 from vyper.venom.passes.store_elimination import StoreElimination
@@ -40,20 +41,22 @@
 def _run_passes(fn: IRFunction, optimize: OptimizationLevel) -> None:
     # Run passes on Venom IR
     # TODO: Add support for optimization levels
 
     ac = IRAnalysesCache(fn)
 
     SimplifyCFGPass(ac, fn).run_pass()
-    Mem2Var(ac, fn).run_pass()
     MakeSSA(ac, fn).run_pass()
-    StoreElimination(ac, fn).run_pass()
+    Mem2Var(ac, fn).run_pass()
     MakeSSA(ac, fn).run_pass()
     SCCP(ac, fn).run_pass()
+    StoreElimination(ac, fn).run_pass()
     SimplifyCFGPass(ac, fn).run_pass()
+    AlgebraicOptimizationPass(ac, fn).run_pass()
+    BranchOptimizationPass(ac, fn).run_pass()
     RemoveUnusedVariablesPass(ac, fn).run_pass()
     DFTPass(ac, fn).run_pass()
 
 
 def generate_ir(ir: IRnode, optimize: OptimizationLevel) -> IRContext:
     # Convert "old" IR to "new" IR
     ctx = ir_node_to_venom(ir)
```

### Comparing `vyper-0.4.0rc5/vyper/venom/analysis/analysis.py` & `vyper-0.4.0rc6/vyper/venom/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/venom/analysis/cfg.py` & `vyper-0.4.0rc6/vyper/venom/analysis/cfg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from vyper.utils import OrderedSet
 from vyper.venom.analysis.analysis import IRAnalysis
-from vyper.venom.basicblock import BB_TERMINATORS, CFG_ALTERING_INSTRUCTIONS
+from vyper.venom.basicblock import CFG_ALTERING_INSTRUCTIONS
 
 
 class CFGAnalysis(IRAnalysis):
     """
     Compute control flow graph information for each basic block in the function.
     """
 
@@ -14,17 +14,15 @@
             bb.cfg_in = OrderedSet()
             bb.cfg_out = OrderedSet()
             bb.out_vars = OrderedSet()
 
         for bb in fn.get_basic_blocks():
             assert len(bb.instructions) > 0, "Basic block should not be empty"
             last_inst = bb.instructions[-1]
-            assert (
-                last_inst.opcode in BB_TERMINATORS
-            ), f"Last instruction should be a terminator {bb}"
+            assert last_inst.is_bb_terminator, f"Last instruction should be a terminator {bb}"
 
             for inst in bb.instructions:
                 if inst.opcode in CFG_ALTERING_INSTRUCTIONS:
                     ops = inst.get_label_operands()
                     for op in ops:
                         fn.get_basic_block(op.value).add_cfg_in(bb)
```

### Comparing `vyper-0.4.0rc5/vyper/venom/analysis/dfg.py` & `vyper-0.4.0rc6/vyper/venom/analysis/dfg.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional
 
 from vyper.venom.analysis.analysis import IRAnalysesCache, IRAnalysis
+from vyper.venom.analysis.liveness import LivenessAnalysis
 from vyper.venom.basicblock import IRInstruction, IRVariable
 from vyper.venom.function import IRFunction
 
 
 class DFGAnalysis(IRAnalysis):
     _dfg_inputs: dict[IRVariable, list[IRInstruction]]
     _dfg_outputs: dict[IRVariable, IRInstruction]
@@ -18,28 +19,36 @@
     def get_uses(self, op: IRVariable) -> list[IRInstruction]:
         return self._dfg_inputs.get(op, [])
 
     # the instruction which produces this variable.
     def get_producing_instruction(self, op: IRVariable) -> Optional[IRInstruction]:
         return self._dfg_outputs.get(op)
 
+    def add_use(self, op: IRVariable, inst: IRInstruction):
+        uses = self._dfg_inputs.setdefault(op, [])
+        uses.append(inst)
+
+    def remove_use(self, op: IRVariable, inst: IRInstruction):
+        uses = self._dfg_inputs.get(op, [])
+        uses.remove(inst)
+
     @property
     def outputs(self) -> dict[IRVariable, IRInstruction]:
         return self._dfg_outputs
 
     def analyze(self):
         # Build DFG
 
         # %15 = add %13 %14
         # %16 = iszero %15
         # dfg_outputs of %15 is (%15 = add %13 %14)
         # dfg_inputs of %15 is all the instructions which *use* %15, ex. [(%16 = iszero %15), ...]
         for bb in self.function.get_basic_blocks():
             for inst in bb.instructions:
-                operands = inst.get_inputs()
+                operands = inst.get_input_variables()
                 res = inst.get_outputs()
 
                 for op in operands:
                     inputs = self._dfg_inputs.setdefault(op, [])
                     inputs.append(inst)
 
                 for op in res:  # type: ignore
@@ -55,9 +64,12 @@
                 for op in input.get_outputs():
                     if isinstance(op, IRVariable):
                         lines.append(f'    " {var.name} " -> " {op.name} "')
 
         lines.append("}")
         return "\n".join(lines)
 
+    def invalidate(self):
+        self.analyses_cache.invalidate_analysis(LivenessAnalysis)
+
     def __repr__(self) -> str:
         return self.as_graph()
```

### Comparing `vyper-0.4.0rc5/vyper/venom/analysis/dominators.py` & `vyper-0.4.0rc6/vyper/venom/analysis/dominators.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/venom/analysis/liveness.py` & `vyper-0.4.0rc6/vyper/venom/analysis/liveness.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         """
         Compute liveness of each instruction in the basic block.
         Returns True if liveness changed
         """
         orig_liveness = bb.instructions[0].liveness.copy()
         liveness = bb.out_vars.copy()
         for instruction in reversed(bb.instructions):
-            ins = instruction.get_inputs()
+            ins = instruction.get_input_variables()
             outs = instruction.get_outputs()
 
             if ins or outs:
                 # perf: only copy if changed
                 liveness = liveness.copy()
                 liveness.update(ins)
                 liveness.dropmany(outs)
```

### Comparing `vyper-0.4.0rc5/vyper/venom/basicblock.py` & `vyper-0.4.0rc6/vyper/venom/basicblock.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 VOLATILE_INSTRUCTIONS = frozenset(
     [
         "param",
         "call",
         "staticcall",
         "delegatecall",
+        "create",
+        "create2",
         "invoke",
         "sload",
         "sstore",
         "iload",
         "istore",
         "tload",
         "tstore",
@@ -30,22 +32,30 @@
         "codecopy",
         "dloadbytes",
         "dload",
         "return",
         "ret",
         "jmp",
         "jnz",
+        "djmp",
+        "log",
+        "selfdestruct",
+        "invalid",
+        "revert",
+        "assert",
+        "assert_unreachable",
+        "stop",
+        "exit",
     ]
 )
 
 NO_OUTPUT_INSTRUCTIONS = frozenset(
     [
         "mstore",
         "sstore",
-        "dstore",
         "istore",
         "tstore",
         "dloadbytes",
         "calldatacopy",
         "mcopy",
         "returndatacopy",
         "codecopy",
@@ -63,14 +73,18 @@
         "djmp",
         "jnz",
         "log",
         "exit",
     ]
 )
 
+assert VOLATILE_INSTRUCTIONS.issuperset(NO_OUTPUT_INSTRUCTIONS), (
+    NO_OUTPUT_INSTRUCTIONS - VOLATILE_INSTRUCTIONS
+)
+
 CFG_ALTERING_INSTRUCTIONS = frozenset(["jmp", "djmp", "jnz"])
 
 if TYPE_CHECKING:
     from vyper.venom.function import IRFunction
 
 
 class IRDebugInfo:
@@ -217,30 +231,34 @@
         self.dup_requirements = OrderedSet()
         self.fence_id = -1
         self.annotation = None
         self.ast_source = None
         self.error_msg = None
 
     @property
-    def volatile(self) -> bool:
+    def is_volatile(self) -> bool:
         return self.opcode in VOLATILE_INSTRUCTIONS
 
+    @property
+    def is_bb_terminator(self) -> bool:
+        return self.opcode in BB_TERMINATORS
+
     def get_label_operands(self) -> Iterator[IRLabel]:
         """
         Get all labels in instruction.
         """
         return (op for op in self.operands if isinstance(op, IRLabel))
 
     def get_non_label_operands(self) -> Iterator[IROperand]:
         """
         Get input operands for instruction which are not labels
         """
         return (op for op in self.operands if not isinstance(op, IRLabel))
 
-    def get_inputs(self) -> Iterator[IRVariable]:
+    def get_input_variables(self) -> Iterator[IRVariable]:
         """
         Get all input operands for instruction.
         """
         return (op for op in self.operands if isinstance(op, IRVariable))
 
     def get_outputs(self) -> list[IROperand]:
         """
@@ -473,15 +491,15 @@
         Get all assignments in basic block.
         """
         return [inst.output for inst in self.instructions if inst.output]
 
     def get_uses(self) -> dict[IRVariable, OrderedSet[IRInstruction]]:
         uses: dict[IRVariable, OrderedSet[IRInstruction]] = {}
         for inst in self.instructions:
-            for op in inst.get_inputs():
+            for op in inst.get_input_variables():
                 if op not in uses:
                     uses[op] = OrderedSet()
                 uses[op].add(inst)
         return uses
 
     @property
     def is_empty(self) -> bool:
@@ -495,25 +513,25 @@
         """
         Check if the basic block is terminal, i.e. the last instruction is a terminator.
         """
         # it's ok to return False here, since we use this to check
         # if we can/need to append instructions to the basic block.
         if len(self.instructions) == 0:
             return False
-        return self.instructions[-1].opcode in BB_TERMINATORS
+        return self.instructions[-1].is_bb_terminator
 
     @property
     def is_terminal(self) -> bool:
         """
         Check if the basic block is terminal.
         """
         return len(self.cfg_out) == 0
 
     @property
-    def in_vars(self) -> OrderedSet[IRVariable]:
+    def liveness_in_vars(self) -> OrderedSet[IRVariable]:
         for inst in self.instructions:
             if inst.opcode != "phi":
                 return inst.liveness
         return OrderedSet()
 
     def copy(self):
         bb = IRBasicBlock(self.label, self.parent)
```

### Comparing `vyper-0.4.0rc5/vyper/venom/context.py` & `vyper-0.4.0rc6/vyper/venom/context.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/venom/function.py` & `vyper-0.4.0rc6/vyper/venom/function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/venom/ir_node_to_venom.py` & `vyper-0.4.0rc6/vyper/venom/ir_node_to_venom.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/venom/passes/base_pass.py` & `vyper-0.4.0rc6/vyper/venom/passes/base_pass.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/venom/passes/dft.py` & `vyper-0.4.0rc6/vyper/venom/passes/dft.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from vyper.utils import OrderedSet
 from vyper.venom.analysis.dfg import DFGAnalysis
-from vyper.venom.basicblock import BB_TERMINATORS, IRBasicBlock, IRInstruction, IRVariable
+from vyper.venom.basicblock import IRBasicBlock, IRInstruction, IRVariable
 from vyper.venom.function import IRFunction
 from vyper.venom.passes.base_pass import IRPass
 
 
 class DFTPass(IRPass):
     function: IRFunction
     inst_order: dict[IRInstruction, int]
@@ -26,40 +26,40 @@
                 self._process_instruction_r(bb, uses_this, offset)
 
         if inst in self.visited_instructions:
             return
         self.visited_instructions.add(inst)
         self.inst_order_num += 1
 
-        if inst.opcode in BB_TERMINATORS:
+        if inst.is_bb_terminator:
             offset = len(bb.instructions)
 
         if inst.opcode == "phi":
             # phi instructions stay at the beginning of the basic block
             # and no input processing is needed
             # bb.instructions.append(inst)
             self.inst_order[inst] = 0
             return
 
-        for op in inst.get_inputs():
+        for op in inst.get_input_variables():
             target = self.dfg.get_producing_instruction(op)
             assert target is not None, f"no producing instruction for {op}"
             if target.parent != inst.parent or target.fence_id != inst.fence_id:
                 # don't reorder across basic block or fence boundaries
                 continue
             self._process_instruction_r(bb, target, offset)
 
         self.inst_order[inst] = self.inst_order_num + offset
 
     def _process_basic_block(self, bb: IRBasicBlock) -> None:
         self.function.append_basic_block(bb)
 
         for inst in bb.instructions:
             inst.fence_id = self.fence_id
-            if inst.volatile:
+            if inst.is_volatile:
                 self.fence_id += 1
 
         # We go throught the instructions and calculate the order in which they should be executed
         # based on the data flow graph. This order is stored in the inst_order dictionary.
         # We then sort the instructions based on this order.
         self.inst_order = {}
         self.inst_order_num = 0
```

### Comparing `vyper-0.4.0rc5/vyper/venom/passes/make_ssa.py` & `vyper-0.4.0rc6/vyper/venom/passes/make_ssa.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,27 @@
     defs: dict[IRVariable, OrderedSet[IRBasicBlock]]
 
     def run_pass(self):
         fn = self.function
 
         self.analyses_cache.request_analysis(CFGAnalysis)
         self.dom = self.analyses_cache.request_analysis(DominatorTreeAnalysis)
+
+        # Request liveness analysis so the `liveness_in_vars` field is valid
         self.analyses_cache.request_analysis(LivenessAnalysis)
 
         self._add_phi_nodes()
 
         self.var_name_counters = {var.name: 0 for var in self.defs.keys()}
         self.var_name_stacks = {var.name: [0] for var in self.defs.keys()}
         self._rename_vars(fn.entry)
         self._remove_degenerate_phis(fn.entry)
 
+        self.analyses_cache.invalidate_analysis(LivenessAnalysis)
+
     def _add_phi_nodes(self):
         """
         Add phi nodes to the function.
         """
         self._compute_defs()
         work = {var: 0 for var in self.dom.dfs_walk}
         has_already = {var: 0 for var in self.dom.dfs_walk}
@@ -50,15 +54,15 @@
                     self._place_phi(var, dom)
                     has_already[dom] = i
                     if work[dom] < i:
                         work[dom] = i
                         defs.append(dom)
 
     def _place_phi(self, var: IRVariable, basic_block: IRBasicBlock):
-        if var not in basic_block.in_vars:
+        if var not in basic_block.liveness_in_vars:
             return
 
         args: list[IROperand] = []
         for bb in basic_block.cfg_in:
             if bb == basic_block:
                 continue
```

### Comparing `vyper-0.4.0rc5/vyper/venom/passes/mem2var.py` & `vyper-0.4.0rc6/vyper/venom/passes/mem2var.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
     function: IRFunction
     defs: dict[IRVariable, OrderedSet[IRBasicBlock]]
 
     def run_pass(self):
         self.analyses_cache.request_analysis(CFGAnalysis)
         dfg = self.analyses_cache.request_analysis(DFGAnalysis)
-        self.analyses_cache.request_analysis(LivenessAnalysis)
 
         self.var_name_count = 0
         for var, inst in dfg.outputs.items():
             if inst.opcode != "alloca":
                 continue
             self._process_alloca_var(dfg, var)
```

### Comparing `vyper-0.4.0rc5/vyper/venom/passes/normalization.py` & `vyper-0.4.0rc6/vyper/venom/passes/normalization.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/venom/passes/remove_unused_variables.py` & `vyper-0.4.0rc6/vyper/venom/analysis/dup_requirements.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,15 @@
-from vyper.venom.analysis.dfg import DFGAnalysis
-from vyper.venom.analysis.liveness import LivenessAnalysis
-from vyper.venom.passes.base_pass import IRPass
+from vyper.utils import OrderedSet
+from vyper.venom.analysis.analysis import IRAnalysis
 
 
-class RemoveUnusedVariablesPass(IRPass):
-    def run_pass(self):
-        removeList = set()
-
-        self.analyses_cache.request_analysis(LivenessAnalysis)
-
+class DupRequirementsAnalysis(IRAnalysis):
+    def analyze(self):
         for bb in self.function.get_basic_blocks():
-            for i, inst in enumerate(bb.instructions[:-1]):
-                if inst.volatile:
-                    continue
-                next_liveness = bb.instructions[i + 1].liveness
-                if (inst.output and inst.output not in next_liveness) or inst.opcode == "nop":
-                    removeList.add(inst)
-
-            bb.instructions = [inst for inst in bb.instructions if inst not in removeList]
-
-        self.analyses_cache.invalidate_analysis(DFGAnalysis)
+            last_liveness = bb.out_vars
+            for inst in reversed(bb.instructions):
+                inst.dup_requirements = OrderedSet()
+                ops = inst.get_input_variables()
+                for op in ops:
+                    if op in last_liveness:
+                        inst.dup_requirements.add(op)
+                last_liveness = inst.liveness
```

### Comparing `vyper-0.4.0rc5/vyper/venom/passes/sccp/eval.py` & `vyper-0.4.0rc6/vyper/venom/passes/sccp/eval.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,96 +9,97 @@
     signed_to_unsigned,
     unsigned_to_signed,
 )
 from vyper.venom.basicblock import IROperand
 
 
 def _unsigned_to_signed(value: int) -> int:
-    if value <= SizeLimits.MAX_INT256:
-        return value  # fast exit
-    else:
-        return unsigned_to_signed(value, 256)
+    assert isinstance(value, int)
+    return unsigned_to_signed(value, 256)
 
 
 def _signed_to_unsigned(value: int) -> int:
-    if value >= 0:
-        return value  # fast exit
-    else:
-        return signed_to_unsigned(value, 256)
+    assert isinstance(value, int)
+    return signed_to_unsigned(value, 256)
 
 
 def _wrap_signed_binop(operation):
     def wrapper(ops: list[IROperand]) -> int:
+        assert len(ops) == 2
         first = _unsigned_to_signed(ops[1].value)
         second = _unsigned_to_signed(ops[0].value)
-        return _signed_to_unsigned(int(operation(first, second)))
+        return _signed_to_unsigned(operation(first, second))
 
     return wrapper
 
 
 def _wrap_binop(operation):
     def wrapper(ops: list[IROperand]) -> int:
+        assert len(ops) == 2
         first = _signed_to_unsigned(ops[1].value)
         second = _signed_to_unsigned(ops[0].value)
         ret = operation(first, second)
-        assert isinstance(ret, int)
         return ret & SizeLimits.MAX_UINT256
 
     return wrapper
 
 
-def _evm_signextend(ops: list[IROperand]) -> int:
-    value = ops[0].value
-    nbytes = ops[1].value
+def _wrap_unop(operation):
+    def wrapper(ops: list[IROperand]) -> int:
+        assert len(ops) == 1
+        value = _signed_to_unsigned(ops[0].value)
+        ret = operation(value)
+        return ret & SizeLimits.MAX_UINT256
+
+    return wrapper
+
 
+def _evm_signextend(nbytes, value) -> int:
     assert 0 <= value <= SizeLimits.MAX_UINT256, "Value out of bounds"
 
     if nbytes > 31:
         return value
 
+    assert nbytes >= 0
+
     sign_bit = 1 << (nbytes * 8 + 7)
     if value & sign_bit:
         value |= SizeLimits.CEILING_UINT256 - sign_bit
     else:
         value &= sign_bit - 1
 
     return value
 
 
-def _evm_iszero(ops: list[IROperand]) -> int:
-    value = ops[0].value
+def _evm_iszero(value: int) -> int:
     assert SizeLimits.MIN_INT256 <= value <= SizeLimits.MAX_UINT256, "Value out of bounds"
     return int(value == 0)  # 1 if True else 0
 
 
-def _evm_shr(ops: list[IROperand]) -> int:
-    value = ops[0].value
-    shift_len = ops[1].value
+def _evm_shr(shift_len: int, value: int) -> int:
     assert 0 <= value <= SizeLimits.MAX_UINT256, "Value out of bounds"
+    assert shift_len >= 0
     return value >> shift_len
 
 
-def _evm_shl(ops: list[IROperand]) -> int:
-    value = ops[0].value
-    shift_len = ops[1].value
+def _evm_shl(shift_len: int, value: int) -> int:
     assert 0 <= value <= SizeLimits.MAX_UINT256, "Value out of bounds"
     if shift_len >= 256:
         return 0
+    assert shift_len >= 0
     return (value << shift_len) & SizeLimits.MAX_UINT256
 
 
-def _evm_sar(ops: list[IROperand]) -> int:
-    value = _unsigned_to_signed(ops[0].value)
+def _evm_sar(shift_len: int, value: int) -> int:
     assert SizeLimits.MIN_INT256 <= value <= SizeLimits.MAX_INT256, "Value out of bounds"
-    shift_len = ops[1].value
+    assert shift_len >= 0
     return value >> shift_len
 
 
-def _evm_not(ops: list[IROperand]) -> int:
-    value = ops[0].value
+def _evm_not(value: int) -> int:
     assert 0 <= value <= SizeLimits.MAX_UINT256, "Value out of bounds"
     return SizeLimits.MAX_UINT256 ^ value
 
 
 ARITHMETIC_OPS: dict[str, Callable[[list[IROperand]], int]] = {
     "add": _wrap_binop(operator.add),
     "sub": _wrap_binop(operator.sub),
@@ -117,15 +118,15 @@
     "slt": _wrap_signed_binop(operator.lt),
     "sle": _wrap_signed_binop(operator.le),
     "sgt": _wrap_signed_binop(operator.gt),
     "sge": _wrap_signed_binop(operator.ge),
     "or": _wrap_binop(operator.or_),
     "and": _wrap_binop(operator.and_),
     "xor": _wrap_binop(operator.xor),
-    "not": _evm_not,
-    "signextend": _evm_signextend,
-    "iszero": _evm_iszero,
-    "shr": _evm_shr,
-    "shl": _evm_shl,
-    "sar": _evm_sar,
+    "not": _wrap_unop(_evm_not),
+    "signextend": _wrap_binop(_evm_signextend),
+    "iszero": _wrap_unop(_evm_iszero),
+    "shr": _wrap_binop(_evm_shr),
+    "shl": _wrap_binop(_evm_shl),
+    "sar": _wrap_signed_binop(_evm_sar),
     "store": lambda ops: ops[0].value,
 }
```

### Comparing `vyper-0.4.0rc5/vyper/venom/passes/sccp/sccp.py` & `vyper-0.4.0rc6/vyper/venom/passes/sccp/sccp.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/venom/passes/simplify_cfg.py` & `vyper-0.4.0rc6/vyper/venom/passes/simplify_cfg.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/venom/passes/stack_reorder.py` & `vyper-0.4.0rc6/vyper/venom/passes/stack_reorder.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/venom/passes/store_elimination.py` & `vyper-0.4.0rc6/vyper/venom/passes/store_elimination.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/venom/stack_model.py` & `vyper-0.4.0rc6/vyper/venom/stack_model.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0rc5/vyper/venom/venom_to_assembly.py` & `vyper-0.4.0rc6/vyper/venom/venom_to_assembly.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,16 +77,16 @@
         "smod",
         "exp",
         "addmod",
         "mulmod",
         "eq",
         "iszero",
         "not",
-        "lg",
         "lt",
+        "gt",
         "slt",
         "sgt",
         "create",
         "create2",
         "msize",
         "balance",
         "call",
@@ -98,14 +98,17 @@
         "blobbasefee",
         "prevrandao",
         "difficulty",
         "invalid",
     ]
 )
 
+COMMUTATIVE_INSTRUCTIONS = frozenset(["add", "mul", "smul", "or", "xor", "and", "eq"])
+
+
 _REVERT_POSTAMBLE = ["_sym___revert", "JUMPDEST", *PUSH(0), "DUP1", "REVERT"]
 
 
 def apply_line_numbers(inst: IRInstruction, asm) -> list[str]:
     ret = []
     for op in asm:
         if isinstance(op, str) and not isinstance(op, Instruction):
@@ -191,16 +194,22 @@
 
         if no_optimize is False:
             optimize_assembly(top_asm)
 
         return top_asm
 
     def _stack_reorder(
-        self, assembly: list, stack: StackModel, stack_ops: list[IRVariable]
-    ) -> None:
+        self, assembly: list, stack: StackModel, stack_ops: list[IROperand], dry_run: bool = False
+    ) -> int:
+        cost = 0
+
+        if dry_run:
+            assert len(assembly) == 0, "Dry run should not work on assembly"
+            stack = stack.copy()
+
         stack_ops_count = len(stack_ops)
 
         counts = Counter(stack_ops)
 
         for i in range(stack_ops_count):
             op = stack_ops[i]
             final_stack_depth = -(stack_ops_count - i - 1)
@@ -212,16 +221,18 @@
 
             if depth == final_stack_depth:
                 continue
 
             if op == stack.peek(final_stack_depth):
                 continue
 
-            self.swap(assembly, stack, depth)
-            self.swap(assembly, stack, final_stack_depth)
+            cost += self.swap(assembly, stack, depth)
+            cost += self.swap(assembly, stack, final_stack_depth)
+
+        return cost
 
     def _emit_input_operands(
         self, assembly: list, inst: IRInstruction, ops: list[IROperand], stack: StackModel
     ) -> None:
         # PRE: we already have all the items on the stack that have
         # been scheduled to be killed. now it's just a matter of emitting
         # SWAPs, DUPs and PUSHes until we match the `ops` argument
@@ -290,15 +301,15 @@
         for bb in basicblock.reachable:
             self._generate_evm_for_basicblock_r(asm, bb, stack.copy())
 
     def _clean_unused_params(self, asm: list, bb: IRBasicBlock, stack: StackModel) -> None:
         for i, inst in enumerate(bb.instructions):
             if inst.opcode != "param":
                 break
-            if inst.volatile and i + 1 < len(bb.instructions):
+            if inst.is_volatile and i + 1 < len(bb.instructions):
                 liveness = bb.instructions[i + 1].liveness
                 if inst.output is not None and inst.output not in liveness:
                     depth = stack.get_depth(inst.output)
                     if depth != 0:
                         self.swap(asm, stack, depth)
                     self.pop(asm, stack)
 
@@ -372,15 +383,15 @@
             assert log_topic_count in [0, 1, 2, 3, 4], "Invalid topic count"
             operands = inst.operands[1:]
         else:
             operands = inst.operands
 
         if opcode == "phi":
             ret = inst.get_outputs()[0]
-            phis = list(inst.get_inputs())
+            phis = list(inst.get_input_variables())
             depth = stack.get_phi_depth(phis)
             # collapse the arguments to the phi node in the stack.
             # example, for `%56 = %label1 %13 %label2 %14`, we will
             # find an instance of %13 *or* %14 in the stack and replace it with %56.
             to_be_replaced = stack.peek(depth)
             if to_be_replaced in inst.dup_requirements:
                 # %13/%14 is still live(!), so we make a copy of it
@@ -402,17 +413,24 @@
             # TODO optimize stack reordering at entry and exit from basic blocks
             # NOTE: stack in general can contain multiple copies of the same variable,
             # however we are safe in the case of jmp/djmp/jnz as it's not going to
             # have multiples.
             target_stack_list = list(target_stack)
             self._stack_reorder(assembly, stack, target_stack_list)
 
+        if opcode in COMMUTATIVE_INSTRUCTIONS:
+            cost_no_swap = self._stack_reorder([], stack, operands, dry_run=True)
+            operands[-1], operands[-2] = operands[-2], operands[-1]
+            cost_with_swap = self._stack_reorder([], stack, operands, dry_run=True)
+            if cost_with_swap > cost_no_swap:
+                operands[-1], operands[-2] = operands[-2], operands[-1]
+
         # final step to get the inputs to this instruction ordered
         # correctly on the stack
-        self._stack_reorder(assembly, stack, operands)  # type: ignore
+        self._stack_reorder(assembly, stack, operands)
 
         # some instructions (i.e. invoke) need to do stack manipulations
         # with the stack model containing the return value(s), so we fiddle
         # with the stack model beforehand.
 
         # Step 4: Push instruction's return value to stack
         stack.pop(len(operands))
@@ -450,18 +468,14 @@
             assembly.append(f"_sym_{inst.operands[0].value}")
             assembly.append("JUMP")
         elif opcode == "djmp":
             assert isinstance(
                 inst.operands[0], IRVariable
             ), f"Expected IRVariable, got {inst.operands[0]}"
             assembly.append("JUMP")
-        elif opcode == "gt":
-            assembly.append("GT")
-        elif opcode == "lt":
-            assembly.append("LT")
         elif opcode == "invoke":
             target = inst.operands[0]
             assert isinstance(
                 target, IRLabel
             ), f"invoke target must be a label (is ${type(target)} ${target})"
             assembly.extend(
                 [
@@ -491,16 +505,14 @@
                     *PUSH(MemoryPositions.FREE_VAR_SPACE2),
                     "MSTORE",
                     *PUSH(64),
                     *PUSH(MemoryPositions.FREE_VAR_SPACE),
                     "SHA3",
                 ]
             )
-        elif opcode == "ceil32":
-            assembly.extend([*PUSH(31), "ADD", *PUSH(31), "NOT", "AND"])
         elif opcode == "assert":
             assembly.extend(["ISZERO", "_sym___revert", "JUMPI"])
         elif opcode == "assert_unreachable":
             end_symbol = mksymbol("reachable")
             assembly.extend([end_symbol, "JUMPI", "INVALID", end_symbol, "JUMPDEST"])
         elif opcode == "iload":
             addr = inst.operands[0]
@@ -523,28 +535,34 @@
         else:
             raise Exception(f"Unknown opcode: {opcode}")
 
         # Step 6: Emit instructions output operands (if any)
         if inst.output is not None:
             if "call" in inst.opcode and inst.output not in next_liveness:
                 self.pop(assembly, stack)
+            elif inst.output in next_liveness:
+                # peek at next_liveness to find the next scheduled item,
+                # and optimistically swap with it
+                next_scheduled = list(next_liveness)[-1]
+                self.swap_op(assembly, stack, next_scheduled)
 
         return apply_line_numbers(inst, assembly)
 
     def pop(self, assembly, stack, num=1):
         stack.pop(num)
         assembly.extend(["POP"] * num)
 
-    def swap(self, assembly, stack, depth):
+    def swap(self, assembly, stack, depth) -> int:
         # Swaps of the top is no op
         if depth == 0:
-            return
+            return 0
 
         stack.swap(depth)
         assembly.append(_evm_swap_for(depth))
+        return 1
 
     def dup(self, assembly, stack, depth):
         stack.dup(depth)
         assembly.append(_evm_dup_for(depth))
 
     def swap_op(self, assembly, stack, op):
         self.swap(assembly, stack, stack.get_depth(op))
```

### Comparing `vyper-0.4.0rc5/vyper.egg-info/PKG-INFO` & `vyper-0.4.0rc6/vyper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vyper
-Version: 0.4.0rc5
+Version: 0.4.0rc6
 Summary: Vyper: the Pythonic Programming Language for the EVM
 Home-page: https://github.com/vyperlang/vyper
 Author: Vyper Team
 Author-email: 
 License: Apache License 2.0
 Keywords: ethereum evm smart contract language
 Classifier: Intended Audience :: Developers
```

### Comparing `vyper-0.4.0rc5/vyper.egg-info/SOURCES.txt` & `vyper-0.4.0rc6/vyper.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 .readthedocs.yaml
 Dockerfile
 FUNDING.yml
 LICENSE
 Makefile
 README.md
 SECURITY.md
+codecov.yml
 make.cmd
 pyproject.toml
 quicktest.sh
 requirements-docs.txt
 setup.cfg
 setup.py
 .github/PULL_REQUEST_TEMPLATE.md
@@ -42,18 +43,19 @@
 docs/release-notes.rst
 docs/resources.rst
 docs/scoping-and-declarations.rst
 docs/statements.rst
 docs/structure-of-a-contract.rst
 docs/style-guide.rst
 docs/testing-contracts-brownie.rst
-docs/testing-contracts-ethtester.rst
+docs/testing-contracts-titanoboa.rst
 docs/testing-contracts.rst
 docs/toctree.rst
 docs/types.rst
+docs/using-modules.rst
 docs/versioning.rst
 docs/vyper-by-example.rst
 docs/_templates/versions.html
 examples/crowdfund.vy
 examples/auctions/blind_auction.vy
 examples/auctions/simple_open_auction.vy
 examples/factory/Exchange.vy
@@ -126,14 +128,15 @@
 tests/functional/codegen/test_interfaces.py
 tests/functional/codegen/test_selector_table.py
 tests/functional/codegen/test_selector_table_stability.py
 tests/functional/codegen/calling_convention/test_default_function.py
 tests/functional/codegen/calling_convention/test_default_parameters.py
 tests/functional/codegen/calling_convention/test_erc20_abi.py
 tests/functional/codegen/calling_convention/test_external_contract_calls.py
+tests/functional/codegen/calling_convention/test_internal_call.py
 tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py
 tests/functional/codegen/calling_convention/test_return.py
 tests/functional/codegen/calling_convention/test_self_call_struct.py
 tests/functional/codegen/environment_variables/test_blobbasefee.py
 tests/functional/codegen/environment_variables/test_block_number.py
 tests/functional/codegen/environment_variables/test_blockhash.py
 tests/functional/codegen/environment_variables/test_tx.py
@@ -146,15 +149,14 @@
 tests/functional/codegen/features/test_comments.py
 tests/functional/codegen/features/test_comparison.py
 tests/functional/codegen/features/test_conditionals.py
 tests/functional/codegen/features/test_constructor.py
 tests/functional/codegen/features/test_gas.py
 tests/functional/codegen/features/test_immutable.py
 tests/functional/codegen/features/test_init.py
-tests/functional/codegen/features/test_internal_call.py
 tests/functional/codegen/features/test_logging.py
 tests/functional/codegen/features/test_logging_bytes_extended.py
 tests/functional/codegen/features/test_logging_from_call.py
 tests/functional/codegen/features/test_memory_alloc.py
 tests/functional/codegen/features/test_memory_dealloc.py
 tests/functional/codegen/features/test_packing.py
 tests/functional/codegen/features/test_reverting.py
@@ -331,16 +333,18 @@
 tests/unit/ast/nodes/test_fold_compare.py
 tests/unit/ast/nodes/test_fold_subscript.py
 tests/unit/ast/nodes/test_fold_unaryop.py
 tests/unit/ast/nodes/test_from_node.py
 tests/unit/ast/nodes/test_get_children.py
 tests/unit/ast/nodes/test_get_descendants.py
 tests/unit/ast/nodes/test_hex.py
+tests/unit/cli/storage_layout/__init__.py
 tests/unit/cli/storage_layout/test_storage_layout.py
 tests/unit/cli/storage_layout/test_storage_layout_overrides.py
+tests/unit/cli/storage_layout/utils.py
 tests/unit/cli/vyper_compile/test_compile_files.py
 tests/unit/cli/vyper_compile/test_parse_args.py
 tests/unit/cli/vyper_json/test_compile_json.py
 tests/unit/cli/vyper_json/test_get_inputs.py
 tests/unit/cli/vyper_json/test_get_settings.py
 tests/unit/cli/vyper_json/test_output_selection.py
 tests/unit/cli/vyper_json/test_parse_args_vyperjson.py
@@ -357,14 +361,16 @@
 tests/unit/compiler/asm/test_asm_optimizer.py
 tests/unit/compiler/ir/__init__.py
 tests/unit/compiler/ir/test_calldatacopy.py
 tests/unit/compiler/ir/test_compile_ir.py
 tests/unit/compiler/ir/test_optimize_ir.py
 tests/unit/compiler/ir/test_repeat.py
 tests/unit/compiler/ir/test_with.py
+tests/unit/compiler/venom/test_algebraic_optimizer.py
+tests/unit/compiler/venom/test_branch_optimizer.py
 tests/unit/compiler/venom/test_convert_basicblock_simple.py
 tests/unit/compiler/venom/test_dominator_tree.py
 tests/unit/compiler/venom/test_duplicate_operands.py
 tests/unit/compiler/venom/test_liveness_simple_loop.py
 tests/unit/compiler/venom/test_make_ssa.py
 tests/unit/compiler/venom/test_multi_entry_block.py
 tests/unit/compiler/venom/test_sccp.py
@@ -501,15 +507,17 @@
 vyper/venom/analysis/__init__.py
 vyper/venom/analysis/analysis.py
 vyper/venom/analysis/cfg.py
 vyper/venom/analysis/dfg.py
 vyper/venom/analysis/dominators.py
 vyper/venom/analysis/dup_requirements.py
 vyper/venom/analysis/liveness.py
+vyper/venom/passes/algebraic_optimization.py
 vyper/venom/passes/base_pass.py
+vyper/venom/passes/branch_optimization.py
 vyper/venom/passes/dft.py
 vyper/venom/passes/make_ssa.py
 vyper/venom/passes/mem2var.py
 vyper/venom/passes/normalization.py
 vyper/venom/passes/remove_unused_variables.py
 vyper/venom/passes/simplify_cfg.py
 vyper/venom/passes/stack_reorder.py
```

### Comparing `vyper-0.4.0rc5/vyper.egg-info/requires.txt` & `vyper-0.4.0rc6/vyper.egg-info/requires.txt`

 * *Files identical despite different names*

