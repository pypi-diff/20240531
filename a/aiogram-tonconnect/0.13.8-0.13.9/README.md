# Comparing `tmp/aiogram-tonconnect-0.13.8.tar.gz` & `tmp/aiogram-tonconnect-0.13.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-tonconnect-0.13.8.tar", last modified: Wed May 29 16:37:36 2024, max compression
+gzip compressed data, was "aiogram-tonconnect-0.13.9.tar", last modified: Fri May 31 01:51:30 2024, max compression
```

## Comparing `aiogram-tonconnect-0.13.8.tar` & `aiogram-tonconnect-0.13.9.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-29 16:37:36.904754 aiogram-tonconnect-0.13.8/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1064 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/LICENSE
--rw-r--r--   0 ness      (1000) ness      (1000)     5438 2024-05-29 16:37:36.900754 aiogram-tonconnect-0.13.8/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     4458 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/README.md
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-29 16:37:36.896754 aiogram-tonconnect-0.13.8/aiogram_tonconnect/
--rw-rw-r--   0 ness      (1000) ness      (1000)       65 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     6377 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/handlers.py
--rw-rw-r--   0 ness      (1000) ness      (1000)    20809 2024-05-27 04:26:10.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/manager.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     5253 2024-05-19 12:46:38.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/middleware.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-29 16:37:36.900754 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/
--rw-rw-r--   0 ness      (1000) ness      (1000)      140 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     7607 2024-05-29 16:34:38.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/models.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     7469 2024-03-30 13:07:39.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/provider.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-29 16:37:36.900754 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/
--rw-rw-r--   0 ness      (1000) ness      (1000)      300 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2047 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/base.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2247 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/callback.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1214 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/session.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1078 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/task.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2197 2024-03-30 13:09:49.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/tonconnect.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     6268 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/transactions.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-29 16:37:36.900754 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/wallet/
--rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/wallet/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     6641 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/wallet/manager.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-29 16:37:36.900754 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/
--rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2416 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/address.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      945 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/exceptions.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     6024 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/keyboards.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1914 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/proof.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-29 16:37:36.900754 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/qrcode/
--rw-rw-r--   0 ness      (1000) ness      (1000)     2348 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/qrcode/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)    31987 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/qrcode/generator.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      947 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/states.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     6120 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/texts.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-29 16:37:36.896754 aiogram-tonconnect-0.13.8/aiogram_tonconnect.egg-info/
--rw-r--r--   0 ness      (1000) ness      (1000)     5438 2024-05-29 16:37:36.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect.egg-info/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     1254 2024-05-29 16:37:36.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect.egg-info/SOURCES.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        1 2024-05-29 16:37:36.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect.egg-info/dependency_links.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       98 2024-05-29 16:37:36.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect.egg-info/requires.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       19 2024-05-29 16:37:36.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect.egg-info/top_level.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       38 2024-05-29 16:37:36.904754 aiogram-tonconnect-0.13.8/setup.cfg
--rw-rw-r--   0 ness      (1000) ness      (1000)     1222 2024-05-29 16:36:37.000000 aiogram-tonconnect-0.13.8/setup.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-31 01:51:30.192968 aiogram-tonconnect-0.13.9/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1064 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/LICENSE
+-rw-r--r--   0 ness      (1000) ness      (1000)     5438 2024-05-31 01:51:30.192968 aiogram-tonconnect-0.13.9/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4458 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/README.md
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-31 01:51:30.188968 aiogram-tonconnect-0.13.9/aiogram_tonconnect/
+-rw-rw-r--   0 ness      (1000) ness      (1000)       65 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6377 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/handlers.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)    20809 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/manager.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     5452 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/middleware.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-31 01:51:30.188968 aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      140 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7607 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/models.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7469 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/provider.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-31 01:51:30.192968 aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/storage/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      300 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/storage/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2047 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/storage/base.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2247 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/storage/callback.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1214 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/storage/session.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1078 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/storage/task.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2341 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/tonconnect.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6268 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/transactions.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-31 01:51:30.192968 aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/wallet/
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/wallet/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7284 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/wallet/manager.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-31 01:51:30.192968 aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2416 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/address.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      945 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/exceptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6024 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/keyboards.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1914 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/proof.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-31 01:51:30.192968 aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/qrcode/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2348 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/qrcode/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)    31987 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/qrcode/generator.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      947 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/states.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6120 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/texts.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-31 01:51:30.188968 aiogram-tonconnect-0.13.9/aiogram_tonconnect.egg-info/
+-rw-r--r--   0 ness      (1000) ness      (1000)     5438 2024-05-31 01:51:30.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect.egg-info/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1282 2024-05-31 01:51:30.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect.egg-info/SOURCES.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        1 2024-05-31 01:51:30.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect.egg-info/dependency_links.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       98 2024-05-31 01:51:30.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect.egg-info/requires.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       19 2024-05-31 01:51:30.000000 aiogram-tonconnect-0.13.9/aiogram_tonconnect.egg-info/top_level.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       38 2024-05-31 01:51:30.192968 aiogram-tonconnect-0.13.9/setup.cfg
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1222 2024-05-31 01:50:34.000000 aiogram-tonconnect-0.13.9/setup.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-31 01:51:30.192968 aiogram-tonconnect-0.13.9/test/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      678 2024-05-31 01:49:57.000000 aiogram-tonconnect-0.13.9/test/test_wallet_manager.py
```

### Comparing `aiogram-tonconnect-0.13.8/LICENSE` & `aiogram-tonconnect-0.13.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/PKG-INFO` & `aiogram-tonconnect-0.13.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram-tonconnect
-Version: 0.13.8
+Version: 0.13.9
 Summary: TON Connect UI for aiogram bots.
 Home-page: https://github.com/nessshon/aiogram-tonconnect/
 Author: nessshon
 Project-URL: Documentation, https://nessshon.github.io/aiogram-tonconnect/
 Project-URL: Bot example, https://t.me/aiogramTONConnectBot/
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `aiogram-tonconnect-0.13.8/README.md` & `aiogram-tonconnect-0.13.9/README.md`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/handlers.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/handlers.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/manager.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/manager.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/middleware.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     :param storage: An instance of ATCStorageBase for data storage.
         Available default classes:
         - ATCMemoryStorage: Stores data in memory.
         - ATCRedisStorage: Stores data in Redis.
     :param manifest_url: URL to the AiogramTonConnect manifest.
     :param redirect_url: URL to the redirect after connecting.
     :param exclude_wallets: List of wallet names to exclude.
+    :param wallets_order: Preferred wallets order.
     :param qrcode_provider: QRImageProviderBase or QRUrlProviderBase instance.
         Available default classes:
         - QRImageProvider: Generates QR codes locally using the library and
         displays message type as 'photo' with the QR code image.
         - QRUrlProvider: Generates QR codes using a third-party API and
         displays message type as 'text' with the image as 'web_page_preview'.
     :param inline_keyboard: InlineKeyboardBase class for managing inline keyboards.
@@ -40,19 +41,21 @@
             manifest_url: str,
             redirect_url: str = None,
             exclude_wallets: List[str] = None,
             text_message: Optional[Type[TextMessageBase]] = None,
             inline_keyboard: Optional[Type[InlineKeyboardBase]] = None,
             qrcode_provider: Optional[Union[QRImageProviderBase, QRUrlProviderBase]] = None,
             tonapi_token: Optional[str] = None,
+            wallets_order: Optional[List[str]] = None,
     ) -> None:
         self.storage = storage
         self.manifest_url = manifest_url
         self.redirect_url = redirect_url
         self.exclude_wallets = exclude_wallets
+        self.wallets_order = wallets_order
 
         self.qrcode_provider = qrcode_provider or QRImageProvider()
         self.text_message = text_message or TextMessage
         self.inline_keyboard = inline_keyboard or InlineKeyboard
 
         self.tonapi_token = tonapi_token
 
@@ -104,14 +107,15 @@
             data["atc_user"] = atc_user
 
             tonconnect = AiogramTonConnect(
                 storage=SessionStorage(self.storage, atc_user.id),
                 manifest_url=self.manifest_url,
                 redirect_url=self.redirect_url,
                 exclude_wallets=self.exclude_wallets,
+                wallets_order=self.wallets_order,
                 tonapi_token=self.tonapi_token,
             )
             atc_manager = ATCManager(
                 storage=self.storage,
                 tonconnect=tonconnect,
                 text_message=self.text_message(atc_user.language_code),
                 inline_keyboard=self.inline_keyboard(atc_user.language_code),
```

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/models.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/models.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/provider.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/provider.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/base.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/storage/base.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/callback.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/storage/callback.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/session.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/storage/session.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/task.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/storage/task.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/tonconnect.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/tonconnect.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,33 +13,35 @@
     """
     AiogramTonConnect class that extends the base AiogramTonConnect functionality.
 
     :param storage: An instance of SessionStorage for session data storage.
     :param manifest_url: URL to the manifest file.
     :param redirect_url: URL to the redirect after connecting.
     :param exclude_wallets: Optional list of wallet names to exclude.
+    :param wallets_order: Optional preferred wallets order.
     :param args: Additional positional arguments.
     :param kwargs: Additional keyword arguments.
     """
 
     def __init__(
             self,
             storage: SessionStorage,
             manifest_url: str,
             redirect_url: str = None,
             exclude_wallets: Optional[List[str]] = None,
             tonapi_token: Optional[str] = None,
+            wallets_order: Optional[List[str]] = None,
             *args,
             **kwargs,
     ) -> None:
         kwargs["storage"] = storage
         kwargs["manifest_url"] = manifest_url
         super().__init__(*args, **kwargs)
         self.redirect_url = redirect_url
-        self.wallet_manager = WalletManager(exclude_wallets=exclude_wallets)
+        self.wallet_manager = WalletManager(exclude_wallets=exclude_wallets, wallets_order=wallets_order)
         self.tonapi_token = tonapi_token
 
     async def get_wallets(self=None) -> List[AppWallet]:
         """
         Get the list of AiogramTonConnect wallets.
 
         :return: List of AiogramTonConnect application wallet instances.
```

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/transactions.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/transactions.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/wallet/manager.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/tonconnect/wallet/manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -91,27 +91,30 @@
     def __init__(
             self,
             wallets_list_source_url: str =
             'https://raw.githubusercontent.com/ton-blockchain/wallets-list/main/wallets-v2.json',
             exclude_wallets: List[str] = None,
             cache_ttl: int = None,
             file_path: str = None,
+            wallets_order: List[str] = None,
     ) -> None:
         """
         Initialize the WalletManager.
 
         :param wallets_list_source_url: URL to fetch the wallets list.
         :param exclude_wallets: List of wallet names to exclude.
+        :param wallets_order: Preferred wallets order.
         :param cache_ttl: Time-to-live for the cache, in seconds.
         :param file_path: Path to the fallback wallets file.
         """
         self.cache_manager = _CachedWalletManager(cache_ttl)
         self.fallback_manager = _FallbackWalletManager(file_path)
 
         self._exclude_wallets = exclude_wallets
+        self._wallets_order = wallets_order
         self._wallets_list_source_url = wallets_list_source_url
 
     async def __fetch(self) -> List[Dict[str, Any]]:
         """
         Fetch the wallets list from the specified URL.
 
         :return: List of dictionaries representing wallets.
@@ -157,18 +160,31 @@
                     break
         return supported_wallets
 
     async def __save_wallets(self, wallets: List[Dict[str, Any]]) -> None:
         await self.cache_manager.save_wallets(wallets)
         await self.fallback_manager.save_wallets(wallets)
 
+    def __order_wallets(self, wallets: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
+        if self._wallets_order is None:
+            return wallets
+
+        def sort_by_order(wallet: Dict[str, Any]) -> int:
+            try:
+                return self._wallets_order.index(wallet["app_name"])
+            except ValueError:
+                return len(self._wallets_order)
+
+        return list(sorted(wallets, key=sort_by_order))
+
     def __process_wallets(self, wallets: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
         excluded_wallets = self.__exclude(wallets)
         supported_wallets = self.__get_supported(excluded_wallets)
-        return supported_wallets
+        ordered_wallets = self.__order_wallets(supported_wallets)
+        return ordered_wallets
 
     async def get_wallets(self) -> List[AppWallet]:
         """
         Get the list of AiogramTonConnect wallets.
 
         :return: List of AiogramTonConnect application wallet instances.
         """
```

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/address.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/address.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/exceptions.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/keyboards.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/keyboards.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/proof.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/proof.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/qrcode/__init__.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/qrcode/__init__.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/qrcode/generator.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/qrcode/generator.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/states.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/states.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/texts.py` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect/utils/texts.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect.egg-info/PKG-INFO` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram-tonconnect
-Version: 0.13.8
+Version: 0.13.9
 Summary: TON Connect UI for aiogram bots.
 Home-page: https://github.com/nessshon/aiogram-tonconnect/
 Author: nessshon
 Project-URL: Documentation, https://nessshon.github.io/aiogram-tonconnect/
 Project-URL: Bot example, https://t.me/aiogramTONConnectBot/
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `aiogram-tonconnect-0.13.8/aiogram_tonconnect.egg-info/SOURCES.txt` & `aiogram-tonconnect-0.13.9/aiogram_tonconnect.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,9 @@
 aiogram_tonconnect/utils/address.py
 aiogram_tonconnect/utils/exceptions.py
 aiogram_tonconnect/utils/keyboards.py
 aiogram_tonconnect/utils/proof.py
 aiogram_tonconnect/utils/states.py
 aiogram_tonconnect/utils/texts.py
 aiogram_tonconnect/utils/qrcode/__init__.py
-aiogram_tonconnect/utils/qrcode/generator.py
+aiogram_tonconnect/utils/qrcode/generator.py
+test/test_wallet_manager.py
```

### Comparing `aiogram-tonconnect-0.13.8/setup.py` & `aiogram-tonconnect-0.13.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aiogram-tonconnect",
-    version="0.13.8",
+    version="0.13.9",
     author="nessshon",
     description="TON Connect UI for aiogram bots.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["example", "docs"]),
     install_requires=[
         "aiofiles",
```

