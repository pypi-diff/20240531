# Comparing `tmp/vanar-safe-eth-py-1.0.0.tar.gz` & `tmp/vanar-safe-eth-py-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanar-safe-eth-py-1.0.0.tar", last modified: Wed May 29 08:41:05 2024, max compression
+gzip compressed data, was "vanar-safe-eth-py-1.1.0.tar", last modified: Fri May 31 04:25:13 2024, max compression
```

## Comparing `vanar-safe-eth-py-1.0.0.tar` & `vanar-safe-eth-py-1.1.0.tar`

### file list

```diff
@@ -1,232 +1,232 @@
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.786044 vanar-safe-eth-py-1.0.0/
--rw-rw-r--   0 awais     (1000) awais     (1000)     1082 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/LICENSE
--rw-rw-r--   0 awais     (1000) awais     (1000)       71 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/MANIFEST.in
--rw-rw-r--   0 awais     (1000) awais     (1000)     8284 2024-05-29 08:41:05.786044 vanar-safe-eth-py-1.0.0/PKG-INFO
--rw-rw-r--   0 awais     (1000) awais     (1000)     5786 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/README.rst
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.670043 vanar-safe-eth-py-1.0.0/docs/
--rw-rw-r--   0 awais     (1000) awais     (1000)      638 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/docs/Makefile
--rw-rw-r--   0 awais     (1000) awais     (1000)      799 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/docs/make.bat
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.674043 vanar-safe-eth-py-1.0.0/docs/source/
--rw-rw-r--   0 awais     (1000) awais     (1000)     1995 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/docs/source/conf.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     1162 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/docs/source/gnosis.eth.clients.rst
--rw-rw-r--   0 awais     (1000) awais     (1000)      183 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/docs/source/gnosis.eth.contracts.rst
--rw-rw-r--   0 awais     (1000) awais     (1000)      954 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/docs/source/gnosis.eth.django.rst
--rw-rw-r--   0 awais     (1000) awais     (1000)      177 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/docs/source/gnosis.eth.eip712.rst
--rw-rw-r--   0 awais     (1000) awais     (1000)     1198 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/docs/source/gnosis.eth.oracles.abis.rst
--rw-rw-r--   0 awais     (1000) awais     (1000)      450 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/docs/source/gnosis.eth.oracles.rst
--rw-rw-r--   0 awais     (1000) awais     (1000)      936 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/docs/source/gnosis.eth.rst
--rw-rw-r--   0 awais     (1000) awais     (1000)      226 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/docs/source/gnosis.rst
--rw-rw-r--   0 awais     (1000) awais     (1000)     1852 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/docs/source/gnosis.safe.rst
--rw-rw-r--   0 awais     (1000) awais     (1000)      894 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/docs/source/index.rst
--rw-rw-r--   0 awais     (1000) awais     (1000)       55 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/docs/source/modules.rst
--rw-rw-r--   0 awais     (1000) awais     (1000)     9218 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/docs/source/quickstart.rst
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.674043 vanar-safe-eth-py-1.0.0/gnosis/
--rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/__init__.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.674043 vanar-safe-eth-py-1.0.0/gnosis/cowsap/
--rw-rw-r--   0 awais     (1000) awais     (1000)      156 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/cowsap/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     8465 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/cowsap/cow_swap_api.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     2700 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/cowsap/order.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.674043 vanar-safe-eth-py-1.0.0/gnosis/cowsap/tests/
--rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/cowsap/tests/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     5604 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/cowsap/tests/test_cow_swap_api.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.674043 vanar-safe-eth-py-1.0.0/gnosis/eth/
--rw-rw-r--   0 awais     (1000) awais     (1000)     1064 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/__init__.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.674043 vanar-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/
--rw-rw-r--   0 awais     (1000) awais     (1000)      366 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     7060 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/bundler_client.py
--rw-rw-r--   0 awais     (1000) awais     (1000)      986 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/constants.py
--rw-rw-r--   0 awais     (1000) awais     (1000)      208 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/exceptions.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     8899 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/user_operation.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     3371 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/user_operation_receipt.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.674043 vanar-safe-eth-py-1.0.0/gnosis/eth/clients/
--rw-rw-r--   0 awais     (1000) awais     (1000)      878 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/clients/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     9846 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/clients/blockscout_client.py
--rw-rw-r--   0 awais     (1000) awais     (1000)      194 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/clients/contract_metadata.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     4922 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/clients/ens_client.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     9880 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/clients/etherscan_client.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     3433 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/clients/sourcify_client.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     1020 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/constants.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.674043 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/
--rw-rw-r--   0 awais     (1000) awais     (1000)    10273 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/__init__.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.774044 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/
--rw-rw-r--   0 awais     (1000) awais     (1000)   328664 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/CPKFactory.json
--rw-rw-r--   0 awais     (1000) awais     (1000)    28908 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json
--rw-rw-r--   0 awais     (1000) awais     (1000)    29485 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json
--rw-rw-r--   0 awais     (1000) awais     (1000)    26897 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/DelegateConstructorProxy.json
--rw-rw-r--   0 awais     (1000) awais     (1000)    29068 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ERC1155.json
--rw-rw-r--   0 awais     (1000) awais     (1000)    54748 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ERC20.json
--rw-rw-r--   0 awais     (1000) awais     (1000)    89890 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ERC20TestToken.json
--rw-rw-r--   0 awais     (1000) awais     (1000)   622260 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ERC721.json
--rw-rw-r--   0 awais     (1000) awais     (1000)   983403 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json
--rw-rw-r--   0 awais     (1000) awais     (1000)  1158944 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json
--rw-rw-r--   0 awais     (1000) awais     (1000)  1347363 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json
--rw-rw-r--   0 awais     (1000) awais     (1000)   119875 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json
--rw-rw-r--   0 awais     (1000) awais     (1000)    19886 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/MultiSend.json
--rw-rw-r--   0 awais     (1000) awais     (1000)    78793 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/PayingProxy.json
--rw-rw-r--   0 awais     (1000) awais     (1000)   136946 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json
--rw-rw-r--   0 awais     (1000) awais     (1000)   288861 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json
--rw-rw-r--   0 awais     (1000) awais     (1000)    18975 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json
--rw-rw-r--   0 awais     (1000) awais     (1000)    15538 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json
--rw-rw-r--   0 awais     (1000) awais     (1000)    32495 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Proxy_V1_0_0.json
--rw-rw-r--   0 awais     (1000) awais     (1000)    39032 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Proxy_V1_1_1.json
--rw-rw-r--   0 awais     (1000) awais     (1000)     1862 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Proxy_V1_3_0.json
--rw-rw-r--   0 awais     (1000) awais     (1000)     1849 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Proxy_V1_4_1.json
--rw-rw-r--   0 awais     (1000) awais     (1000)   121611 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Safe_V1_4_1.json
--rw-rw-r--   0 awais     (1000) awais     (1000)     5069 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/SignMessageLib.json
--rw-rw-r--   0 awais     (1000) awais     (1000)     4913 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json
--rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     7351 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/kyber_network_proxy.json
--rw-rw-r--   0 awais     (1000) awais     (1000)    19012 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/multicall.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    17165 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_exchange.json
--rw-rw-r--   0 awais     (1000) awais     (1000)     2480 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_factory.json
--rw-rw-r--   0 awais     (1000) awais     (1000)     2242 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_v2_factory.json
--rw-rw-r--   0 awais     (1000) awais     (1000)     8293 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_v2_pair.json
--rw-rw-r--   0 awais     (1000) awais     (1000)    11889 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_v2_router.json
--rw-rw-r--   0 awais     (1000) awais     (1000)      954 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/contract_base.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.774044 vanar-safe-eth-py-1.0.0/gnosis/eth/django/
--rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/django/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     3735 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/django/admin.py
--rw-rw-r--   0 awais     (1000) awais     (1000)      269 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/django/filters.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     2435 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/django/forms.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     9936 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/django/models.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     6191 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/django/serializers.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.778044 vanar-safe-eth-py-1.0.0/gnosis/eth/django/tests/
--rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/django/tests/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)      711 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/django/tests/models.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     3028 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/django/tests/test_forms.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     8621 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/django/tests/test_models.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     7877 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/django/tests/test_serializers.py
--rw-rw-r--   0 awais     (1000) awais     (1000)      484 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/django/tests/test_validators.py
--rw-rw-r--   0 awais     (1000) awais     (1000)      320 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/django/validators.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.778044 vanar-safe-eth-py-1.0.0/gnosis/eth/eip712/
--rw-rw-r--   0 awais     (1000) awais     (1000)     5915 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/eip712/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    82106 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/ethereum_client.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    35780 2024-05-28 14:21:08.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/ethereum_network.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     1332 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/exceptions.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    13617 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/multicall.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.778044 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/
--rw-rw-r--   0 awais     (1000) awais     (1000)     1093 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/__init__.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.778044 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/
--rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    15986 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/aave_abis.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    30036 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/balancer_abis.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    29731 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/cream_abis.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    27567 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/curve_abis.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    25872 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/mooniswap_abis.py
--rw-rw-r--   0 awais     (1000) awais     (1000)      239 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/superfluid_abis.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    45208 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/uniswap_v3.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    36257 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/yearn_abis.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     1464 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/zerion_abis.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     2375 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/cowswap.py
--rw-rw-r--   0 awais     (1000) awais     (1000)      161 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/exceptions.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.778044 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/helpers/
--rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/helpers/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     5856 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/helpers/curve_gauge_list.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     4117 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/kyber.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    32169 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/oracles.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     1677 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/superfluid.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     1516 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/sushiswap.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     7154 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/uniswap_v3.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     1064 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/utils.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.778044 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/
--rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/__init__.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.778044 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/
--rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     6695 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/test_bundler_client.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     3593 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/test_e2e_bundler_client.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     1316 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/test_user_operation.py
--rw-rw-r--   0 awais     (1000) awais     (1000)      947 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/test_user_operation_receipt.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.778044 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/clients/
--rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/clients/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)   107388 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/clients/mocks.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     1047 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/clients/test_blockscout_client.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     6185 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/clients/test_ens_client.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     1686 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/clients/test_etherscan_client.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     2845 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/clients/test_sourcify_client.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.778044 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/eip712/
--rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/eip712/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    13327 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/eip712/test_eip712.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     3189 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/ethereum_test_case.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.782044 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/
--rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    33073 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_bundler.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    31306 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_internal_txs.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    10570 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_log_receipts.py
--rw-rw-r--   0 awais     (1000) awais     (1000)   792720 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_trace_block.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    92795 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_trace_filter.py
--rw-rw-r--   0 awais     (1000) awais     (1000)   171076 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_trace_transaction.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.782044 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/
--rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     2706 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_cowswap.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     1820 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_kyber.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     1460 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_superfluid.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     2043 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_sushiswap.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     3544 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_uniswap_v3.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    61025 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/test_ethereum_client.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     7087 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/test_multicall.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    21137 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/test_oracles.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     7287 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/test_utils.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     5069 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/tests/utils.py
--rw-rw-r--   0 awais     (1000) awais     (1000)      390 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/typing.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     6977 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/eth/utils.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.782044 vanar-safe-eth-py-1.0.0/gnosis/safe/
--rw-rw-r--   0 awais     (1000) awais     (1000)      742 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/__init__.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.782044 vanar-safe-eth-py-1.0.0/gnosis/safe/account_abstraction/
--rw-rw-r--   0 awais     (1000) awais     (1000)      101 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/account_abstraction/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     5647 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/account_abstraction/safe_operation.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    68779 2024-05-28 15:28:14.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/addresses.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.782044 vanar-safe-eth-py-1.0.0/gnosis/safe/api/
--rw-rw-r--   0 awais     (1000) awais     (1000)      186 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/api/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     2224 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/api/base_api.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.782044 vanar-safe-eth-py-1.0.0/gnosis/safe/api/transaction_service_api/
--rw-rw-r--   0 awais     (1000) awais     (1000)      103 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/api/transaction_service_api/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    14431 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/api/transaction_service_api/transaction_service_api.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     1784 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/api/transaction_service_api/transaction_service_messages.py
--rw-rw-r--   0 awais     (1000) awais     (1000)      252 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/api/transaction_service_api/transaction_service_tx.py
--rw-rw-r--   0 awais     (1000) awais     (1000)      105 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/enums.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     1451 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/exceptions.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    11459 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/multi_send.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    10479 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/proxy_factory.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    36823 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/safe.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    11975 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/safe_create2_tx.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     9736 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/safe_creator.py
--rw-rw-r--   0 awais     (1000) awais     (1000)   157076 2024-05-28 15:31:43.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/safe_deployments.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    12587 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/safe_signature.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    17225 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/safe_tx.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     4194 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/serializers.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     2000 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/signatures.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.786044 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/
--rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/__init__.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.786044 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/account_abstraction/
--rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/account_abstraction/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     3469 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/account_abstraction/test_safe_operation.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.786044 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/api/
--rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/api/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     5341 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/api/test_transaction_service_api.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    20692 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/safe_test_case.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     1398 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_addresses.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    10515 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_multi_send.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.786044 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_proxy_factory/
--rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_proxy_factory/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     7798 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    33486 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    16674 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_create2_tx.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    18510 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_signature.py
--rw-rw-r--   0 awais     (1000) awais     (1000)    13004 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_tx.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     2563 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_v1_0_0.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     1073 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_v1_3_0.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     3731 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_serializers.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     3711 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_signatures.py
--rw-rw-r--   0 awais     (1000) awais     (1000)      287 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/safe/tests/utils.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.786044 vanar-safe-eth-py-1.0.0/gnosis/util/
--rw-rw-r--   0 awais     (1000) awais     (1000)       83 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/util/__init__.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     1003 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/util/http.py
--rw-rw-r--   0 awais     (1000) awais     (1000)      450 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/gnosis/util/util.py
--rw-rw-r--   0 awais     (1000) awais     (1000)     2479 2024-05-29 08:41:05.786044 vanar-safe-eth-py-1.0.0/setup.cfg
--rw-rw-r--   0 awais     (1000) awais     (1000)       69 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.0.0/setup.py
-drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-29 08:41:05.786044 vanar-safe-eth-py-1.0.0/vanar_safe_eth_py.egg-info/
--rw-rw-r--   0 awais     (1000) awais     (1000)     8284 2024-05-29 08:41:05.000000 vanar-safe-eth-py-1.0.0/vanar_safe_eth_py.egg-info/PKG-INFO
--rw-rw-r--   0 awais     (1000) awais     (1000)     7438 2024-05-29 08:41:05.000000 vanar-safe-eth-py-1.0.0/vanar_safe_eth_py.egg-info/SOURCES.txt
--rw-rw-r--   0 awais     (1000) awais     (1000)        1 2024-05-29 08:41:05.000000 vanar-safe-eth-py-1.0.0/vanar_safe_eth_py.egg-info/dependency_links.txt
--rw-rw-r--   0 awais     (1000) awais     (1000)      129 2024-05-29 08:41:05.000000 vanar-safe-eth-py-1.0.0/vanar_safe_eth_py.egg-info/requires.txt
--rw-rw-r--   0 awais     (1000) awais     (1000)        7 2024-05-29 08:41:05.000000 vanar-safe-eth-py-1.0.0/vanar_safe_eth_py.egg-info/top_level.txt
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.325938 vanar-safe-eth-py-1.1.0/
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1082 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/LICENSE
+-rw-rw-r--   0 awais     (1000) awais     (1000)       71 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/MANIFEST.in
+-rw-rw-r--   0 awais     (1000) awais     (1000)     8308 2024-05-31 04:25:13.325938 vanar-safe-eth-py-1.1.0/PKG-INFO
+-rw-rw-r--   0 awais     (1000) awais     (1000)     5786 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/README.rst
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.173936 vanar-safe-eth-py-1.1.0/docs/
+-rw-rw-r--   0 awais     (1000) awais     (1000)      638 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/docs/Makefile
+-rw-rw-r--   0 awais     (1000) awais     (1000)      799 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/docs/make.bat
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.177936 vanar-safe-eth-py-1.1.0/docs/source/
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1995 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/docs/source/conf.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1162 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/docs/source/gnosis.eth.clients.rst
+-rw-rw-r--   0 awais     (1000) awais     (1000)      183 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/docs/source/gnosis.eth.contracts.rst
+-rw-rw-r--   0 awais     (1000) awais     (1000)      954 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/docs/source/gnosis.eth.django.rst
+-rw-rw-r--   0 awais     (1000) awais     (1000)      177 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/docs/source/gnosis.eth.eip712.rst
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1198 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/docs/source/gnosis.eth.oracles.abis.rst
+-rw-rw-r--   0 awais     (1000) awais     (1000)      450 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/docs/source/gnosis.eth.oracles.rst
+-rw-rw-r--   0 awais     (1000) awais     (1000)      936 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/docs/source/gnosis.eth.rst
+-rw-rw-r--   0 awais     (1000) awais     (1000)      226 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/docs/source/gnosis.rst
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1852 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/docs/source/gnosis.safe.rst
+-rw-rw-r--   0 awais     (1000) awais     (1000)      894 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/docs/source/index.rst
+-rw-rw-r--   0 awais     (1000) awais     (1000)       55 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/docs/source/modules.rst
+-rw-rw-r--   0 awais     (1000) awais     (1000)     9218 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/docs/source/quickstart.rst
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.177936 vanar-safe-eth-py-1.1.0/gnosis/
+-rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/__init__.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.177936 vanar-safe-eth-py-1.1.0/gnosis/cowsap/
+-rw-rw-r--   0 awais     (1000) awais     (1000)      156 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/cowsap/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     8465 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/cowsap/cow_swap_api.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     2700 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/cowsap/order.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.177936 vanar-safe-eth-py-1.1.0/gnosis/cowsap/tests/
+-rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/cowsap/tests/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     5604 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/cowsap/tests/test_cow_swap_api.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.177936 vanar-safe-eth-py-1.1.0/gnosis/eth/
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1064 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/__init__.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.177936 vanar-safe-eth-py-1.1.0/gnosis/eth/account_abstraction/
+-rw-rw-r--   0 awais     (1000) awais     (1000)      366 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/account_abstraction/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     7060 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/account_abstraction/bundler_client.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)      986 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/account_abstraction/constants.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)      208 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/account_abstraction/exceptions.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     8899 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/account_abstraction/user_operation.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     3371 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/account_abstraction/user_operation_receipt.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.177936 vanar-safe-eth-py-1.1.0/gnosis/eth/clients/
+-rw-rw-r--   0 awais     (1000) awais     (1000)      878 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/clients/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     9846 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/clients/blockscout_client.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)      194 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/clients/contract_metadata.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     4922 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/clients/ens_client.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     9880 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/clients/etherscan_client.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     3433 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/clients/sourcify_client.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1020 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/constants.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.177936 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/
+-rw-rw-r--   0 awais     (1000) awais     (1000)    10273 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/__init__.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.305937 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/
+-rw-rw-r--   0 awais     (1000) awais     (1000)   328664 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/CPKFactory.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)    28908 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)    29485 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)    26897 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/DelegateConstructorProxy.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)    29068 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/ERC1155.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)    54748 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/ERC20.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)    89890 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/ERC20TestToken.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)   622260 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/ERC721.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)   983403 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)  1158944 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)  1347363 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)   119875 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)    19886 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/MultiSend.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)    78793 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/PayingProxy.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)   136946 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)   288861 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)    18975 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)    15538 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)    32495 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/Proxy_V1_0_0.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)    39032 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/Proxy_V1_1_1.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1862 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/Proxy_V1_3_0.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1849 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/Proxy_V1_4_1.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)   121611 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/Safe_V1_4_1.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)     5069 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/SignMessageLib.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)     4913 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     7351 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/kyber_network_proxy.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)    19012 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/multicall.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    17165 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/uniswap_exchange.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)     2480 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/uniswap_factory.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)     2242 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/uniswap_v2_factory.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)     8293 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/uniswap_v2_pair.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)    11889 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/uniswap_v2_router.json
+-rw-rw-r--   0 awais     (1000) awais     (1000)      954 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/contract_base.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.309937 vanar-safe-eth-py-1.1.0/gnosis/eth/django/
+-rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/django/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     3735 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/django/admin.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)      269 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/django/filters.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     2435 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/django/forms.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     9936 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/django/models.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     6191 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/django/serializers.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.309937 vanar-safe-eth-py-1.1.0/gnosis/eth/django/tests/
+-rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/django/tests/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)      711 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/django/tests/models.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     3028 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/django/tests/test_forms.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     8621 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/django/tests/test_models.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     7877 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/django/tests/test_serializers.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)      484 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/django/tests/test_validators.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)      320 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/django/validators.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.309937 vanar-safe-eth-py-1.1.0/gnosis/eth/eip712/
+-rw-rw-r--   0 awais     (1000) awais     (1000)     5915 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/eip712/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    82106 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/ethereum_client.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    35780 2024-05-28 14:21:08.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/ethereum_network.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1332 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/exceptions.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    13617 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/multicall.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.309937 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1093 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/__init__.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.313937 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/
+-rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    15986 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/aave_abis.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    30036 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/balancer_abis.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    29731 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/cream_abis.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    27567 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/curve_abis.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    25872 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/mooniswap_abis.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)      239 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/superfluid_abis.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    45208 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/uniswap_v3.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    36257 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/yearn_abis.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1464 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/zerion_abis.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     2375 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/cowswap.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)      161 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/exceptions.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.313937 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/helpers/
+-rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/helpers/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     5856 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/helpers/curve_gauge_list.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     4117 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/kyber.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    32169 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/oracles.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1677 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/superfluid.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1516 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/sushiswap.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     7154 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/uniswap_v3.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1064 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/utils.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.313937 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/
+-rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/__init__.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.313937 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/account_abstraction/
+-rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/account_abstraction/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     6695 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/account_abstraction/test_bundler_client.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     3593 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/account_abstraction/test_e2e_bundler_client.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1316 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/account_abstraction/test_user_operation.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)      947 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/account_abstraction/test_user_operation_receipt.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.313937 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/clients/
+-rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/clients/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)   107388 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/clients/mocks.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1047 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/clients/test_blockscout_client.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     6185 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/clients/test_ens_client.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1686 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/clients/test_etherscan_client.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     2845 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/clients/test_sourcify_client.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.313937 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/eip712/
+-rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/eip712/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    13327 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/eip712/test_eip712.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     3189 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/ethereum_test_case.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.317937 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/mocks/
+-rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/mocks/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    33073 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/mocks/mock_bundler.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    31306 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/mocks/mock_internal_txs.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    10570 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/mocks/mock_log_receipts.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)   792720 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/mocks/mock_trace_block.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    92795 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/mocks/mock_trace_filter.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)   171076 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/mocks/mock_trace_transaction.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.317937 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/oracles/
+-rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/oracles/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     2706 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/oracles/test_cowswap.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1820 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/oracles/test_kyber.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1460 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/oracles/test_superfluid.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     2043 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/oracles/test_sushiswap.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     3544 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/oracles/test_uniswap_v3.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    61025 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/test_ethereum_client.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     7087 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/test_multicall.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    21137 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/test_oracles.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     7287 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/test_utils.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     5069 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/tests/utils.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)      390 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/typing.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     6977 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/eth/utils.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.317937 vanar-safe-eth-py-1.1.0/gnosis/safe/
+-rw-rw-r--   0 awais     (1000) awais     (1000)      742 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/__init__.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.317937 vanar-safe-eth-py-1.1.0/gnosis/safe/account_abstraction/
+-rw-rw-r--   0 awais     (1000) awais     (1000)      101 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/account_abstraction/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     5647 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/account_abstraction/safe_operation.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    68974 2024-05-31 04:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/addresses.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.321937 vanar-safe-eth-py-1.1.0/gnosis/safe/api/
+-rw-rw-r--   0 awais     (1000) awais     (1000)      186 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/api/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     2224 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/api/base_api.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.321937 vanar-safe-eth-py-1.1.0/gnosis/safe/api/transaction_service_api/
+-rw-rw-r--   0 awais     (1000) awais     (1000)      103 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/api/transaction_service_api/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    14431 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/api/transaction_service_api/transaction_service_api.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1784 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/api/transaction_service_api/transaction_service_messages.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)      252 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/api/transaction_service_api/transaction_service_tx.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)      105 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/enums.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1451 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/exceptions.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    11459 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/multi_send.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    10479 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/proxy_factory.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    36823 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/safe.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    11975 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/safe_create2_tx.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     9736 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/safe_creator.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)   157670 2024-05-31 04:24:24.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/safe_deployments.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    12587 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/safe_signature.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    17225 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/safe_tx.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     4194 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/serializers.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     2000 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/signatures.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.321937 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/
+-rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/__init__.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.321937 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/account_abstraction/
+-rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/account_abstraction/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     3469 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/account_abstraction/test_safe_operation.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.321937 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/api/
+-rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/api/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     5341 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/api/test_transaction_service_api.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    20692 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/safe_test_case.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1398 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_addresses.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    10515 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_multi_send.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.321937 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_proxy_factory/
+-rw-rw-r--   0 awais     (1000) awais     (1000)        0 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_proxy_factory/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     7798 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    33486 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_safe.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    16674 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_safe_create2_tx.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    18510 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_safe_signature.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)    13004 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_safe_tx.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     2563 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_safe_v1_0_0.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1073 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_safe_v1_3_0.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     3731 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_serializers.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     3711 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_signatures.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)      287 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/safe/tests/utils.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.325938 vanar-safe-eth-py-1.1.0/gnosis/util/
+-rw-rw-r--   0 awais     (1000) awais     (1000)       83 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/util/__init__.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     1003 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/util/http.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)      450 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/gnosis/util/util.py
+-rw-rw-r--   0 awais     (1000) awais     (1000)     2503 2024-05-31 04:25:13.325938 vanar-safe-eth-py-1.1.0/setup.cfg
+-rw-rw-r--   0 awais     (1000) awais     (1000)       69 2024-05-28 14:17:44.000000 vanar-safe-eth-py-1.1.0/setup.py
+drwxrwxr-x   0 awais     (1000) awais     (1000)        0 2024-05-31 04:25:13.325938 vanar-safe-eth-py-1.1.0/vanar_safe_eth_py.egg-info/
+-rw-rw-r--   0 awais     (1000) awais     (1000)     8308 2024-05-31 04:25:13.000000 vanar-safe-eth-py-1.1.0/vanar_safe_eth_py.egg-info/PKG-INFO
+-rw-rw-r--   0 awais     (1000) awais     (1000)     7438 2024-05-31 04:25:13.000000 vanar-safe-eth-py-1.1.0/vanar_safe_eth_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 awais     (1000) awais     (1000)        1 2024-05-31 04:25:13.000000 vanar-safe-eth-py-1.1.0/vanar_safe_eth_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 awais     (1000) awais     (1000)      129 2024-05-31 04:25:13.000000 vanar-safe-eth-py-1.1.0/vanar_safe_eth_py.egg-info/requires.txt
+-rw-rw-r--   0 awais     (1000) awais     (1000)        7 2024-05-31 04:25:13.000000 vanar-safe-eth-py-1.1.0/vanar_safe_eth_py.egg-info/top_level.txt
```

### Comparing `vanar-safe-eth-py-1.0.0/LICENSE` & `vanar-safe-eth-py-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/PKG-INFO` & `vanar-safe-eth-py-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vanar-safe-eth-py
-Version: 1.0.0
-Summary: Safe Ecosystem Foundation utilities for Ethereum projects
+Version: 1.1.0
+Summary: Safe Ecosystem Foundation utilities for Ethereum projects (including Vanar Chain)
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
 Project-URL: Tracker, https://github.com/safe-global/safe-eth-py/issues
```

### Comparing `vanar-safe-eth-py-1.0.0/README.rst` & `vanar-safe-eth-py-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/docs/Makefile` & `vanar-safe-eth-py-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/docs/make.bat` & `vanar-safe-eth-py-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/docs/source/conf.py` & `vanar-safe-eth-py-1.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/docs/source/gnosis.eth.clients.rst` & `vanar-safe-eth-py-1.1.0/docs/source/gnosis.eth.clients.rst`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/docs/source/gnosis.eth.django.rst` & `vanar-safe-eth-py-1.1.0/docs/source/gnosis.eth.django.rst`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/docs/source/gnosis.eth.oracles.abis.rst` & `vanar-safe-eth-py-1.1.0/docs/source/gnosis.eth.oracles.abis.rst`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/docs/source/gnosis.eth.rst` & `vanar-safe-eth-py-1.1.0/docs/source/gnosis.eth.rst`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/docs/source/gnosis.safe.rst` & `vanar-safe-eth-py-1.1.0/docs/source/gnosis.safe.rst`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/docs/source/index.rst` & `vanar-safe-eth-py-1.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/docs/source/quickstart.rst` & `vanar-safe-eth-py-1.1.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/cowsap/cow_swap_api.py` & `vanar-safe-eth-py-1.1.0/gnosis/cowsap/cow_swap_api.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/cowsap/order.py` & `vanar-safe-eth-py-1.1.0/gnosis/cowsap/order.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/cowsap/tests/test_cow_swap_api.py` & `vanar-safe-eth-py-1.1.0/gnosis/cowsap/tests/test_cow_swap_api.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/__init__.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/__init__.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/bundler_client.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/account_abstraction/bundler_client.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/constants.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/account_abstraction/constants.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/user_operation.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/account_abstraction/user_operation.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/account_abstraction/user_operation_receipt.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/account_abstraction/user_operation_receipt.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/clients/__init__.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/clients/blockscout_client.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/clients/blockscout_client.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/clients/ens_client.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/clients/ens_client.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/clients/etherscan_client.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/clients/etherscan_client.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/clients/sourcify_client.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/clients/sourcify_client.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/constants.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/constants.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/__init__.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/CPKFactory.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/CPKFactory.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/CompatibilityFallbackHandler_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/DelegateConstructorProxy.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/DelegateConstructorProxy.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ERC1155.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/ERC1155.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ERC20.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/ERC20.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ERC20TestToken.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/ERC20TestToken.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ERC721.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/ERC721.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/GnosisSafe_V0_0_1.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/GnosisSafe_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/GnosisSafe_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/GnosisSafe_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/MultiSend.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/MultiSend.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/PayingProxy.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/PayingProxy.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/ProxyFactory_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/ProxyFactory_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/ProxyFactory_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/ProxyFactory_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Proxy_V1_0_0.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/Proxy_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Proxy_V1_1_1.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/Proxy_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Proxy_V1_3_0.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/Proxy_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Proxy_V1_4_1.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/Proxy_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/Safe_V1_4_1.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/Safe_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/SignMessageLib.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/SignMessageLib.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/SimulateTxAccessor_V1_4_1.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/kyber_network_proxy.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/kyber_network_proxy.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/multicall.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/multicall.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_exchange.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/uniswap_exchange.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_factory.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/uniswap_factory.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_v2_factory.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/uniswap_v2_factory.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_v2_pair.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/uniswap_v2_pair.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/abis/uniswap_v2_router.json` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/abis/uniswap_v2_router.json`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/contracts/contract_base.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/contracts/contract_base.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/django/admin.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/django/admin.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/django/forms.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/django/forms.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/django/models.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/django/models.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/django/serializers.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/django/serializers.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/django/tests/models.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/django/tests/models.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/django/tests/test_forms.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/django/tests/test_models.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/django/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/django/tests/test_serializers.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/django/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/eip712/__init__.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/eip712/__init__.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/ethereum_client.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/ethereum_client.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/ethereum_network.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/ethereum_network.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/exceptions.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/exceptions.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/multicall.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/multicall.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/__init__.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/__init__.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/aave_abis.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/aave_abis.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/balancer_abis.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/balancer_abis.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/cream_abis.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/cream_abis.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/curve_abis.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/curve_abis.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/mooniswap_abis.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/mooniswap_abis.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/uniswap_v3.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/yearn_abis.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/yearn_abis.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/abis/zerion_abis.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/abis/zerion_abis.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/cowswap.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/cowswap.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/helpers/curve_gauge_list.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/helpers/curve_gauge_list.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/kyber.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/kyber.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/oracles.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/oracles.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/superfluid.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/superfluid.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/sushiswap.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/sushiswap.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/uniswap_v3.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/oracles/utils.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/oracles/utils.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/test_bundler_client.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/account_abstraction/test_bundler_client.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/test_e2e_bundler_client.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/account_abstraction/test_e2e_bundler_client.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/test_user_operation.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/account_abstraction/test_user_operation.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/account_abstraction/test_user_operation_receipt.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/account_abstraction/test_user_operation_receipt.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/clients/mocks.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/clients/mocks.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/clients/test_blockscout_client.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/clients/test_blockscout_client.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/clients/test_ens_client.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/clients/test_ens_client.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/clients/test_etherscan_client.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/clients/test_etherscan_client.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/clients/test_sourcify_client.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/clients/test_sourcify_client.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/eip712/test_eip712.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/eip712/test_eip712.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/ethereum_test_case.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/ethereum_test_case.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_bundler.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/mocks/mock_bundler.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_internal_txs.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/mocks/mock_internal_txs.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_log_receipts.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/mocks/mock_log_receipts.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_trace_block.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/mocks/mock_trace_block.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_trace_filter.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/mocks/mock_trace_filter.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/mocks/mock_trace_transaction.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/mocks/mock_trace_transaction.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_cowswap.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/oracles/test_cowswap.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_kyber.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/oracles/test_kyber.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_superfluid.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/oracles/test_superfluid.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_sushiswap.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/oracles/test_sushiswap.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/oracles/test_uniswap_v3.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/oracles/test_uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/test_ethereum_client.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/test_ethereum_client.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/test_multicall.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/test_multicall.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/test_oracles.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/test_oracles.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/test_utils.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/tests/utils.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/tests/utils.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/eth/utils.py` & `vanar-safe-eth-py-1.1.0/gnosis/eth/utils.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/__init__.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/__init__.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/account_abstraction/safe_operation.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/account_abstraction/safe_operation.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/addresses.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/addresses.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,14 +147,18 @@
         (
             "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
             79000,
             "1.3.0+L2",
         ),  # default singleton address
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 79000, "1.3.0"),
     ],
+    EthereumNetwork.VANAR_MAINNET: [
+        ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 1716178, "1.3.0+L2"),
+        ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 1716181, "1.3.0"),
+    ],
     EthereumNetwork.VANAR_VANGUARD: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 3836806, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 3836810, "1.3.0"),
     ],
     EthereumNetwork.MUMBAI: [
         ("0x3E5c63644E683549055b9Be8653de26E0B4CD36E", 13736914, "1.3.0+L2"),
         ("0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552", 13736914, "1.3.0"),
```

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/api/base_api.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/api/base_api.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/api/transaction_service_api/transaction_service_api.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/api/transaction_service_api/transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/api/transaction_service_api/transaction_service_messages.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/api/transaction_service_api/transaction_service_messages.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/exceptions.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/exceptions.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/multi_send.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/multi_send.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/proxy_factory.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/proxy_factory.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/safe.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/safe.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/safe_create2_tx.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/safe_creator.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/safe_creator.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/safe_deployments.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/safe_deployments.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,14 +190,15 @@
             "2008": "0xf48f2B2d2a534e402487b3ee7C18c33Aec0Fe5e4",
             "2019": "0xf48f2B2d2a534e402487b3ee7C18c33Aec0Fe5e4",
             "2020": "0xf48f2B2d2a534e402487b3ee7C18c33Aec0Fe5e4",
             "2021": "0xf48f2B2d2a534e402487b3ee7C18c33Aec0Fe5e4",
             "2221": "0xf48f2B2d2a534e402487b3ee7C18c33Aec0Fe5e4",
             "2222": "0xf48f2B2d2a534e402487b3ee7C18c33Aec0Fe5e4",
             "2331": "0xf48f2B2d2a534e402487b3ee7C18c33Aec0Fe5e4",
+            "2040": "0xf48f2B2d2a534e402487b3ee7C18c33Aec0Fe5e4",
             "2358": "0x017062a1dE2FE6b99BE3d9d37841FeD19F573804",
             "3737": "0xf48f2B2d2a534e402487b3ee7C18c33Aec0Fe5e4",
             "3776": "0xf48f2B2d2a534e402487b3ee7C18c33Aec0Fe5e4",
             "4002": "0xf48f2B2d2a534e402487b3ee7C18c33Aec0Fe5e4",
             "4157": "0x017062a1dE2FE6b99BE3d9d37841FeD19F573804",
             "4202": "0xf48f2B2d2a534e402487b3ee7C18c33Aec0Fe5e4",
             "4337": "0xf48f2B2d2a534e402487b3ee7C18c33Aec0Fe5e4",
@@ -407,14 +408,15 @@
             "2008": "0x7cbB62EaA69F79e6873cD1ecB2392971036cFAa4",
             "2019": "0x7cbB62EaA69F79e6873cD1ecB2392971036cFAa4",
             "2020": "0x7cbB62EaA69F79e6873cD1ecB2392971036cFAa4",
             "2021": "0x7cbB62EaA69F79e6873cD1ecB2392971036cFAa4",
             "2221": "0x7cbB62EaA69F79e6873cD1ecB2392971036cFAa4",
             "2222": "0x7cbB62EaA69F79e6873cD1ecB2392971036cFAa4",
             "2331": "0x7cbB62EaA69F79e6873cD1ecB2392971036cFAa4",
+            "2040": "0x7cbB62EaA69F79e6873cD1ecB2392971036cFAa4",
             "2358": "0xB19D6FFc2182150F8Eb585b79D4ABcd7C5640A9d",
             "3737": "0x7cbB62EaA69F79e6873cD1ecB2392971036cFAa4",
             "3776": "0x7cbB62EaA69F79e6873cD1ecB2392971036cFAa4",
             "4002": "0x7cbB62EaA69F79e6873cD1ecB2392971036cFAa4",
             "4157": "0xB19D6FFc2182150F8Eb585b79D4ABcd7C5640A9d",
             "4202": "0x7cbB62EaA69F79e6873cD1ecB2392971036cFAa4",
             "4337": "0x7cbB62EaA69F79e6873cD1ecB2392971036cFAa4",
@@ -624,14 +626,15 @@
             "2008": "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
             "2019": "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
             "2020": "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
             "2021": "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
             "2221": "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
             "2222": "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
             "2331": "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
+            "2040": "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
             "2358": "0x69f4D1788e39c87893C980c06EdF4b7f686e2938",
             "3737": "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
             "3776": "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
             "4002": "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
             "4157": "0x69f4D1788e39c87893C980c06EdF4b7f686e2938",
             "4202": "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
             "4337": "0xd9Db270c1B5E3Bd161E8c8503c55cEABeE709552",
@@ -841,14 +844,15 @@
             "2008": "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
             "2019": "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
             "2020": "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
             "2021": "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
             "2221": "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
             "2222": "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
             "2331": "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
+            "2040": "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
             "2358": "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA",
             "3737": "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
             "3776": "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
             "4002": "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
             "4157": "0xfb1bffC9d739B8D520DaF37dF666da4C687191EA",
             "4202": "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
             "4337": "0x3E5c63644E683549055b9Be8653de26E0B4CD36E",
@@ -1058,14 +1062,15 @@
             "2008": "0xA238CBeb142c10Ef7Ad8442C6D1f9E89e07e7761",
             "2019": "0xA238CBeb142c10Ef7Ad8442C6D1f9E89e07e7761",
             "2020": "0xA238CBeb142c10Ef7Ad8442C6D1f9E89e07e7761",
             "2021": "0xA238CBeb142c10Ef7Ad8442C6D1f9E89e07e7761",
             "2221": "0xA238CBeb142c10Ef7Ad8442C6D1f9E89e07e7761",
             "2222": "0xA238CBeb142c10Ef7Ad8442C6D1f9E89e07e7761",
             "2331": "0xA238CBeb142c10Ef7Ad8442C6D1f9E89e07e7761",
+            "2040": "0xA238CBeb142c10Ef7Ad8442C6D1f9E89e07e7761",
             "2358": "0x998739BFdAAdde7C933B942a68053933098f9EDa",
             "3737": "0xA238CBeb142c10Ef7Ad8442C6D1f9E89e07e7761",
             "3776": "0xA238CBeb142c10Ef7Ad8442C6D1f9E89e07e7761",
             "4002": "0xA238CBeb142c10Ef7Ad8442C6D1f9E89e07e7761",
             "4157": "0x998739BFdAAdde7C933B942a68053933098f9EDa",
             "4202": "0xA238CBeb142c10Ef7Ad8442C6D1f9E89e07e7761",
             "4337": "0xA238CBeb142c10Ef7Ad8442C6D1f9E89e07e7761",
@@ -1275,14 +1280,15 @@
             "2008": "0x40A2aCCbd92BCA938b02010E17A5b8929b49130D",
             "2019": "0x40A2aCCbd92BCA938b02010E17A5b8929b49130D",
             "2020": "0x40A2aCCbd92BCA938b02010E17A5b8929b49130D",
             "2021": "0x40A2aCCbd92BCA938b02010E17A5b8929b49130D",
             "2221": "0x40A2aCCbd92BCA938b02010E17A5b8929b49130D",
             "2222": "0x40A2aCCbd92BCA938b02010E17A5b8929b49130D",
             "2331": "0x40A2aCCbd92BCA938b02010E17A5b8929b49130D",
+            "2040": "0x40A2aCCbd92BCA938b02010E17A5b8929b49130D",
             "2358": "0xA1dabEF33b3B82c7814B6D82A79e50F4AC44102B",
             "3737": "0x40A2aCCbd92BCA938b02010E17A5b8929b49130D",
             "3776": "0x40A2aCCbd92BCA938b02010E17A5b8929b49130D",
             "4002": "0x40A2aCCbd92BCA938b02010E17A5b8929b49130D",
             "4157": "0xA1dabEF33b3B82c7814B6D82A79e50F4AC44102B",
             "4202": "0x40A2aCCbd92BCA938b02010E17A5b8929b49130D",
             "4337": "0x40A2aCCbd92BCA938b02010E17A5b8929b49130D",
@@ -1492,14 +1498,15 @@
             "2008": "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
             "2019": "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
             "2020": "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
             "2021": "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
             "2221": "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
             "2222": "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
             "2331": "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
+            "2040": "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
             "2358": "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
             "3737": "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
             "3776": "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
             "4002": "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
             "4157": "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
             "4202": "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
             "4337": "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
@@ -1709,14 +1716,15 @@
             "2008": "0xA65387F16B013cf2Af4605Ad8aA5ec25a2cbA3a2",
             "2019": "0xA65387F16B013cf2Af4605Ad8aA5ec25a2cbA3a2",
             "2020": "0xA65387F16B013cf2Af4605Ad8aA5ec25a2cbA3a2",
             "2021": "0xA65387F16B013cf2Af4605Ad8aA5ec25a2cbA3a2",
             "2221": "0xA65387F16B013cf2Af4605Ad8aA5ec25a2cbA3a2",
             "2222": "0xA65387F16B013cf2Af4605Ad8aA5ec25a2cbA3a2",
             "2331": "0xA65387F16B013cf2Af4605Ad8aA5ec25a2cbA3a2",
+            "2040": "0xA65387F16B013cf2Af4605Ad8aA5ec25a2cbA3a2",
             "2358": "0x98FFBBF51bb33A056B08ddf711f289936AafF717",
             "3737": "0xA65387F16B013cf2Af4605Ad8aA5ec25a2cbA3a2",
             "3776": "0xA65387F16B013cf2Af4605Ad8aA5ec25a2cbA3a2",
             "4002": "0xA65387F16B013cf2Af4605Ad8aA5ec25a2cbA3a2",
             "4157": "0x98FFBBF51bb33A056B08ddf711f289936AafF717",
             "4202": "0xA65387F16B013cf2Af4605Ad8aA5ec25a2cbA3a2",
             "4337": "0xA65387F16B013cf2Af4605Ad8aA5ec25a2cbA3a2",
@@ -1926,14 +1934,15 @@
             "2008": "0x59AD6735bCd8152B84860Cb256dD9e96b85F69Da",
             "2019": "0x59AD6735bCd8152B84860Cb256dD9e96b85F69Da",
             "2020": "0x59AD6735bCd8152B84860Cb256dD9e96b85F69Da",
             "2021": "0x59AD6735bCd8152B84860Cb256dD9e96b85F69Da",
             "2221": "0x59AD6735bCd8152B84860Cb256dD9e96b85F69Da",
             "2222": "0x59AD6735bCd8152B84860Cb256dD9e96b85F69Da",
             "2331": "0x59AD6735bCd8152B84860Cb256dD9e96b85F69Da",
+            "2040": "0x59AD6735bCd8152B84860Cb256dD9e96b85F69Da",
             "2358": "0x727a77a074D1E6c4530e814F89E618a3298FC044",
             "3737": "0x59AD6735bCd8152B84860Cb256dD9e96b85F69Da",
             "3776": "0x59AD6735bCd8152B84860Cb256dD9e96b85F69Da",
             "4002": "0x59AD6735bCd8152B84860Cb256dD9e96b85F69Da",
             "4157": "0x727a77a074D1E6c4530e814F89E618a3298FC044",
             "4202": "0x59AD6735bCd8152B84860Cb256dD9e96b85F69Da",
             "4337": "0x59AD6735bCd8152B84860Cb256dD9e96b85F69Da",
```

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/safe_signature.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/safe_signature.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/safe_tx.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/safe_tx.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/serializers.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/serializers.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/signatures.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/signatures.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/tests/account_abstraction/test_safe_operation.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/tests/account_abstraction/test_safe_operation.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/tests/api/test_transaction_service_api.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/tests/api/test_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/tests/safe_test_case.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/tests/safe_test_case.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_addresses.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_addresses.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_multi_send.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_multi_send.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_proxy_factory/test_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_safe.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_create2_tx.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_signature.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_safe_signature.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_tx.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_safe_tx.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_v1_0_0.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_safe_v1_0_0.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_safe_v1_3_0.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_safe_v1_3_0.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_serializers.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/safe/tests/test_signatures.py` & `vanar-safe-eth-py-1.1.0/gnosis/safe/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/gnosis/util/http.py` & `vanar-safe-eth-py-1.1.0/gnosis/util/http.py`

 * *Files identical despite different names*

### Comparing `vanar-safe-eth-py-1.0.0/setup.cfg` & `vanar-safe-eth-py-1.1.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = vanar-safe-eth-py
-version = 1.0.0
-description = Safe Ecosystem Foundation utilities for Ethereum projects
+version = 1.1.0
+description = Safe Ecosystem Foundation utilities for Ethereum projects (including Vanar Chain)
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 keywords = 
 	ethereum
 	web3
 	django
 	safe
```

### Comparing `vanar-safe-eth-py-1.0.0/vanar_safe_eth_py.egg-info/PKG-INFO` & `vanar-safe-eth-py-1.1.0/vanar_safe_eth_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vanar-safe-eth-py
-Version: 1.0.0
-Summary: Safe Ecosystem Foundation utilities for Ethereum projects
+Version: 1.1.0
+Summary: Safe Ecosystem Foundation utilities for Ethereum projects (including Vanar Chain)
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
 Project-URL: Tracker, https://github.com/safe-global/safe-eth-py/issues
```

### Comparing `vanar-safe-eth-py-1.0.0/vanar_safe_eth_py.egg-info/SOURCES.txt` & `vanar-safe-eth-py-1.1.0/vanar_safe_eth_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

