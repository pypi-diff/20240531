# Comparing `tmp/suiutils-py-1.0.7.tar.gz` & `tmp/suiutils_py-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suiutils-py-1.0.7.tar", last modified: Thu May  4 20:28:58 2023, max compression
+gzip compressed data, was "suiutils_py-1.0.9.tar", last modified: Thu May 30 22:09:39 2024, max compression
```

## Comparing `suiutils-py-1.0.7.tar` & `suiutils_py-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 guomaoye   (501) staff       (20)        0 2023-05-04 20:28:58.025896 suiutils-py-1.0.7/
--rw-r--r--   0 guomaoye   (501) staff       (20)      301 2023-05-04 20:28:58.025703 suiutils-py-1.0.7/PKG-INFO
--rw-r--r--   0 guomaoye   (501) staff       (20)     2837 2023-05-04 20:28:15.000000 suiutils-py-1.0.7/README.md
--rw-r--r--   0 guomaoye   (501) staff       (20)       38 2023-05-04 20:28:58.025959 suiutils-py-1.0.7/setup.cfg
--rw-r--r--   0 guomaoye   (501) staff       (20)      413 2023-05-04 20:28:48.000000 suiutils-py-1.0.7/setup.py
-drwxr-xr-x   0 guomaoye   (501) staff       (20)        0 2023-05-04 20:28:58.023621 suiutils-py-1.0.7/suiutils_py/
--rw-r--r--   0 guomaoye   (501) staff       (20)       85 2023-05-02 05:04:49.000000 suiutils-py-1.0.7/suiutils_py/__init__.py
--rw-r--r--   0 guomaoye   (501) staff       (20)     1428 2023-05-02 05:04:49.000000 suiutils-py-1.0.7/suiutils_py/models.py
--rw-r--r--   0 guomaoye   (501) staff       (20)    15691 2023-05-02 23:35:01.000000 suiutils-py-1.0.7/suiutils_py/provider.py
--rw-r--r--   0 guomaoye   (501) staff       (20)     1924 2023-05-04 20:18:43.000000 suiutils-py-1.0.7/suiutils_py/rpc_tx_data_serializer.py
--rw-r--r--   0 guomaoye   (501) staff       (20)     1258 2023-05-02 05:04:49.000000 suiutils-py-1.0.7/suiutils_py/signer.py
--rw-r--r--   0 guomaoye   (501) staff       (20)     3543 2023-05-04 20:18:43.000000 suiutils-py-1.0.7/suiutils_py/signer_with_provider.py
--rw-r--r--   0 guomaoye   (501) staff       (20)     1578 2023-05-02 23:37:47.000000 suiutils-py-1.0.7/suiutils_py/wallet.py
-drwxr-xr-x   0 guomaoye   (501) staff       (20)        0 2023-05-04 20:28:58.025433 suiutils-py-1.0.7/suiutils_py.egg-info/
--rw-r--r--   0 guomaoye   (501) staff       (20)      301 2023-05-04 20:28:57.000000 suiutils-py-1.0.7/suiutils_py.egg-info/PKG-INFO
--rw-r--r--   0 guomaoye   (501) staff       (20)      380 2023-05-04 20:28:57.000000 suiutils-py-1.0.7/suiutils_py.egg-info/SOURCES.txt
--rw-r--r--   0 guomaoye   (501) staff       (20)        1 2023-05-04 20:28:57.000000 suiutils-py-1.0.7/suiutils_py.egg-info/dependency_links.txt
--rw-r--r--   0 guomaoye   (501) staff       (20)       13 2023-05-04 20:28:57.000000 suiutils-py-1.0.7/suiutils_py.egg-info/requires.txt
--rw-r--r--   0 guomaoye   (501) staff       (20)       12 2023-05-04 20:28:57.000000 suiutils-py-1.0.7/suiutils_py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 22:09:39.235962 suiutils_py-1.0.9/
+-rw-rw-rw-   0        0        0     3619 2024-05-30 22:09:39.234509 suiutils_py-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2851 2024-05-30 13:32:29.000000 suiutils_py-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-30 22:09:39.235962 suiutils_py-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      967 2024-05-30 22:07:40.000000 suiutils_py-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 22:09:39.228385 suiutils_py-1.0.9/suiutils_py/
+-rw-rw-rw-   0        0        0       85 2024-05-30 13:32:29.000000 suiutils_py-1.0.9/suiutils_py/__init__.py
+-rw-rw-rw-   0        0        0     1428 2024-05-30 13:32:29.000000 suiutils_py-1.0.9/suiutils_py/models.py
+-rw-rw-rw-   0        0        0    15691 2024-05-30 13:32:29.000000 suiutils_py-1.0.9/suiutils_py/provider.py
+-rw-rw-rw-   0        0        0     1924 2024-05-30 13:32:29.000000 suiutils_py-1.0.9/suiutils_py/rpc_tx_data_serializer.py
+-rw-rw-rw-   0        0        0     1258 2024-05-30 13:32:29.000000 suiutils_py-1.0.9/suiutils_py/signer.py
+-rw-rw-rw-   0        0        0     3543 2024-05-30 13:32:29.000000 suiutils_py-1.0.9/suiutils_py/signer_with_provider.py
+-rw-rw-rw-   0        0        0     1578 2024-05-30 13:32:29.000000 suiutils_py-1.0.9/suiutils_py/wallet.py
+drwxrwxrwx   0        0        0        0 2024-05-30 22:09:39.232509 suiutils_py-1.0.9/suiutils_py.egg-info/
+-rw-rw-rw-   0        0        0     3619 2024-05-30 22:09:38.000000 suiutils_py-1.0.9/suiutils_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2024-05-30 22:09:39.000000 suiutils_py-1.0.9/suiutils_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 22:09:38.000000 suiutils_py-1.0.9/suiutils_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2024-05-30 22:09:38.000000 suiutils_py-1.0.9/suiutils_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-30 22:09:38.000000 suiutils_py-1.0.9/suiutils_py.egg-info/top_level.txt
```

### Comparing `suiutils-py-1.0.7/README.md` & `suiutils_py-1.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 this project can only use for some simple methods or transaction
 
-if you want to get more professional and complex methods or programmable transaction
+if you want to get more Professional，Constructable complex methods or Programmable Transaction
 
 please move here and use [pysui](https://github.com/FrankC01/pysui)
 
 
 -------------
 
 Python SDK to interact with Sui Blockchain 
@@ -60,16 +60,16 @@
 random_wallet.get_address()
 >'0x97534f7d430793fa4ff4619a5431c3d72fe8397d'
 ```
 
 ### Providers
 ```python
 # Setup Providers
-rpc_url = "https://fullnode.devnet.sui.io"
-faucet_url ="https://faucet.devnet.sui.io/gas"
+rpc_url = "https://fullnode.testnet.sui.io"
+faucet_url ="https://faucet.testnet.sui.io/gas"
 
 provider = SuiJsonRpcProvider(rpc_url=rpc_url, faucet_url=faucet_url)
 serializer = RpcTxDataSerializer(rpc_url=rpc_url)
 signer = SignerWithProvider(provider=provider, serializer=serializer, signer_wallet=my_wallet)
 ```
 
 ```python
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `suiutils-py-1.0.7/suiutils_py/models.py` & `suiutils_py-1.0.9/suiutils_py/models.py`

 * *Files identical despite different names*

### Comparing `suiutils-py-1.0.7/suiutils_py/provider.py` & `suiutils_py-1.0.9/suiutils_py/provider.py`

 * *Files identical despite different names*

### Comparing `suiutils-py-1.0.7/suiutils_py/rpc_tx_data_serializer.py` & `suiutils_py-1.0.9/suiutils_py/rpc_tx_data_serializer.py`

 * *Files identical despite different names*

### Comparing `suiutils-py-1.0.7/suiutils_py/signer.py` & `suiutils_py-1.0.9/suiutils_py/signer.py`

 * *Files identical despite different names*

### Comparing `suiutils-py-1.0.7/suiutils_py/signer_with_provider.py` & `suiutils_py-1.0.9/suiutils_py/signer_with_provider.py`

 * *Files identical despite different names*

### Comparing `suiutils-py-1.0.7/suiutils_py/wallet.py` & `suiutils_py-1.0.9/suiutils_py/wallet.py`

 * *Files identical despite different names*

