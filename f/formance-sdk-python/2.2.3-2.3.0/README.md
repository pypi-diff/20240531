# Comparing `tmp/formance-sdk-python-2.2.3.tar.gz` & `tmp/formance-sdk-python-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formance-sdk-python-2.2.3.tar", last modified: Mon Apr 29 14:33:45 2024, max compression
+gzip compressed data, was "formance-sdk-python-2.3.0.tar", last modified: Fri May 31 09:35:22 2024, max compression
```

## Comparing `formance-sdk-python-2.2.3.tar` & `formance-sdk-python-2.3.0.tar`

### file list

```diff
@@ -1,544 +1,559 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:45.352038 formance-sdk-python-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    37654 2024-04-29 14:33:45.348038 formance-sdk-python-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23165 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:33:45.352038 formance-sdk-python-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:45.264037 formance-sdk-python-2.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:45.264037 formance-sdk-python-2.2.3/src/formance_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    37654 2024-04-29 14:33:44.000000 formance-sdk-python-2.2.3/src/formance_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23120 2024-04-29 14:33:45.000000 formance-sdk-python-2.2.3/src/formance_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:33:44.000000 formance-sdk-python-2.2.3/src/formance_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-29 14:33:44.000000 formance-sdk-python-2.2.3/src/formance_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-29 14:33:44.000000 formance-sdk-python-2.2.3/src/formance_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:45.268037 formance-sdk-python-2.2.3/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:45.268037 formance-sdk-python-2.2.3/src/sdk/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    24252 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)   137737 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/ledger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:45.268037 formance-sdk-python-2.2.3/src/sdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:45.268037 formance-sdk-python-2.2.3/src/sdk/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/errors/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/errors/errorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/errors/reconciliationerrorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/errors/sdkerror.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/errors/v2error.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/errors/v2errorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/errors/walletserrorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/errors/webhookserrorresponse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:45.296037 formance-sdk-python-2.2.3/src/sdk/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/activateconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/addaccounttopool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/addmetadataontransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/addmetadatatoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/cancelevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/changeconfigsecret.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/confirmhold.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/connectorstransfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/countaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/counttransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/createaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/createbalance.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/createbankaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/createclient.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/createpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/createpolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/createpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/createsecret.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/createtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/createtransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/createtransferinitiation.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/createtrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/createwallet.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/createworkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/creditwallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/deactivateconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/debitwallet.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/deleteclient.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/deleteconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/deletepolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/deletepool.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/deletesecret.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/deletetransferinitiation.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/deletetrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/deleteworkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/forwardbankaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getaccountbalances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getbalance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getbalances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getbalancesaggregated.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getbankaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getconnectortask.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getconnectortaskv1.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/gethold.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getholds.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getinstance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getinstancehistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getinstancestagehistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getledgerinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getmanyconfigs.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getmapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getoidcwellknowns.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getpolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getpoolbalances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getreconciliation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/gettransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/gettransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/gettransferinitiation.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getversions.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getwallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getwalletsummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/getworkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/insertconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/installconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listallconnectors.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listbalances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listbankaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listclients.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listconfigsavailableconnectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listconnectortasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listconnectortasksv1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listinstances.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listlogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listpayments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listpolicies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listpools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listreconciliations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listtransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listtransferinitiations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listtriggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listtriggersoccurrences.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listusers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listwallets.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/listworkflows.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/orchestrationgetserverinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/paymentsgetaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/paymentsgetserverinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/paymentslistaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/readclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/readconnectorconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/readconnectorconfigv1.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/readstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/readtrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/readuser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/reconcile.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/reconciliationgetserverinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/removeaccountfrompool.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/resetconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/resetconnectorv1.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/retrytransferinitiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/reversetransferinitiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/reverttransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/runscript.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/runworkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/searchgetserverinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/sendevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/testconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/testtrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/udpatetransferinitiationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/uninstallconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/uninstallconnectorv1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/updatebankaccountmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/updateclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/updateconnectorconfigv1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/updatemapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/updatemetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/updatewallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2addmetadataontransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2addmetadatatoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2cancelevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2countaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2counttransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2createbulk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2createledger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2createtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2createtrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2createworkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2deleteaccountmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2deleteledgermetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2deletetransactionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2deletetrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2deleteworkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2getaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2getbalancesaggregated.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2getinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2getinstance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2getinstancehistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2getinstancestagehistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2getledger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2getledgerinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2getserverinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2gettransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2getvolumeswithbalances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2getworkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2listaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2listinstances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2listledgers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2listlogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2listtransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2listtriggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2listtriggersoccurrences.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2listworkflows.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2readstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2readtrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2reverttransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2runworkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2sendevent.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/v2updateledgermetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/voidhold.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/operations/walletsgetserverinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:45.348038 formance-sdk-python-2.2.3/src/sdk/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)    20407 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/accountbalance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/accountrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/accountresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/accountscursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/accountscursorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/accounttype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/accountwithvolumesandbalances.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/activityconfirmhold.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/activitycreatetransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/activitycreatetransactionoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/activitycreditwallet.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/activitydebitwallet.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/activitydebitwalletoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/activitygetaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/activitygetaccountoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/activitygetpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/activitygetpaymentoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/activitygetwallet.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/activitygetwalletoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/activitylistwallets.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/activityreverttransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/activityreverttransactionoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/activitystripetransfer.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/activityvoidhold.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/addaccounttopoolrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/adyenconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/aggregatebalancesresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/assetholder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/atlarconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/attempt.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/attemptresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/balancescursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/balancescursorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/balancewithassets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/bankaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/bankaccountrelatedaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/bankaccountrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/bankaccountresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/bankaccountscursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/bankingcircleconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/clientsecret.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/configchangesecret.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/configinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/configinforesponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/configresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/configsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/configuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/confirmholdrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/connectorconfigresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/connectorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/connectorsconfigsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/connectorsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/createbalancerequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/createbalanceresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/createclientrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/createclientresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/createsecretrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/createsecretresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/createtriggerresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/createwalletrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/createwalletresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/createworkflowrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/createworkflowresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/creditwalletrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/currencycloudconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/debitwalletrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/debitwalletresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/dummypayconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/errorsenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/expandeddebithold.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/forwardbankaccountrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/genericconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/getbalanceresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/getholdresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/getholdsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/gettransactionsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/getversionsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/getwalletresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/getwalletsummaryresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/getworkflowinstancehistoryresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/getworkflowinstanceresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/getworkflowresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/hold.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/ledgeraccountsubject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/ledgerinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/ledgerinforesponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/ledgerstorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/listbalancesresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/listclientsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/listrunsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/listtriggersoccurrencesresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/listtriggersresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/listusersresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/listwalletsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/listworkflowsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/logscursorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/mangopayconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/mappingresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/migrationinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/modulrconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/monetary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/moneycorpconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationlistwalletsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationpaymentadjustment.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationpaymentmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationpaymentstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationposttransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationv2transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/paymentadjustment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/paymentrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/paymentresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/paymentsaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/paymentsaccountresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/paymentscheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/paymentscursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/paymentstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/paymenttype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/policiescursorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/policyrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/policyresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/poolbalance.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/poolbalances.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/poolbalancesresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/poolrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/poolresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/poolscursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/posting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/posttransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/readclientresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/readtriggerresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/readuserresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/reconciliation.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/reconciliationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/reconciliationresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/reconciliationscursorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/reversetransferinitiationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/runworkflowresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/scriptresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/serverinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/stagedelay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/stagesend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/stagesenddestination.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/stagesenddestinationaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/stagesenddestinationpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/stagesenddestinationwallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/stagesendsource.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/stagesendsourceaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/stagesendsourcepayment.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/stagesendsourcewallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/stagestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/stagewaitevent.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/statsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/stripeconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/taskbankingcircle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/taskcurrencycloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/taskdummypay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/taskmangopay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/taskmodulr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/taskmoneycorp.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/taskresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/taskscursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/taskstripe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/taskwise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/transactiondata.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/transactionresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/transactionscursorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/transactionsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/transferinitiation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/transferinitiationadjusments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/transferinitiationpayments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/transferinitiationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/transferinitiationresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/transferinitiationscursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/transferinitiationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/transferrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/transferresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/triggerdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/triggeroccurrence.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/updatebankaccountmetadatarequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/updateclientrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/updateclientresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/updatetransferinitiationstatusrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2account.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2accountresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2accountscursorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2activityconfirmhold.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitycreatetransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitycreatetransactionoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitycreditwallet.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitydebitwallet.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitydebitwalletoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitygetaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitygetaccountoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitygetpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitygetpaymentoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitygetwallet.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitygetwalletoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitylistwallets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitystripetransfer.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2activityvoidhold.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2aggregatebalancesresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2assetholder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2bulkelementaddmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2bulkelementcreatetransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2bulkelementdeletemetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2bulkelementresult.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2bulkelementreverttransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2bulkresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2configinforesponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2connector.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2createledgerrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2createtransactionresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2createtriggerresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2createworkflowrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2createworkflowresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2creditwalletrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2debitwalletrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2errorsenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2expandedtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2getledgerresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2gettransactionresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2getworkflowinstancehistoryresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2getworkflowinstancehistorystageresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2getworkflowinstanceresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2getworkflowresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2hold.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2ledger.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2ledgeraccountsubject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2ledgerinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2ledgerinforesponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2ledgerlistresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2listrunsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2listtriggersoccurrencesresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2listtriggersresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2listwalletsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2listworkflowsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2logscursorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2migrationinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2monetary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2paymentadjustment.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2paymentmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2paymentstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2posting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2posttransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2readtriggerresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2reverttransactionresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2runworkflowresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2serverinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagedelay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagesend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagesenddestination.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagesenddestinationaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagesenddestinationpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagesenddestinationwallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagesendsource.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagesendsourceaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagesendsourcepayment.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagesendsourcewallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagewaitevent.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2statsresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2targettype.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2testtriggerresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2transactionscursorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2triggerdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2triggeroccurrence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2triggertest.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2volume.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2volumeswithbalance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2volumeswithbalancecursorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2walletsubject.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2walletwithbalances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2workflowconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2workflowinstance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2workflowinstancehistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2workflowinstancehistorystage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2workflowinstancehistorystageinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/v2workflowinstancehistorystageoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/walletstransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/walletsubject.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/walletsvolume.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/walletwithbalances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/webhooksconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/webhookserrorsenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/wiseconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/workflowconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/workflowinstance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/workflowinstancehistory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/workflowinstancehistorystage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/workflowinstancehistorystageinput.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/models/shared/workflowinstancehistorystageoutput.py
--rw-r--r--   0 runner    (1001) docker     (127)   107272 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/orchestration.py
--rw-r--r--   0 runner    (1001) docker     (127)   118661 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/payments.py
--rw-r--r--   0 runner    (1001) docker     (127)    25271 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/reconciliation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:45.348038 formance-sdk-python-2.2.3/src/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    48539 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)    22924 2024-04-29 14:33:33.000000 formance-sdk-python-2.2.3/src/sdk/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:35:22.763372 formance-sdk-python-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    37644 2024-05-31 09:35:22.763372 formance-sdk-python-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23163 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 09:35:22.763372 formance-sdk-python-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:35:22.679372 formance-sdk-python-2.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:35:22.679372 formance-sdk-python-2.3.0/src/formance_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    37644 2024-05-31 09:35:22.000000 formance-sdk-python-2.3.0/src/formance_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23711 2024-05-31 09:35:22.000000 formance-sdk-python-2.3.0/src/formance_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 09:35:22.000000 formance-sdk-python-2.3.0/src/formance_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-31 09:35:22.000000 formance-sdk-python-2.3.0/src/formance_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-31 09:35:22.000000 formance-sdk-python-2.3.0/src/formance_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:35:22.683372 formance-sdk-python-2.3.0/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:35:22.683372 formance-sdk-python-2.3.0/src/sdk/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24574 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)   141022 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/ledger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:35:22.683372 formance-sdk-python-2.3.0/src/sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:35:22.687372 formance-sdk-python-2.3.0/src/sdk/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/errors/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/errors/errorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/errors/paymentserrorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/errors/reconciliationerrorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/errors/sdkerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/errors/v2error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/errors/v2errorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/errors/walletserrorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/errors/webhookserrorresponse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:35:22.711372 formance-sdk-python-2.3.0/src/sdk/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/activateconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/addaccounttopool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/addmetadataontransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/addmetadatatoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/cancelevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/changeconfigsecret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/confirmhold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/connectorstransfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/countaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/counttransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/createaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/createbalance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/createbankaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/createclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/createpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/createpolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/createpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/createsecret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/createtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/createtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/createtransferinitiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/createtrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/createwallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/createworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/creditwallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/deactivateconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/debitwallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/deleteclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/deleteconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/deletepolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/deletepool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/deletesecret.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/deletetransferinitiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/deletetrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/deleteworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/forwardbankaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getaccountbalances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getbalance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getbalances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getbalancesaggregated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getbankaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getconnectortask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getconnectortaskv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/gethold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getholds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getinstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getinstancehistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getinstancestagehistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getledgerinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getmanyconfigs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getmapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getoidcwellknowns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getpolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getpoolbalances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getreconciliation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/gettransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/gettransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/gettransferinitiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getwallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getwalletsummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/getworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/insertconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/installconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listallconnectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listbalances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listbankaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listclients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listconfigsavailableconnectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listconnectortasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listconnectortasksv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listinstances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listlogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listpayments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listpolicies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listpools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listreconciliations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listtransferinitiations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listtriggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listtriggersoccurrences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listusers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listwallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/listworkflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/orchestrationgetserverinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/paymentsgetaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/paymentsgetserverinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/paymentslistaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/readclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/readconnectorconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/readconnectorconfigv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/readstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/readtrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/readuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/reconcile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/reconciliationgetserverinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/removeaccountfrompool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/resetconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/resetconnectorv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/retrytransferinitiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/reversetransferinitiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/reverttransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/runscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/runworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/searchgetserverinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/sendevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/testconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/testtrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/udpatetransferinitiationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/uninstallconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/uninstallconnectorv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/updatebankaccountmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/updateclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/updateconnectorconfigv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/updatemapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/updatemetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/updatewallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2addmetadataontransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2addmetadatatoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2cancelevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2countaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2counttransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2createbulk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2createledger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2createtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2createtrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2createworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2deleteaccountmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2deleteledgermetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2deletetransactionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2deletetrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2deleteworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2getaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2getbalancesaggregated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2getinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2getinstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2getinstancehistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2getinstancestagehistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2getledger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2getledgerinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2getserverinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2gettransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2getvolumeswithbalances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2getworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2listaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2listinstances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2listledgers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2listlogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2listtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2listtriggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2listtriggersoccurrences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2listworkflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2readstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2readtrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2reverttransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2runworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2sendevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/v2updateledgermetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/voidhold.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/operations/walletsgetserverinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:35:22.763372 formance-sdk-python-2.3.0/src/sdk/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)    21092 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/accountbalance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/accountrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/accountresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/accountscursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/accountscursorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/accounttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/accountwithvolumesandbalances.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activityaddaccountmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activityconfirmhold.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activitycreatetransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activitycreatetransactionoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activitycreditwallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activitydebitwallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activitydebitwalletoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activitygetaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activitygetaccountoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activitygetpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activitygetpaymentoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activitygetwallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activitygetwalletoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activitylistwallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activityreverttransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activityreverttransactionoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activitystripetransfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/activityvoidhold.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/addaccounttopoolrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/adyenconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/aggregatebalancesresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/assetholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/atlarconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/attempt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/attemptresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/balancescursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/balancescursorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/balancewithassets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/bankaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/bankaccountrelatedaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/bankaccountrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/bankaccountresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/bankaccountscursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/bankingcircleconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/clientsecret.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/configchangesecret.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/configinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/configinforesponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/configresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/configsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/configuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/confirmholdrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/connectorconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/connectorconfigresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/connectorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/connectorsconfigsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/connectorsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/createbalancerequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/createbalanceresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/createclientrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/createclientresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/createsecretrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/createsecretresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/createtriggerresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/createwalletrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/createwalletresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/createworkflowrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/createworkflowresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/creditwalletrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/currencycloudconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/debitwalletrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/debitwalletresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/dummypayconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/errorsenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/expandeddebithold.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/forwardbankaccountrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/genericconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/getbalanceresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/getholdresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/getholdsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/gettransactionsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/getversionsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/getwalletresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/getwalletsummaryresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/getworkflowinstancehistoryresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/getworkflowinstanceresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/getworkflowresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/hold.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/ledgeraccountsubject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/ledgerinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/ledgerinforesponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/ledgerstorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/listbalancesresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/listclientsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/listrunsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/listtriggersoccurrencesresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/listtriggersresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/listusersresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/listwalletsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/listworkflowsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/logscursorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/mangopayconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/mappingresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/migrationinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/modulrconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/monetary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/moneycorpconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationlistwalletsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationpaymentadjustment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationpaymentmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationpaymentstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationposttransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationv2transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/paymentadjustment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/paymentrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/paymentresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/paymentsaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/paymentsaccountresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/paymentscheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/paymentscursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/paymentserrorsenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/paymentstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/paymenttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/policiescursorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/policyrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/policyresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/poolbalance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/poolbalances.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/poolbalancesresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/poolrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/poolresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/poolscursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/posting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/posttransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/readclientresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/readtriggerresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/readuserresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/reconciliation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/reconciliationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/reconciliationresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/reconciliationscursorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/reversetransferinitiationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/runworkflowresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/scriptresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/serverinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/stagedelay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/stagesend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/stagesenddestination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/stagesenddestinationaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/stagesenddestinationpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/stagesenddestinationwallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/stagesendsource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/stagesendsourceaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/stagesendsourcepayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/stagesendsourcewallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/stagestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/stagewaitevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/statsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/stripeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/taskbankingcircle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/taskcurrencycloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/taskdummypay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/taskmangopay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/taskmodulr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/taskmoneycorp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/taskresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/taskscursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/taskstripe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/taskwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/transactiondata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/transactionresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/transactionscursorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/transactionsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/transferinitiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/transferinitiationadjusments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/transferinitiationpayments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/transferinitiationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/transferinitiationresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/transferinitiationscursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/transferinitiationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/transferrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/transferresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/triggerdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/triggeroccurrence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/updateaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/updatebankaccountmetadatarequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/updateclientrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/updateclientresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/updatetransferinitiationstatusrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2accountresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2accountscursorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2activityaddaccountmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2activityconfirmhold.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitycreatetransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitycreatetransactionoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitycreditwallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitydebitwallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitydebitwalletoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitygetaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitygetaccountoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitygetpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitygetpaymentoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitygetwallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitygetwalletoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitylistwallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitystripetransfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2activityvoidhold.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2aggregatebalancesresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2assetholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2bulkelement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2bulkelementaddmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2bulkelementcreatetransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2bulkelementdeletemetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2bulkelementresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2bulkelementreverttransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2bulkresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2configinforesponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2createledgerrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2createtransactionresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2createtriggerresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2createworkflowrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2createworkflowresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2creditwalletrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2debitwalletrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2errorsenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2expandedtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2getledgerresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2gettransactionresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2getworkflowinstancehistoryresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2getworkflowinstancehistorystageresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2getworkflowinstanceresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2getworkflowresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2hold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2ledger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2ledgeraccountsubject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2ledgerinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2ledgerinforesponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2ledgerlistresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2listrunsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2listtriggersoccurrencesresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2listtriggersresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2listwalletsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2listworkflowsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2logscursorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2migrationinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2monetary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2paymentadjustment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2paymentmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2paymentstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2posting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2posttransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2readtriggerresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2reverttransactionresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2runworkflowresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2serverinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagedelay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagesend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagesenddestination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagesenddestinationaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagesenddestinationpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagesenddestinationwallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagesendsource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagesendsourceaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagesendsourcepayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagesendsourcewallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagewaitevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2statsresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2targetid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2targettype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2testtriggerresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2transactionscursorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2triggerdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2triggeroccurrence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2triggertest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2updateaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2volumeswithbalance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2volumeswithbalancecursorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2walletsubject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2walletwithbalances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2workflowconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2workflowinstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2workflowinstancehistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2workflowinstancehistorystage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2workflowinstancehistorystageinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/v2workflowinstancehistorystageoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/walletstransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/walletsubject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/walletsvolume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/walletwithbalances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/webhooksconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/webhookserrorsenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/wiseconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/workflowconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/workflowinstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/workflowinstancehistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/workflowinstancehistorystage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/workflowinstancehistorystageinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/models/shared/workflowinstancehistorystageoutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)   110090 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/orchestration.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137262 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25946 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/reconciliation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:35:22.763372 formance-sdk-python-2.3.0/src/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32697 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49761 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23509 2024-05-31 09:35:13.000000 formance-sdk-python-2.3.0/src/sdk/webhooks.py
```

### Comparing `formance-sdk-python-2.2.3/LICENSE` & `formance-sdk-python-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/PKG-INFO` & `formance-sdk-python-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formance-sdk-python
-Version: 2.2.3
+Version: 2.3.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/formancehq/formance-sdk-python.git
 Author: Formance
 License: UNKNOWN
 Description: # formance-sdk-python
         
         <div align="left">
@@ -266,15 +266,17 @@
         import sdk
         from sdk.models import errors, operations, shared
         
         s = sdk.SDK(
             authorization="<YOUR_AUTHORIZATION_HERE>",
         )
         
-        req = operations.CreateTransactionsRequest(
+        res = None
+        try:
+            res = s.ledger.create_transactions(request=operations.CreateTransactionsRequest(
             transactions=shared.Transactions(
                 transactions=[
                     shared.TransactionData(
                         postings=[
                             shared.Posting(
                                 amount=100,
                                 asset='COIN',
@@ -283,19 +285,16 @@
                             ),
                         ],
                         reference='ref:001',
                     ),
                 ],
             ),
             ledger='ledger001',
-        )
+        ))
         
-        res = None
-        try:
-            res = s.ledger.create_transactions(req)
         except errors.ErrorResponse as e:
             # handle exception
             raise(e)
         except errors.SDKError as e:
             # handle exception
             raise(e)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: formance-sdk-python Version: 2.2.3 Summary: Python
+Metadata-Version: 2.1 Name: formance-sdk-python Version: 2.3.0 Summary: Python
 Client SDK Generated by Speakeasy Home-page: https://github.com/formancehq/
 formance-sdk-python.git Author: Formance License: UNKNOWN Description: #
 formance-sdk-python
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## ð **Welcome to your new SDK!** ð It has been generated successfully
@@ -395,48 +395,49 @@
 this SDK should largely match your expectations. All operations return a
 response object or raise an error. If Error objects are specified in your
 OpenAPI Spec, the SDK will raise the appropriate Error type. | Error Object |
 Status Code | Content Type | | -------------------- | -------------------- | --
 ------------------ | | errors.ErrorResponse | default | application/json | |
 errors.SDKError | 4xx-5xx | */* | ### Example ```python import sdk from
 sdk.models import errors, operations, shared s = sdk.SDK( authorization="", )
-req = operations.CreateTransactionsRequest( transactions=shared.Transactions
+res = None try: res = s.ledger.create_transactions
+(request=operations.CreateTransactionsRequest( transactions=shared.Transactions
 ( transactions=[ shared.TransactionData( postings=[ shared.Posting( amount=100,
 asset='COIN', destination='users:002', source='users:001', ), ],
-reference='ref:001', ), ], ), ledger='ledger001', ) res = None try: res =
-s.ledger.create_transactions(req) except errors.ErrorResponse as e: # handle
-exception raise(e) except errors.SDKError as e: # handle exception raise(e) if
-res.transactions_response is not None: # handle response pass ``` ## Server
-Selection ### Select Server by Index You can override the default server
-globally by passing a server index to the `server_idx: int` optional parameter
-when initializing the SDK client instance. The selected server will then be
-used as the default on the operations that use it. This table lists the indexes
-associated with the available servers: | # | Server | Variables | | - | -----
-- | --------- | | 0 | `http://localhost` | None | #### Example ```python import
-sdk s = sdk.SDK( server_idx=0, authorization="", ) res = s.get_oidc_well_knowns
-() if res is not None: # handle response pass ``` ### Override Server URL Per-
-Client The default server can also be overridden globally by passing a URL to
-the `server_url: str` optional parameter when initializing the SDK client
-instance. For example: ```python import sdk s = sdk.SDK( server_url="http://
-localhost", authorization="", ) res = s.get_oidc_well_knowns() if res is not
-None: # handle response pass ``` ## Custom HTTP Client The Python SDK makes API
-calls using the [requests](https://pypi.org/project/requests/) HTTP library. In
-order to provide a convenient way to configure timeouts, cookies, proxies,
-custom headers, and other low-level configuration, you can initialize the SDK
-client with a custom `requests.Session` object. For example, you could specify
-a header for every request that this sdk makes as follows: ```python import sdk
-import requests http_client = requests.Session() http_client.headers.update(
-{'x-custom-header': 'someValue'}) s = sdk.SDK(client=http_client) ``` ##
-Authentication ### Per-Client Security Schemes This SDK supports the following
-security scheme globally: | Name | Type | Scheme | | --------------- | --------
-------- | --------------- | | `authorization` | oauth2 | OAuth2 token | To
-authenticate with the API the `authorization` parameter must be set when
-initializing the SDK client instance. For example: ```python import sdk s =
-sdk.SDK( authorization="", ) res = s.get_oidc_well_knowns() if res is not None:
-# handle response pass ``` # Development ## Maturity This SDK is in beta, and
+reference='ref:001', ), ], ), ledger='ledger001', )) except
+errors.ErrorResponse as e: # handle exception raise(e) except errors.SDKError
+as e: # handle exception raise(e) if res.transactions_response is not None: #
+handle response pass ``` ## Server Selection ### Select Server by Index You can
+override the default server globally by passing a server index to the
+`server_idx: int` optional parameter when initializing the SDK client instance.
+The selected server will then be used as the default on the operations that use
+it. This table lists the indexes associated with the available servers: | # |
+Server | Variables | | - | ------ | --------- | | 0 | `http://localhost` | None
+| #### Example ```python import sdk s = sdk.SDK( server_idx=0,
+authorization="", ) res = s.get_oidc_well_knowns() if res is not None: # handle
+response pass ``` ### Override Server URL Per-Client The default server can
+also be overridden globally by passing a URL to the `server_url: str` optional
+parameter when initializing the SDK client instance. For example: ```python
+import sdk s = sdk.SDK( server_url="http://localhost", authorization="", ) res
+= s.get_oidc_well_knowns() if res is not None: # handle response pass ``` ##
+Custom HTTP Client The Python SDK makes API calls using the [requests](https://
+pypi.org/project/requests/) HTTP library. In order to provide a convenient way
+to configure timeouts, cookies, proxies, custom headers, and other low-level
+configuration, you can initialize the SDK client with a custom
+`requests.Session` object. For example, you could specify a header for every
+request that this sdk makes as follows: ```python import sdk import requests
+http_client = requests.Session() http_client.headers.update({'x-custom-header':
+'someValue'}) s = sdk.SDK(client=http_client) ``` ## Authentication ### Per-
+Client Security Schemes This SDK supports the following security scheme
+globally: | Name | Type | Scheme | | --------------- | --------------- | ------
+--------- | | `authorization` | oauth2 | OAuth2 token | To authenticate with
+the API the `authorization` parameter must be set when initializing the SDK
+client instance. For example: ```python import sdk s = sdk.SDK
+( authorization="", ) res = s.get_oidc_well_knowns() if res is not None: #
+handle response pass ``` # Development ## Maturity This SDK is in beta, and
 there may be breaking changes between versions without a major version update.
 Therefore, we recommend pinning usage to a specific package version. This way,
 you can install the same version each time without breaking changes unless you
 are intentionally looking for the latest version. ## Contributions While we
 value open-source contributions to this SDK, this library is generated
 programmatically. Feel free to open a PR or a Github issue as a proof of
 concept and we'll do our best to include it in a future release! ### SDK
```

### Comparing `formance-sdk-python-2.2.3/README.md` & `formance-sdk-python-2.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,17 @@
 import sdk
 from sdk.models import errors, operations, shared
 
 s = sdk.SDK(
     authorization="<YOUR_AUTHORIZATION_HERE>",
 )
 
-req = operations.CreateTransactionsRequest(
+res = None
+try:
+    res = s.ledger.create_transactions(request=operations.CreateTransactionsRequest(
     transactions=shared.Transactions(
         transactions=[
             shared.TransactionData(
                 postings=[
                     shared.Posting(
                         amount=100,
                         asset='COIN',
@@ -276,19 +278,16 @@
                     ),
                 ],
                 reference='ref:001',
             ),
         ],
     ),
     ledger='ledger001',
-)
+))
 
-res = None
-try:
-    res = s.ledger.create_transactions(req)
 except errors.ErrorResponse as e:
     # handle exception
     raise(e)
 except errors.SDKError as e:
     # handle exception
     raise(e)
```

#### html2text {}

```diff
@@ -254,19 +254,19 @@
 Handling errors in this SDK should largely match your expectations. All
 operations return a response object or raise an error. If Error objects are
 specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
 | Error Object | Status Code | Content Type | | -------------------- | --------
 ------------ | -------------------- | | errors.ErrorResponse | default |
 application/json | | errors.SDKError | 4xx-5xx | */* | ### Example ```python
 import sdk from sdk.models import errors, operations, shared s = sdk.SDK
-( authorization="", ) req = operations.CreateTransactionsRequest
-( transactions=shared.Transactions( transactions=[ shared.TransactionData
-( postings=[ shared.Posting( amount=100, asset='COIN', destination='users:002',
-source='users:001', ), ], reference='ref:001', ), ], ), ledger='ledger001', )
-res = None try: res = s.ledger.create_transactions(req) except
+( authorization="", ) res = None try: res = s.ledger.create_transactions
+(request=operations.CreateTransactionsRequest( transactions=shared.Transactions
+( transactions=[ shared.TransactionData( postings=[ shared.Posting( amount=100,
+asset='COIN', destination='users:002', source='users:001', ), ],
+reference='ref:001', ), ], ), ledger='ledger001', )) except
 errors.ErrorResponse as e: # handle exception raise(e) except errors.SDKError
 as e: # handle exception raise(e) if res.transactions_response is not None: #
 handle response pass ``` ## Server Selection ### Select Server by Index You can
 override the default server globally by passing a server index to the
 `server_idx: int` optional parameter when initializing the SDK client instance.
 The selected server will then be used as the default on the operations that use
 it. This table lists the indexes associated with the available servers: | # |
```

### Comparing `formance-sdk-python-2.2.3/setup.py` & `formance-sdk-python-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='formance-sdk-python',
-    version='2.2.3',
+    version='2.3.0',
     author='Formance',
     description='Python Client SDK Generated by Speakeasy',
     url='https://github.com/formancehq/formance-sdk-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `formance-sdk-python-2.2.3/src/formance_sdk_python.egg-info/PKG-INFO` & `formance-sdk-python-2.3.0/src/formance_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formance-sdk-python
-Version: 2.2.3
+Version: 2.3.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/formancehq/formance-sdk-python.git
 Author: Formance
 License: UNKNOWN
 Description: # formance-sdk-python
         
         <div align="left">
@@ -266,15 +266,17 @@
         import sdk
         from sdk.models import errors, operations, shared
         
         s = sdk.SDK(
             authorization="<YOUR_AUTHORIZATION_HERE>",
         )
         
-        req = operations.CreateTransactionsRequest(
+        res = None
+        try:
+            res = s.ledger.create_transactions(request=operations.CreateTransactionsRequest(
             transactions=shared.Transactions(
                 transactions=[
                     shared.TransactionData(
                         postings=[
                             shared.Posting(
                                 amount=100,
                                 asset='COIN',
@@ -283,19 +285,16 @@
                             ),
                         ],
                         reference='ref:001',
                     ),
                 ],
             ),
             ledger='ledger001',
-        )
+        ))
         
-        res = None
-        try:
-            res = s.ledger.create_transactions(req)
         except errors.ErrorResponse as e:
             # handle exception
             raise(e)
         except errors.SDKError as e:
             # handle exception
             raise(e)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: formance-sdk-python Version: 2.2.3 Summary: Python
+Metadata-Version: 2.1 Name: formance-sdk-python Version: 2.3.0 Summary: Python
 Client SDK Generated by Speakeasy Home-page: https://github.com/formancehq/
 formance-sdk-python.git Author: Formance License: UNKNOWN Description: #
 formance-sdk-python
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
 ## ð **Welcome to your new SDK!** ð It has been generated successfully
@@ -395,48 +395,49 @@
 this SDK should largely match your expectations. All operations return a
 response object or raise an error. If Error objects are specified in your
 OpenAPI Spec, the SDK will raise the appropriate Error type. | Error Object |
 Status Code | Content Type | | -------------------- | -------------------- | --
 ------------------ | | errors.ErrorResponse | default | application/json | |
 errors.SDKError | 4xx-5xx | */* | ### Example ```python import sdk from
 sdk.models import errors, operations, shared s = sdk.SDK( authorization="", )
-req = operations.CreateTransactionsRequest( transactions=shared.Transactions
+res = None try: res = s.ledger.create_transactions
+(request=operations.CreateTransactionsRequest( transactions=shared.Transactions
 ( transactions=[ shared.TransactionData( postings=[ shared.Posting( amount=100,
 asset='COIN', destination='users:002', source='users:001', ), ],
-reference='ref:001', ), ], ), ledger='ledger001', ) res = None try: res =
-s.ledger.create_transactions(req) except errors.ErrorResponse as e: # handle
-exception raise(e) except errors.SDKError as e: # handle exception raise(e) if
-res.transactions_response is not None: # handle response pass ``` ## Server
-Selection ### Select Server by Index You can override the default server
-globally by passing a server index to the `server_idx: int` optional parameter
-when initializing the SDK client instance. The selected server will then be
-used as the default on the operations that use it. This table lists the indexes
-associated with the available servers: | # | Server | Variables | | - | -----
-- | --------- | | 0 | `http://localhost` | None | #### Example ```python import
-sdk s = sdk.SDK( server_idx=0, authorization="", ) res = s.get_oidc_well_knowns
-() if res is not None: # handle response pass ``` ### Override Server URL Per-
-Client The default server can also be overridden globally by passing a URL to
-the `server_url: str` optional parameter when initializing the SDK client
-instance. For example: ```python import sdk s = sdk.SDK( server_url="http://
-localhost", authorization="", ) res = s.get_oidc_well_knowns() if res is not
-None: # handle response pass ``` ## Custom HTTP Client The Python SDK makes API
-calls using the [requests](https://pypi.org/project/requests/) HTTP library. In
-order to provide a convenient way to configure timeouts, cookies, proxies,
-custom headers, and other low-level configuration, you can initialize the SDK
-client with a custom `requests.Session` object. For example, you could specify
-a header for every request that this sdk makes as follows: ```python import sdk
-import requests http_client = requests.Session() http_client.headers.update(
-{'x-custom-header': 'someValue'}) s = sdk.SDK(client=http_client) ``` ##
-Authentication ### Per-Client Security Schemes This SDK supports the following
-security scheme globally: | Name | Type | Scheme | | --------------- | --------
-------- | --------------- | | `authorization` | oauth2 | OAuth2 token | To
-authenticate with the API the `authorization` parameter must be set when
-initializing the SDK client instance. For example: ```python import sdk s =
-sdk.SDK( authorization="", ) res = s.get_oidc_well_knowns() if res is not None:
-# handle response pass ``` # Development ## Maturity This SDK is in beta, and
+reference='ref:001', ), ], ), ledger='ledger001', )) except
+errors.ErrorResponse as e: # handle exception raise(e) except errors.SDKError
+as e: # handle exception raise(e) if res.transactions_response is not None: #
+handle response pass ``` ## Server Selection ### Select Server by Index You can
+override the default server globally by passing a server index to the
+`server_idx: int` optional parameter when initializing the SDK client instance.
+The selected server will then be used as the default on the operations that use
+it. This table lists the indexes associated with the available servers: | # |
+Server | Variables | | - | ------ | --------- | | 0 | `http://localhost` | None
+| #### Example ```python import sdk s = sdk.SDK( server_idx=0,
+authorization="", ) res = s.get_oidc_well_knowns() if res is not None: # handle
+response pass ``` ### Override Server URL Per-Client The default server can
+also be overridden globally by passing a URL to the `server_url: str` optional
+parameter when initializing the SDK client instance. For example: ```python
+import sdk s = sdk.SDK( server_url="http://localhost", authorization="", ) res
+= s.get_oidc_well_knowns() if res is not None: # handle response pass ``` ##
+Custom HTTP Client The Python SDK makes API calls using the [requests](https://
+pypi.org/project/requests/) HTTP library. In order to provide a convenient way
+to configure timeouts, cookies, proxies, custom headers, and other low-level
+configuration, you can initialize the SDK client with a custom
+`requests.Session` object. For example, you could specify a header for every
+request that this sdk makes as follows: ```python import sdk import requests
+http_client = requests.Session() http_client.headers.update({'x-custom-header':
+'someValue'}) s = sdk.SDK(client=http_client) ``` ## Authentication ### Per-
+Client Security Schemes This SDK supports the following security scheme
+globally: | Name | Type | Scheme | | --------------- | --------------- | ------
+--------- | | `authorization` | oauth2 | OAuth2 token | To authenticate with
+the API the `authorization` parameter must be set when initializing the SDK
+client instance. For example: ```python import sdk s = sdk.SDK
+( authorization="", ) res = s.get_oidc_well_knowns() if res is not None: #
+handle response pass ``` # Development ## Maturity This SDK is in beta, and
 there may be breaking changes between versions without a major version update.
 Therefore, we recommend pinning usage to a specific package version. This way,
 you can install the same version each time without breaking changes unless you
 are intentionally looking for the latest version. ## Contributions While we
 value open-source contributions to this SDK, this library is generated
 programmatically. Feel free to open a PR or a Github issue as a proof of
 concept and we'll do our best to include it in a future release! ### SDK
```

### Comparing `formance-sdk-python-2.2.3/src/formance_sdk_python.egg-info/SOURCES.txt` & `formance-sdk-python-2.3.0/src/formance_sdk_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 src/sdk/_hooks/registration.py
 src/sdk/_hooks/sdkhooks.py
 src/sdk/_hooks/types.py
 src/sdk/models/__init__.py
 src/sdk/models/errors/__init__.py
 src/sdk/models/errors/error.py
 src/sdk/models/errors/errorresponse.py
+src/sdk/models/errors/paymentserrorresponse.py
 src/sdk/models/errors/reconciliationerrorresponse.py
 src/sdk/models/errors/sdkerror.py
 src/sdk/models/errors/v2error.py
 src/sdk/models/errors/v2errorresponse.py
 src/sdk/models/errors/walletserrorresponse.py
 src/sdk/models/errors/webhookserrorresponse.py
 src/sdk/models/operations/__init__.py
@@ -203,14 +204,15 @@
 src/sdk/models/shared/accountbalance.py
 src/sdk/models/shared/accountrequest.py
 src/sdk/models/shared/accountresponse.py
 src/sdk/models/shared/accountscursor.py
 src/sdk/models/shared/accountscursorresponse.py
 src/sdk/models/shared/accounttype.py
 src/sdk/models/shared/accountwithvolumesandbalances.py
+src/sdk/models/shared/activityaddaccountmetadata.py
 src/sdk/models/shared/activityconfirmhold.py
 src/sdk/models/shared/activitycreatetransaction.py
 src/sdk/models/shared/activitycreatetransactionoutput.py
 src/sdk/models/shared/activitycreditwallet.py
 src/sdk/models/shared/activitydebitwallet.py
 src/sdk/models/shared/activitydebitwalletoutput.py
 src/sdk/models/shared/activitygetaccount.py
@@ -248,14 +250,15 @@
 src/sdk/models/shared/configinfo.py
 src/sdk/models/shared/configinforesponse.py
 src/sdk/models/shared/configresponse.py
 src/sdk/models/shared/configsresponse.py
 src/sdk/models/shared/configuser.py
 src/sdk/models/shared/confirmholdrequest.py
 src/sdk/models/shared/connector.py
+src/sdk/models/shared/connectorconfig.py
 src/sdk/models/shared/connectorconfigresponse.py
 src/sdk/models/shared/connectorresponse.py
 src/sdk/models/shared/connectorsconfigsresponse.py
 src/sdk/models/shared/connectorsresponse.py
 src/sdk/models/shared/contract.py
 src/sdk/models/shared/createbalancerequest.py
 src/sdk/models/shared/createbalanceresponse.py
@@ -324,14 +327,15 @@
 src/sdk/models/shared/paymentadjustment.py
 src/sdk/models/shared/paymentrequest.py
 src/sdk/models/shared/paymentresponse.py
 src/sdk/models/shared/paymentsaccount.py
 src/sdk/models/shared/paymentsaccountresponse.py
 src/sdk/models/shared/paymentscheme.py
 src/sdk/models/shared/paymentscursor.py
+src/sdk/models/shared/paymentserrorsenum.py
 src/sdk/models/shared/paymentstatus.py
 src/sdk/models/shared/paymenttype.py
 src/sdk/models/shared/policiescursorresponse.py
 src/sdk/models/shared/policy.py
 src/sdk/models/shared/policyrequest.py
 src/sdk/models/shared/policyresponse.py
 src/sdk/models/shared/pool.py
@@ -355,14 +359,15 @@
 src/sdk/models/shared/reversetransferinitiationrequest.py
 src/sdk/models/shared/runworkflowresponse.py
 src/sdk/models/shared/script.py
 src/sdk/models/shared/scriptresponse.py
 src/sdk/models/shared/secret.py
 src/sdk/models/shared/security.py
 src/sdk/models/shared/serverinfo.py
+src/sdk/models/shared/stage.py
 src/sdk/models/shared/stagedelay.py
 src/sdk/models/shared/stagesend.py
 src/sdk/models/shared/stagesenddestination.py
 src/sdk/models/shared/stagesenddestinationaccount.py
 src/sdk/models/shared/stagesenddestinationpayment.py
 src/sdk/models/shared/stagesenddestinationwallet.py
 src/sdk/models/shared/stagesendsource.py
@@ -370,14 +375,15 @@
 src/sdk/models/shared/stagesendsourcepayment.py
 src/sdk/models/shared/stagesendsourcewallet.py
 src/sdk/models/shared/stagestatus.py
 src/sdk/models/shared/stagewaitevent.py
 src/sdk/models/shared/stats.py
 src/sdk/models/shared/statsresponse.py
 src/sdk/models/shared/stripeconfig.py
+src/sdk/models/shared/subject.py
 src/sdk/models/shared/taskbankingcircle.py
 src/sdk/models/shared/taskcurrencycloud.py
 src/sdk/models/shared/taskdummypay.py
 src/sdk/models/shared/taskmangopay.py
 src/sdk/models/shared/taskmodulr.py
 src/sdk/models/shared/taskmoneycorp.py
 src/sdk/models/shared/taskresponse.py
@@ -398,22 +404,25 @@
 src/sdk/models/shared/transferinitiationscursor.py
 src/sdk/models/shared/transferinitiationstatus.py
 src/sdk/models/shared/transferrequest.py
 src/sdk/models/shared/transferresponse.py
 src/sdk/models/shared/trigger.py
 src/sdk/models/shared/triggerdata.py
 src/sdk/models/shared/triggeroccurrence.py
+src/sdk/models/shared/update.py
+src/sdk/models/shared/updateaccount.py
 src/sdk/models/shared/updatebankaccountmetadatarequest.py
 src/sdk/models/shared/updateclientrequest.py
 src/sdk/models/shared/updateclientresponse.py
 src/sdk/models/shared/updatetransferinitiationstatusrequest.py
 src/sdk/models/shared/user.py
 src/sdk/models/shared/v2account.py
 src/sdk/models/shared/v2accountresponse.py
 src/sdk/models/shared/v2accountscursorresponse.py
+src/sdk/models/shared/v2activityaddaccountmetadata.py
 src/sdk/models/shared/v2activityconfirmhold.py
 src/sdk/models/shared/v2activitycreatetransaction.py
 src/sdk/models/shared/v2activitycreatetransactionoutput.py
 src/sdk/models/shared/v2activitycreditwallet.py
 src/sdk/models/shared/v2activitydebitwallet.py
 src/sdk/models/shared/v2activitydebitwalletoutput.py
 src/sdk/models/shared/v2activitygetaccount.py
@@ -423,14 +432,15 @@
 src/sdk/models/shared/v2activitygetwallet.py
 src/sdk/models/shared/v2activitygetwalletoutput.py
 src/sdk/models/shared/v2activitylistwallets.py
 src/sdk/models/shared/v2activitystripetransfer.py
 src/sdk/models/shared/v2activityvoidhold.py
 src/sdk/models/shared/v2aggregatebalancesresponse.py
 src/sdk/models/shared/v2assetholder.py
+src/sdk/models/shared/v2bulkelement.py
 src/sdk/models/shared/v2bulkelementaddmetadata.py
 src/sdk/models/shared/v2bulkelementcreatetransaction.py
 src/sdk/models/shared/v2bulkelementdeletemetadata.py
 src/sdk/models/shared/v2bulkelementresult.py
 src/sdk/models/shared/v2bulkelementreverttransaction.py
 src/sdk/models/shared/v2bulkresponse.py
 src/sdk/models/shared/v2configinforesponse.py
@@ -471,36 +481,41 @@
 src/sdk/models/shared/v2paymentstatus.py
 src/sdk/models/shared/v2posting.py
 src/sdk/models/shared/v2posttransaction.py
 src/sdk/models/shared/v2readtriggerresponse.py
 src/sdk/models/shared/v2reverttransactionresponse.py
 src/sdk/models/shared/v2runworkflowresponse.py
 src/sdk/models/shared/v2serverinfo.py
+src/sdk/models/shared/v2stage.py
 src/sdk/models/shared/v2stagedelay.py
 src/sdk/models/shared/v2stagesend.py
 src/sdk/models/shared/v2stagesenddestination.py
 src/sdk/models/shared/v2stagesenddestinationaccount.py
 src/sdk/models/shared/v2stagesenddestinationpayment.py
 src/sdk/models/shared/v2stagesenddestinationwallet.py
 src/sdk/models/shared/v2stagesendsource.py
 src/sdk/models/shared/v2stagesendsourceaccount.py
 src/sdk/models/shared/v2stagesendsourcepayment.py
 src/sdk/models/shared/v2stagesendsourcewallet.py
 src/sdk/models/shared/v2stagestatus.py
 src/sdk/models/shared/v2stagewaitevent.py
 src/sdk/models/shared/v2stats.py
 src/sdk/models/shared/v2statsresponse.py
+src/sdk/models/shared/v2subject.py
+src/sdk/models/shared/v2targetid.py
 src/sdk/models/shared/v2targettype.py
 src/sdk/models/shared/v2testtriggerresponse.py
 src/sdk/models/shared/v2transaction.py
 src/sdk/models/shared/v2transactionscursorresponse.py
 src/sdk/models/shared/v2trigger.py
 src/sdk/models/shared/v2triggerdata.py
 src/sdk/models/shared/v2triggeroccurrence.py
 src/sdk/models/shared/v2triggertest.py
+src/sdk/models/shared/v2update.py
+src/sdk/models/shared/v2updateaccount.py
 src/sdk/models/shared/v2volume.py
 src/sdk/models/shared/v2volumeswithbalance.py
 src/sdk/models/shared/v2volumeswithbalancecursorresponse.py
 src/sdk/models/shared/v2wallet.py
 src/sdk/models/shared/v2walletsubject.py
 src/sdk/models/shared/v2walletwithbalances.py
 src/sdk/models/shared/v2workflow.py
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/_hooks/registration.py` & `formance-sdk-python-2.3.0/src/sdk/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/_hooks/sdkhooks.py` & `formance-sdk-python-2.3.0/src/sdk/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/_hooks/types.py` & `formance-sdk-python-2.3.0/src/sdk/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/auth.py` & `formance-sdk-python-2.3.0/src/sdk/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create_client(self, request: Optional[shared.CreateClientRequest]) -> operations.CreateClientResponse:
+    def create_client(self, request: Optional[shared.CreateClientRequest] = None) -> operations.CreateClientResponse:
         r"""Create client"""
         hook_ctx = HookContext(operation_id='createClient', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/api/auth/clients'
         
         if callable(self.sdk_configuration.security):
@@ -53,14 +53,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateClientResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CreateClientResponse])
                 res.create_client_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -108,14 +109,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateSecretResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CreateSecretResponse])
                 res.create_secret_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -254,14 +256,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListClientsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ListClientsResponse])
                 res.list_clients_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -308,14 +311,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListUsersResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ListUsersResponse])
                 res.list_users_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -360,14 +364,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ReadClientResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ReadClientResponse])
                 res.read_client_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -414,14 +419,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ReadUserResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ReadUserResponse])
                 res.read_user_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -469,14 +475,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateClientResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.UpdateClientResponse])
                 res.update_client_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/ledger.py` & `formance-sdk-python-2.3.0/src/sdk/ledger.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,21 +55,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateTransactionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TransactionsResponse])
                 res.transactions_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -117,14 +119,15 @@
         
         
         res = operations.AddMetadataOnTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -174,14 +177,15 @@
         
         
         res = operations.AddMetadataToAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -228,14 +232,15 @@
         
         res = operations.CountAccountsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -282,14 +287,15 @@
         
         res = operations.CountTransactionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 200:
             res.headers = http_res.headers
             
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -338,21 +344,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TransactionsResponse])
                 res.transactions_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -395,21 +403,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountResponse])
                 res.account_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -453,21 +463,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetBalancesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.BalancesCursorResponse])
                 res.balances_cursor_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -511,21 +523,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetBalancesAggregatedResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AggregateBalancesResponse])
                 res.aggregate_balances_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -568,21 +582,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetInfoResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ConfigInfoResponse])
                 res.config_info_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -625,21 +641,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetLedgerInfoResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.LedgerInfoResponse])
                 res.ledger_info_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -682,21 +700,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetMappingResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MappingResponse])
                 res.mapping_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -739,21 +759,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TransactionResponse])
                 res.transaction_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -799,21 +821,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAccountsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountsCursorResponse])
                 res.accounts_cursor_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -859,21 +883,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListLogsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.LogsCursorResponse])
                 res.logs_cursor_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -919,21 +945,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListTransactionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TransactionsCursorResponse])
                 res.transactions_cursor_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -978,21 +1006,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ReadStatsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.StatsResponse])
                 res.stats_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1036,21 +1066,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.RevertTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TransactionResponse])
                 res.transaction_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1103,14 +1135,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.RunScriptResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ScriptResponse])
                 res.script_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -1160,21 +1193,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.UpdateMappingResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.MappingResponse])
                 res.mapping_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1224,14 +1259,15 @@
         
         
         res = operations.V2AddMetadataOnTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1283,14 +1319,15 @@
         
         
         res = operations.V2AddMetadataToAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1340,14 +1377,15 @@
         
         res = operations.V2CountAccountsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 204:
             res.headers = http_res.headers
             
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1397,14 +1435,15 @@
         
         res = operations.V2CountTransactionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res, headers=None)
         
         if http_res.status_code == 204:
             res.headers = http_res.headers
             
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1450,21 +1489,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2CreateBulkResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code in [200, 400]:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2BulkResponse])
                 res.v2_bulk_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1512,14 +1553,15 @@
         
         
         res = operations.V2CreateLedgerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1569,21 +1611,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2CreateTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2CreateTransactionResponse])
                 res.v2_create_transaction_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1677,14 +1721,15 @@
         
         
         res = operations.V2DeleteLedgerMetadataResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1731,14 +1776,15 @@
         
         
         res = operations.V2DeleteTransactionMetadataResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code >= 200 and http_res.status_code < 300:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1782,21 +1828,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2GetAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2AccountResponse])
                 res.v2_account_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1843,21 +1891,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2GetBalancesAggregatedResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2AggregateBalancesResponse])
                 res.v2_aggregate_balances_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1900,21 +1950,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2GetInfoResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2ConfigInfoResponse])
                 res.v2_config_info_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1957,21 +2009,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2GetLedgerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2GetLedgerResponse])
                 res.v2_get_ledger_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -2014,21 +2068,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2GetLedgerInfoResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2LedgerInfoResponse])
                 res.v2_ledger_info_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -2072,21 +2128,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2GetTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2GetTransactionResponse])
                 res.v2_get_transaction_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -2133,21 +2191,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2GetVolumesWithBalancesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2VolumesWithBalanceCursorResponse])
                 res.v2_volumes_with_balance_cursor_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -2196,21 +2256,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2ListAccountsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2AccountsCursorResponse])
                 res.v2_accounts_cursor_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -2254,21 +2316,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2ListLedgersResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2LedgerListResponse])
                 res.v2_ledger_list_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -2317,21 +2381,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2ListLogsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2LogsCursorResponse])
                 res.v2_logs_cursor_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -2380,21 +2446,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2ListTransactionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2TransactionsCursorResponse])
                 res.v2_transactions_cursor_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -2439,21 +2507,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2ReadStatsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2StatsResponse])
                 res.v2_stats_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -2497,21 +2567,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2RevertTransactionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2RevertTransactionResponse])
                 res.v2_revert_transaction_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -2559,14 +2631,15 @@
         
         
         res = operations.V2UpdateLedgerMetadataResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/errors/error.py` & `formance-sdk-python-2.3.0/src/sdk/models/errors/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from sdk import utils
 
+
 class ErrorCode(str, Enum):
     VALIDATION = 'VALIDATION'
     NOT_FOUND = 'NOT_FOUND'
     INTERNAL = 'INTERNAL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/errors/errorresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/errors/errorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/errors/reconciliationerrorresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/errors/reconciliationerrorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/errors/sdkerror.py` & `formance-sdk-python-2.3.0/src/sdk/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/errors/v2error.py` & `formance-sdk-python-2.3.0/src/sdk/models/errors/v2error.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from sdk import utils
 
+
 class SchemasErrorCode(str, Enum):
     VALIDATION = 'VALIDATION'
     NOT_FOUND = 'NOT_FOUND'
     INTERNAL = 'INTERNAL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/errors/v2errorresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/errors/v2errorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/errors/walletserrorresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/errors/walletserrorresponse.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from sdk import utils
 
+
 class SchemasWalletsErrorResponseErrorCode(str, Enum):
     VALIDATION = 'VALIDATION'
     INTERNAL_ERROR = 'INTERNAL_ERROR'
     INSUFFICIENT_FUND = 'INSUFFICIENT_FUND'
     HOLD_CLOSED = 'HOLD_CLOSED'
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/errors/webhookserrorresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/errors/webhookserrorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/__init__.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/activateconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/activateconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/addaccounttopool.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/addaccounttopool.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/addmetadataontransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/addmetadataontransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/addmetadatatoaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/addmetadatatoaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/cancelevent.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/cancelevent.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/changeconfigsecret.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/changeconfigsecret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/confirmhold.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/confirmhold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/connectorstransfer.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/connectorstransfer.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/countaccounts.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/countaccounts.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/counttransactions.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/counttransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/createaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/createaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/createbalance.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/createbalance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/createbankaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/createbankaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/createclient.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/createclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/createpayment.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/createpayment.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/createpolicy.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/createpolicy.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/createpool.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/createpool.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/createsecret.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/createsecret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/createtransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/createtransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/createtransactions.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/createtransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/createtransferinitiation.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/createtransferinitiation.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/createtrigger.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/createtrigger.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/createwallet.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/createwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/createworkflow.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/createworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/creditwallet.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/creditwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/deactivateconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/deactivateconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/debitwallet.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/debitwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/deleteclient.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/deleteclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/deleteconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/deleteconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/deletepolicy.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/deletepolicy.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/deletepool.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/deletepool.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/deletesecret.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/deletesecret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/deletetransferinitiation.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/deletetransferinitiation.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/deletetrigger.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/deletetrigger.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/deleteworkflow.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/deleteworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/forwardbankaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/forwardbankaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getaccountbalances.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getaccountbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getbalance.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getbalance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getbalances.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getbalancesaggregated.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getbalancesaggregated.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getbankaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getbankaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getconnectortask.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getconnectortask.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getconnectortaskv1.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getconnectortaskv1.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/gethold.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/gethold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getholds.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getholds.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getinfo.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getinstance.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getinstance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getinstancehistory.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getinstancehistory.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getinstancestagehistory.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getinstancestagehistory.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getledgerinfo.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getledgerinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getmanyconfigs.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getmanyconfigs.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getmapping.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getmapping.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getoidcwellknowns.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getoidcwellknowns.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getpayment.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getpayment.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getpolicy.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getpolicy.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getpool.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getpool.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getpoolbalances.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getpoolbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getreconciliation.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getreconciliation.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/gettransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/gettransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/gettransactions.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/gettransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/gettransferinitiation.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/gettransferinitiation.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getversions.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getversions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getwallet.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getwalletsummary.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getwalletsummary.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/getworkflow.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/getworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/insertconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/insertconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listaccounts.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listaccounts.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listallconnectors.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listallconnectors.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listbalances.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listbankaccounts.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listbankaccounts.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listclients.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listclients.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listconfigsavailableconnectors.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listconfigsavailableconnectors.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listconnectortasks.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listconnectortasks.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listconnectortasksv1.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listconnectortasksv1.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listinstances.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listinstances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listlogs.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listlogs.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listpayments.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listpayments.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listpolicies.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listpolicies.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listpools.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listpools.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listreconciliations.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listreconciliations.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listtransactions.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listtransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listtransferinitiations.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listtransferinitiations.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listtriggers.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listtriggers.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listtriggersoccurrences.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listtriggersoccurrences.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listusers.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listusers.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listwallets.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listwallets.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/listworkflows.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/listworkflows.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/orchestrationgetserverinfo.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/orchestrationgetserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/paymentsgetaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/paymentsgetaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/paymentsgetserverinfo.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/paymentsgetserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/paymentslistaccounts.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/paymentslistaccounts.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     r"""Parameter used in pagination requests. Maximum page size is set to 15.
     Set to the value of next for the next page of results.
     Set to the value of previous for the previous page of results.
     No other parameters can be set when this parameter is set.
     """
     page_size: Optional[int] = dataclasses.field(default=15, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
     r"""The maximum number of results to return per page."""
+    query: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'query', 'style': 'form', 'explode': True }})
+    r"""Filters used to filter resources."""
     sort: Optional[List[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'sort', 'style': 'form', 'explode': True }})
     r"""Fields used to sort payments (default is date:desc)."""
     
 
 
 
 @dataclasses.dataclass
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/readclient.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/readclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/readconnectorconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/readconnectorconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/readconnectorconfigv1.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/readconnectorconfigv1.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/readstats.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/readstats.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/readtrigger.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/readtrigger.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/readuser.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/readuser.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/reconcile.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/reconcile.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/reconciliationgetserverinfo.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/reconciliationgetserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/removeaccountfrompool.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/removeaccountfrompool.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/resetconnector.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/resetconnector.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/resetconnectorv1.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/resetconnectorv1.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/retrytransferinitiation.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/retrytransferinitiation.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/reversetransferinitiation.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/reversetransferinitiation.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/reverttransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/reverttransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/runscript.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/runscript.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/runworkflow.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/runworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/search.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/search.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/searchgetserverinfo.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/searchgetserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/sendevent.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/sendevent.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/testconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/testconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/testtrigger.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/testtrigger.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/udpatetransferinitiationstatus.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/udpatetransferinitiationstatus.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/uninstallconnector.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/uninstallconnector.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/uninstallconnectorv1.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/uninstallconnectorv1.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/updatebankaccountmetadata.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/updatebankaccountmetadata.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/updateclient.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/updateclient.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/updatemapping.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/updatemapping.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/updatemetadata.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/updatemetadata.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/updatewallet.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/updatewallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2addmetadataontransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2addmetadataontransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2addmetadatatoaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2addmetadatatoaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2cancelevent.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2cancelevent.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2countaccounts.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2countaccounts.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2counttransactions.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2counttransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2createbulk.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2createbulk.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ...models.shared import v2bulkelementaddmetadata as shared_v2bulkelementaddmetadata
-from ...models.shared import v2bulkelementcreatetransaction as shared_v2bulkelementcreatetransaction
-from ...models.shared import v2bulkelementdeletemetadata as shared_v2bulkelementdeletemetadata
-from ...models.shared import v2bulkelementreverttransaction as shared_v2bulkelementreverttransaction
+from ...models.shared import v2bulkelement as shared_v2bulkelement
 from ...models.shared import v2bulkresponse as shared_v2bulkresponse
-from typing import List, Optional, Union
+from typing import List, Optional
 
 
 @dataclasses.dataclass
 class V2CreateBulkRequest:
     ledger: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ledger', 'style': 'simple', 'explode': False }})
     r"""Name of the ledger."""
-    request_body: Optional[List[Union[shared_v2bulkelementcreatetransaction.V2BulkElementCreateTransaction, shared_v2bulkelementaddmetadata.V2BulkElementAddMetadata, shared_v2bulkelementreverttransaction.V2BulkElementRevertTransaction, shared_v2bulkelementdeletemetadata.V2BulkElementDeleteMetadata]]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    request_body: Optional[List[shared_v2bulkelement.V2BulkElement]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
 
 
 @dataclasses.dataclass
 class V2CreateBulkResponse:
     content_type: str = dataclasses.field()
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2createledger.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2createledger.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2createtransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2createtransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2createtrigger.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2createtrigger.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2createworkflow.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2createworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2deleteaccountmetadata.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2deleteaccountmetadata.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2deleteledgermetadata.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2deleteledgermetadata.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2deletetransactionmetadata.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2deletetransactionmetadata.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2deletetrigger.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2deletetrigger.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2deleteworkflow.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2deleteworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2getaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2getaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2getbalancesaggregated.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2getbalancesaggregated.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2getinfo.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2getinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2getinstance.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2getinstance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2getinstancehistory.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2getinstancehistory.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2getinstancestagehistory.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2getinstancestagehistory.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2getledger.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2getledger.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2getledgerinfo.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2getledgerinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2getserverinfo.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2getserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2gettransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2gettransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2getvolumeswithbalances.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2getvolumeswithbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2getworkflow.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2getworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2listaccounts.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2listaccounts.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2listinstances.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2listinstances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2listledgers.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2listledgers.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2listlogs.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2listlogs.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2listtransactions.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2listtransactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2listtriggers.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2listtriggers.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2listtriggersoccurrences.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2listtriggersoccurrences.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2listworkflows.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2listworkflows.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2readstats.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2readstats.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2readtrigger.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2readtrigger.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2reverttransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2reverttransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2runworkflow.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2runworkflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2sendevent.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2sendevent.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/v2updateledgermetadata.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/v2updateledgermetadata.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/voidhold.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/voidhold.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/operations/walletsgetserverinfo.py` & `formance-sdk-python-2.3.0/src/sdk/models/operations/walletsgetserverinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/__init__.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .accountbalance import *
 from .accountrequest import *
 from .accountresponse import *
 from .accountscursor import *
 from .accountscursorresponse import *
 from .accounttype import *
 from .accountwithvolumesandbalances import *
+from .activityaddaccountmetadata import *
 from .activityconfirmhold import *
 from .activitycreatetransaction import *
 from .activitycreatetransactionoutput import *
 from .activitycreditwallet import *
 from .activitydebitwallet import *
 from .activitydebitwalletoutput import *
 from .activitygetaccount import *
@@ -49,14 +50,15 @@
 from .configinfo import *
 from .configinforesponse import *
 from .configresponse import *
 from .configsresponse import *
 from .configuser import *
 from .confirmholdrequest import *
 from .connector import *
+from .connectorconfig import *
 from .connectorconfigresponse import *
 from .connectorresponse import *
 from .connectorsconfigsresponse import *
 from .connectorsresponse import *
 from .contract import *
 from .createbalancerequest import *
 from .createbalanceresponse import *
@@ -125,14 +127,15 @@
 from .paymentadjustment import *
 from .paymentrequest import *
 from .paymentresponse import *
 from .paymentsaccount import *
 from .paymentsaccountresponse import *
 from .paymentscheme import *
 from .paymentscursor import *
+from .paymentserrorsenum import *
 from .paymentstatus import *
 from .paymenttype import *
 from .policiescursorresponse import *
 from .policy import *
 from .policyrequest import *
 from .policyresponse import *
 from .pool import *
@@ -156,14 +159,15 @@
 from .reversetransferinitiationrequest import *
 from .runworkflowresponse import *
 from .script import *
 from .scriptresponse import *
 from .secret import *
 from .security import *
 from .serverinfo import *
+from .stage import *
 from .stagedelay import *
 from .stagesend import *
 from .stagesenddestination import *
 from .stagesenddestinationaccount import *
 from .stagesenddestinationpayment import *
 from .stagesenddestinationwallet import *
 from .stagesendsource import *
@@ -171,14 +175,15 @@
 from .stagesendsourcepayment import *
 from .stagesendsourcewallet import *
 from .stagestatus import *
 from .stagewaitevent import *
 from .stats import *
 from .statsresponse import *
 from .stripeconfig import *
+from .subject import *
 from .taskbankingcircle import *
 from .taskcurrencycloud import *
 from .taskdummypay import *
 from .taskmangopay import *
 from .taskmodulr import *
 from .taskmoneycorp import *
 from .taskresponse import *
@@ -199,22 +204,25 @@
 from .transferinitiationscursor import *
 from .transferinitiationstatus import *
 from .transferrequest import *
 from .transferresponse import *
 from .trigger import *
 from .triggerdata import *
 from .triggeroccurrence import *
+from .update import *
+from .updateaccount import *
 from .updatebankaccountmetadatarequest import *
 from .updateclientrequest import *
 from .updateclientresponse import *
 from .updatetransferinitiationstatusrequest import *
 from .user import *
 from .v2account import *
 from .v2accountresponse import *
 from .v2accountscursorresponse import *
+from .v2activityaddaccountmetadata import *
 from .v2activityconfirmhold import *
 from .v2activitycreatetransaction import *
 from .v2activitycreatetransactionoutput import *
 from .v2activitycreditwallet import *
 from .v2activitydebitwallet import *
 from .v2activitydebitwalletoutput import *
 from .v2activitygetaccount import *
@@ -224,14 +232,15 @@
 from .v2activitygetwallet import *
 from .v2activitygetwalletoutput import *
 from .v2activitylistwallets import *
 from .v2activitystripetransfer import *
 from .v2activityvoidhold import *
 from .v2aggregatebalancesresponse import *
 from .v2assetholder import *
+from .v2bulkelement import *
 from .v2bulkelementaddmetadata import *
 from .v2bulkelementcreatetransaction import *
 from .v2bulkelementdeletemetadata import *
 from .v2bulkelementresult import *
 from .v2bulkelementreverttransaction import *
 from .v2bulkresponse import *
 from .v2configinforesponse import *
@@ -272,36 +281,41 @@
 from .v2paymentstatus import *
 from .v2posting import *
 from .v2posttransaction import *
 from .v2readtriggerresponse import *
 from .v2reverttransactionresponse import *
 from .v2runworkflowresponse import *
 from .v2serverinfo import *
+from .v2stage import *
 from .v2stagedelay import *
 from .v2stagesend import *
 from .v2stagesenddestination import *
 from .v2stagesenddestinationaccount import *
 from .v2stagesenddestinationpayment import *
 from .v2stagesenddestinationwallet import *
 from .v2stagesendsource import *
 from .v2stagesendsourceaccount import *
 from .v2stagesendsourcepayment import *
 from .v2stagesendsourcewallet import *
 from .v2stagestatus import *
 from .v2stagewaitevent import *
 from .v2stats import *
 from .v2statsresponse import *
+from .v2subject import *
+from .v2targetid import *
 from .v2targettype import *
 from .v2testtriggerresponse import *
 from .v2transaction import *
 from .v2transactionscursorresponse import *
 from .v2trigger import *
 from .v2triggerdata import *
 from .v2triggeroccurrence import *
 from .v2triggertest import *
+from .v2update import *
+from .v2updateaccount import *
 from .v2volume import *
 from .v2volumeswithbalance import *
 from .v2volumeswithbalancecursorresponse import *
 from .v2wallet import *
 from .v2walletsubject import *
 from .v2walletwithbalances import *
 from .v2workflow import *
@@ -325,8 +339,8 @@
 from .workflowconfig import *
 from .workflowinstance import *
 from .workflowinstancehistory import *
 from .workflowinstancehistorystage import *
 from .workflowinstancehistorystageinput import *
 from .workflowinstancehistorystageoutput import *
 
-__all__ = ["Account","AccountBalance","AccountRequest","AccountResponse","AccountType","AccountWithVolumesAndBalances","AccountsCursor","AccountsCursorResponse","AccountsCursorResponseCursor","ActivityConfirmHold","ActivityCreateTransaction","ActivityCreateTransactionOutput","ActivityCreditWallet","ActivityDebitWallet","ActivityDebitWalletOutput","ActivityGetAccount","ActivityGetAccountOutput","ActivityGetPayment","ActivityGetPaymentOutput","ActivityGetWallet","ActivityGetWalletOutput","ActivityListWallets","ActivityRevertTransaction","ActivityRevertTransactionOutput","ActivityStripeTransfer","ActivityVoidHold","AddAccountToPoolRequest","AdyenConfig","AggregateBalancesResponse","AssetHolder","AtlarConfig","Attempt","AttemptResponse","Balance","BalanceWithAssets","Balances","BalancesCursor","BalancesCursorCursor","BalancesCursorResponse","BalancesCursorResponseCursor","BankAccount","BankAccountRelatedAccounts","BankAccountRequest","BankAccountResponse","BankAccountsCursor","BankAccountsCursorCursor","BankingCircleConfig","Client","ClientSecret","Config","ConfigChangeSecret","ConfigInfo","ConfigInfoResponse","ConfigResponse","ConfigUser","ConfigsResponse","ConfigsResponseCursor","ConfirmHoldRequest","Connector","ConnectorConfigResponse","ConnectorResponse","ConnectorsConfigsResponse","ConnectorsConfigsResponseConnector","ConnectorsConfigsResponseData","ConnectorsResponse","ConnectorsResponseData","Contract","CreateBalanceRequest","CreateBalanceResponse","CreateClientRequest","CreateClientResponse","CreateSecretRequest","CreateSecretResponse","CreateTriggerResponse","CreateWalletRequest","CreateWalletResponse","CreateWorkflowRequest","CreateWorkflowResponse","CreditWalletRequest","CurrencyCloudConfig","Cursor","Data","DebitWalletRequest","DebitWalletResponse","Descriptor","DummyPayConfig","ErrorsEnum","ExpandedDebitHold","Expr","Filter","ForwardBankAccountRequest","GenericConfig","GetBalanceResponse","GetHoldResponse","GetHoldsResponse","GetHoldsResponseCursor","GetTransactionsResponse","GetTransactionsResponseCursor","GetVersionsResponse","GetWalletResponse","GetWalletSummaryResponse","GetWorkflowInstanceHistoryResponse","GetWorkflowInstanceHistoryStageResponse","GetWorkflowInstanceResponse","GetWorkflowResponse","Hold","Key","LedgerAccountSubject","LedgerInfo","LedgerInfoResponse","LedgerStorage","ListBalancesResponse","ListBalancesResponseCursor","ListClientsResponse","ListRunsResponse","ListTriggersOccurrencesResponse","ListTriggersResponse","ListUsersResponse","ListWalletsResponse","ListWalletsResponseCursor","ListWorkflowsResponse","Log","LogsCursorResponse","LogsCursorResponseCursor","MangoPayConfig","Mapping","MappingResponse","Metadata","MigrationInfo","ModulrConfig","Monetary","MoneycorpConfig","OrchestrationAccount","OrchestrationConnector","OrchestrationListWalletsResponse","OrchestrationListWalletsResponseCursor","OrchestrationPayment","OrchestrationPaymentAdjustment","OrchestrationPaymentAdjustmentRaw","OrchestrationPaymentMetadata","OrchestrationPaymentRaw","OrchestrationPaymentScheme","OrchestrationPaymentStatus","OrchestrationPaymentType","OrchestrationPostTransaction","OrchestrationPostTransactionScript","OrchestrationTransaction","OrchestrationV2Transaction","Payment","PaymentAdjustment","PaymentAdjustmentRaw","PaymentRequest","PaymentResponse","PaymentScheme","PaymentStatus","PaymentType","PaymentsAccount","PaymentsAccountRaw","PaymentsAccountResponse","PaymentsCursor","PaymentsCursorCursor","PoliciesCursorResponse","PoliciesCursorResponseCursor","Policy","PolicyRequest","PolicyResponse","Pool","PoolBalance","PoolBalances","PoolBalancesResponse","PoolRequest","PoolResponse","PoolsCursor","PoolsCursorCursor","PostTransaction","PostTransactionScript","Posting","Query","QueryRaw","Raw","ReadClientResponse","ReadTriggerResponse","ReadUserResponse","Reconciliation","ReconciliationRequest","ReconciliationResponse","ReconciliationsCursorResponse","ReconciliationsCursorResponseCursor","Response","ResponseCursor","ReverseTransferInitiationRequest","RunWorkflowResponse","Schemas","Scheme","Script","ScriptResponse","Secret","Security","ServerInfo","StageDelay","StageSend","StageSendDestination","StageSendDestinationAccount","StageSendDestinationPayment","StageSendDestinationWallet","StageSendSource","StageSendSourceAccount","StageSendSourcePayment","StageSendSourceWallet","StageStatus","StageWaitEvent","State","Stats","StatsResponse","Status","Storage","StripeConfig","TaskBankingCircle","TaskBankingCircleState","TaskCurrencyCloud","TaskCurrencyCloudDescriptor","TaskCurrencyCloudState","TaskDummyPay","TaskDummyPayDescriptor","TaskDummyPayState","TaskMangoPay","TaskMangoPayDescriptor","TaskMangoPayState","TaskModulr","TaskModulrDescriptor","TaskModulrState","TaskMoneycorp","TaskMoneycorpDescriptor","TaskMoneycorpState","TaskResponse","TaskStripe","TaskStripeDescriptor","TaskStripeState","TaskWise","TaskWiseDescriptor","TaskWiseState","TasksCursor","TasksCursorCursor","Total","Transaction","TransactionData","TransactionResponse","Transactions","TransactionsCursorResponse","TransactionsCursorResponseCursor","TransactionsResponse","TransferInitiation","TransferInitiationAdjusments","TransferInitiationPayments","TransferInitiationRequest","TransferInitiationRequestType","TransferInitiationResponse","TransferInitiationStatus","TransferInitiationType","TransferInitiationsCursor","TransferInitiationsCursorCursor","TransferRequest","TransferResponse","Trigger","TriggerData","TriggerOccurrence","Type","UpdateBankAccountMetadataRequest","UpdateClientRequest","UpdateClientResponse","UpdateTransferInitiationStatusRequest","User","V2Account","V2AccountResponse","V2AccountsCursorResponse","V2AccountsCursorResponseCursor","V2ActivityConfirmHold","V2ActivityCreateTransaction","V2ActivityCreateTransactionOutput","V2ActivityCreditWallet","V2ActivityDebitWallet","V2ActivityDebitWalletOutput","V2ActivityGetAccount","V2ActivityGetAccountOutput","V2ActivityGetPayment","V2ActivityGetPaymentOutput","V2ActivityGetWallet","V2ActivityGetWalletOutput","V2ActivityListWallets","V2ActivityStripeTransfer","V2ActivityStripeTransferMetadata","V2ActivityVoidHold","V2AggregateBalancesResponse","V2AssetHolder","V2BulkElementAddMetadata","V2BulkElementAddMetadataData","V2BulkElementCreateTransaction","V2BulkElementDeleteMetadata","V2BulkElementDeleteMetadataData","V2BulkElementResultCreateTransactionSchemas","V2BulkElementResultDeleteMetadataSchemas","V2BulkElementResultErrorSchemas","V2BulkElementResultRevertTransactionSchemas","V2BulkElementRevertTransaction","V2BulkElementRevertTransactionData","V2BulkResponse","V2ConfigInfoResponse","V2Connector","V2CreateLedgerRequest","V2CreateTransactionResponse","V2CreateTriggerResponse","V2CreateWorkflowRequest","V2CreateWorkflowResponse","V2CreditWalletRequest","V2DebitWalletRequest","V2ErrorsEnum","V2ExpandedTransaction","V2GetLedgerResponse","V2GetTransactionResponse","V2GetWorkflowInstanceHistoryResponse","V2GetWorkflowInstanceHistoryStageResponse","V2GetWorkflowInstanceResponse","V2GetWorkflowResponse","V2Hold","V2Ledger","V2LedgerAccountSubject","V2LedgerInfo","V2LedgerInfoResponse","V2LedgerInfoStorage","V2LedgerListResponse","V2LedgerListResponseCursor","V2ListRunsResponse","V2ListRunsResponseCursor","V2ListTriggersOccurrencesResponse","V2ListTriggersOccurrencesResponseCursor","V2ListTriggersResponse","V2ListTriggersResponseCursor","V2ListWalletsResponse","V2ListWalletsResponseCursor","V2ListWorkflowsResponse","V2ListWorkflowsResponseCursor","V2Log","V2LogType","V2LogsCursorResponse","V2LogsCursorResponseCursor","V2MigrationInfo","V2MigrationInfoState","V2Monetary","V2Payment","V2PaymentAdjustment","V2PaymentAdjustmentRaw","V2PaymentMetadata","V2PaymentRaw","V2PaymentStatus","V2PaymentType","V2PostTransaction","V2PostTransactionScript","V2Posting","V2ReadTriggerResponse","V2RevertTransactionResponse","V2RunWorkflowResponse","V2ServerInfo","V2StageDelay","V2StageSend","V2StageSendDestination","V2StageSendDestinationAccount","V2StageSendDestinationPayment","V2StageSendDestinationWallet","V2StageSendSource","V2StageSendSourceAccount","V2StageSendSourcePayment","V2StageSendSourceWallet","V2StageStatus","V2StageWaitEvent","V2Stats","V2StatsResponse","V2TargetType","V2TestTriggerResponse","V2Transaction","V2TransactionsCursorResponse","V2TransactionsCursorResponseCursor","V2Trigger","V2TriggerData","V2TriggerOccurrence","V2TriggerTest","V2Volume","V2VolumesWithBalance","V2VolumesWithBalanceCursorResponse","V2VolumesWithBalanceCursorResponseCursor","V2Wallet","V2WalletSubject","V2WalletWithBalances","V2Workflow","V2WorkflowConfig","V2WorkflowInstance","V2WorkflowInstanceHistory","V2WorkflowInstanceHistoryStage","V2WorkflowInstanceHistoryStageInput","V2WorkflowInstanceHistoryStageOutput","Variables","Version","Volume","Wallet","WalletSubject","WalletWithBalances","WalletWithBalancesBalances","WalletsTransaction","WalletsVolume","WebhooksConfig","WebhooksErrorsEnum","WiseConfig","Workflow","WorkflowConfig","WorkflowInstance","WorkflowInstanceHistory","WorkflowInstanceHistoryStage","WorkflowInstanceHistoryStageInput","WorkflowInstanceHistoryStageOutput"]
+__all__ = ["Account","AccountBalance","AccountRequest","AccountResponse","AccountType","AccountWithVolumesAndBalances","AccountsCursor","AccountsCursorResponse","AccountsCursorResponseCursor","ActivityAddAccountMetadata","ActivityConfirmHold","ActivityCreateTransaction","ActivityCreateTransactionOutput","ActivityCreditWallet","ActivityDebitWallet","ActivityDebitWalletOutput","ActivityGetAccount","ActivityGetAccountOutput","ActivityGetPayment","ActivityGetPaymentOutput","ActivityGetWallet","ActivityGetWalletOutput","ActivityListWallets","ActivityRevertTransaction","ActivityRevertTransactionOutput","ActivityStripeTransfer","ActivityVoidHold","AddAccountToPoolRequest","AdyenConfig","AggregateBalancesResponse","AssetHolder","AtlarConfig","Attempt","AttemptResponse","Balance","BalanceWithAssets","Balances","BalancesCursor","BalancesCursorCursor","BalancesCursorResponse","BalancesCursorResponseCursor","BankAccount","BankAccountRelatedAccounts","BankAccountRequest","BankAccountResponse","BankAccountsCursor","BankAccountsCursorCursor","BankingCircleConfig","Client","ClientSecret","Config","ConfigChangeSecret","ConfigInfo","ConfigInfoResponse","ConfigResponse","ConfigUser","ConfigsResponse","ConfigsResponseCursor","ConfirmHoldRequest","Connector","ConnectorConfig","ConnectorConfigResponse","ConnectorResponse","ConnectorsConfigsResponse","ConnectorsConfigsResponseConnector","ConnectorsConfigsResponseData","ConnectorsResponse","ConnectorsResponseData","Contract","CreateBalanceRequest","CreateBalanceResponse","CreateClientRequest","CreateClientResponse","CreateSecretRequest","CreateSecretResponse","CreateTriggerResponse","CreateWalletRequest","CreateWalletResponse","CreateWorkflowRequest","CreateWorkflowResponse","CreditWalletRequest","CurrencyCloudConfig","Cursor","Data","DebitWalletRequest","DebitWalletResponse","Descriptor","DummyPayConfig","ErrorsEnum","ExpandedDebitHold","Expr","Filter","ForwardBankAccountRequest","GenericConfig","GetBalanceResponse","GetHoldResponse","GetHoldsResponse","GetHoldsResponseCursor","GetTransactionsResponse","GetTransactionsResponseCursor","GetVersionsResponse","GetWalletResponse","GetWalletSummaryResponse","GetWorkflowInstanceHistoryResponse","GetWorkflowInstanceHistoryStageResponse","GetWorkflowInstanceResponse","GetWorkflowResponse","Hold","Key","LedgerAccountSubject","LedgerInfo","LedgerInfoResponse","LedgerStorage","ListBalancesResponse","ListBalancesResponseCursor","ListClientsResponse","ListRunsResponse","ListTriggersOccurrencesResponse","ListTriggersResponse","ListUsersResponse","ListWalletsResponse","ListWalletsResponseCursor","ListWorkflowsResponse","Log","LogsCursorResponse","LogsCursorResponseCursor","MangoPayConfig","Mapping","MappingResponse","Metadata","MigrationInfo","ModulrConfig","Monetary","MoneycorpConfig","OrchestrationAccount","OrchestrationConnector","OrchestrationListWalletsResponse","OrchestrationListWalletsResponseCursor","OrchestrationPayment","OrchestrationPaymentAdjustment","OrchestrationPaymentAdjustmentRaw","OrchestrationPaymentMetadata","OrchestrationPaymentRaw","OrchestrationPaymentScheme","OrchestrationPaymentStatus","OrchestrationPaymentType","OrchestrationPostTransaction","OrchestrationPostTransactionScript","OrchestrationTransaction","OrchestrationV2Transaction","Payment","PaymentAdjustment","PaymentAdjustmentRaw","PaymentRequest","PaymentResponse","PaymentScheme","PaymentStatus","PaymentType","PaymentsAccount","PaymentsAccountRaw","PaymentsAccountResponse","PaymentsCursor","PaymentsCursorCursor","PaymentsErrorsEnum","PoliciesCursorResponse","PoliciesCursorResponseCursor","Policy","PolicyRequest","PolicyResponse","Pool","PoolBalance","PoolBalances","PoolBalancesResponse","PoolRequest","PoolResponse","PoolsCursor","PoolsCursorCursor","PostTransaction","PostTransactionScript","Posting","Query","QueryRaw","Raw","ReadClientResponse","ReadTriggerResponse","ReadUserResponse","Reconciliation","ReconciliationRequest","ReconciliationResponse","ReconciliationsCursorResponse","ReconciliationsCursorResponseCursor","Response","ResponseCursor","ReverseTransferInitiationRequest","RunWorkflowResponse","Schemas","Scheme","Script","ScriptResponse","Secret","Security","ServerInfo","Stage","StageDelay","StageSend","StageSendDestination","StageSendDestinationAccount","StageSendDestinationPayment","StageSendDestinationWallet","StageSendSource","StageSendSourceAccount","StageSendSourcePayment","StageSendSourceWallet","StageStatus","StageWaitEvent","State","Stats","StatsResponse","Status","Storage","StripeConfig","Subject","TaskBankingCircle","TaskBankingCircleState","TaskCurrencyCloud","TaskCurrencyCloudDescriptor","TaskCurrencyCloudState","TaskDummyPay","TaskDummyPayDescriptor","TaskDummyPayState","TaskMangoPay","TaskMangoPayDescriptor","TaskMangoPayState","TaskModulr","TaskModulrDescriptor","TaskModulrState","TaskMoneycorp","TaskMoneycorpDescriptor","TaskMoneycorpState","TaskResponse","TaskResponseData","TaskStripe","TaskStripeDescriptor","TaskStripeState","TaskWise","TaskWiseDescriptor","TaskWiseState","TasksCursor","TasksCursorCursor","TasksCursorData","Total","Transaction","TransactionData","TransactionResponse","Transactions","TransactionsCursorResponse","TransactionsCursorResponseCursor","TransactionsResponse","TransferInitiation","TransferInitiationAdjusments","TransferInitiationPayments","TransferInitiationRequest","TransferInitiationRequestType","TransferInitiationResponse","TransferInitiationStatus","TransferInitiationType","TransferInitiationsCursor","TransferInitiationsCursorCursor","TransferRequest","TransferResponse","Trigger","TriggerData","TriggerOccurrence","Type","Update","UpdateAccount","UpdateBankAccountMetadataRequest","UpdateClientRequest","UpdateClientResponse","UpdateTransferInitiationStatusRequest","User","V2Account","V2AccountResponse","V2AccountsCursorResponse","V2AccountsCursorResponseCursor","V2ActivityAddAccountMetadata","V2ActivityConfirmHold","V2ActivityCreateTransaction","V2ActivityCreateTransactionOutput","V2ActivityCreditWallet","V2ActivityDebitWallet","V2ActivityDebitWalletOutput","V2ActivityGetAccount","V2ActivityGetAccountOutput","V2ActivityGetPayment","V2ActivityGetPaymentOutput","V2ActivityGetWallet","V2ActivityGetWalletOutput","V2ActivityListWallets","V2ActivityStripeTransfer","V2ActivityStripeTransferMetadata","V2ActivityVoidHold","V2AggregateBalancesResponse","V2AssetHolder","V2BulkElement","V2BulkElementAddMetadata","V2BulkElementAddMetadataData","V2BulkElementCreateTransaction","V2BulkElementDeleteMetadata","V2BulkElementDeleteMetadataData","V2BulkElementResult","V2BulkElementResultCreateTransactionSchemas","V2BulkElementResultDeleteMetadataSchemas","V2BulkElementResultErrorSchemas","V2BulkElementResultRevertTransactionSchemas","V2BulkElementRevertTransaction","V2BulkElementRevertTransactionData","V2BulkResponse","V2ConfigInfoResponse","V2Connector","V2CreateLedgerRequest","V2CreateTransactionResponse","V2CreateTriggerResponse","V2CreateWorkflowRequest","V2CreateWorkflowResponse","V2CreditWalletRequest","V2DebitWalletRequest","V2ErrorsEnum","V2ExpandedTransaction","V2GetLedgerResponse","V2GetTransactionResponse","V2GetWorkflowInstanceHistoryResponse","V2GetWorkflowInstanceHistoryStageResponse","V2GetWorkflowInstanceResponse","V2GetWorkflowResponse","V2Hold","V2Ledger","V2LedgerAccountSubject","V2LedgerInfo","V2LedgerInfoResponse","V2LedgerInfoStorage","V2LedgerListResponse","V2LedgerListResponseCursor","V2ListRunsResponse","V2ListRunsResponseCursor","V2ListTriggersOccurrencesResponse","V2ListTriggersOccurrencesResponseCursor","V2ListTriggersResponse","V2ListTriggersResponseCursor","V2ListWalletsResponse","V2ListWalletsResponseCursor","V2ListWorkflowsResponse","V2ListWorkflowsResponseCursor","V2Log","V2LogType","V2LogsCursorResponse","V2LogsCursorResponseCursor","V2MigrationInfo","V2MigrationInfoState","V2Monetary","V2Payment","V2PaymentAdjustment","V2PaymentAdjustmentRaw","V2PaymentMetadata","V2PaymentRaw","V2PaymentStatus","V2PaymentType","V2PostTransaction","V2PostTransactionScript","V2Posting","V2ReadTriggerResponse","V2RevertTransactionResponse","V2RunWorkflowResponse","V2ServerInfo","V2Stage","V2StageDelay","V2StageSend","V2StageSendDestination","V2StageSendDestinationAccount","V2StageSendDestinationPayment","V2StageSendDestinationWallet","V2StageSendSource","V2StageSendSourceAccount","V2StageSendSourcePayment","V2StageSendSourceWallet","V2StageStatus","V2StageWaitEvent","V2Stats","V2StatsResponse","V2Subject","V2TargetID","V2TargetType","V2TestTriggerResponse","V2Transaction","V2TransactionsCursorResponse","V2TransactionsCursorResponseCursor","V2Trigger","V2TriggerData","V2TriggerOccurrence","V2TriggerTest","V2Update","V2UpdateAccount","V2Volume","V2VolumesWithBalance","V2VolumesWithBalanceCursorResponse","V2VolumesWithBalanceCursorResponseCursor","V2Wallet","V2WalletSubject","V2WalletWithBalances","V2Workflow","V2WorkflowConfig","V2WorkflowInstance","V2WorkflowInstanceHistory","V2WorkflowInstanceHistoryStage","V2WorkflowInstanceHistoryStageInput","V2WorkflowInstanceHistoryStageOutput","Variables","Version","Volume","Wallet","WalletSubject","WalletWithBalances","WalletWithBalancesBalances","WalletsTransaction","WalletsVolume","WebhooksConfig","WebhooksErrorsEnum","WiseConfig","Workflow","WorkflowConfig","WorkflowInstance","WorkflowInstanceHistory","WorkflowInstanceHistoryStage","WorkflowInstanceHistoryStageInput","WorkflowInstanceHistoryStageOutput"]
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/account.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/account.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/accountbalance.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/accountbalance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/accountrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/accountrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/accountresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/accountresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/accountscursor.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/accountscursor.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/accountscursorresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/accountscursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/accountwithvolumesandbalances.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/accountwithvolumesandbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/activitycreatetransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/activitycreatetransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/activitycreatetransactionoutput.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/activitycreatetransactionoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/activitycreditwallet.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/activitycreditwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/activitydebitwallet.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/activitydebitwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/activitygetaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/activitygetaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/activityreverttransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/activityreverttransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/activityreverttransactionoutput.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/activityreverttransactionoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/activitystripetransfer.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/activitystripetransfer.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/adyenconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/adyenconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/atlarconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/atlarconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/attempt.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/attempt.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/balance.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/balance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/balancescursor.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/balancescursor.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/balancescursorresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/balancescursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/balancewithassets.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/balancewithassets.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/bankaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/bankaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/bankaccountrelatedaccounts.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/bankaccountrelatedaccounts.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/bankaccountrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/bankaccountrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/bankaccountscursor.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/bankaccountscursor.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/bankingcircleconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/bankingcircleconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/client.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/client.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/clientsecret.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/clientsecret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/configinfo.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/configinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/configsresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/configsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/configuser.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/configuser.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/confirmholdrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/confirmholdrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/connectorresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/connectorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/connectorsconfigsresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/connectorsconfigsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/connectorsresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/connectorsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/contract.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/contract.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/createbalancerequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/createbalancerequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/createclientrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/createclientrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/createclientresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/createclientresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/createsecretrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/createsecretrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/createsecretresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/createsecretresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/createwalletrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/createwalletrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/createworkflowrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/createworkflowrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/creditwalletrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/creditwalletrequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from .ledgeraccountsubject import LedgerAccountSubject
 from .monetary import Monetary
-from .walletsubject import WalletSubject
+from .subject import Subject
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from sdk import utils
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CreditWalletRequest:
     amount: Monetary = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
     metadata: Dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
     r"""Metadata associated with the wallet."""
-    sources: List[Union[LedgerAccountSubject, WalletSubject]] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sources') }})
+    sources: List[Subject] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sources') }})
     balance: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
     r"""The balance to credit"""
     reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
     timestamp: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/currencycloudconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/currencycloudconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/debitwalletrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/debitwalletrequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from .ledgeraccountsubject import LedgerAccountSubject
 from .monetary import Monetary
-from .walletsubject import WalletSubject
+from .subject import Subject
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from sdk import utils
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DebitWalletRequest:
     amount: Monetary = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
     metadata: Dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
     r"""Metadata associated with the wallet."""
     balances: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balances'), 'exclude': lambda f: f is None }})
     description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    destination: Optional[Union[LedgerAccountSubject, WalletSubject]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination'), 'exclude': lambda f: f is None }})
+    destination: Optional[Subject] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination'), 'exclude': lambda f: f is None }})
     pending: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pending'), 'exclude': lambda f: f is None }})
     r"""Set to true to create a pending hold. If false, the wallet will be debited immediately."""
     timestamp: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""cannot be used in conjunction with `pending` property"""
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/dummypayconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/dummypayconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/expandeddebithold.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/workflowinstancehistorystage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .ledgeraccountsubject import LedgerAccountSubject
-from .walletsubject import WalletSubject
+import dateutil.parser
+from .workflowinstancehistorystageinput import WorkflowInstanceHistoryStageInput
+from .workflowinstancehistorystageoutput import WorkflowInstanceHistoryStageOutput
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
 from sdk import utils
-from typing import Dict, Optional, Union
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ExpandedDebitHold:
-    description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""The unique ID of the hold."""
-    metadata: Dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
-    r"""Metadata associated with the hold."""
-    original_amount: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('originalAmount') }})
-    r"""Original amount on hold"""
-    remaining: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('remaining') }})
-    r"""Remaining amount on hold"""
-    wallet_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('walletID') }})
-    r"""The ID of the wallet the hold is associated with."""
-    destination: Optional[Union[LedgerAccountSubject, WalletSubject]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination'), 'exclude': lambda f: f is None }})
+class WorkflowInstanceHistoryStage:
+    attempt: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('attempt') }})
+    input: WorkflowInstanceHistoryStageInput = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('input') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    started_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
+    terminated: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminated') }})
+    error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
+    last_failure: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastFailure'), 'exclude': lambda f: f is None }})
+    next_execution: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextExecution'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
+    output: Optional[WorkflowInstanceHistoryStageOutput] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('output'), 'exclude': lambda f: f is None }})
+    terminated_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminatedAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/genericconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/genericconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/getholdsresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/getholdsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/gettransactionsresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/gettransactionsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/getversionsresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/getversionsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/getwalletsummaryresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/getwalletsummaryresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/getworkflowinstancehistoryresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/getworkflowinstancehistoryresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/getworkflowinstancehistorystageresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/hold.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/hold.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .ledgeraccountsubject import LedgerAccountSubject
-from .walletsubject import WalletSubject
+from .subject import Subject
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Dict, Optional, Union
+from typing import Dict, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Hold:
     description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     r"""The unique ID of the hold."""
     metadata: Dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
     r"""Metadata associated with the hold."""
     wallet_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('walletID') }})
     r"""The ID of the wallet the hold is associated with."""
-    destination: Optional[Union[LedgerAccountSubject, WalletSubject]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination'), 'exclude': lambda f: f is None }})
+    destination: Optional[Subject] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination'), 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/ledgeraccountsubject.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/ledgeraccountsubject.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/ledgerinfo.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/ledgerinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/ledgerinforesponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/ledgerinforesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/ledgerstorage.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/ledgerstorage.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/listbalancesresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/listbalancesresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/listclientsresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/listclientsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/listtriggersoccurrencesresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/listtriggersoccurrencesresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/listusersresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/listusersresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/listwalletsresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/listwalletsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/log.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from sdk import utils
 from typing import Any, Dict
 
+
 class Type(str, Enum):
     NEW_TRANSACTION = 'NEW_TRANSACTION'
     SET_METADATA = 'SET_METADATA'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/logscursorresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/logscursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/mangopayconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/mangopayconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/mappingresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/mappingresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/migrationinfo.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/migrationinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from sdk import utils
 from typing import Optional
 
+
 class State(str, Enum):
     TO_DO = 'TO DO'
     DONE = 'DONE'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/modulrconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/modulrconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/monetary.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/monetary.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/moneycorpconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/moneycorpconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationlistwalletsresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationlistwalletsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationpayment.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationpayment.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from typing import List, Optional
 
 
 @dataclasses.dataclass
 class OrchestrationPaymentRaw:
     pass
 
+
 class OrchestrationPaymentScheme(str, Enum):
     VISA = 'visa'
     MASTERCARD = 'mastercard'
     AMEX = 'amex'
     DINERS = 'diners'
     DISCOVER = 'discover'
     JCB = 'jcb'
@@ -34,14 +35,15 @@
     A2A = 'a2a'
     ACH_DEBIT = 'ach debit'
     ACH = 'ach'
     RTP = 'rtp'
     UNKNOWN = 'unknown'
     OTHER = 'other'
 
+
 class OrchestrationPaymentType(str, Enum):
     PAY_IN = 'PAY-IN'
     PAYOUT = 'PAYOUT'
     TRANSFER = 'TRANSFER'
     OTHER = 'OTHER'
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationpaymentadjustment.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationpaymentadjustment.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationpaymentmetadata.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationpaymentmetadata.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationposttransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationposttransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationtransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationtransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/orchestrationv2transaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/orchestrationv2transaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/payment.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/payment.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/paymentadjustment.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/paymentadjustment.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/paymentrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/paymentrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/paymentsaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/paymentsaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/paymentscheme.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/paymentscheme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
+
 class PaymentScheme(str, Enum):
     UNKNOWN = 'unknown'
     OTHER = 'other'
     VISA = 'visa'
     MASTERCARD = 'mastercard'
     AMEX = 'amex'
     DINERS = 'diners'
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/paymentscursor.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/paymentscursor.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/policiescursorresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/policiescursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/policy.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/policy.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/policyrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/policyrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/pool.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/pool.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/poolbalance.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/poolbalance.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/poolrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/poolrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/poolscursor.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/poolscursor.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/posting.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/posting.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/posttransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/posttransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/query.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/query.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/readclientresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/readclientresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/readuserresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/readuserresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/reconciliation.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/reconciliation.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/reconciliationrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/reconciliationrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/reconciliationscursorresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/reconciliationscursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/response.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/response.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/reversetransferinitiationrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/reversetransferinitiationrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/script.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/script.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/scriptresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/scriptresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/secret.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/secret.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/stagedelay.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/stagedelay.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/stagesend.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/stagesend.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/stagesenddestination.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/stagesenddestination.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/stagesenddestinationaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/stagesenddestinationaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/stagesenddestinationwallet.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/stagesenddestinationwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/stagesendsource.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/stagesendsource.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/stagesendsourceaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/stagesendsourceaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/stagesendsourcewallet.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/stagesendsourcewallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/stagestatus.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/stagestatus.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/stats.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/stats.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/stripeconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/stripeconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/taskbankingcircle.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/taskbankingcircle.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/taskcurrencycloud.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/taskcurrencycloud.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/taskdummypay.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/taskdummypay.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/taskmangopay.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/taskmangopay.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/taskmodulr.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/taskmodulr.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/taskmoneycorp.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/taskmoneycorp.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/taskresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/taskresponse.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from .taskmoneycorp import TaskMoneycorp
 from .taskstripe import TaskStripe
 from .taskwise import TaskWise
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import Union
 
+TaskResponseData = Union[TaskStripe, TaskWise, TaskCurrencyCloud, TaskDummyPay, TaskModulr, TaskBankingCircle, TaskMangoPay, TaskMoneycorp]
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TaskResponse:
-    data: Union[TaskStripe, TaskWise, TaskCurrencyCloud, TaskDummyPay, TaskModulr, TaskBankingCircle, TaskMangoPay, TaskMoneycorp] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+    data: TaskResponseData = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/taskscursor.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/taskscursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 from .taskmoneycorp import TaskMoneycorp
 from .taskstripe import TaskStripe
 from .taskwise import TaskWise
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
 from typing import List, Optional, Union
 
+TasksCursorData = Union[TaskStripe, TaskWise, TaskCurrencyCloud, TaskDummyPay, TaskModulr, TaskBankingCircle, TaskMangoPay, TaskMoneycorp]
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TasksCursorCursor:
-    data: List[Union[TaskStripe, TaskWise, TaskCurrencyCloud, TaskDummyPay, TaskModulr, TaskBankingCircle, TaskMangoPay, TaskMoneycorp]] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+    data: List[TasksCursorData] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore') }})
     page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
     next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
     previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/taskstripe.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/taskstripe.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/taskwise.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/taskwise.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/transaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/transaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/transactiondata.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/transactiondata.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/transactions.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/transactions.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/transactionscursorresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/transactionscursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/transferinitiation.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/transferinitiation.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .transferinitiationstatus import TransferInitiationStatus
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from sdk import utils
 from typing import Dict, List, Optional
 
+
 class TransferInitiationType(str, Enum):
     TRANSFER = 'TRANSFER'
     PAYOUT = 'PAYOUT'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/transferinitiationadjusments.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/transferinitiationadjusments.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/transferinitiationpayments.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/transferinitiationpayments.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/transferinitiationrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/transferinitiationrequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .connector import Connector
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from sdk import utils
 from typing import Dict, Optional
 
+
 class TransferInitiationRequestType(str, Enum):
     TRANSFER = 'TRANSFER'
     PAYOUT = 'PAYOUT'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/transferinitiationscursor.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/transferinitiationscursor.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/transferinitiationstatus.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/transferinitiationstatus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
+
 class TransferInitiationStatus(str, Enum):
     WAITING_FOR_VALIDATION = 'WAITING_FOR_VALIDATION'
     PROCESSING = 'PROCESSING'
     PROCESSED = 'PROCESSED'
     FAILED = 'FAILED'
     REJECTED = 'REJECTED'
     VALIDATED = 'VALIDATED'
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/transferrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/transferrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/trigger.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/trigger.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/triggerdata.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/triggerdata.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/triggeroccurrence.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/triggeroccurrence.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/updateclientrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/updateclientrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/updateclientresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/updateclientresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/updatetransferinitiationstatusrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/updatetransferinitiationstatusrequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from sdk import utils
 
+
 class Status(str, Enum):
     WAITING_FOR_VALIDATION = 'WAITING_FOR_VALIDATION'
     PROCESSING = 'PROCESSING'
     PROCESSED = 'PROCESSED'
     FAILED = 'FAILED'
     REJECTED = 'REJECTED'
     VALIDATED = 'VALIDATED'
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/user.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/user.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2account.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2account.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2accountscursorresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2accountscursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitycreatetransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitycreatetransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitycreatetransactionoutput.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitycreatetransactionoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitycreditwallet.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitycreditwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitydebitwallet.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitydebitwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitygetaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitygetaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2activitystripetransfer.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2activitystripetransfer.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2bulkelementaddmetadata.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2bulkelementaddmetadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from .v2targetid import V2TargetID
 from .v2targettype import V2TargetType
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Dict, Optional, Union
+from typing import Dict, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class V2BulkElementAddMetadataData:
     metadata: Dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
-    target_id: Union[str, int] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('targetId') }})
+    target_id: V2TargetID = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('targetId') }})
     target_type: V2TargetType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('targetType') }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2bulkelementcreatetransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2bulkelementcreatetransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2bulkelementdeletemetadata.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2bulkelementdeletemetadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from .v2targetid import V2TargetID
 from .v2targettype import V2TargetType
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Optional, Union
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class V2BulkElementDeleteMetadataData:
     key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})
-    target_id: Union[str, int] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('targetId') }})
+    target_id: V2TargetID = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('targetId') }})
     target_type: V2TargetType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('targetType') }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2bulkelementresult.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2transactionscursorresponse.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .v2transaction import V2Transaction
+from .v2expandedtransaction import V2ExpandedTransaction
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Optional
+from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class V2BulkElementResultErrorSchemas:
-    error_code: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorCode') }})
-    error_description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorDescription') }})
-    response_type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('responseType') }})
-    error_details: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorDetails'), 'exclude': lambda f: f is None }})
+class V2TransactionsCursorResponseCursor:
+    data: List[V2ExpandedTransaction] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+    has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore') }})
+    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
+    next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
+    previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class V2BulkElementResultDeleteMetadataSchemas:
-    response_type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('responseType') }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class V2BulkElementResultRevertTransactionSchemas:
-    data: V2Transaction = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-    response_type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('responseType') }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class Schemas:
-    response_type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('responseType') }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class V2BulkElementResultCreateTransactionSchemas:
-    data: V2Transaction = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-    response_type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('responseType') }})
+class V2TransactionsCursorResponse:
+    cursor: V2TransactionsCursorResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2bulkelementreverttransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2bulkelementreverttransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2configinforesponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2configinforesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2createledgerrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2createledgerrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2createworkflowrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2createworkflowrequest.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2creditwalletrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/expandeddebithold.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-from .v2ledgeraccountsubject import V2LedgerAccountSubject
-from .v2monetary import V2Monetary
-from .v2walletsubject import V2WalletSubject
+from .subject import Subject
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
 from sdk import utils
-from typing import Dict, List, Optional, Union
+from typing import Dict, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class V2CreditWalletRequest:
-    amount: V2Monetary = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
+class ExpandedDebitHold:
+    description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    r"""The unique ID of the hold."""
     metadata: Dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
-    r"""Metadata associated with the wallet."""
-    sources: List[Union[V2LedgerAccountSubject, V2WalletSubject]] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sources') }})
-    balance: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
-    r"""The balance to credit"""
-    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
-    timestamp: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
+    r"""Metadata associated with the hold."""
+    original_amount: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('originalAmount') }})
+    r"""Original amount on hold"""
+    remaining: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('remaining') }})
+    r"""Remaining amount on hold"""
+    wallet_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('walletID') }})
+    r"""The ID of the wallet the hold is associated with."""
+    destination: Optional[Subject] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination'), 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2debitwalletrequest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2debitwalletrequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from .v2ledgeraccountsubject import V2LedgerAccountSubject
 from .v2monetary import V2Monetary
-from .v2walletsubject import V2WalletSubject
+from .v2subject import V2Subject
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from sdk import utils
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class V2DebitWalletRequest:
     amount: V2Monetary = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
     metadata: Dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
     r"""Metadata associated with the wallet."""
     balances: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balances'), 'exclude': lambda f: f is None }})
     description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
-    destination: Optional[Union[V2LedgerAccountSubject, V2WalletSubject]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination'), 'exclude': lambda f: f is None }})
+    destination: Optional[V2Subject] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination'), 'exclude': lambda f: f is None }})
     pending: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pending'), 'exclude': lambda f: f is None }})
     r"""Set to true to create a pending hold. If false, the wallet will be debited immediately."""
     timestamp: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""cannot be used in conjunction with `pending` property"""
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2errorsenum.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2errorsenum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
+
 class V2ErrorsEnum(str, Enum):
     INTERNAL = 'INTERNAL'
     INSUFFICIENT_FUND = 'INSUFFICIENT_FUND'
     VALIDATION = 'VALIDATION'
     CONFLICT = 'CONFLICT'
     COMPILATION_FAILED = 'COMPILATION_FAILED'
     METADATA_OVERRIDE = 'METADATA_OVERRIDE'
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2expandedtransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2expandedtransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2getworkflowinstancehistoryresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2getworkflowinstancehistoryresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2getworkflowinstancehistorystageresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2getworkflowinstancehistorystageresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2hold.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2posttransaction.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .v2ledgeraccountsubject import V2LedgerAccountSubject
-from .v2walletsubject import V2WalletSubject
+import dateutil.parser
+from .v2posting import V2Posting
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
 from sdk import utils
-from typing import Dict, Optional, Union
+from typing import Any, Dict, List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class V2Hold:
-    description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""The unique ID of the hold."""
+class V2PostTransactionScript:
+    plain: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('plain') }})
+    vars: Optional[Dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('vars'), 'exclude': lambda f: f is None }})
+    
+
+
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class V2PostTransaction:
     metadata: Dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
-    r"""Metadata associated with the hold."""
-    wallet_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('walletID') }})
-    r"""The ID of the wallet the hold is associated with."""
-    destination: Optional[Union[V2LedgerAccountSubject, V2WalletSubject]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination'), 'exclude': lambda f: f is None }})
+    postings: Optional[List[V2Posting]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postings'), 'exclude': lambda f: f is None }})
+    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
+    script: Optional[V2PostTransactionScript] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('script'), 'exclude': lambda f: f is None }})
+    timestamp: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2ledger.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2ledger.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2ledgeraccountsubject.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2ledgeraccountsubject.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2ledgerinfo.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2ledgerinfo.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2ledgerinforesponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2ledgerinforesponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2ledgerlistresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2ledgerlistresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2listrunsresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2listrunsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2listtriggersoccurrencesresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2listtriggersoccurrencesresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2listtriggersresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2listtriggersresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2listwalletsresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2listwalletsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2listworkflowsresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2listworkflowsresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2log.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2log.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from sdk import utils
 from typing import Any, Dict
 
+
 class V2LogType(str, Enum):
     NEW_TRANSACTION = 'NEW_TRANSACTION'
     SET_METADATA = 'SET_METADATA'
     REVERTED_TRANSACTION = 'REVERTED_TRANSACTION'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2logscursorresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2logscursorresponse.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2migrationinfo.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2migrationinfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from sdk import utils
 from typing import Optional
 
+
 class V2MigrationInfoState(str, Enum):
     TO_DO = 'TO DO'
     DONE = 'DONE'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2monetary.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2monetary.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2payment.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2payment.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from typing import List, Optional
 
 
 @dataclasses.dataclass
 class V2PaymentRaw:
     pass
 
+
 class Scheme(str, Enum):
     VISA = 'visa'
     MASTERCARD = 'mastercard'
     AMEX = 'amex'
     DINERS = 'diners'
     DISCOVER = 'discover'
     JCB = 'jcb'
@@ -34,14 +35,15 @@
     A2A = 'a2a'
     ACH_DEBIT = 'ach debit'
     ACH = 'ach'
     RTP = 'rtp'
     UNKNOWN = 'unknown'
     OTHER = 'other'
 
+
 class V2PaymentType(str, Enum):
     PAY_IN = 'PAY-IN'
     PAYOUT = 'PAYOUT'
     TRANSFER = 'TRANSFER'
     OTHER = 'OTHER'
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2paymentadjustment.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2paymentadjustment.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2posting.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2posting.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2posttransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2triggertest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-from .v2posting import V2Posting
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
 from sdk import utils
-from typing import Any, Dict, List, Optional
+from typing import Dict, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class V2PostTransactionScript:
-    plain: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('plain') }})
-    vars: Optional[Dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('vars'), 'exclude': lambda f: f is None }})
+class Filter:
+    error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
+    match: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('match'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class V2PostTransaction:
-    metadata: Dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
-    postings: Optional[List[V2Posting]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postings'), 'exclude': lambda f: f is None }})
-    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
-    script: Optional[V2PostTransactionScript] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('script'), 'exclude': lambda f: f is None }})
-    timestamp: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
+class Variables:
+    error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
+    value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value'), 'exclude': lambda f: f is None }})
+    
+
+
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class V2TriggerTest:
+    filter_: Optional[Filter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filter'), 'exclude': lambda f: f is None }})
+    variables: Optional[Dict[str, Variables]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('variables'), 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagedelay.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagedelay.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagesend.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagesend.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagesenddestination.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagesenddestination.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagesenddestinationaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagesenddestinationaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagesenddestinationwallet.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagesenddestinationwallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagesendsource.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagesendsource.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagesendsourceaccount.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagesendsourceaccount.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagesendsourcewallet.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagesendsourcewallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2stagestatus.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2stagestatus.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2stats.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2stats.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2transaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2transaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2transactionscursorresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2volumeswithbalance.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .v2expandedtransaction import V2ExpandedTransaction
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class V2TransactionsCursorResponseCursor:
-    data: List[V2ExpandedTransaction] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-    has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore') }})
-    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
-    next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
-    previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class V2TransactionsCursorResponse:
-    cursor: V2TransactionsCursorResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
+class V2VolumesWithBalance:
+    account: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account') }})
+    asset: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('asset') }})
+    balance: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance') }})
+    input: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('input') }})
+    output: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('output') }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2trigger.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2trigger.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2triggerdata.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2triggerdata.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2triggeroccurrence.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2triggeroccurrence.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2triggertest.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2volumeswithbalancecursorresponse.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from .v2volumeswithbalance import V2VolumesWithBalance
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
-from typing import Dict, Optional
+from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Filter:
-    error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
-    match: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('match'), 'exclude': lambda f: f is None }})
+class V2VolumesWithBalanceCursorResponseCursor:
+    data: List[V2VolumesWithBalance] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
+    has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore') }})
+    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
+    next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
+    previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class Variables:
-    error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
-    value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value'), 'exclude': lambda f: f is None }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class V2TriggerTest:
-    filter_: Optional[Filter] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filter'), 'exclude': lambda f: f is None }})
-    variables: Optional[Dict[str, Variables]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('variables'), 'exclude': lambda f: f is None }})
+class V2VolumesWithBalanceCursorResponse:
+    cursor: V2VolumesWithBalanceCursorResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2volume.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2volume.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2volumeswithbalance.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2activityaddaccountmetadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from sdk import utils
+from typing import Dict
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class V2VolumesWithBalance:
-    account: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account') }})
-    asset: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('asset') }})
-    balance: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance') }})
-    input: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('input') }})
-    output: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('output') }})
+class V2ActivityAddAccountMetadata:
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    ledger: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ledger') }})
+    metadata: Dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2volumeswithbalancecursorresponse.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2workflowinstance.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .v2volumeswithbalance import V2VolumesWithBalance
+import dateutil.parser
+from .v2stagestatus import V2StageStatus
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
 from sdk import utils
 from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class V2VolumesWithBalanceCursorResponseCursor:
-    data: List[V2VolumesWithBalance] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-    has_more: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasMore') }})
-    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})
-    next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
-    previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
-    
-
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class V2VolumesWithBalanceCursorResponse:
-    cursor: V2VolumesWithBalanceCursorResponseCursor = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursor') }})
+class V2WorkflowInstance:
+    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    terminated: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminated') }})
+    updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
+    workflow_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workflowID') }})
+    error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
+    status: Optional[List[V2StageStatus]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    terminated_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminatedAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2wallet.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2wallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2walletsubject.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2walletsubject.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2walletwithbalances.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2walletwithbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2workflow.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2workflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2workflowconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2workflowconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2workflowinstance.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/workflowinstance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from .v2stagestatus import V2StageStatus
+from .stagestatus import StageStatus
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from sdk import utils
 from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class V2WorkflowInstance:
+class WorkflowInstance:
     created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     terminated: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminated') }})
     updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
     workflow_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workflowID') }})
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
-    status: Optional[List[V2StageStatus]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    status: Optional[List[StageStatus]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
     terminated_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminatedAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2workflowinstancehistory.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2workflowinstancehistorystage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from .v2stagedelay import V2StageDelay
-from .v2stagesend import V2StageSend
-from .v2stagewaitevent import V2StageWaitEvent
+from .v2workflowinstancehistorystageinput import V2WorkflowInstanceHistoryStageInput
+from .v2workflowinstancehistorystageoutput import V2WorkflowInstanceHistoryStageOutput
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from sdk import utils
-from typing import Optional, Union
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class V2WorkflowInstanceHistory:
-    input: Union[V2StageSend, V2StageDelay, V2StageWaitEvent] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('input') }})
+class V2WorkflowInstanceHistoryStage:
+    attempt: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('attempt') }})
+    input: V2WorkflowInstanceHistoryStageInput = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('input') }})
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     started_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
     terminated: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminated') }})
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
+    last_failure: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastFailure'), 'exclude': lambda f: f is None }})
+    next_execution: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextExecution'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
+    output: Optional[V2WorkflowInstanceHistoryStageOutput] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('output'), 'exclude': lambda f: f is None }})
     terminated_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminatedAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2workflowinstancehistorystage.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2creditwalletrequest.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from .v2workflowinstancehistorystageinput import V2WorkflowInstanceHistoryStageInput
-from .v2workflowinstancehistorystageoutput import V2WorkflowInstanceHistoryStageOutput
+from .v2monetary import V2Monetary
+from .v2subject import V2Subject
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from sdk import utils
-from typing import Optional
+from typing import Dict, List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class V2WorkflowInstanceHistoryStage:
-    attempt: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('attempt') }})
-    input: V2WorkflowInstanceHistoryStageInput = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('input') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    started_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
-    terminated: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminated') }})
-    error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
-    last_failure: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastFailure'), 'exclude': lambda f: f is None }})
-    next_execution: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nextExecution'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
-    output: Optional[V2WorkflowInstanceHistoryStageOutput] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('output'), 'exclude': lambda f: f is None }})
-    terminated_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminatedAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
+class V2CreditWalletRequest:
+    amount: V2Monetary = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amount') }})
+    metadata: Dict[str, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata') }})
+    r"""Metadata associated with the wallet."""
+    sources: List[V2Subject] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sources') }})
+    balance: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
+    r"""The balance to credit"""
+    reference: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference'), 'exclude': lambda f: f is None }})
+    timestamp: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timestamp'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2workflowinstancehistorystageinput.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2workflowinstancehistorystageinput.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from .v2activityaddaccountmetadata import V2ActivityAddAccountMetadata
 from .v2activityconfirmhold import V2ActivityConfirmHold
 from .v2activitycreatetransaction import V2ActivityCreateTransaction
 from .v2activitycreditwallet import V2ActivityCreditWallet
 from .v2activitydebitwallet import V2ActivityDebitWallet
 from .v2activitygetaccount import V2ActivityGetAccount
 from .v2activitygetpayment import V2ActivityGetPayment
 from .v2activitygetwallet import V2ActivityGetWallet
@@ -16,14 +17,15 @@
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class V2WorkflowInstanceHistoryStageInput:
+    add_account_metadata: Optional[V2ActivityAddAccountMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('AddAccountMetadata'), 'exclude': lambda f: f is None }})
     confirm_hold: Optional[V2ActivityConfirmHold] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ConfirmHold'), 'exclude': lambda f: f is None }})
     create_transaction: Optional[V2ActivityCreateTransaction] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('CreateTransaction'), 'exclude': lambda f: f is None }})
     credit_wallet: Optional[V2ActivityCreditWallet] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('CreditWallet'), 'exclude': lambda f: f is None }})
     debit_wallet: Optional[V2ActivityDebitWallet] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('DebitWallet'), 'exclude': lambda f: f is None }})
     get_account: Optional[V2ActivityGetAccount] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('GetAccount'), 'exclude': lambda f: f is None }})
     get_payment: Optional[V2ActivityGetPayment] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('GetPayment'), 'exclude': lambda f: f is None }})
     get_wallet: Optional[V2ActivityGetWallet] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('GetWallet'), 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/v2workflowinstancehistorystageoutput.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2workflowinstancehistorystageoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/version.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/version.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/volume.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/volume.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/wallet.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/wallet.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/walletstransaction.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/walletstransaction.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/walletsubject.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/walletsubject.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/walletsvolume.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/walletsvolume.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/walletwithbalances.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/walletwithbalances.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/webhooksconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/webhooksconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/wiseconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/wiseconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/workflow.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/workflow.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/workflowconfig.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/workflowconfig.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/workflowinstance.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/workflowinstancehistory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from .stagestatus import StageStatus
+from .stage import Stage
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from sdk import utils
-from typing import List, Optional
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class WorkflowInstance:
-    created_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+class WorkflowInstanceHistory:
+    input: Stage = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('input') }})
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    started_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
     terminated: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminated') }})
-    updated_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('updatedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
-    workflow_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workflowID') }})
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
-    status: Optional[List[StageStatus]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
     terminated_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminatedAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/workflowinstancehistory.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/v2workflowinstancehistory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from .stagedelay import StageDelay
-from .stagesend import StageSend
-from .stagewaitevent import StageWaitEvent
+from .v2stage import V2Stage
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from sdk import utils
-from typing import Optional, Union
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class WorkflowInstanceHistory:
-    input: Union[StageSend, StageDelay, StageWaitEvent] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('input') }})
+class V2WorkflowInstanceHistory:
+    input: V2Stage = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('input') }})
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     started_at: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startedAt'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
     terminated: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminated') }})
     error: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('error'), 'exclude': lambda f: f is None }})
     terminated_at: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terminatedAt'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/workflowinstancehistorystageinput.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/workflowinstancehistorystageinput.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from .activityaddaccountmetadata import ActivityAddAccountMetadata
 from .activityconfirmhold import ActivityConfirmHold
 from .activitycreatetransaction import ActivityCreateTransaction
 from .activitycreditwallet import ActivityCreditWallet
 from .activitydebitwallet import ActivityDebitWallet
 from .activitygetaccount import ActivityGetAccount
 from .activitygetpayment import ActivityGetPayment
 from .activitygetwallet import ActivityGetWallet
@@ -17,14 +18,15 @@
 from sdk import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class WorkflowInstanceHistoryStageInput:
+    add_account_metadata: Optional[ActivityAddAccountMetadata] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('AddAccountMetadata'), 'exclude': lambda f: f is None }})
     confirm_hold: Optional[ActivityConfirmHold] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ConfirmHold'), 'exclude': lambda f: f is None }})
     create_transaction: Optional[ActivityCreateTransaction] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('CreateTransaction'), 'exclude': lambda f: f is None }})
     credit_wallet: Optional[ActivityCreditWallet] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('CreditWallet'), 'exclude': lambda f: f is None }})
     debit_wallet: Optional[ActivityDebitWallet] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('DebitWallet'), 'exclude': lambda f: f is None }})
     get_account: Optional[ActivityGetAccount] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('GetAccount'), 'exclude': lambda f: f is None }})
     get_payment: Optional[ActivityGetPayment] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('GetPayment'), 'exclude': lambda f: f is None }})
     get_wallet: Optional[ActivityGetWallet] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('GetWallet'), 'exclude': lambda f: f is None }})
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/models/shared/workflowinstancehistorystageoutput.py` & `formance-sdk-python-2.3.0/src/sdk/models/shared/workflowinstancehistorystageoutput.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/orchestration.py` & `formance-sdk-python-2.3.0/src/sdk/orchestration.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,26 +54,27 @@
         
         
         res = operations.CancelEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def create_trigger(self, request: Optional[shared.TriggerData]) -> operations.CreateTriggerResponse:
+    def create_trigger(self, request: Optional[shared.TriggerData] = None) -> operations.CreateTriggerResponse:
         r"""Create trigger
         Create trigger
         """
         hook_ctx = HookContext(operation_id='createTrigger', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/api/orchestration/triggers'
@@ -109,33 +110,35 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateTriggerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CreateTriggerResponse])
                 res.create_trigger_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def create_workflow(self, request: Optional[shared.CreateWorkflowRequest]) -> operations.CreateWorkflowResponse:
+    def create_workflow(self, request: Optional[shared.CreateWorkflowRequest] = None) -> operations.CreateWorkflowResponse:
         r"""Create workflow
         Create a workflow
         """
         hook_ctx = HookContext(operation_id='createWorkflow', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/api/orchestration/workflows'
@@ -171,21 +174,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateWorkflowResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CreateWorkflowResponse])
                 res.create_workflow_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -232,14 +237,15 @@
         
         
         res = operations.DeleteTriggerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -286,14 +292,15 @@
         
         
         res = operations.DeleteWorkflowResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -338,21 +345,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetInstanceResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.GetWorkflowInstanceResponse])
                 res.get_workflow_instance_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -397,21 +406,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetInstanceHistoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.GetWorkflowInstanceHistoryResponse])
                 res.get_workflow_instance_history_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -456,21 +467,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetInstanceStageHistoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.GetWorkflowInstanceHistoryStageResponse])
                 res.get_workflow_instance_history_stage_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -515,21 +528,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetWorkflowResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.GetWorkflowResponse])
                 res.get_workflow_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -575,21 +590,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListInstancesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ListRunsResponse])
                 res.list_runs_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -635,21 +652,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListTriggersResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ListTriggersResponse])
                 res.list_triggers_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -694,21 +713,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListTriggersOccurrencesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ListTriggersOccurrencesResponse])
                 res.list_triggers_occurrences_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -753,21 +774,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListWorkflowsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ListWorkflowsResponse])
                 res.list_workflows_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -810,21 +833,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.OrchestrationgetServerInfoResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ServerInfo])
                 res.server_info = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -869,21 +894,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ReadTriggerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ReadTriggerResponse])
                 res.read_trigger_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -932,21 +959,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.RunWorkflowResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.RunWorkflowResponse])
                 res.run_workflow_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -996,14 +1025,15 @@
         
         
         res = operations.SendEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1051,21 +1081,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.TestTriggerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2TestTriggerResponse])
                 res.v2_test_trigger_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1112,26 +1144,27 @@
         
         
         res = operations.V2CancelEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def v2_create_trigger(self, request: Optional[shared.V2TriggerData]) -> operations.V2CreateTriggerResponse:
+    def v2_create_trigger(self, request: Optional[shared.V2TriggerData] = None) -> operations.V2CreateTriggerResponse:
         r"""Create trigger
         Create trigger
         """
         hook_ctx = HookContext(operation_id='v2CreateTrigger', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/api/orchestration/v2/triggers'
@@ -1167,33 +1200,35 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2CreateTriggerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2CreateTriggerResponse])
                 res.v2_create_trigger_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def v2_create_workflow(self, request: Optional[shared.V2CreateWorkflowRequest]) -> operations.V2CreateWorkflowResponse:
+    def v2_create_workflow(self, request: Optional[shared.V2CreateWorkflowRequest] = None) -> operations.V2CreateWorkflowResponse:
         r"""Create workflow
         Create a workflow
         """
         hook_ctx = HookContext(operation_id='v2CreateWorkflow', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/api/orchestration/v2/workflows'
@@ -1229,21 +1264,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2CreateWorkflowResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2CreateWorkflowResponse])
                 res.v2_create_workflow_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1290,14 +1327,15 @@
         
         
         res = operations.V2DeleteTriggerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1344,14 +1382,15 @@
         
         
         res = operations.V2DeleteWorkflowResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1396,21 +1435,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2GetInstanceResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2GetWorkflowInstanceResponse])
                 res.v2_get_workflow_instance_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1455,21 +1496,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2GetInstanceHistoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2GetWorkflowInstanceHistoryResponse])
                 res.v2_get_workflow_instance_history_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1514,21 +1557,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2GetInstanceStageHistoryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2GetWorkflowInstanceHistoryStageResponse])
                 res.v2_get_workflow_instance_history_stage_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1571,21 +1616,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2GetServerInfoResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2ServerInfo])
                 res.v2_server_info = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1630,21 +1677,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2GetWorkflowResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2GetWorkflowResponse])
                 res.v2_get_workflow_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1690,21 +1739,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2ListInstancesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2ListRunsResponse])
                 res.v2_list_runs_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1750,21 +1801,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2ListTriggersResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2ListTriggersResponse])
                 res.v2_list_triggers_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1810,21 +1863,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2ListTriggersOccurrencesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2ListTriggersOccurrencesResponse])
                 res.v2_list_triggers_occurrences_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1870,21 +1925,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2ListWorkflowsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2ListWorkflowsResponse])
                 res.v2_list_workflows_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1929,21 +1986,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2ReadTriggerResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2ReadTriggerResponse])
                 res.v2_read_trigger_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -1992,21 +2051,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.V2RunWorkflowResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.V2RunWorkflowResponse])
                 res.v2_run_workflow_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -2056,14 +2117,15 @@
         
         
         res = operations.V2SendEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.V2Error)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/payments.py` & `formance-sdk-python-2.3.0/src/sdk/payments.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.AddAccountToPoolRequest, "add_account_to_pool_request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
-        headers['Accept'] = '*/*'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -59,15 +59,21 @@
         
         
         res = operations.AddAccountToPoolResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def connectors_transfer(self, request: operations.ConnectorsTransferRequest) -> operations.ConnectorsTransferResponse:
         r"""Transfer funds between Connector accounts
@@ -111,22 +117,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ConnectorsTransferResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TransferResponse])
                 res.transfer_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def create_account(self, request: shared.AccountRequest) -> operations.CreateAccountResponse:
         r"""Create an account
@@ -170,22 +183,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentsAccountResponse])
                 res.payments_account_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def create_bank_account(self, request: shared.BankAccountRequest) -> operations.CreateBankAccountResponse:
         r"""Create a BankAccount in Payments and on the PSP
@@ -229,22 +249,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateBankAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.BankAccountResponse])
                 res.bank_account_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def create_payment(self, request: shared.PaymentRequest) -> operations.CreatePaymentResponse:
         r"""Create a payment
@@ -288,22 +315,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreatePaymentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentResponse])
                 res.payment_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def create_pool(self, request: shared.PoolRequest) -> operations.CreatePoolResponse:
         r"""Create a Pool
@@ -347,22 +381,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreatePoolResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PoolResponse])
                 res.pool_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def create_transfer_initiation(self, request: shared.TransferInitiationRequest) -> operations.CreateTransferInitiationResponse:
         r"""Create a TransferInitiation
@@ -406,22 +447,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateTransferInitiationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TransferInitiationResponse])
                 res.transfer_initiation_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def delete_pool(self, request: operations.DeletePoolRequest) -> operations.DeletePoolResponse:
         r"""Delete a Pool
@@ -433,15 +481,15 @@
         url = utils.generate_url(base_url, '/api/payments/pools/{poolId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers['Accept'] = '*/*'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -462,15 +510,21 @@
         
         
         res = operations.DeletePoolResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def delete_transfer_initiation(self, request: operations.DeleteTransferInitiationRequest) -> operations.DeleteTransferInitiationResponse:
         r"""Delete a transfer initiation
@@ -482,15 +536,15 @@
         url = utils.generate_url(base_url, '/api/payments/transfer-initiations/{transferId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers['Accept'] = '*/*'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -511,15 +565,21 @@
         
         
         res = operations.DeleteTransferInitiationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def forward_bank_account(self, request: operations.ForwardBankAccountRequest) -> operations.ForwardBankAccountResponse:
         r"""Forward a bank account to a connector"""
@@ -561,22 +621,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ForwardBankAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.BankAccountResponse])
                 res.bank_account_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def get_account_balances(self, request: operations.GetAccountBalancesRequest) -> operations.GetAccountBalancesResponse:
         r"""Get account balances"""
@@ -614,22 +681,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetAccountBalancesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.BalancesCursor])
                 res.balances_cursor = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def get_bank_account(self, request: operations.GetBankAccountRequest) -> operations.GetBankAccountResponse:
         r"""Get a bank account created by user on Formance"""
@@ -666,22 +740,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetBankAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.BankAccountResponse])
                 res.bank_account_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def get_connector_task(self, request: operations.GetConnectorTaskRequest) -> operations.GetConnectorTaskResponse:
         r"""Read a specific task of the connector
@@ -722,22 +803,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetConnectorTaskResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TaskResponse])
                 res.task_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def get_connector_task_v1(self, request: operations.GetConnectorTaskV1Request) -> operations.GetConnectorTaskV1Response:
         r"""Read a specific task of the connector
@@ -776,22 +864,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetConnectorTaskV1Response(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TaskResponse])
                 res.task_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def get_payment(self, request: operations.GetPaymentRequest) -> operations.GetPaymentResponse:
         r"""Get a payment"""
@@ -828,22 +923,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetPaymentResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentResponse])
                 res.payment_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def get_pool(self, request: operations.GetPoolRequest) -> operations.GetPoolResponse:
         r"""Get a Pool"""
@@ -880,22 +982,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetPoolResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PoolResponse])
                 res.pool_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def get_pool_balances(self, request: operations.GetPoolBalancesRequest) -> operations.GetPoolBalancesResponse:
         r"""Get pool balances"""
@@ -933,22 +1042,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetPoolBalancesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PoolBalancesResponse])
                 res.pool_balances_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def get_transfer_initiation(self, request: operations.GetTransferInitiationRequest) -> operations.GetTransferInitiationResponse:
         r"""Get a transfer initiation"""
@@ -985,22 +1101,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetTransferInitiationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TransferInitiationResponse])
                 res.transfer_initiation_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def install_connector(self, request: operations.InstallConnectorRequest) -> operations.InstallConnectorResponse:
         r"""Install a connector
@@ -1044,22 +1167,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.InstallConnectorResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ConnectorResponse])
                 res.connector_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def list_all_connectors(self) -> operations.ListAllConnectorsResponse:
         r"""List all installed connectors
@@ -1098,22 +1228,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListAllConnectorsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ConnectorsResponse])
                 res.connectors_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def list_bank_accounts(self, request: operations.ListBankAccountsRequest) -> operations.ListBankAccountsResponse:
         r"""List bank accounts created by user on Formance
@@ -1153,22 +1290,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListBankAccountsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.BankAccountsCursor])
                 res.bank_accounts_cursor = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def list_configs_available_connectors(self) -> operations.ListConfigsAvailableConnectorsResponse:
         r"""List the configs of each available connector
@@ -1207,22 +1351,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListConfigsAvailableConnectorsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ConnectorsConfigsResponse])
                 res.connectors_configs_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def list_connector_tasks(self, request: operations.ListConnectorTasksRequest) -> operations.ListConnectorTasksResponse:
         r"""List tasks from a connector
@@ -1264,22 +1415,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListConnectorTasksResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TasksCursor])
                 res.tasks_cursor = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def list_connector_tasks_v1(self, request: operations.ListConnectorTasksV1Request) -> operations.ListConnectorTasksV1Response:
         r"""List tasks from a connector
@@ -1319,22 +1477,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListConnectorTasksV1Response(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TasksCursor])
                 res.tasks_cursor = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def list_payments(self, request: operations.ListPaymentsRequest) -> operations.ListPaymentsResponse:
         r"""List payments"""
@@ -1372,22 +1537,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListPaymentsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentsCursor])
                 res.payments_cursor = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def list_pools(self, request: operations.ListPoolsRequest) -> operations.ListPoolsResponse:
         r"""List Pools"""
@@ -1425,22 +1597,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListPoolsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PoolsCursor])
                 res.pools_cursor = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def list_transfer_initiations(self, request: operations.ListTransferInitiationsRequest) -> operations.ListTransferInitiationsResponse:
         r"""List Transfer Initiations"""
@@ -1478,22 +1657,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListTransferInitiationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.TransferInitiationsCursor])
                 res.transfer_initiations_cursor = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def paymentsget_account(self, request: operations.PaymentsgetAccountRequest) -> operations.PaymentsgetAccountResponse:
         r"""Get an account"""
@@ -1530,22 +1716,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PaymentsgetAccountResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentsAccountResponse])
                 res.payments_account_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def paymentsget_server_info(self) -> operations.PaymentsgetServerInfoResponse:
         r"""Get server info"""
@@ -1582,22 +1775,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PaymentsgetServerInfoResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ServerInfo])
                 res.server_info = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def paymentslist_accounts(self, request: operations.PaymentslistAccountsRequest) -> operations.PaymentslistAccountsResponse:
         r"""List accounts"""
@@ -1638,22 +1838,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.PaymentslistAccountsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AccountsCursor])
                 res.accounts_cursor = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def read_connector_config(self, request: operations.ReadConnectorConfigRequest) -> operations.ReadConnectorConfigResponse:
         r"""Read the config of a connector
@@ -1694,22 +1901,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ReadConnectorConfigResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ConnectorConfigResponse])
                 res.connector_config_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def read_connector_config_v1(self, request: operations.ReadConnectorConfigV1Request) -> operations.ReadConnectorConfigV1Response:
         r"""Read the config of a connector
@@ -1748,22 +1962,29 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ReadConnectorConfigV1Response(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ConnectorConfigResponse])
                 res.connector_config_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def remove_account_from_pool(self, request: operations.RemoveAccountFromPoolRequest) -> operations.RemoveAccountFromPoolResponse:
         r"""Remove an account from a pool
@@ -1775,15 +1996,15 @@
         url = utils.generate_url(base_url, '/api/payments/pools/{poolId}/accounts/{accountId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers['Accept'] = '*/*'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -1804,15 +2025,21 @@
         
         
         res = operations.RemoveAccountFromPoolResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def reset_connector(self, request: operations.ResetConnectorRequest) -> operations.ResetConnectorResponse:
         r"""Reset a connector
@@ -1827,15 +2054,15 @@
         url = utils.generate_url(base_url, '/api/payments/connectors/{connector}/reset', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers['Accept'] = '*/*'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -1856,15 +2083,21 @@
         
         
         res = operations.ResetConnectorResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def reset_connector_v1(self, request: operations.ResetConnectorV1Request) -> operations.ResetConnectorV1Response:
         r"""Reset a connector
@@ -1877,15 +2110,15 @@
         url = utils.generate_url(base_url, '/api/payments/connectors/{connector}/{connectorId}/reset', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers['Accept'] = '*/*'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -1906,15 +2139,21 @@
         
         
         res = operations.ResetConnectorV1Response(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def retry_transfer_initiation(self, request: operations.RetryTransferInitiationRequest) -> operations.RetryTransferInitiationResponse:
         r"""Retry a failed transfer initiation
@@ -1926,15 +2165,15 @@
         url = utils.generate_url(base_url, '/api/payments/transfer-initiations/{transferId}/retry', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers['Accept'] = '*/*'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -1955,15 +2194,21 @@
         
         
         res = operations.RetryTransferInitiationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def reverse_transfer_initiation(self, request: operations.ReverseTransferInitiationRequest) -> operations.ReverseTransferInitiationResponse:
         r"""Reverse a transfer initiation
@@ -1980,15 +2225,15 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.ReverseTransferInitiationRequest, "reverse_transfer_initiation_request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
-        headers['Accept'] = '*/*'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -2009,15 +2254,21 @@
         
         
         res = operations.ReverseTransferInitiationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def udpate_transfer_initiation_status(self, request: operations.UdpateTransferInitiationStatusRequest) -> operations.UdpateTransferInitiationStatusResponse:
         r"""Update the status of a transfer initiation
@@ -2034,15 +2285,15 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UdpateTransferInitiationStatusRequest, "update_transfer_initiation_status_request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
-        headers['Accept'] = '*/*'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -2063,15 +2314,21 @@
         
         
         res = operations.UdpateTransferInitiationStatusResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def uninstall_connector(self, request: operations.UninstallConnectorRequest) -> operations.UninstallConnectorResponse:
         r"""Uninstall a connector
@@ -2085,15 +2342,15 @@
         url = utils.generate_url(base_url, '/api/payments/connectors/{connector}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers['Accept'] = '*/*'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -2114,15 +2371,21 @@
         
         
         res = operations.UninstallConnectorResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def uninstall_connector_v1(self, request: operations.UninstallConnectorV1Request) -> operations.UninstallConnectorV1Response:
         r"""Uninstall a connector
@@ -2134,15 +2397,15 @@
         url = utils.generate_url(base_url, '/api/payments/connectors/{connector}/{connectorId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers['Accept'] = '*/*'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -2163,15 +2426,21 @@
         
         
         res = operations.UninstallConnectorV1Response(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def update_bank_account_metadata(self, request: operations.UpdateBankAccountMetadataRequest) -> operations.UpdateBankAccountMetadataResponse:
         r"""Update metadata of a bank account"""
@@ -2186,15 +2455,15 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateBankAccountMetadataRequest, "update_bank_account_metadata_request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
-        headers['Accept'] = '*/*'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('PATCH', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -2215,15 +2484,21 @@
         
         
         res = operations.UpdateBankAccountMetadataResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def update_connector_config_v1(self, request: operations.UpdateConnectorConfigV1Request) -> operations.UpdateConnectorConfigV1Response:
         r"""Update the config of a connector
@@ -2240,15 +2515,15 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateConnectorConfigV1Request, "connector_config", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
-        headers['Accept'] = '*/*'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -2269,15 +2544,21 @@
         
         
         res = operations.UpdateConnectorConfigV1Response(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
     def update_metadata(self, request: operations.UpdateMetadataRequest) -> operations.UpdateMetadataResponse:
         r"""Update metadata"""
@@ -2292,15 +2573,15 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateMetadataRequest, "request_body", True, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
-        headers['Accept'] = '*/*'
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('PATCH', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
@@ -2321,13 +2602,19 @@
         
         
         res = operations.UpdateMetadataResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.PaymentsErrorResponse)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/reconciliation.py` & `formance-sdk-python-2.3.0/src/sdk/reconciliation.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,21 +57,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreatePolicyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PolicyResponse])
                 res.policy_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ReconciliationErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -118,14 +120,15 @@
         
         
         res = operations.DeletePolicyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ReconciliationErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -168,21 +171,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetPolicyResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PolicyResponse])
                 res.policy_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ReconciliationErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -225,21 +230,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetReconciliationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ReconciliationResponse])
                 res.reconciliation_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ReconciliationErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -283,21 +290,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListPoliciesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.PoliciesCursorResponse])
                 res.policies_cursor_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ReconciliationErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -341,21 +350,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListReconciliationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ReconciliationsCursorResponse])
                 res.reconciliations_cursor_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ReconciliationErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -405,21 +416,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ReconcileResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ReconciliationResponse])
                 res.reconciliation_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ReconciliationErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -462,21 +475,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ReconciliationgetServerInfoResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ServerInfo])
                 res.server_info = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ReconciliationErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/sdk.py` & `formance-sdk-python-2.3.0/src/sdk/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetVersionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.GetVersionsResponse])
                 res.get_versions_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/sdkconfiguration.py` & `formance-sdk-python-2.3.0/src/sdk/sdkconfiguration.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 @dataclass
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
-    openapi_doc_version: str = 'v2.0.0-rc.26'
-    sdk_version: str = '2.2.3'
-    gen_version: str = '2.314.0'
-    user_agent: str = 'speakeasy-sdk/python 2.2.3 2.314.0 v2.0.0-rc.26 formance-sdk-python'
+    openapi_doc_version: str = 'v2.0.0-rc.31'
+    sdk_version: str = '2.3.0'
+    gen_version: str = '2.338.7'
+    user_agent: str = 'speakeasy-sdk/python 2.3.0 2.338.7 v2.0.0-rc.31 formance-sdk-python'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/search.py` & `formance-sdk-python-2.3.0/src/sdk/search.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,14 +57,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.SearchResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.Response])
                 res.response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -109,14 +110,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.SearchgetServerInfoResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ServerInfo])
                 res.server_info = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/utils/retries.py` & `formance-sdk-python-2.3.0/src/sdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `formance-sdk-python-2.2.3/src/sdk/utils/utils.py` & `formance-sdk-python-2.3.0/src/sdk/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -814,19 +814,19 @@
             return ",".join(items)
     else:
         return f"{_val_to_string(obj)}"
 
     return ""
 
 
-def unmarshal_json(data, typ, decoder=None):
+def unmarshal_json(data, typ, decoder=None, infer_missing=False):
     unmarshal = make_dataclass("Unmarshal", [("res", typ)], bases=(DataClassJsonMixin,))
     json_dict = json.loads(data)
     try:
-        out = unmarshal.from_dict({"res": json_dict})
+        out = unmarshal.from_dict({"res": json_dict}, infer_missing=infer_missing)
     except AttributeError as attr_err:
         raise AttributeError(
             f"unable to unmarshal {data} as {typ} - {attr_err}"
         ) from attr_err
 
     return out.res if decoder is None else decoder(out.res)
 
@@ -904,14 +904,41 @@
 
 
 def bigintdecoder(val):
     if isinstance(val, float):
         raise ValueError(f"{val} is a float")
     return int(val)
 
+def integerstrencoder(optional: bool):
+    def integerstrencode(val: int):
+        if optional and val is None:
+            return None
+        return str(val)
+
+    return integerstrencode
+
+
+def integerstrdecoder(val):
+    if isinstance(val, float):
+        raise ValueError(f"{val} is a float")
+    return int(val)
+
+
+def numberstrencoder(optional: bool):
+    def numberstrencode(val: float):
+        if optional and val is None:
+            return None
+        return str(val)
+
+    return numberstrencode
+
+
+def numberstrdecoder(val):
+    return float(val)
+
 
 def decimalencoder(optional: bool, as_str: bool):
     def decimalencode(val: Decimal):
         if optional and val is None:
             return None
 
         if as_str:
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/wallets.py` & `formance-sdk-python-2.3.0/src/sdk/wallets.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         
         
         res = operations.ConfirmHoldResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WalletsErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -108,33 +109,35 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateBalanceResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CreateBalanceResponse])
                 res.create_balance_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WalletsErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def create_wallet(self, request: Optional[shared.CreateWalletRequest]) -> operations.CreateWalletResponse:
+    def create_wallet(self, request: Optional[shared.CreateWalletRequest] = None) -> operations.CreateWalletResponse:
         r"""Create a new wallet"""
         hook_ctx = HookContext(operation_id='createWallet', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/api/wallets/wallets'
         
         if callable(self.sdk_configuration.security):
@@ -168,21 +171,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.CreateWalletResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.CreateWalletResponse])
                 res.create_wallet_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WalletsErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -230,14 +235,15 @@
         
         
         res = operations.CreditWalletResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WalletsErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -283,23 +289,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.DebitWalletResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.DebitWalletResponse])
                 res.debit_wallet_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WalletsErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -342,21 +350,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetBalanceResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.GetBalanceResponse])
                 res.get_balance_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WalletsErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -399,21 +409,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetHoldResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.GetHoldResponse])
                 res.get_hold_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WalletsErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -457,21 +469,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetHoldsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.GetHoldsResponse])
                 res.get_holds_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WalletsErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -514,21 +528,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetTransactionsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.GetTransactionsResponse])
                 res.get_transactions_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WalletsErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -571,23 +587,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetWalletResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.GetWalletResponse])
                 res.get_wallet_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WalletsErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -630,23 +648,25 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetWalletSummaryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.GetWalletSummaryResponse])
                 res.get_wallet_summary_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WalletsErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -689,14 +709,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListBalancesResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ListBalancesResponse])
                 res.list_balances_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
@@ -742,21 +763,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ListWalletsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ListWalletsResponse])
                 res.list_wallets_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WalletsErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -804,14 +827,15 @@
         
         
         res = operations.UpdateWalletResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WalletsErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -856,14 +880,15 @@
         
         
         res = operations.VoidHoldResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 204:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WalletsErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -906,21 +931,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.WalletsgetServerInfoResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ServerInfo])
                 res.server_info = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WalletsErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

### Comparing `formance-sdk-python-2.2.3/src/sdk/webhooks.py` & `formance-sdk-python-2.3.0/src/sdk/webhooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,21 +52,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ActivateConfigResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ConfigResponse])
                 res.config_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WebhooksErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -117,21 +119,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.ChangeConfigSecretResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ConfigResponse])
                 res.config_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WebhooksErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -176,21 +180,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.DeactivateConfigResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ConfigResponse])
                 res.config_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WebhooksErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -237,14 +243,15 @@
         
         
         res = operations.DeleteConfigResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WebhooksErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -290,21 +297,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.GetManyConfigsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ConfigsResponse])
                 res.configs_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WebhooksErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -362,21 +371,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.InsertConfigResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.ConfigResponse])
                 res.config_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WebhooksErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
@@ -421,21 +432,23 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         res = operations.TestConfigResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[shared.AttemptResponse])
                 res.attempt_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         else:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.WebhooksErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
```

