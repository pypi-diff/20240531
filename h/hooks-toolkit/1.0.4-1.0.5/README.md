# Comparing `tmp/hooks_toolkit-1.0.4.tar.gz` & `tmp/hooks_toolkit-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hooks_toolkit-1.0.4.tar", max compression
+gzip compressed data, was "hooks_toolkit-1.0.5.tar", max compression
```

## Comparing `hooks_toolkit-1.0.4.tar` & `hooks_toolkit-1.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     3006 2024-02-02 01:30:41.030882 hooks_toolkit-1.0.4/hooks_toolkit/asyncio_set_hook.py
--rw-r--r--   0        0        0      993 2024-02-02 01:43:45.864461 hooks_toolkit-1.0.4/hooks_toolkit/asyncio_xrpld.py
--rw-r--r--   0        0        0      227 2024-02-01 15:55:33.459231 hooks_toolkit-1.0.4/hooks_toolkit/libs/asyncio/keylet_utils/__init__.py
--rw-r--r--   0        0        0     2750 2024-02-02 01:33:36.214072 hooks_toolkit-1.0.4/hooks_toolkit/libs/asyncio/keylet_utils/execution_utility.py
--rw-r--r--   0        0        0     2000 2024-02-02 01:56:16.002569 hooks_toolkit-1.0.4/hooks_toolkit/libs/asyncio/keylet_utils/state_utility.py
--rw-r--r--   0        0        0        0 2024-02-01 15:58:40.704177 hooks_toolkit-1.0.4/hooks_toolkit/libs/asyncio/xrpl_helpers/__init__.py
--rw-r--r--   0        0        0     2229 2024-02-02 01:28:09.071988 hooks_toolkit-1.0.4/hooks_toolkit/libs/asyncio/xrpl_helpers/fund_system.py
--rw-r--r--   0        0        0     3981 2024-03-11 10:36:58.592137 hooks_toolkit-1.0.4/hooks_toolkit/libs/asyncio/xrpl_helpers/setup.py
--rw-r--r--   0        0        0     8325 2024-02-02 01:23:45.785025 hooks_toolkit-1.0.4/hooks_toolkit/libs/asyncio/xrpl_helpers/tools.py
--rw-r--r--   0        0        0     3236 2024-03-11 10:37:01.809990 hooks_toolkit-1.0.4/hooks_toolkit/libs/asyncio/xrpl_helpers/transaction.py
--rw-r--r--   0        0        0     1484 2024-01-23 11:17:27.401747 hooks_toolkit-1.0.4/hooks_toolkit/libs/binary_models/__init__.py
--rw-r--r--   0        0        0      632 2024-01-26 13:13:36.262575 hooks_toolkit-1.0.4/hooks_toolkit/libs/binary_models/amount_model.py
--rw-r--r--   0        0        0     9618 2024-04-19 14:27:02.555625 hooks_toolkit-1.0.4/hooks_toolkit/libs/binary_models/base_model.py
--rw-r--r--   0        0        0      710 2024-01-26 13:11:26.835752 hooks_toolkit-1.0.4/hooks_toolkit/libs/binary_models/test_model.py
--rw-r--r--   0        0        0     1115 2024-01-23 11:17:20.967602 hooks_toolkit-1.0.4/hooks_toolkit/libs/binary_models/utils/__init__.py
--rw-r--r--   0        0        0     2974 2024-01-29 20:31:19.040070 hooks_toolkit-1.0.4/hooks_toolkit/libs/binary_models/utils/decode.py
--rw-r--r--   0        0        0     3018 2024-01-26 13:35:36.244232 hooks_toolkit-1.0.4/hooks_toolkit/libs/binary_models/utils/encode.py
--rw-r--r--   0        0        0      772 2024-01-23 11:17:23.670680 hooks_toolkit-1.0.4/hooks_toolkit/libs/binary_models/utils/types.py
--rw-r--r--   0        0        0      227 2024-01-31 22:42:35.070750 hooks_toolkit-1.0.4/hooks_toolkit/libs/keylet_utils/__init__.py
--rw-r--r--   0        0        0     2708 2024-02-02 00:55:11.376123 hooks_toolkit-1.0.4/hooks_toolkit/libs/keylet_utils/execution_utility.py
--rw-r--r--   0        0        0     1891 2024-02-02 00:21:49.314839 hooks_toolkit-1.0.4/hooks_toolkit/libs/keylet_utils/state_utility.py
--rw-r--r--   0        0        0        0 2023-07-17 02:14:32.770473 hooks_toolkit-1.0.4/hooks_toolkit/libs/xrpl_helpers/__init__.py
--rw-r--r--   0        0        0     2555 2023-12-02 12:02:16.713240 hooks_toolkit-1.0.4/hooks_toolkit/libs/xrpl_helpers/constants.py
--rw-r--r--   0        0        0     2147 2024-01-26 13:35:18.601335 hooks_toolkit-1.0.4/hooks_toolkit/libs/xrpl_helpers/fund_system.py
--rw-r--r--   0        0        0      368 2024-03-11 10:37:06.853629 hooks_toolkit-1.0.4/hooks_toolkit/libs/xrpl_helpers/server_url.py
--rw-r--r--   0        0        0     3906 2024-03-11 10:37:11.132405 hooks_toolkit-1.0.4/hooks_toolkit/libs/xrpl_helpers/setup.py
--rw-r--r--   0        0        0     7959 2024-01-26 13:34:59.396838 hooks_toolkit-1.0.4/hooks_toolkit/libs/xrpl_helpers/tools.py
--rw-r--r--   0        0        0     3060 2024-03-11 10:37:13.590014 hooks_toolkit-1.0.4/hooks_toolkit/libs/xrpl_helpers/transaction.py
--rw-r--r--   0        0        0     1067 2023-12-02 12:07:18.783701 hooks_toolkit-1.0.4/hooks_toolkit/models/grants.py
--rw-r--r--   0        0        0     1507 2023-12-03 14:14:09.254946 hooks_toolkit-1.0.4/hooks_toolkit/models/parameters.py
--rw-r--r--   0        0        0      919 2023-07-17 02:14:32.771673 hooks_toolkit-1.0.4/hooks_toolkit/models/state.py
--rw-r--r--   0        0        0     2902 2024-01-26 14:06:50.059704 hooks_toolkit-1.0.4/hooks_toolkit/set_hook.py
--rw-r--r--   0        0        0      742 2024-01-26 13:32:56.459660 hooks_toolkit-1.0.4/hooks_toolkit/types.py
--rw-r--r--   0        0        0     3740 2024-01-26 13:33:41.049497 hooks_toolkit-1.0.4/hooks_toolkit/utils.py
--rw-r--r--   0        0        0      972 2024-02-02 01:43:51.258146 hooks_toolkit-1.0.4/hooks_toolkit/xrpld.py
--rw-r--r--   0        0        0      283 2024-04-20 09:31:45.946471 hooks_toolkit-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 hooks_toolkit-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3235 2024-05-31 09:10:55.760043 hooks_toolkit-1.0.5/hooks_toolkit/asyncio_set_hook.py
+-rw-r--r--   0        0        0      993 2024-02-02 01:43:45.864461 hooks_toolkit-1.0.5/hooks_toolkit/asyncio_xrpld.py
+-rw-r--r--   0        0        0      227 2024-02-01 15:55:33.459231 hooks_toolkit-1.0.5/hooks_toolkit/libs/asyncio/keylet_utils/__init__.py
+-rw-r--r--   0        0        0     2750 2024-02-02 01:33:36.214072 hooks_toolkit-1.0.5/hooks_toolkit/libs/asyncio/keylet_utils/execution_utility.py
+-rw-r--r--   0        0        0     2000 2024-02-02 01:56:16.002569 hooks_toolkit-1.0.5/hooks_toolkit/libs/asyncio/keylet_utils/state_utility.py
+-rw-r--r--   0        0        0        0 2024-02-01 15:58:40.704177 hooks_toolkit-1.0.5/hooks_toolkit/libs/asyncio/xrpl_helpers/__init__.py
+-rw-r--r--   0        0        0     2229 2024-02-02 01:28:09.071988 hooks_toolkit-1.0.5/hooks_toolkit/libs/asyncio/xrpl_helpers/fund_system.py
+-rw-r--r--   0        0        0     3981 2024-03-11 10:36:58.592137 hooks_toolkit-1.0.5/hooks_toolkit/libs/asyncio/xrpl_helpers/setup.py
+-rw-r--r--   0        0        0     8325 2024-02-02 01:23:45.785025 hooks_toolkit-1.0.5/hooks_toolkit/libs/asyncio/xrpl_helpers/tools.py
+-rw-r--r--   0        0        0     3236 2024-03-11 10:37:01.809990 hooks_toolkit-1.0.5/hooks_toolkit/libs/asyncio/xrpl_helpers/transaction.py
+-rw-r--r--   0        0        0     1484 2024-01-23 11:17:27.401747 hooks_toolkit-1.0.5/hooks_toolkit/libs/binary_models/__init__.py
+-rw-r--r--   0        0        0      632 2024-01-26 13:13:36.262575 hooks_toolkit-1.0.5/hooks_toolkit/libs/binary_models/amount_model.py
+-rw-r--r--   0        0        0     9618 2024-04-19 14:27:02.555625 hooks_toolkit-1.0.5/hooks_toolkit/libs/binary_models/base_model.py
+-rw-r--r--   0        0        0      710 2024-01-26 13:11:26.835752 hooks_toolkit-1.0.5/hooks_toolkit/libs/binary_models/test_model.py
+-rw-r--r--   0        0        0     1115 2024-01-23 11:17:20.967602 hooks_toolkit-1.0.5/hooks_toolkit/libs/binary_models/utils/__init__.py
+-rw-r--r--   0        0        0     2974 2024-01-29 20:31:19.040070 hooks_toolkit-1.0.5/hooks_toolkit/libs/binary_models/utils/decode.py
+-rw-r--r--   0        0        0     3018 2024-01-26 13:35:36.244232 hooks_toolkit-1.0.5/hooks_toolkit/libs/binary_models/utils/encode.py
+-rw-r--r--   0        0        0      772 2024-01-23 11:17:23.670680 hooks_toolkit-1.0.5/hooks_toolkit/libs/binary_models/utils/types.py
+-rw-r--r--   0        0        0      227 2024-01-31 22:42:35.070750 hooks_toolkit-1.0.5/hooks_toolkit/libs/keylet_utils/__init__.py
+-rw-r--r--   0        0        0     2708 2024-02-02 00:55:11.376123 hooks_toolkit-1.0.5/hooks_toolkit/libs/keylet_utils/execution_utility.py
+-rw-r--r--   0        0        0     1891 2024-02-02 00:21:49.314839 hooks_toolkit-1.0.5/hooks_toolkit/libs/keylet_utils/state_utility.py
+-rw-r--r--   0        0        0        0 2024-05-31 09:18:28.802965 hooks_toolkit-1.0.5/hooks_toolkit/libs/xrpl_helpers/__init__.py
+-rw-r--r--   0        0        0     2555 2023-12-02 12:02:16.713240 hooks_toolkit-1.0.5/hooks_toolkit/libs/xrpl_helpers/constants.py
+-rw-r--r--   0        0        0     2147 2024-01-26 13:35:18.601335 hooks_toolkit-1.0.5/hooks_toolkit/libs/xrpl_helpers/fund_system.py
+-rw-r--r--   0        0        0      368 2024-03-11 10:37:06.853629 hooks_toolkit-1.0.5/hooks_toolkit/libs/xrpl_helpers/server_url.py
+-rw-r--r--   0        0        0     3906 2024-03-11 10:37:11.132405 hooks_toolkit-1.0.5/hooks_toolkit/libs/xrpl_helpers/setup.py
+-rw-r--r--   0        0        0     7959 2024-01-26 13:34:59.396838 hooks_toolkit-1.0.5/hooks_toolkit/libs/xrpl_helpers/tools.py
+-rw-r--r--   0        0        0     3060 2024-03-11 10:37:13.590014 hooks_toolkit-1.0.5/hooks_toolkit/libs/xrpl_helpers/transaction.py
+-rw-r--r--   0        0        0     1067 2023-12-02 12:07:18.783701 hooks_toolkit-1.0.5/hooks_toolkit/models/grants.py
+-rw-r--r--   0        0        0     1507 2023-12-03 14:14:09.254946 hooks_toolkit-1.0.5/hooks_toolkit/models/parameters.py
+-rw-r--r--   0        0        0      919 2023-07-17 02:14:32.771673 hooks_toolkit-1.0.5/hooks_toolkit/models/state.py
+-rw-r--r--   0        0        0     3144 2024-05-31 09:05:43.696202 hooks_toolkit-1.0.5/hooks_toolkit/set_hook.py
+-rw-r--r--   0        0        0      742 2024-01-26 13:32:56.459660 hooks_toolkit-1.0.5/hooks_toolkit/types.py
+-rw-r--r--   0        0        0     3914 2024-05-31 09:10:53.452717 hooks_toolkit-1.0.5/hooks_toolkit/utils.py
+-rw-r--r--   0        0        0      972 2024-02-02 01:43:51.258146 hooks_toolkit-1.0.5/hooks_toolkit/xrpld.py
+-rw-r--r--   0        0        0      285 2024-05-31 09:12:13.221608 hooks_toolkit-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 hooks_toolkit-1.0.5/PKG-INFO
```

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/asyncio_set_hook.py` & `hooks_toolkit-1.0.5/hooks_toolkit/asyncio_set_hook.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,22 @@
 ) -> Hook:
     kwargs: Dict[str, Any] = {
         "hook_api_version": params.version,
         "hook_namespace": hex_namespace(params.namespace),
     }
 
     if params.create_file is not None:
-        kwargs["create_code"] = read_hook_binary_hex_from_ns(params.create_file)
+        if params.version == 0:
+            kwargs["create_code"] = read_hook_binary_hex_from_ns(
+                params.create_file, "wasm"
+            )
+        elif params.version == 1:
+            kwargs["create_code"] = read_hook_binary_hex_from_ns(
+                params.create_file, "bc"
+            )
 
     if params.hook_on_array is not None:
         kwargs["hook_on"] = calculate_hook_on(params.hook_on_array)
 
     if params.hook_hash is not None:
         kwargs["hook_hash"] = params.hook_hash
```

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/asyncio_xrpld.py` & `hooks_toolkit-1.0.5/hooks_toolkit/asyncio_xrpld.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/asyncio/keylet_utils/execution_utility.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/asyncio/keylet_utils/execution_utility.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/asyncio/keylet_utils/state_utility.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/asyncio/keylet_utils/state_utility.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/asyncio/xrpl_helpers/fund_system.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/asyncio/xrpl_helpers/fund_system.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/asyncio/xrpl_helpers/setup.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/asyncio/xrpl_helpers/setup.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/asyncio/xrpl_helpers/tools.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/asyncio/xrpl_helpers/tools.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/asyncio/xrpl_helpers/transaction.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/asyncio/xrpl_helpers/transaction.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/binary_models/__init__.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/binary_models/__init__.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/binary_models/amount_model.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/binary_models/amount_model.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/binary_models/base_model.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/binary_models/base_model.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/binary_models/test_model.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/binary_models/test_model.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/binary_models/utils/__init__.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/binary_models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/binary_models/utils/decode.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/binary_models/utils/decode.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/binary_models/utils/encode.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/binary_models/utils/encode.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/binary_models/utils/types.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/binary_models/utils/types.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/keylet_utils/execution_utility.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/keylet_utils/execution_utility.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/keylet_utils/state_utility.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/keylet_utils/state_utility.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/xrpl_helpers/constants.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/xrpl_helpers/constants.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/xrpl_helpers/fund_system.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/xrpl_helpers/fund_system.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/xrpl_helpers/setup.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/xrpl_helpers/setup.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/xrpl_helpers/tools.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/xrpl_helpers/tools.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/libs/xrpl_helpers/transaction.py` & `hooks_toolkit-1.0.5/hooks_toolkit/libs/xrpl_helpers/transaction.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/models/grants.py` & `hooks_toolkit-1.0.5/hooks_toolkit/models/grants.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/models/parameters.py` & `hooks_toolkit-1.0.5/hooks_toolkit/models/parameters.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/models/state.py` & `hooks_toolkit-1.0.5/hooks_toolkit/models/state.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/set_hook.py` & `hooks_toolkit-1.0.5/hooks_toolkit/set_hook.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,28 +10,38 @@
 from xrpl.utils import calculate_hook_on
 from xrpl.models.transactions import SetHookFlag
 
 from hooks_toolkit.libs.xrpl_helpers.transaction import (
     get_transaction_fee,
     app_transaction,
 )
-from hooks_toolkit.utils import hex_namespace, read_hook_binary_hex_from_ns
+from hooks_toolkit.utils import (
+    hex_namespace,
+    read_hook_binary_hex_from_ns,
+)
 from hooks_toolkit.types import SetHookParams
 
 
 def create_hook_payload(
     params: SetHookParams,
 ) -> Hook:
     kwargs: Dict[str, Any] = {
         "hook_api_version": params.version,
         "hook_namespace": hex_namespace(params.namespace),
     }
 
     if params.create_file is not None:
-        kwargs["create_code"] = read_hook_binary_hex_from_ns(params.create_file)
+        if params.version == 0:
+            kwargs["create_code"] = read_hook_binary_hex_from_ns(
+                params.create_file, "wasm"
+            )
+        elif params.version == 1:
+            kwargs["create_code"] = read_hook_binary_hex_from_ns(
+                params.create_file, "bc"
+            )
 
     if params.hook_on_array is not None:
         kwargs["hook_on"] = calculate_hook_on(params.hook_on_array)
 
     if params.hook_hash is not None:
         kwargs["hook_hash"] = params.hook_hash
```

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/types.py` & `hooks_toolkit-1.0.5/hooks_toolkit/types.py`

 * *Files identical despite different names*

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/utils.py` & `hooks_toolkit-1.0.5/hooks_toolkit/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -149,16 +149,22 @@
 
 
 def int_to_hex(integer, byte_length):
     hex_string = hex(integer)[2:].zfill(byte_length * 2)
     return hex_string
 
 
-def read_hook_binary_hex_from_ns(filename: str):
-    with open(f"build/{filename}.wasm", "rb") as file:
+def read_hook_binary_hex_from_ns(filename: str, ext: str):
+    with open(f"build/{filename}.{ext}", "rb") as file:
+        wasm = file.read()
+    return wasm.hex().upper()
+
+
+def read_jshook_binary_hex_from_ns(filename: str):
+    with open(f"build/{filename}.bc", "rb") as file:
         wasm = file.read()
     return wasm.hex().upper()
 
 
 def hex_namespace(hook_namespace_seed: str):
     return hashlib.sha256(hook_namespace_seed.encode()).hexdigest().upper()
```

### Comparing `hooks_toolkit-1.0.4/hooks_toolkit/xrpld.py` & `hooks_toolkit-1.0.5/hooks_toolkit/xrpld.py`

 * *Files identical despite different names*

