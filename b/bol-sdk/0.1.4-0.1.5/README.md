# Comparing `tmp/bol_sdk-0.1.4.tar.gz` & `tmp/bol_sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bol_sdk-0.1.4.tar", max compression
+gzip compressed data, was "bol_sdk-0.1.5.tar", max compression
```

## Comparing `bol_sdk-0.1.4.tar` & `bol_sdk-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       45 2024-05-03 17:53:19.404594 bol_sdk-0.1.4/bol_SDK/__init__.py
--rw-r--r--   0        0        0      895 2024-05-06 09:27:23.359081 bol_sdk-0.1.4/bol_SDK/__main__.py
--rw-r--r--   0        0        0    15932 2024-05-06 09:27:23.357641 bol_sdk-0.1.4/bol_SDK/bol_SDK.py
--rw-r--r--   0        0        0       43 2024-05-03 17:53:19.405330 bol_sdk-0.1.4/bol_SDK/constants.py
--rw-r--r--   0        0        0      381 2024-05-31 17:04:24.904573 bol_sdk-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 bol_sdk-0.1.4/setup.py
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 bol_sdk-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       45 2024-05-03 17:53:19.404594 bol_sdk-0.1.5/bol_SDK/__init__.py
+-rw-r--r--   0        0        0      882 2024-05-31 17:17:47.822337 bol_sdk-0.1.5/bol_SDK/__main__.py
+-rw-r--r--   0        0        0    15938 2024-05-31 17:17:18.064850 bol_sdk-0.1.5/bol_SDK/bol_SDK.py
+-rw-r--r--   0        0        0       43 2024-05-03 17:53:19.405330 bol_sdk-0.1.5/bol_SDK/constants.py
+-rw-r--r--   0        0        0      381 2024-05-31 17:18:22.185909 bol_sdk-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 bol_sdk-0.1.5/setup.py
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 bol_sdk-0.1.5/PKG-INFO
```

### Comparing `bol_sdk-0.1.4/bol_SDK/__main__.py` & `bol_sdk-0.1.5/bol_SDK/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import pprint
 
-from bol_SDK import bol_SDK as bol
+import bol_SDK as bol
 from dotenv import load_dotenv
 
 
 def main():
   load_dotenv()
   pp = pprint.PrettyPrinter(indent=4)
```

### Comparing `bol_sdk-0.1.4/bol_SDK/bol_SDK.py` & `bol_sdk-0.1.5/bol_SDK/bol_SDK.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     import constants as CONSTANTS # For local development   
 # ==== DEBUG =======
 import os
 # import numpy as np
 import requests
 import pprint
 import time
-from typing import List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 # =============================================================================
 #
 # Calling the API credentials:
 # ----------------------------
 from dotenv import load_dotenv
 load_dotenv()
@@ -32,16 +32,16 @@
 Helpers
 
 """
 
 
 def get_request_hearders(access_token):
     return  {'Authorization': f'Bearer {access_token}',
-            'Content-Type': f'application/vnd.retailer.v{constants.API_VERSION}+json',
-            'Accept': f'application/vnd.retailer.v{constants.API_VERSION}+json'}
+            'Content-Type': f'application/vnd.retailer.v{CONSTANTS.API_VERSION}+json',
+            'Accept': f'application/vnd.retailer.v{CONSTANTS.API_VERSION}+json'}
     # return  {'Authorization': f'Bearer {access_token}',
     #     'Content-Type': f'application/json',
     #     'Accept': f'application/json' }
 
 
 #split the date string into date integers
 def split_date_string(date_string):
@@ -189,15 +189,15 @@
             os.sys.exit(f"An unexpected error occured while requesting the process status of the offer list export. Status {status}: {response.json()}. Abort script.")
     print(f"(2/3) Successfully got the entity ID of the export request: {entityId}.")
 
     #Step 3: Retrieve an offer export file by offer export id
     while(1):
         order_request = f"https://api.bol.com/retailer/offers/export/{entityId}"
         export_headers = headers
-        export_headers['Accept'] = f'application/vnd.retailer.v{constants.API_VERSION}+csv'
+        export_headers['Accept'] = f'application/vnd.retailer.v{CONSTANTS.API_VERSION}+csv'
         offers = requests.get(order_request, headers = export_headers)
         status, response = logApiResponse(offers)
         if status == 200:
             offers_list = []
             reader = csv.reader(response.text.split('\n'), delimiter=',')
             index = 0
             for row in reader:
@@ -245,15 +245,15 @@
         access_token = get_access_token(client_id, client_secret)
 
     # The maximum number of attempts to send out an update requst.
     update_attempt_count = 0
     headers = get_request_hearders(access_token = access_token)
     post_data = json.dumps({ 'amount': stock_amount,
                              'managedByRetailer' : False })
-    while(update_attempt_count < constants.MAX_REQUEST_ATTEMPTS):
+    while(update_attempt_count < CONSTANTS.MAX_REQUEST_ATTEMPTS):
         order_request_url = f"https://api.bol.com/retailer/offers/" \
                             f"{bol_offer_id}/stock"
         # ------!!! DEV !!! ---------------------------------
         # return 'FAILURE'
         # return 'SUCCESS'
         # ---------------------------------------------------
         response_payload = json.loads(requests.put( order_request_url,
@@ -290,15 +290,15 @@
             print('-----response----')
             pp.pprint(response_payload)
             print('-----------------')
             break
 
     if status != 'SUCCESS':
         status = 'FAILURE'
-        print(f"{status}, {constants.MAX_REQUEST_ATTEMPTS - 1} attempts were made to upload the stock of product {bol_offer_id} on Bol, but all failed. Abort updating this product.")
+        print(f"{status}, {CONSTANTS.MAX_REQUEST_ATTEMPTS - 1} attempts were made to upload the stock of product {bol_offer_id} on Bol, but all failed. Abort updating this product.")
         pp.pprint(response_payload)
 
     return status
 
 #test
 #update_stock(6935670512420,23)
```

### Comparing `bol_sdk-0.1.4/setup.py` & `bol_sdk-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['numpy>=1.23.1,<2.0.0',
  'pandas>=1.4.3,<2.0.0',
  'python-dotenv>=1.0.1,<2.0.0',
  'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'bol-sdk',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': '',
     'long_description': 'None',
     'author': 'Genhao Li',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

