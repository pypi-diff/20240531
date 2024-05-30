# Comparing `tmp/cuenca-1.0.0.tar.gz` & `tmp/cuenca-1.0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuenca-1.0.0.tar", last modified: Mon Apr  1 23:57:56 2024, max compression
+gzip compressed data, was "cuenca-1.0.1.dev1.tar", last modified: Thu May 30 23:23:20 2024, max compression
```

## Comparing `cuenca-1.0.0.tar` & `cuenca-1.0.1.dev1.tar`

### file list

```diff
@@ -1,115 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:56.632049 cuenca-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-01 23:57:50.000000 cuenca-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-01 23:57:56.632049 cuenca-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-01 23:57:50.000000 cuenca-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:56.612049 cuenca-1.0.0/cuenca/
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:56.612049 cuenca-1.0.0/cuenca/http/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/http/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:56.620050 cuenca-1.0.0/cuenca/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/arpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/balance_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/bill_payments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/card_activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/card_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/card_validations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/cards.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/cash_references.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/clabes.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/commissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/curp_validations.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/deposits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/file_batches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/identities.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/identity_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/kyc_validations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/kyc_verifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/limited_wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/login_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/platforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/questionnaires.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/savings.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/service_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/statements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/user_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/user_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/user_lists_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/user_logins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/verifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/wallet_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/resources/whatsapp_transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-01 23:57:50.000000 cuenca-1.0.0/cuenca/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:56.632049 cuenca-1.0.0/cuenca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-01 23:57:56.000000 cuenca-1.0.0/cuenca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-01 23:57:56.000000 cuenca-1.0.0/cuenca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 23:57:56.000000 cuenca-1.0.0/cuenca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-01 23:57:56.000000 cuenca-1.0.0/cuenca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 23:57:56.000000 cuenca-1.0.0/cuenca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-01 23:57:56.632049 cuenca-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-01 23:57:50.000000 cuenca-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:56.624050 cuenca-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:56.624050 cuenca-1.0.0/tests/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/http/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/http/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:56.632049 cuenca-1.0.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_arpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_balance_entries.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_bill_payments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_card_activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_card_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_card_validations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_cards.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_cash_references.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_clabes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_commissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_curp_validations.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_deposits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_file_batches.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_identities.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_identity_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_kyc_validations.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_kyc_verifications.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_limited_wallets.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_login_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_platforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_questionnaires.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_savings.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_service_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_statements.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_user_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_user_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_user_lists_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_user_logins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_verifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_wallet_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/resources/test_whatsapp_transfers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/test_cuenca.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-01 23:57:50.000000 cuenca-1.0.0/tests/test_jwt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:23:20.895781 cuenca-1.0.1.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-30 23:23:20.895781 cuenca-1.0.1.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:23:20.875781 cuenca-1.0.1.dev1/cuenca/
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:23:20.875781 cuenca-1.0.1.dev1/cuenca/http/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:23:20.883781 cuenca-1.0.1.dev1/cuenca/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/arpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/balance_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/bill_payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/card_activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/card_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/card_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/cash_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/clabes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/commissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/curp_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/deposits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/file_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/identities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/identity_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/kyc_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/kyc_verifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/limited_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/login_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/otps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/questionnaires.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/savings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/service_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/statements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/user_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/user_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/user_lists_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/user_logins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/verifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/wallet_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/resources/whatsapp_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/cuenca/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:23:20.891781 cuenca-1.0.1.dev1/cuenca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-30 23:23:20.000000 cuenca-1.0.1.dev1/cuenca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-30 23:23:20.000000 cuenca-1.0.1.dev1/cuenca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 23:23:20.000000 cuenca-1.0.1.dev1/cuenca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 23:23:20.000000 cuenca-1.0.1.dev1/cuenca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 23:23:20.000000 cuenca-1.0.1.dev1/cuenca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-30 23:23:20.895781 cuenca-1.0.1.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:23:20.883781 cuenca-1.0.1.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:23:20.887781 cuenca-1.0.1.dev1/tests/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/http/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/http/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:23:20.891781 cuenca-1.0.1.dev1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_arpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_balance_entries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_bill_payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_card_activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_card_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_card_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_cash_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_clabes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_commissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_curp_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_deposits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_file_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_identities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_identity_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_kyc_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_kyc_verifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_limited_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_login_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_questionnaires.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_savings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_service_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_statements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_user_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_user_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_user_lists_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_user_logins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_verifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_wallet_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/resources/test_whatsapp_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/test_cuenca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-30 23:23:09.000000 cuenca-1.0.1.dev1/tests/test_jwt.py
```

### Comparing `cuenca-1.0.0/LICENSE` & `cuenca-1.0.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/PKG-INFO` & `cuenca-1.0.1.dev1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuenca
-Version: 1.0.0
+Version: 1.0.1.dev1
 Summary: Cuenca API Client
 Home-page: https://github.com/cuenca-mx/cuenca-python
 Author: Cuenca
 Author-email: dev@cuenca.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cuenca-1.0.0/README.md` & `cuenca-1.0.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/__init__.py` & `cuenca-1.0.1.dev1/cuenca/__init__.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/exc.py` & `cuenca-1.0.1.dev1/cuenca/exc.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/http/client.py` & `cuenca-1.0.1.dev1/cuenca/http/client.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/jwt.py` & `cuenca-1.0.1.dev1/cuenca/jwt.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/__init__.py` & `cuenca-1.0.1.dev1/cuenca/resources/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     'FileBatch',
     'Identity',
     'IdentityEvent',
     'KYCValidation',
     'KYCVerification',
     'LimitedWallet',
     'LoginToken',
+    'Otp',
     'Platform',
     'Questionnaires',
     'Saving',
     'ServiceProvider',
     'Session',
     'Statement',
     'Transfer',
@@ -58,14 +59,15 @@
 from .files import File
 from .identities import Identity
 from .identity_events import IdentityEvent
 from .kyc_validations import KYCValidation
 from .kyc_verifications import KYCVerification
 from .limited_wallets import LimitedWallet
 from .login_tokens import LoginToken
+from .otps import Otp
 from .platforms import Platform
 from .questionnaires import Questionnaires
 from .resources import RESOURCES
 from .savings import Saving
 from .service_providers import ServiceProvider
 from .sessions import Session
 from .statements import Statement
```

### Comparing `cuenca-1.0.0/cuenca/resources/api_keys.py` & `cuenca-1.0.1.dev1/cuenca/resources/api_keys.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/arpc.py` & `cuenca-1.0.1.dev1/cuenca/resources/arpc.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/balance_entries.py` & `cuenca-1.0.1.dev1/cuenca/resources/balance_entries.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/base.py` & `cuenca-1.0.1.dev1/cuenca/resources/base.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/bill_payments.py` & `cuenca-1.0.1.dev1/cuenca/resources/bill_payments.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/card_activations.py` & `cuenca-1.0.1.dev1/cuenca/resources/card_activations.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/card_transactions.py` & `cuenca-1.0.1.dev1/cuenca/resources/card_transactions.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/card_validations.py` & `cuenca-1.0.1.dev1/cuenca/resources/card_validations.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/cards.py` & `cuenca-1.0.1.dev1/cuenca/resources/cards.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/commissions.py` & `cuenca-1.0.1.dev1/cuenca/resources/commissions.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/curp_validations.py` & `cuenca-1.0.1.dev1/cuenca/resources/curp_validations.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/deposits.py` & `cuenca-1.0.1.dev1/cuenca/resources/deposits.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/endpoints.py` & `cuenca-1.0.1.dev1/cuenca/resources/endpoints.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/file_batches.py` & `cuenca-1.0.1.dev1/cuenca/resources/file_batches.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/files.py` & `cuenca-1.0.1.dev1/cuenca/resources/files.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/identities.py` & `cuenca-1.0.1.dev1/cuenca/resources/identities.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/kyc_validations.py` & `cuenca-1.0.1.dev1/cuenca/resources/kyc_validations.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/kyc_verifications.py` & `cuenca-1.0.1.dev1/cuenca/resources/kyc_verifications.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/limited_wallets.py` & `cuenca-1.0.1.dev1/cuenca/resources/limited_wallets.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/login_tokens.py` & `cuenca-1.0.1.dev1/cuenca/resources/login_tokens.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/platforms.py` & `cuenca-1.0.1.dev1/cuenca/resources/platforms.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/questionnaires.py` & `cuenca-1.0.1.dev1/cuenca/resources/questionnaires.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/resources.py` & `cuenca-1.0.1.dev1/cuenca/resources/resources.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/savings.py` & `cuenca-1.0.1.dev1/cuenca/resources/savings.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/sessions.py` & `cuenca-1.0.1.dev1/cuenca/resources/sessions.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/transfers.py` & `cuenca-1.0.1.dev1/cuenca/resources/transfers.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/user_credentials.py` & `cuenca-1.0.1.dev1/cuenca/resources/user_credentials.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/user_events.py` & `cuenca-1.0.1.dev1/cuenca/resources/user_events.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/user_lists_validation.py` & `cuenca-1.0.1.dev1/cuenca/resources/user_lists_validation.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/user_logins.py` & `cuenca-1.0.1.dev1/cuenca/resources/user_logins.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/users.py` & `cuenca-1.0.1.dev1/cuenca/resources/users.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/verifications.py` & `cuenca-1.0.1.dev1/cuenca/resources/verifications.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/wallet_transactions.py` & `cuenca-1.0.1.dev1/cuenca/resources/wallet_transactions.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca/resources/whatsapp_transfers.py` & `cuenca-1.0.1.dev1/cuenca/resources/whatsapp_transfers.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/cuenca.egg-info/PKG-INFO` & `cuenca-1.0.1.dev1/cuenca.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuenca
-Version: 1.0.0
+Version: 1.0.1.dev1
 Summary: Cuenca API Client
 Home-page: https://github.com/cuenca-mx/cuenca-python
 Author: Cuenca
 Author-email: dev@cuenca.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cuenca-1.0.0/cuenca.egg-info/SOURCES.txt` & `cuenca-1.0.1.dev1/cuenca.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 cuenca/resources/files.py
 cuenca/resources/identities.py
 cuenca/resources/identity_events.py
 cuenca/resources/kyc_validations.py
 cuenca/resources/kyc_verifications.py
 cuenca/resources/limited_wallets.py
 cuenca/resources/login_tokens.py
+cuenca/resources/otps.py
 cuenca/resources/platforms.py
 cuenca/resources/questionnaires.py
 cuenca/resources/resources.py
 cuenca/resources/savings.py
 cuenca/resources/service_providers.py
 cuenca/resources/sessions.py
 cuenca/resources/statements.py
```

### Comparing `cuenca-1.0.0/setup.py` & `cuenca-1.0.1.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/conftest.py` & `cuenca-1.0.1.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/http/test_client.py` & `cuenca-1.0.1.dev1/tests/http/test_client.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_api_keys.py` & `cuenca-1.0.1.dev1/tests/resources/test_api_keys.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_balance_entries.py` & `cuenca-1.0.1.dev1/tests/resources/test_balance_entries.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_card_activations.py` & `cuenca-1.0.1.dev1/tests/resources/test_card_activations.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_card_transactions.py` & `cuenca-1.0.1.dev1/tests/resources/test_card_transactions.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_card_validations.py` & `cuenca-1.0.1.dev1/tests/resources/test_card_validations.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_cards.py` & `cuenca-1.0.1.dev1/tests/resources/test_cards.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_commissions.py` & `cuenca-1.0.1.dev1/tests/resources/test_commissions.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_curp_validations.py` & `cuenca-1.0.1.dev1/tests/resources/test_curp_validations.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_endpoints.py` & `cuenca-1.0.1.dev1/tests/resources/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_file_batches.py` & `cuenca-1.0.1.dev1/tests/resources/test_file_batches.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_files.py` & `cuenca-1.0.1.dev1/tests/resources/test_files.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_kyc_verifications.py` & `cuenca-1.0.1.dev1/tests/resources/test_kyc_verifications.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_limited_wallets.py` & `cuenca-1.0.1.dev1/tests/resources/test_limited_wallets.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_login_tokens.py` & `cuenca-1.0.1.dev1/tests/resources/test_login_tokens.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_savings.py` & `cuenca-1.0.1.dev1/tests/resources/test_savings.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_service_providers.py` & `cuenca-1.0.1.dev1/tests/resources/test_service_providers.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_sessions.py` & `cuenca-1.0.1.dev1/tests/resources/test_sessions.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_transfers.py` & `cuenca-1.0.1.dev1/tests/resources/test_transfers.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_user_credentials.py` & `cuenca-1.0.1.dev1/tests/resources/test_user_credentials.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_user_lists_validation.py` & `cuenca-1.0.1.dev1/tests/resources/test_user_lists_validation.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_user_logins.py` & `cuenca-1.0.1.dev1/tests/resources/test_user_logins.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_users.py` & `cuenca-1.0.1.dev1/tests/resources/test_users.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_verifications.py` & `cuenca-1.0.1.dev1/tests/resources/test_verifications.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_wallet_transactions.py` & `cuenca-1.0.1.dev1/tests/resources/test_wallet_transactions.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/resources/test_whatsapp_transfers.py` & `cuenca-1.0.1.dev1/tests/resources/test_whatsapp_transfers.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/test_cuenca.py` & `cuenca-1.0.1.dev1/tests/test_cuenca.py`

 * *Files identical despite different names*

### Comparing `cuenca-1.0.0/tests/test_jwt.py` & `cuenca-1.0.1.dev1/tests/test_jwt.py`

 * *Files identical despite different names*

