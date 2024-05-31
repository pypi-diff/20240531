# Comparing `tmp/xchainpy2_crypto-0.0.6.tar.gz` & `tmp/xchainpy2_crypto-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchainpy2_crypto-0.0.6.tar", last modified: Sun Jan  7 19:34:59 2024, max compression
+gzip compressed data, was "xchainpy2_crypto-0.0.7.tar", last modified: Fri May 31 14:22:53 2024, max compression
```

## Comparing `xchainpy2_crypto-0.0.6.tar` & `xchainpy2_crypto-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-07 19:34:59.427456 xchainpy2_crypto-0.0.6/
--rw-r--r--   0 tirinox    (501) staff       (20)     1086 2023-04-22 16:09:04.000000 xchainpy2_crypto-0.0.6/LICENSE
--rw-r--r--   0 tirinox    (501) staff       (20)     1786 2024-01-07 19:34:59.427217 xchainpy2_crypto-0.0.6/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)      740 2023-04-22 16:09:04.000000 xchainpy2_crypto-0.0.6/README.md
--rw-r--r--   0 tirinox    (501) staff       (20)     1320 2024-01-07 19:34:28.000000 xchainpy2_crypto-0.0.6/pyproject.toml
--rw-r--r--   0 tirinox    (501) staff       (20)       38 2024-01-07 19:34:59.427519 xchainpy2_crypto-0.0.6/setup.cfg
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-07 19:34:59.424756 xchainpy2_crypto-0.0.6/xchainpy2_crypto/
--rw-r--r--   0 tirinox    (501) staff       (20)       65 2023-04-22 16:40:51.000000 xchainpy2_crypto-0.0.6/xchainpy2_crypto/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)      119 2023-04-22 16:09:04.000000 xchainpy2_crypto-0.0.6/xchainpy2_crypto/keys.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4698 2024-01-06 10:52:21.000000 xchainpy2_crypto-0.0.6/xchainpy2_crypto/keystore.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-07 19:34:59.426420 xchainpy2_crypto-0.0.6/xchainpy2_crypto/tests/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-04-22 19:35:45.000000 xchainpy2_crypto-0.0.6/xchainpy2_crypto/tests/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1557 2023-06-01 10:46:54.000000 xchainpy2_crypto-0.0.6/xchainpy2_crypto/tests/test_address.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1778 2024-01-06 10:55:58.000000 xchainpy2_crypto-0.0.6/xchainpy2_crypto/tests/test_keystore.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1817 2023-05-29 06:13:27.000000 xchainpy2_crypto-0.0.6/xchainpy2_crypto/tests/test_mnemonic.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4005 2023-12-01 19:24:10.000000 xchainpy2_crypto-0.0.6/xchainpy2_crypto/utils.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-07 19:34:59.426758 xchainpy2_crypto-0.0.6/xchainpy2_crypto.egg-info/
--rw-r--r--   0 tirinox    (501) staff       (20)     1786 2024-01-07 19:34:59.000000 xchainpy2_crypto-0.0.6/xchainpy2_crypto.egg-info/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)      494 2024-01-07 19:34:59.000000 xchainpy2_crypto-0.0.6/xchainpy2_crypto.egg-info/SOURCES.txt
--rw-r--r--   0 tirinox    (501) staff       (20)        1 2024-01-07 19:34:59.000000 xchainpy2_crypto-0.0.6/xchainpy2_crypto.egg-info/dependency_links.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       63 2024-01-07 19:34:59.000000 xchainpy2_crypto-0.0.6/xchainpy2_crypto.egg-info/requires.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       17 2024-01-07 19:34:59.000000 xchainpy2_crypto-0.0.6/xchainpy2_crypto.egg-info/top_level.txt
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:22:53.807603 xchainpy2_crypto-0.0.7/
+-rw-r--r--   0 tirinox    (501) staff       (20)     1086 2024-03-03 09:20:52.000000 xchainpy2_crypto-0.0.7/LICENSE
+-rw-r--r--   0 tirinox    (501) staff       (20)     1786 2024-05-31 14:22:53.807398 xchainpy2_crypto-0.0.7/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)      740 2024-03-03 09:20:52.000000 xchainpy2_crypto-0.0.7/README.md
+-rw-r--r--   0 tirinox    (501) staff       (20)     1320 2024-03-07 10:37:31.000000 xchainpy2_crypto-0.0.7/pyproject.toml
+-rw-r--r--   0 tirinox    (501) staff       (20)       38 2024-05-31 14:22:53.807634 xchainpy2_crypto-0.0.7/setup.cfg
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:22:53.805559 xchainpy2_crypto-0.0.7/xchainpy2_crypto/
+-rw-r--r--   0 tirinox    (501) staff       (20)       65 2024-03-07 10:37:31.000000 xchainpy2_crypto-0.0.7/xchainpy2_crypto/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      119 2024-03-07 10:37:31.000000 xchainpy2_crypto-0.0.7/xchainpy2_crypto/keys.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4915 2024-03-07 10:37:31.000000 xchainpy2_crypto-0.0.7/xchainpy2_crypto/keystore.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:22:53.806793 xchainpy2_crypto-0.0.7/xchainpy2_crypto/tests/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2024-03-07 10:37:31.000000 xchainpy2_crypto-0.0.7/xchainpy2_crypto/tests/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1557 2024-03-07 10:37:31.000000 xchainpy2_crypto-0.0.7/xchainpy2_crypto/tests/test_address.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1778 2024-03-07 10:37:31.000000 xchainpy2_crypto-0.0.7/xchainpy2_crypto/tests/test_keystore.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1817 2024-03-07 10:37:31.000000 xchainpy2_crypto-0.0.7/xchainpy2_crypto/tests/test_mnemonic.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4005 2024-03-07 10:37:31.000000 xchainpy2_crypto-0.0.7/xchainpy2_crypto/utils.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:22:53.807031 xchainpy2_crypto-0.0.7/xchainpy2_crypto.egg-info/
+-rw-r--r--   0 tirinox    (501) staff       (20)     1786 2024-05-31 14:22:53.000000 xchainpy2_crypto-0.0.7/xchainpy2_crypto.egg-info/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)      494 2024-05-31 14:22:53.000000 xchainpy2_crypto-0.0.7/xchainpy2_crypto.egg-info/SOURCES.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)        1 2024-05-31 14:22:53.000000 xchainpy2_crypto-0.0.7/xchainpy2_crypto.egg-info/dependency_links.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       63 2024-05-31 14:22:53.000000 xchainpy2_crypto-0.0.7/xchainpy2_crypto.egg-info/requires.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       17 2024-05-31 14:22:53.000000 xchainpy2_crypto-0.0.7/xchainpy2_crypto.egg-info/top_level.txt
```

### Comparing `xchainpy2_crypto-0.0.6/LICENSE` & `xchainpy2_crypto-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xchainpy2_crypto-0.0.6/PKG-INFO` & `xchainpy2_crypto-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2_crypto
-Version: 0.0.6
+Version: 0.0.7
 Summary: XChainPy2 Crypto utils and keystore management
 Author-email: Tirinox <developer@tirinox.ru>
 License: MIT
 Project-URL: source, https://github.com/tirinox/xchainpy
 Keywords: Crypto,THORChain,Blockchain,XChain
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `xchainpy2_crypto-0.0.6/README.md` & `xchainpy2_crypto-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `xchainpy2_crypto-0.0.6/pyproject.toml` & `xchainpy2_crypto-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xchainpy2_crypto"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "Tirinox", email = "developer@tirinox.ru" },
 ]
 description = "XChainPy2 Crypto utils and keystore management"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["Crypto", "THORChain", "Blockchain", "XChain"]
```

### Comparing `xchainpy2_crypto-0.0.6/xchainpy2_crypto/keystore.py` & `xchainpy2_crypto-0.0.7/xchainpy2_crypto/keystore.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import urandom
 from typing import NamedTuple
 
 from Crypto.Cipher import AES
 from Crypto.Hash import BLAKE2b
 from Crypto.Util import Counter
 
-from .utils import validate_mnemonic
+from .utils import validate_mnemonic, generate_mnemonic
 
 CIPHER = 'aes-128-ctr'
 NBITS = 128
 KDF = 'pbkdf2'
 PRF = 'hmac-sha256'
 DKLEN = 32
 C = 262144
@@ -163,7 +163,12 @@
         if mac != self.mac:
             raise InvalidPasswordException("Invalid password")
 
         ctr = Counter.new(NBITS, initial_value=int(self.cipherparams_iv, 16))
         aes_cipher = AES.new(derived_key[0:16], AES.MODE_CTR, counter=ctr)
         phrase = aes_cipher.decrypt(cipher_bytes)
         return phrase.decode("utf8")
+
+    @classmethod
+    def generate_and_encrypt(cls, password: str, *args, **kwargs):
+        mnemonic = generate_mnemonic(*args, **kwargs)
+        return cls.encrypt_to_keystore(mnemonic, password)
```

### Comparing `xchainpy2_crypto-0.0.6/xchainpy2_crypto/tests/test_address.py` & `xchainpy2_crypto-0.0.7/xchainpy2_crypto/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_crypto-0.0.6/xchainpy2_crypto/tests/test_keystore.py` & `xchainpy2_crypto-0.0.7/xchainpy2_crypto/tests/test_keystore.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_crypto-0.0.6/xchainpy2_crypto/tests/test_mnemonic.py` & `xchainpy2_crypto-0.0.7/xchainpy2_crypto/tests/test_mnemonic.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_crypto-0.0.6/xchainpy2_crypto/utils.py` & `xchainpy2_crypto-0.0.7/xchainpy2_crypto/utils.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_crypto-0.0.6/xchainpy2_crypto.egg-info/PKG-INFO` & `xchainpy2_crypto-0.0.7/xchainpy2_crypto.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2_crypto
-Version: 0.0.6
+Version: 0.0.7
 Summary: XChainPy2 Crypto utils and keystore management
 Author-email: Tirinox <developer@tirinox.ru>
 License: MIT
 Project-URL: source, https://github.com/tirinox/xchainpy
 Keywords: Crypto,THORChain,Blockchain,XChain
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

