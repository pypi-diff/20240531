# Comparing `tmp/xchainpy2-mayanode-1.108.1.tar.gz` & `tmp/xchainpy2_mayanode-1.109.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchainpy2-mayanode-1.108.1.tar", last modified: Sun Jan 21 10:17:41 2024, max compression
+gzip compressed data, was "xchainpy2_mayanode-1.109.0.tar", last modified: Fri May 31 12:55:14 2024, max compression
```

## Comparing `xchainpy2-mayanode-1.108.1.tar` & `xchainpy2_mayanode-1.109.0.tar`

### file list

```diff
@@ -1,187 +1,203 @@
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-21 10:17:41.544716 xchainpy2-mayanode-1.108.1/
--rw-r--r--   0 tirinox    (501) staff       (20)     2124 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/LICENSE
--rw-r--r--   0 tirinox    (501) staff       (20)     9116 2024-01-21 10:17:41.544223 xchainpy2-mayanode-1.108.1/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)     8760 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/README.md
--rw-r--r--   0 tirinox    (501) staff       (20)       38 2024-01-21 10:17:41.544777 xchainpy2-mayanode-1.108.1/setup.cfg
--rw-r--r--   0 tirinox    (501) staff       (20)     1270 2024-01-21 10:16:24.000000 xchainpy2-mayanode-1.108.1/setup.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-21 10:17:41.517696 xchainpy2-mayanode-1.108.1/test/
--rw-r--r--   0 tirinox    (501) staff       (20)       15 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/test/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_ban_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_chain_height.py
--rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_coin.py
--rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_constants_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      733 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_health_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_inbound_address.py
--rw-r--r--   0 tirinox    (501) staff       (20)      977 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_inbound_addresses_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_keygen_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_keygen_metric1.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_keygen_metric2.py
--rw-r--r--   0 tirinox    (501) staff       (20)      953 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_keygen_metrics_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_keysign_info.py
--rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_keysign_metrics.py
--rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_keysign_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_last_block.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_last_block_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_liquidity_provider.py
--rw-r--r--   0 tirinox    (501) staff       (20)      985 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_liquidity_provider_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      977 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_liquidity_provider_summary.py
--rw-r--r--   0 tirinox    (501) staff       (20)      934 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/test/test_liquidity_providers_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      993 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_liquidity_providers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      881 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_lp_bonded_node.py
--rw-r--r--   0 tirinox    (501) staff       (20)      845 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_mayaname.py
--rw-r--r--   0 tirinox    (501) staff       (20)      853 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_mayaname1.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_mayaname_alias.py
--rw-r--r--   0 tirinox    (501) staff       (20)      911 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_mayaname_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      756 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/test/test_mayanames_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_metrics_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1108 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/test/test_mimir_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      929 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_mimir_nodes_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_mimir_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_mimir_vote.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1398 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/test/test_network_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_network_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_node.py
--rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_node_bond_provider.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_node_bond_providers.py
--rw-r--r--   0 tirinox    (501) staff       (20)      847 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_node_jail.py
--rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_node_keygen_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)      937 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_node_preflight_status.py
--rw-r--r--   0 tirinox    (501) staff       (20)      891 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_node_pub_key_set.py
--rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_node_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      812 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/test/test_nodes_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_nodes_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      863 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_observed_tx.py
--rw-r--r--   0 tirinox    (501) staff       (20)      911 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_outbound_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_ping.py
--rw-r--r--   0 tirinox    (501) staff       (20)      716 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/test/test_pol_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_pol_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_pool_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      812 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/test/test_pools_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_pools_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      936 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/test/test_queue_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_queue_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      956 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/test/test_quote_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_quote_fees.py
--rw-r--r--   0 tirinox    (501) staff       (20)      987 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_quote_saver_deposit_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      995 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_quote_saver_withdraw_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_quote_swap_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      821 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_saver.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_saver_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      821 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/test/test_savers_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_savers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_scheduled_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      853 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/test/test_transactions_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1016 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/test/test_tss_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_tss_keysign_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_tss_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)      797 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_tx.py
--rw-r--r--   0 tirinox    (501) staff       (20)      857 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_tx_out_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)      863 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_tx_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_tx_signers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      821 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_vault.py
--rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_vault_address.py
--rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_vault_info.py
--rw-r--r--   0 tirinox    (501) staff       (20)      945 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_vault_pubkeys_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_vault_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_vault_router.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1013 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/test/test_vaults_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_vaults_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/test/test_version_response.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-21 10:17:41.519068 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/
--rw-r--r--   0 tirinox    (501) staff       (20)     5906 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-21 10:17:41.524700 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/
--rw-r--r--   0 tirinox    (501) staff       (20)      894 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3591 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/health_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     9189 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/liquidity_providers_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4584 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/mayanames_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    18390 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/mimir_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    28645 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/network_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7800 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/nodes_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4014 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/pol_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7738 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/pools_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    10740 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/queue_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14188 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/quote_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     8757 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/savers_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     8325 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/transactions_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    16122 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/tss_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14408 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/vaults_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    25046 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api_client.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7927 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/configuration.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-21 10:17:41.543382 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/
--rw-r--r--   0 tirinox    (501) staff       (20)     4939 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4499 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/ban_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3757 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/chain_height.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4298 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/coin.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4796 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/constants_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14028 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/inbound_address.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2436 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/inbound_addresses_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3950 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/keygen_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3962 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/keygen_metric1.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3932 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/keygen_metric2.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2424 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/keygen_metrics_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4071 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/keysign_info.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3820 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/keysign_metrics.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3760 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/keysign_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5575 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/last_block.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2408 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/last_block_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    20146 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/liquidity_provider.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2440 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/liquidity_provider_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    11875 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/liquidity_provider_summary.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2444 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/liquidity_providers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3895 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/lp_bonded_node.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6003 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/mayaname.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5014 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/mayaname1.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3632 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/mayaname_alias.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2404 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/mayaname_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3763 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/metrics_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3087 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/mimir_nodes_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2628 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/mimir_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4109 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/mimir_vote.py
--rw-r--r--   0 tirinox    (501) staff       (20)     9627 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/network_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    21860 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/node.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3748 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/node_bond_provider.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4756 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/node_bond_providers.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4453 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/node_jail.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3728 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/node_keygen_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4804 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/node_preflight_status.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3712 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/node_pub_key_set.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2388 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/node_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/nodes_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    11685 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/observed_tx.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2404 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/outbound_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2899 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/ping.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7017 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/pol_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14372 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2388 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/pool_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/pools_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5872 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/queue_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4528 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/quote_fees.py
--rw-r--r--   0 tirinox    (501) staff       (20)     9900 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/quote_saver_deposit_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    11158 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/quote_saver_withdraw_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    11998 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/quote_swap_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     8754 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/saver.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/saver_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2396 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/savers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2408 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/scheduled_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3937 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/tss_keysign_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3644 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/tss_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6573 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/tx.py
--rw-r--r--   0 tirinox    (501) staff       (20)     9115 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/tx_out_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3916 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/tx_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     9832 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/tx_signers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    12631 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/vault.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3620 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/vault_address.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3838 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/vault_info.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4021 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/vault_pubkeys_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/vault_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3588 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/vault_router.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2396 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/vaults_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4762 2024-01-21 10:11:43.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/version_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    10622 2024-01-21 10:11:44.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/rest.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-21 10:17:41.543756 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode.egg-info/
--rw-r--r--   0 tirinox    (501) staff       (20)     9116 2024-01-21 10:17:41.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode.egg-info/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)     6316 2024-01-21 10:17:41.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode.egg-info/SOURCES.txt
--rw-r--r--   0 tirinox    (501) staff       (20)        1 2024-01-21 10:17:41.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode.egg-info/dependency_links.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       56 2024-01-21 10:17:41.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode.egg-info/requires.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       24 2024-01-21 10:17:41.000000 xchainpy2-mayanode-1.108.1/xchainpy2_mayanode.egg-info/top_level.txt
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 12:55:14.086321 xchainpy2_mayanode-1.109.0/
+-rw-r--r--   0 tirinox    (501) staff       (20)     2124 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/LICENSE
+-rw-r--r--   0 tirinox    (501) staff       (20)     9504 2024-05-31 12:55:14.086030 xchainpy2_mayanode-1.109.0/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)     9148 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/README.md
+-rw-r--r--   0 tirinox    (501) staff       (20)       38 2024-05-31 12:55:14.086353 xchainpy2_mayanode-1.109.0/setup.cfg
+-rw-r--r--   0 tirinox    (501) staff       (20)     1270 2024-05-31 12:53:48.000000 xchainpy2_mayanode-1.109.0/setup.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 12:55:14.070291 xchainpy2_mayanode-1.109.0/test/
+-rw-r--r--   0 tirinox    (501) staff       (20)       15 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/test/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_ban_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_base_quote_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_block_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      937 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_block_response_header.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      995 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_block_response_header_version.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      905 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_block_response_id.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      947 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_block_response_id_parts.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      839 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_block_tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      889 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_block_tx_result.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_chain_height.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_coin.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_constants_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      733 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/test/test_health_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_inbound_address.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      977 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_inbound_addresses_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_keygen_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_keygen_metric1.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_keygen_metric2.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      953 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_keygen_metrics_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_keysign_info.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_keysign_metrics.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_keysign_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_last_block.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_last_block_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_liquidity_provider.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      985 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_liquidity_provider_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      977 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_liquidity_provider_summary.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      934 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/test/test_liquidity_providers_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      993 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_liquidity_providers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      881 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_lp_bonded_node.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      845 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_mayaname.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      853 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_mayaname1.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_mayaname_alias.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      911 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_mayaname_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      756 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/test/test_mayanames_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_metrics_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1108 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/test/test_mimir_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      929 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_mimir_nodes_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_mimir_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_mimir_vote.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1398 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/test/test_network_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_network_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_node.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_node_bond_provider.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_node_bond_providers.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      847 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_node_jail.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_node_keygen_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      937 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_node_preflight_status.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      891 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_node_pub_key_set.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_node_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      812 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/test/test_nodes_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_nodes_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      863 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_observed_tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      911 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_outbound_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_ping.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      716 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/test/test_pol_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_pol_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_pool_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      812 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/test/test_pools_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_pools_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      936 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/test/test_queue_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_queue_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      956 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/test/test_quote_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_quote_fees.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      987 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_quote_saver_deposit_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      995 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_quote_saver_withdraw_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_quote_swap_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      821 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_saver.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_saver_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      821 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/test/test_savers_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_savers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_scheduled_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      853 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/test/test_transactions_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1016 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/test/test_tss_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_tss_keysign_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_tss_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      797 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      857 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_tx_out_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      863 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_tx_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_tx_signers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      821 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_vault.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_vault_address.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_vault_info.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      945 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_vault_pubkeys_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_vault_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_vault_router.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1013 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/test/test_vaults_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_vaults_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/test/test_version_response.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 12:55:14.070917 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/
+-rw-r--r--   0 tirinox    (501) staff       (20)     6502 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 12:55:14.074020 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/
+-rw-r--r--   0 tirinox    (501) staff       (20)      894 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3591 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/health_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     9228 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/liquidity_providers_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4584 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/mayanames_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    18390 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/mimir_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    28645 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/network_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7800 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/nodes_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4014 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/pol_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7738 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/pools_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    10740 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/queue_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14188 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/quote_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8757 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/savers_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8325 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/transactions_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    16122 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/tss_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14408 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/vaults_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    25046 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api_client.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8023 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/configuration.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 12:55:14.085491 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/
+-rw-r--r--   0 tirinox    (501) staff       (20)     5535 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4499 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/ban_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    15121 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/base_quote_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6451 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/block_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14461 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/block_response_header.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3874 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/block_response_header_version.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3814 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/block_response_id.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3823 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/block_response_id_parts.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4358 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/block_tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7409 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/block_tx_result.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3757 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/chain_height.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4298 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/coin.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4796 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/constants_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14028 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/inbound_address.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2436 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/inbound_addresses_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3950 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/keygen_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3962 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/keygen_metric1.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3932 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/keygen_metric2.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2424 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/keygen_metrics_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4071 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/keysign_info.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3820 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/keysign_metrics.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3760 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/keysign_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5575 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/last_block.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2408 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/last_block_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    20146 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/liquidity_provider.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2440 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/liquidity_provider_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    11875 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/liquidity_provider_summary.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2444 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/liquidity_providers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3895 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/lp_bonded_node.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6003 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/mayaname.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5014 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/mayaname1.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3632 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/mayaname_alias.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2404 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/mayaname_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3763 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/metrics_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3087 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/mimir_nodes_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2628 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/mimir_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4109 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/mimir_vote.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     9627 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/network_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    21860 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/node.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3748 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/node_bond_provider.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4756 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/node_bond_providers.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4453 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/node_jail.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3728 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/node_keygen_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4804 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/node_preflight_status.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3712 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/node_pub_key_set.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2388 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/node_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/nodes_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    11685 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/observed_tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2404 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/outbound_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2899 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/ping.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7017 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/pol_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14372 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2388 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/pool_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/pools_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5872 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/queue_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8184 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/quote_fees.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    19358 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/quote_saver_deposit_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    19693 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/quote_saver_withdraw_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    17633 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/quote_swap_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8754 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/saver.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/saver_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2396 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/savers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2408 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/scheduled_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3937 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/tss_keysign_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3644 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/tss_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6573 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     9115 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/tx_out_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3916 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/tx_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     9832 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/tx_signers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    12631 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/vault.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3620 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/vault_address.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3838 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/vault_info.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4021 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/vault_pubkeys_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/vault_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3588 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/vault_router.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2396 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/vaults_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4762 2024-05-31 12:53:22.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/version_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    10622 2024-05-31 12:53:23.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/rest.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 12:55:14.085722 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode.egg-info/
+-rw-r--r--   0 tirinox    (501) staff       (20)     9504 2024-05-31 12:55:14.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode.egg-info/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)     6960 2024-05-31 12:55:14.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode.egg-info/SOURCES.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)        1 2024-05-31 12:55:14.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode.egg-info/dependency_links.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       56 2024-05-31 12:55:14.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode.egg-info/requires.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       24 2024-05-31 12:55:14.000000 xchainpy2_mayanode-1.109.0/xchainpy2_mayanode.egg-info/top_level.txt
```

### Comparing `xchainpy2-mayanode-1.108.1/LICENSE` & `xchainpy2_mayanode-1.109.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Tirinox (aka TRX1 aka account1242 aka Old1)
+Copyright (c) 2024 Tirinox (aka TRX1 aka account1242 aka Old1)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `xchainpy2-mayanode-1.108.1/PKG-INFO` & `xchainpy2_mayanode-1.109.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2-mayanode
-Version: 1.108.1
+Version: 1.109.0
 Summary: Mayanode API
 Home-page: 
 Author-email: devs@mayachain.org
 Keywords: Swagger,Mayanode API
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urllib3>=1.15
@@ -14,16 +14,16 @@
 Requires-Dist: aiohttp
 
 # xchainpy2-mayanode
 Mayanode REST API.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.108.1
-- Package version: 1.107.3
+- API version: 1.109.0
+- Package version: 1.109.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -122,14 +122,22 @@
 *VaultsApi* | [**vault**](docs/VaultsApi.md#vault) | **GET** /mayachain/vaults/{pubkey} | 
 *VaultsApi* | [**vault_pubkeys**](docs/VaultsApi.md#vault_pubkeys) | **GET** /mayachain/vaults/pubkeys | 
 *VaultsApi* | [**yggdrasil**](docs/VaultsApi.md#yggdrasil) | **GET** /mayachain/vaults/yggdrasil | 
 
 ## Documentation For Models
 
  - [BanResponse](docs/BanResponse.md)
+ - [BaseQuoteResponse](docs/BaseQuoteResponse.md)
+ - [BlockResponse](docs/BlockResponse.md)
+ - [BlockResponseHeader](docs/BlockResponseHeader.md)
+ - [BlockResponseHeaderVersion](docs/BlockResponseHeaderVersion.md)
+ - [BlockResponseId](docs/BlockResponseId.md)
+ - [BlockResponseIdParts](docs/BlockResponseIdParts.md)
+ - [BlockTx](docs/BlockTx.md)
+ - [BlockTxResult](docs/BlockTxResult.md)
  - [ChainHeight](docs/ChainHeight.md)
  - [Coin](docs/Coin.md)
  - [ConstantsResponse](docs/ConstantsResponse.md)
  - [InboundAddress](docs/InboundAddress.md)
  - [InboundAddressesResponse](docs/InboundAddressesResponse.md)
  - [KeygenMetric](docs/KeygenMetric.md)
  - [KeygenMetric1](docs/KeygenMetric1.md)
```

### Comparing `xchainpy2-mayanode-1.108.1/README.md` & `xchainpy2_mayanode-1.109.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # xchainpy2-mayanode
 Mayanode REST API.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.108.1
-- Package version: 1.107.3
+- API version: 1.109.0
+- Package version: 1.109.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -107,14 +107,22 @@
 *VaultsApi* | [**vault**](docs/VaultsApi.md#vault) | **GET** /mayachain/vaults/{pubkey} | 
 *VaultsApi* | [**vault_pubkeys**](docs/VaultsApi.md#vault_pubkeys) | **GET** /mayachain/vaults/pubkeys | 
 *VaultsApi* | [**yggdrasil**](docs/VaultsApi.md#yggdrasil) | **GET** /mayachain/vaults/yggdrasil | 
 
 ## Documentation For Models
 
  - [BanResponse](docs/BanResponse.md)
+ - [BaseQuoteResponse](docs/BaseQuoteResponse.md)
+ - [BlockResponse](docs/BlockResponse.md)
+ - [BlockResponseHeader](docs/BlockResponseHeader.md)
+ - [BlockResponseHeaderVersion](docs/BlockResponseHeaderVersion.md)
+ - [BlockResponseId](docs/BlockResponseId.md)
+ - [BlockResponseIdParts](docs/BlockResponseIdParts.md)
+ - [BlockTx](docs/BlockTx.md)
+ - [BlockTxResult](docs/BlockTxResult.md)
  - [ChainHeight](docs/ChainHeight.md)
  - [Coin](docs/Coin.md)
  - [ConstantsResponse](docs/ConstantsResponse.md)
  - [InboundAddress](docs/InboundAddress.md)
  - [InboundAddressesResponse](docs/InboundAddressesResponse.md)
  - [KeygenMetric](docs/KeygenMetric.md)
  - [KeygenMetric1](docs/KeygenMetric1.md)
```

### Comparing `xchainpy2-mayanode-1.108.1/setup.py` & `xchainpy2_mayanode-1.109.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "xchainpy2-mayanode"
-VERSION = "1.108.1"
+VERSION = "1.109.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_ban_response.py` & `xchainpy2_mayanode-1.109.0/test/test_vault_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_mayanode
-from xchainpy2_mayanode.models.ban_response import BanResponse  # noqa: E501
+from xchainpy2_mayanode.models.vault_response import VaultResponse  # noqa: E501
 from xchainpy2_mayanode.rest import ApiException
 
 
-class TestBanResponse(unittest.TestCase):
-    """BanResponse unit test stubs"""
+class TestVaultResponse(unittest.TestCase):
+    """VaultResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBanResponse(self):
-        """Test BanResponse"""
+    def testVaultResponse(self):
+        """Test VaultResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_mayanode.models.ban_response.BanResponse()  # noqa: E501
+        # model = xchainpy2_mayanode.models.vault_response.VaultResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_chain_height.py` & `xchainpy2_mayanode-1.109.0/test/test_chain_height.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_coin.py` & `xchainpy2_mayanode-1.109.0/test/test_coin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_constants_response.py` & `xchainpy2_mayanode-1.109.0/test/test_constants_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_health_api.py` & `xchainpy2_mayanode-1.109.0/test/test_health_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_inbound_address.py` & `xchainpy2_mayanode-1.109.0/test/test_inbound_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_inbound_addresses_response.py` & `xchainpy2_mayanode-1.109.0/test/test_inbound_addresses_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_keygen_metric.py` & `xchainpy2_mayanode-1.109.0/test/test_keygen_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_keygen_metric1.py` & `xchainpy2_mayanode-1.109.0/test/test_keygen_metric1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_keygen_metric2.py` & `xchainpy2_mayanode-1.109.0/test/test_keygen_metric2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_keygen_metrics_response.py` & `xchainpy2_mayanode-1.109.0/test/test_keygen_metrics_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_keysign_info.py` & `xchainpy2_mayanode-1.109.0/test/test_keysign_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_keysign_metrics.py` & `xchainpy2_mayanode-1.109.0/test/test_keysign_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_keysign_response.py` & `xchainpy2_mayanode-1.109.0/test/test_ban_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_mayanode
-from xchainpy2_mayanode.models.keysign_response import KeysignResponse  # noqa: E501
+from xchainpy2_mayanode.models.ban_response import BanResponse  # noqa: E501
 from xchainpy2_mayanode.rest import ApiException
 
 
-class TestKeysignResponse(unittest.TestCase):
-    """KeysignResponse unit test stubs"""
+class TestBanResponse(unittest.TestCase):
+    """BanResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testKeysignResponse(self):
-        """Test KeysignResponse"""
+    def testBanResponse(self):
+        """Test BanResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_mayanode.models.keysign_response.KeysignResponse()  # noqa: E501
+        # model = xchainpy2_mayanode.models.ban_response.BanResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_last_block.py` & `xchainpy2_mayanode-1.109.0/test/test_pool.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_mayanode
-from xchainpy2_mayanode.models.last_block import LastBlock  # noqa: E501
+from xchainpy2_mayanode.models.pool import Pool  # noqa: E501
 from xchainpy2_mayanode.rest import ApiException
 
 
-class TestLastBlock(unittest.TestCase):
-    """LastBlock unit test stubs"""
+class TestPool(unittest.TestCase):
+    """Pool unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testLastBlock(self):
-        """Test LastBlock"""
+    def testPool(self):
+        """Test Pool"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_mayanode.models.last_block.LastBlock()  # noqa: E501
+        # model = xchainpy2_mayanode.models.pool.Pool()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_last_block_response.py` & `xchainpy2_mayanode-1.109.0/test/test_last_block_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_liquidity_provider.py` & `xchainpy2_mayanode-1.109.0/test/test_liquidity_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_liquidity_provider_response.py` & `xchainpy2_mayanode-1.109.0/test/test_liquidity_provider_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_liquidity_provider_summary.py` & `xchainpy2_mayanode-1.109.0/test/test_liquidity_provider_summary.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_liquidity_providers_api.py` & `xchainpy2_mayanode-1.109.0/test/test_liquidity_providers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_liquidity_providers_response.py` & `xchainpy2_mayanode-1.109.0/test/test_liquidity_providers_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_lp_bonded_node.py` & `xchainpy2_mayanode-1.109.0/test/test_lp_bonded_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_mayaname.py` & `xchainpy2_mayanode-1.109.0/test/test_mayaname.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_mayaname1.py` & `xchainpy2_mayanode-1.109.0/test/test_mayaname1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_mayaname_alias.py` & `xchainpy2_mayanode-1.109.0/test/test_mayaname_alias.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_mayaname_response.py` & `xchainpy2_mayanode-1.109.0/test/test_mayaname_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_mayanames_api.py` & `xchainpy2_mayanode-1.109.0/test/test_mayanames_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_metrics_response.py` & `xchainpy2_mayanode-1.109.0/test/test_metrics_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_mimir_api.py` & `xchainpy2_mayanode-1.109.0/test/test_mimir_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_mimir_nodes_response.py` & `xchainpy2_mayanode-1.109.0/test/test_mimir_nodes_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_mimir_response.py` & `xchainpy2_mayanode-1.109.0/test/test_mimir_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_mimir_vote.py` & `xchainpy2_mayanode-1.109.0/test/test_mimir_vote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_network_api.py` & `xchainpy2_mayanode-1.109.0/test/test_network_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_network_response.py` & `xchainpy2_mayanode-1.109.0/test/test_network_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_node.py` & `xchainpy2_mayanode-1.109.0/test/test_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_node_bond_provider.py` & `xchainpy2_mayanode-1.109.0/test/test_node_bond_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_node_bond_providers.py` & `xchainpy2_mayanode-1.109.0/test/test_node_bond_providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_node_jail.py` & `xchainpy2_mayanode-1.109.0/test/test_node_jail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_node_keygen_metric.py` & `xchainpy2_mayanode-1.109.0/test/test_node_keygen_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_node_preflight_status.py` & `xchainpy2_mayanode-1.109.0/test/test_node_preflight_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_node_pub_key_set.py` & `xchainpy2_mayanode-1.109.0/test/test_node_pub_key_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_node_response.py` & `xchainpy2_mayanode-1.109.0/test/test_node_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_nodes_api.py` & `xchainpy2_mayanode-1.109.0/test/test_nodes_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_nodes_response.py` & `xchainpy2_mayanode-1.109.0/test/test_nodes_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_observed_tx.py` & `xchainpy2_mayanode-1.109.0/test/test_observed_tx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_outbound_response.py` & `xchainpy2_mayanode-1.109.0/test/test_outbound_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_ping.py` & `xchainpy2_mayanode-1.109.0/test/test_ping.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_pol_api.py` & `xchainpy2_mayanode-1.109.0/test/test_pol_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_pol_response.py` & `xchainpy2_mayanode-1.109.0/test/test_pol_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_pool.py` & `xchainpy2_mayanode-1.109.0/test/test_vault.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_mayanode
-from xchainpy2_mayanode.models.pool import Pool  # noqa: E501
+from xchainpy2_mayanode.models.vault import Vault  # noqa: E501
 from xchainpy2_mayanode.rest import ApiException
 
 
-class TestPool(unittest.TestCase):
-    """Pool unit test stubs"""
+class TestVault(unittest.TestCase):
+    """Vault unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPool(self):
-        """Test Pool"""
+    def testVault(self):
+        """Test Vault"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_mayanode.models.pool.Pool()  # noqa: E501
+        # model = xchainpy2_mayanode.models.vault.Vault()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_pool_response.py` & `xchainpy2_mayanode-1.109.0/test/test_pool_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_pools_api.py` & `xchainpy2_mayanode-1.109.0/test/test_pools_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_pools_response.py` & `xchainpy2_mayanode-1.109.0/test/test_pools_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_queue_api.py` & `xchainpy2_mayanode-1.109.0/test/test_queue_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_queue_response.py` & `xchainpy2_mayanode-1.109.0/test/test_tx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_mayanode
-from xchainpy2_mayanode.models.queue_response import QueueResponse  # noqa: E501
+from xchainpy2_mayanode.models.tx import Tx  # noqa: E501
 from xchainpy2_mayanode.rest import ApiException
 
 
-class TestQueueResponse(unittest.TestCase):
-    """QueueResponse unit test stubs"""
+class TestTx(unittest.TestCase):
+    """Tx unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testQueueResponse(self):
-        """Test QueueResponse"""
+    def testTx(self):
+        """Test Tx"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_mayanode.models.queue_response.QueueResponse()  # noqa: E501
+        # model = xchainpy2_mayanode.models.tx.Tx()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_quote_api.py` & `xchainpy2_mayanode-1.109.0/test/test_quote_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_quote_fees.py` & `xchainpy2_mayanode-1.109.0/test/test_quote_fees.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_quote_saver_deposit_response.py` & `xchainpy2_mayanode-1.109.0/test/test_quote_saver_deposit_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_quote_saver_withdraw_response.py` & `xchainpy2_mayanode-1.109.0/test/test_quote_saver_withdraw_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_quote_swap_response.py` & `xchainpy2_mayanode-1.109.0/test/test_quote_swap_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_saver.py` & `xchainpy2_mayanode-1.109.0/test/test_saver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_saver_response.py` & `xchainpy2_mayanode-1.109.0/test/test_saver_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_savers_api.py` & `xchainpy2_mayanode-1.109.0/test/test_savers_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_savers_response.py` & `xchainpy2_mayanode-1.109.0/test/test_savers_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_scheduled_response.py` & `xchainpy2_mayanode-1.109.0/test/test_scheduled_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_transactions_api.py` & `xchainpy2_mayanode-1.109.0/test/test_transactions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_tss_api.py` & `xchainpy2_mayanode-1.109.0/test/test_tss_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_tss_keysign_metric.py` & `xchainpy2_mayanode-1.109.0/test/test_tss_keysign_metric.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_tss_metric.py` & `xchainpy2_mayanode-1.109.0/test/test_tss_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_tx.py` & `xchainpy2_mayanode-1.109.0/test/test_block_tx.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_mayanode
-from xchainpy2_mayanode.models.tx import Tx  # noqa: E501
+from xchainpy2_mayanode.models.block_tx import BlockTx  # noqa: E501
 from xchainpy2_mayanode.rest import ApiException
 
 
-class TestTx(unittest.TestCase):
-    """Tx unit test stubs"""
+class TestBlockTx(unittest.TestCase):
+    """BlockTx unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTx(self):
-        """Test Tx"""
+    def testBlockTx(self):
+        """Test BlockTx"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_mayanode.models.tx.Tx()  # noqa: E501
+        # model = xchainpy2_mayanode.models.block_tx.BlockTx()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_tx_out_item.py` & `xchainpy2_mayanode-1.109.0/test/test_tx_out_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_tx_response.py` & `xchainpy2_mayanode-1.109.0/test/test_tx_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_tx_signers_response.py` & `xchainpy2_mayanode-1.109.0/test/test_tx_signers_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_vault.py` & `xchainpy2_mayanode-1.109.0/test/test_block_tx_result.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_mayanode
-from xchainpy2_mayanode.models.vault import Vault  # noqa: E501
+from xchainpy2_mayanode.models.block_tx_result import BlockTxResult  # noqa: E501
 from xchainpy2_mayanode.rest import ApiException
 
 
-class TestVault(unittest.TestCase):
-    """Vault unit test stubs"""
+class TestBlockTxResult(unittest.TestCase):
+    """BlockTxResult unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testVault(self):
-        """Test Vault"""
+    def testBlockTxResult(self):
+        """Test BlockTxResult"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_mayanode.models.vault.Vault()  # noqa: E501
+        # model = xchainpy2_mayanode.models.block_tx_result.BlockTxResult()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_vault_address.py` & `xchainpy2_mayanode-1.109.0/test/test_vault_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_vault_info.py` & `xchainpy2_mayanode-1.109.0/test/test_block_response_id.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_mayanode
-from xchainpy2_mayanode.models.vault_info import VaultInfo  # noqa: E501
+from xchainpy2_mayanode.models.block_response_id import BlockResponseId  # noqa: E501
 from xchainpy2_mayanode.rest import ApiException
 
 
-class TestVaultInfo(unittest.TestCase):
-    """VaultInfo unit test stubs"""
+class TestBlockResponseId(unittest.TestCase):
+    """BlockResponseId unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testVaultInfo(self):
-        """Test VaultInfo"""
+    def testBlockResponseId(self):
+        """Test BlockResponseId"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_mayanode.models.vault_info.VaultInfo()  # noqa: E501
+        # model = xchainpy2_mayanode.models.block_response_id.BlockResponseId()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_vault_pubkeys_response.py` & `xchainpy2_mayanode-1.109.0/test/test_vault_pubkeys_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_vault_response.py` & `xchainpy2_mayanode-1.109.0/test/test_vaults_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_mayanode
-from xchainpy2_mayanode.models.vault_response import VaultResponse  # noqa: E501
+from xchainpy2_mayanode.models.vaults_response import VaultsResponse  # noqa: E501
 from xchainpy2_mayanode.rest import ApiException
 
 
-class TestVaultResponse(unittest.TestCase):
-    """VaultResponse unit test stubs"""
+class TestVaultsResponse(unittest.TestCase):
+    """VaultsResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testVaultResponse(self):
-        """Test VaultResponse"""
+    def testVaultsResponse(self):
+        """Test VaultsResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_mayanode.models.vault_response.VaultResponse()  # noqa: E501
+        # model = xchainpy2_mayanode.models.vaults_response.VaultsResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_vault_router.py` & `xchainpy2_mayanode-1.109.0/test/test_version_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_mayanode
-from xchainpy2_mayanode.models.vault_router import VaultRouter  # noqa: E501
+from xchainpy2_mayanode.models.version_response import VersionResponse  # noqa: E501
 from xchainpy2_mayanode.rest import ApiException
 
 
-class TestVaultRouter(unittest.TestCase):
-    """VaultRouter unit test stubs"""
+class TestVersionResponse(unittest.TestCase):
+    """VersionResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testVaultRouter(self):
-        """Test VaultRouter"""
+    def testVersionResponse(self):
+        """Test VersionResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_mayanode.models.vault_router.VaultRouter()  # noqa: E501
+        # model = xchainpy2_mayanode.models.version_response.VersionResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_vaults_api.py` & `xchainpy2_mayanode-1.109.0/test/test_vaults_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_vaults_response.py` & `xchainpy2_mayanode-1.109.0/test/test_block_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_mayanode
-from xchainpy2_mayanode.models.vaults_response import VaultsResponse  # noqa: E501
+from xchainpy2_mayanode.models.block_response import BlockResponse  # noqa: E501
 from xchainpy2_mayanode.rest import ApiException
 
 
-class TestVaultsResponse(unittest.TestCase):
-    """VaultsResponse unit test stubs"""
+class TestBlockResponse(unittest.TestCase):
+    """BlockResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testVaultsResponse(self):
-        """Test VaultsResponse"""
+    def testBlockResponse(self):
+        """Test BlockResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_mayanode.models.vaults_response.VaultsResponse()  # noqa: E501
+        # model = xchainpy2_mayanode.models.block_response.BlockResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-mayanode-1.108.1/test/test_version_response.py` & `xchainpy2_mayanode-1.109.0/test/test_keysign_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_mayanode
-from xchainpy2_mayanode.models.version_response import VersionResponse  # noqa: E501
+from xchainpy2_mayanode.models.keysign_response import KeysignResponse  # noqa: E501
 from xchainpy2_mayanode.rest import ApiException
 
 
-class TestVersionResponse(unittest.TestCase):
-    """VersionResponse unit test stubs"""
+class TestKeysignResponse(unittest.TestCase):
+    """KeysignResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testVersionResponse(self):
-        """Test VersionResponse"""
+    def testKeysignResponse(self):
+        """Test KeysignResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_mayanode.models.version_response.VersionResponse()  # noqa: E501
+        # model = xchainpy2_mayanode.models.keysign_response.KeysignResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/__init__.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import apis into sdk package
@@ -30,14 +30,22 @@
 from xchainpy2_mayanode.api.transactions_api import TransactionsApi
 from xchainpy2_mayanode.api.vaults_api import VaultsApi
 # import ApiClient
 from xchainpy2_mayanode.api_client import ApiClient
 from xchainpy2_mayanode.configuration import Configuration
 # import models into sdk package
 from xchainpy2_mayanode.models.ban_response import BanResponse
+from xchainpy2_mayanode.models.base_quote_response import BaseQuoteResponse
+from xchainpy2_mayanode.models.block_response import BlockResponse
+from xchainpy2_mayanode.models.block_response_header import BlockResponseHeader
+from xchainpy2_mayanode.models.block_response_header_version import BlockResponseHeaderVersion
+from xchainpy2_mayanode.models.block_response_id import BlockResponseId
+from xchainpy2_mayanode.models.block_response_id_parts import BlockResponseIdParts
+from xchainpy2_mayanode.models.block_tx import BlockTx
+from xchainpy2_mayanode.models.block_tx_result import BlockTxResult
 from xchainpy2_mayanode.models.chain_height import ChainHeight
 from xchainpy2_mayanode.models.coin import Coin
 from xchainpy2_mayanode.models.constants_response import ConstantsResponse
 from xchainpy2_mayanode.models.inbound_address import InboundAddress
 from xchainpy2_mayanode.models.inbound_addresses_response import InboundAddressesResponse
 from xchainpy2_mayanode.models.keygen_metric import KeygenMetric
 from xchainpy2_mayanode.models.keygen_metric1 import KeygenMetric1
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/__init__.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/__init__.py`

 * *Files identical despite different names*

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/health_api.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/health_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/liquidity_providers_api.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/liquidity_providers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -147,15 +147,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.liquidity_providers(asset, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str asset: (required)
         :param int height: optional block height, defaults to current tip
-        :return: LiquidityProvider
+        :return: list[LiquidityProviderSummary]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.liquidity_providers_with_http_info(asset, **kwargs)  # noqa: E501
         else:
@@ -170,15 +170,15 @@
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.liquidity_providers_with_http_info(asset, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str asset: (required)
         :param int height: optional block height, defaults to current tip
-        :return: LiquidityProvider
+        :return: list[LiquidityProviderSummary]
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['asset', 'height']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -226,14 +226,14 @@
             '/mayachain/pool/{asset}/liquidity_providers', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='LiquidityProvider',  # noqa: E501
+            response_type='list[LiquidityProviderSummary]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/mayanames_api.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/mayanames_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/mimir_api.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/mimir_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/network_api.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/network_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/nodes_api.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/nodes_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/pol_api.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/pol_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/pools_api.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/pools_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/queue_api.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/queue_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/quote_api.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/quote_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/savers_api.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/savers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/transactions_api.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/transactions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/tss_api.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/tss_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api/vaults_api.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api/vaults_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/api_client.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 from __future__ import absolute_import
 
 import datetime
 import json
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/1.107.3/python'
+        self.user_agent = 'Swagger-Codegen/1.109.0/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/configuration.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import copy
@@ -215,17 +215,20 @@
                 return key
 
     def get_basic_auth_token(self):
         """Gets HTTP basic authentication header (string).
 
         :return: The token for basic HTTP authentication.
         """
-        return urllib3.util.make_headers(
-            basic_auth=self.username + ':' + self.password
-        ).get('authorization')
+        token = ""
+        if self.username or self.password:
+            token = urllib3.util.make_headers(
+                basic_auth=self.username + ':' + self.password
+            ).get('authorization')
+        return token
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         return {
@@ -235,10 +238,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.108.1\n"\
-               "SDK Package Version: 1.107.3".\
+               "Version of the API: 1.109.0\n"\
+               "SDK Package Version: 1.109.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/__init__.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,31 @@
 
 # flake8: noqa
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import models into model package
 from xchainpy2_mayanode.models.ban_response import BanResponse
+from xchainpy2_mayanode.models.base_quote_response import BaseQuoteResponse
+from xchainpy2_mayanode.models.block_response import BlockResponse
+from xchainpy2_mayanode.models.block_response_header import BlockResponseHeader
+from xchainpy2_mayanode.models.block_response_header_version import BlockResponseHeaderVersion
+from xchainpy2_mayanode.models.block_response_id import BlockResponseId
+from xchainpy2_mayanode.models.block_response_id_parts import BlockResponseIdParts
+from xchainpy2_mayanode.models.block_tx import BlockTx
+from xchainpy2_mayanode.models.block_tx_result import BlockTxResult
 from xchainpy2_mayanode.models.chain_height import ChainHeight
 from xchainpy2_mayanode.models.coin import Coin
 from xchainpy2_mayanode.models.constants_response import ConstantsResponse
 from xchainpy2_mayanode.models.inbound_address import InboundAddress
 from xchainpy2_mayanode.models.inbound_addresses_response import InboundAddressesResponse
 from xchainpy2_mayanode.models.keygen_metric import KeygenMetric
 from xchainpy2_mayanode.models.keygen_metric1 import KeygenMetric1
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/ban_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/ban_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/chain_height.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/chain_height.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/coin.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/coin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/constants_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/constants_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/inbound_address.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/inbound_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/inbound_addresses_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/inbound_addresses_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/keygen_metric.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/keygen_metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/keygen_metric1.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/keygen_metric1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/keygen_metric2.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/keygen_metric2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/keygen_metrics_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/keygen_metrics_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/keysign_info.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/keysign_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/keysign_metrics.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/keysign_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/keysign_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/keysign_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/last_block.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/last_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/last_block_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/last_block_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/liquidity_provider.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/liquidity_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/liquidity_provider_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/liquidity_provider_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/liquidity_provider_summary.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/liquidity_provider_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/liquidity_providers_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/liquidity_providers_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/lp_bonded_node.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/lp_bonded_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/mayaname.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/mayaname.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/mayaname1.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/mayaname1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/mayaname_alias.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/mayaname_alias.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/mayaname_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/mayaname_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/metrics_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/metrics_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/mimir_nodes_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/mimir_nodes_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/mimir_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/mimir_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/mimir_vote.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/mimir_vote.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/network_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/network_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/node.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/node_bond_provider.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/node_bond_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/node_bond_providers.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/node_bond_providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/node_jail.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/node_jail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/node_keygen_metric.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/node_keygen_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/node_preflight_status.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/node_preflight_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/node_pub_key_set.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/node_pub_key_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/node_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/node_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/nodes_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/pools_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class NodesResponse(object):
+class PoolsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """NodesResponse - a model defined in Swagger"""  # noqa: E501
+        """PoolsResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(NodesResponse, dict):
+        if issubclass(PoolsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, NodesResponse):
+        if not isinstance(other, PoolsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/observed_tx.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/observed_tx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/outbound_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/outbound_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/ping.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/ping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/pol_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/pol_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/pool.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/pool_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/vaults_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class PoolResponse(object):
+class VaultsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """PoolResponse - a model defined in Swagger"""  # noqa: E501
+        """VaultsResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(PoolResponse, dict):
+        if issubclass(VaultsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, PoolResponse):
+        if not isinstance(other, VaultsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/pools_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/savers_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class PoolsResponse(object):
+class SaversResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """PoolsResponse - a model defined in Swagger"""  # noqa: E501
+        """SaversResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(PoolsResponse, dict):
+        if issubclass(SaversResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, PoolsResponse):
+        if not isinstance(other, SaversResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/queue_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/queue_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/quote_fees.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/block_tx.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,126 +1,126 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class QuoteFees(object):
+class BlockTx(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'asset': 'str',
-        'affiliate': 'str',
-        'outbound': 'str'
+        'hash': 'str',
+        'tx': 'dict(str, object)',
+        'result': 'BlockTxResult'
     }
 
     attribute_map = {
-        'asset': 'asset',
-        'affiliate': 'affiliate',
-        'outbound': 'outbound'
+        'hash': 'hash',
+        'tx': 'tx',
+        'result': 'result'
     }
 
-    def __init__(self, asset=None, affiliate=None, outbound=None):  # noqa: E501
-        """QuoteFees - a model defined in Swagger"""  # noqa: E501
-        self._asset = None
-        self._affiliate = None
-        self._outbound = None
+    def __init__(self, hash=None, tx=None, result=None):  # noqa: E501
+        """BlockTx - a model defined in Swagger"""  # noqa: E501
+        self._hash = None
+        self._tx = None
+        self._result = None
         self.discriminator = None
-        self.asset = asset
-        self.affiliate = affiliate
-        self.outbound = outbound
+        self.hash = hash
+        self.tx = tx
+        self.result = result
 
     @property
-    def asset(self):
-        """Gets the asset of this QuoteFees.  # noqa: E501
+    def hash(self):
+        """Gets the hash of this BlockTx.  # noqa: E501
 
 
-        :return: The asset of this QuoteFees.  # noqa: E501
+        :return: The hash of this BlockTx.  # noqa: E501
         :rtype: str
         """
-        return self._asset
+        return self._hash
 
-    @asset.setter
-    def asset(self, asset):
-        """Sets the asset of this QuoteFees.
+    @hash.setter
+    def hash(self, hash):
+        """Sets the hash of this BlockTx.
 
 
-        :param asset: The asset of this QuoteFees.  # noqa: E501
+        :param hash: The hash of this BlockTx.  # noqa: E501
         :type: str
         """
-        if asset is None:
-            raise ValueError("Invalid value for `asset`, must not be `None`")  # noqa: E501
+        if hash is None:
+            raise ValueError("Invalid value for `hash`, must not be `None`")  # noqa: E501
 
-        self._asset = asset
+        self._hash = hash
 
     @property
-    def affiliate(self):
-        """Gets the affiliate of this QuoteFees.  # noqa: E501
+    def tx(self):
+        """Gets the tx of this BlockTx.  # noqa: E501
 
 
-        :return: The affiliate of this QuoteFees.  # noqa: E501
-        :rtype: str
+        :return: The tx of this BlockTx.  # noqa: E501
+        :rtype: dict(str, object)
         """
-        return self._affiliate
+        return self._tx
 
-    @affiliate.setter
-    def affiliate(self, affiliate):
-        """Sets the affiliate of this QuoteFees.
+    @tx.setter
+    def tx(self, tx):
+        """Sets the tx of this BlockTx.
 
 
-        :param affiliate: The affiliate of this QuoteFees.  # noqa: E501
-        :type: str
+        :param tx: The tx of this BlockTx.  # noqa: E501
+        :type: dict(str, object)
         """
-        if affiliate is None:
-            raise ValueError("Invalid value for `affiliate`, must not be `None`")  # noqa: E501
+        if tx is None:
+            raise ValueError("Invalid value for `tx`, must not be `None`")  # noqa: E501
 
-        self._affiliate = affiliate
+        self._tx = tx
 
     @property
-    def outbound(self):
-        """Gets the outbound of this QuoteFees.  # noqa: E501
+    def result(self):
+        """Gets the result of this BlockTx.  # noqa: E501
 
 
-        :return: The outbound of this QuoteFees.  # noqa: E501
-        :rtype: str
+        :return: The result of this BlockTx.  # noqa: E501
+        :rtype: BlockTxResult
         """
-        return self._outbound
+        return self._result
 
-    @outbound.setter
-    def outbound(self, outbound):
-        """Sets the outbound of this QuoteFees.
+    @result.setter
+    def result(self, result):
+        """Sets the result of this BlockTx.
 
 
-        :param outbound: The outbound of this QuoteFees.  # noqa: E501
-        :type: str
+        :param result: The result of this BlockTx.  # noqa: E501
+        :type: BlockTxResult
         """
-        if outbound is None:
-            raise ValueError("Invalid value for `outbound`, must not be `None`")  # noqa: E501
+        if result is None:
+            raise ValueError("Invalid value for `result`, must not be `None`")  # noqa: E501
 
-        self._outbound = outbound
+        self._result = result
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -135,15 +135,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(QuoteFees, dict):
+        if issubclass(BlockTx, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -151,15 +151,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, QuoteFees):
+        if not isinstance(other, BlockTx):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/quote_saver_withdraw_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/quote_saver_withdraw_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -25,53 +25,90 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'inbound_address': 'str',
-        'memo': 'str',
-        'dust_amount': 'str',
-        'expected_amount_out': 'str',
+        'inbound_confirmation_blocks': 'int',
+        'inbound_confirmation_seconds': 'int',
         'outbound_delay_blocks': 'int',
         'outbound_delay_seconds': 'int',
         'fees': 'QuoteFees',
-        'slippage_bps': 'int'
+        'slippage_bps': 'int',
+        'router': 'str',
+        'expiry': 'int',
+        'warning': 'str',
+        'notes': 'str',
+        'dust_threshold': 'str',
+        'recommended_min_amount_in': 'str',
+        'memo': 'str',
+        'dust_amount': 'str',
+        'expected_amount_out': 'str'
     }
 
     attribute_map = {
         'inbound_address': 'inbound_address',
-        'memo': 'memo',
-        'dust_amount': 'dust_amount',
-        'expected_amount_out': 'expected_amount_out',
+        'inbound_confirmation_blocks': 'inbound_confirmation_blocks',
+        'inbound_confirmation_seconds': 'inbound_confirmation_seconds',
         'outbound_delay_blocks': 'outbound_delay_blocks',
         'outbound_delay_seconds': 'outbound_delay_seconds',
         'fees': 'fees',
-        'slippage_bps': 'slippage_bps'
+        'slippage_bps': 'slippage_bps',
+        'router': 'router',
+        'expiry': 'expiry',
+        'warning': 'warning',
+        'notes': 'notes',
+        'dust_threshold': 'dust_threshold',
+        'recommended_min_amount_in': 'recommended_min_amount_in',
+        'memo': 'memo',
+        'dust_amount': 'dust_amount',
+        'expected_amount_out': 'expected_amount_out'
     }
 
-    def __init__(self, inbound_address=None, memo=None, dust_amount=None, expected_amount_out=None, outbound_delay_blocks=None, outbound_delay_seconds=None, fees=None, slippage_bps=None):  # noqa: E501
+    def __init__(self, inbound_address=None, inbound_confirmation_blocks=None, inbound_confirmation_seconds=None, outbound_delay_blocks=None, outbound_delay_seconds=None, fees=None, slippage_bps=None, router=None, expiry=None, warning=None, notes=None, dust_threshold=None, recommended_min_amount_in=None, memo=None, dust_amount=None, expected_amount_out=None):  # noqa: E501
         """QuoteSaverWithdrawResponse - a model defined in Swagger"""  # noqa: E501
         self._inbound_address = None
-        self._memo = None
-        self._dust_amount = None
-        self._expected_amount_out = None
+        self._inbound_confirmation_blocks = None
+        self._inbound_confirmation_seconds = None
         self._outbound_delay_blocks = None
         self._outbound_delay_seconds = None
         self._fees = None
         self._slippage_bps = None
+        self._router = None
+        self._expiry = None
+        self._warning = None
+        self._notes = None
+        self._dust_threshold = None
+        self._recommended_min_amount_in = None
+        self._memo = None
+        self._dust_amount = None
+        self._expected_amount_out = None
         self.discriminator = None
         self.inbound_address = inbound_address
-        self.memo = memo
-        self.dust_amount = dust_amount
-        self.expected_amount_out = expected_amount_out
+        if inbound_confirmation_blocks is not None:
+            self.inbound_confirmation_blocks = inbound_confirmation_blocks
+        if inbound_confirmation_seconds is not None:
+            self.inbound_confirmation_seconds = inbound_confirmation_seconds
         self.outbound_delay_blocks = outbound_delay_blocks
         self.outbound_delay_seconds = outbound_delay_seconds
         self.fees = fees
         self.slippage_bps = slippage_bps
+        if router is not None:
+            self.router = router
+        self.expiry = expiry
+        self.warning = warning
+        self.notes = notes
+        if dust_threshold is not None:
+            self.dust_threshold = dust_threshold
+        if recommended_min_amount_in is not None:
+            self.recommended_min_amount_in = recommended_min_amount_in
+        self.memo = memo
+        self.dust_amount = dust_amount
+        self.expected_amount_out = expected_amount_out
 
     @property
     def inbound_address(self):
         """Gets the inbound_address of this QuoteSaverWithdrawResponse.  # noqa: E501
 
         the inbound address for the transaction on the source chain  # noqa: E501
 
@@ -91,104 +128,75 @@
         """
         if inbound_address is None:
             raise ValueError("Invalid value for `inbound_address`, must not be `None`")  # noqa: E501
 
         self._inbound_address = inbound_address
 
     @property
-    def memo(self):
-        """Gets the memo of this QuoteSaverWithdrawResponse.  # noqa: E501
-
-        generated memo for the withdraw, the client can use this OR send the dust amount  # noqa: E501
-
-        :return: The memo of this QuoteSaverWithdrawResponse.  # noqa: E501
-        :rtype: str
-        """
-        return self._memo
-
-    @memo.setter
-    def memo(self, memo):
-        """Sets the memo of this QuoteSaverWithdrawResponse.
-
-        generated memo for the withdraw, the client can use this OR send the dust amount  # noqa: E501
-
-        :param memo: The memo of this QuoteSaverWithdrawResponse.  # noqa: E501
-        :type: str
-        """
-        if memo is None:
-            raise ValueError("Invalid value for `memo`, must not be `None`")  # noqa: E501
-
-        self._memo = memo
-
-    @property
-    def dust_amount(self):
-        """Gets the dust_amount of this QuoteSaverWithdrawResponse.  # noqa: E501
+    def inbound_confirmation_blocks(self):
+        """Gets the inbound_confirmation_blocks of this QuoteSaverWithdrawResponse.  # noqa: E501
 
-        the dust amount of the target asset the user should send to initialize the withdraw, the client can send this OR provide the memo  # noqa: E501
+        the approximate number of source chain blocks required before processing  # noqa: E501
 
-        :return: The dust_amount of this QuoteSaverWithdrawResponse.  # noqa: E501
-        :rtype: str
+        :return: The inbound_confirmation_blocks of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :rtype: int
         """
-        return self._dust_amount
+        return self._inbound_confirmation_blocks
 
-    @dust_amount.setter
-    def dust_amount(self, dust_amount):
-        """Sets the dust_amount of this QuoteSaverWithdrawResponse.
+    @inbound_confirmation_blocks.setter
+    def inbound_confirmation_blocks(self, inbound_confirmation_blocks):
+        """Sets the inbound_confirmation_blocks of this QuoteSaverWithdrawResponse.
 
-        the dust amount of the target asset the user should send to initialize the withdraw, the client can send this OR provide the memo  # noqa: E501
+        the approximate number of source chain blocks required before processing  # noqa: E501
 
-        :param dust_amount: The dust_amount of this QuoteSaverWithdrawResponse.  # noqa: E501
-        :type: str
+        :param inbound_confirmation_blocks: The inbound_confirmation_blocks of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :type: int
         """
-        if dust_amount is None:
-            raise ValueError("Invalid value for `dust_amount`, must not be `None`")  # noqa: E501
 
-        self._dust_amount = dust_amount
+        self._inbound_confirmation_blocks = inbound_confirmation_blocks
 
     @property
-    def expected_amount_out(self):
-        """Gets the expected_amount_out of this QuoteSaverWithdrawResponse.  # noqa: E501
+    def inbound_confirmation_seconds(self):
+        """Gets the inbound_confirmation_seconds of this QuoteSaverWithdrawResponse.  # noqa: E501
 
-        the minimum amount of the target asset the user can expect to withdraw after fees in 1e8 decimals  # noqa: E501
+        the approximate seconds for block confirmations required before processing  # noqa: E501
 
-        :return: The expected_amount_out of this QuoteSaverWithdrawResponse.  # noqa: E501
-        :rtype: str
+        :return: The inbound_confirmation_seconds of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :rtype: int
         """
-        return self._expected_amount_out
+        return self._inbound_confirmation_seconds
 
-    @expected_amount_out.setter
-    def expected_amount_out(self, expected_amount_out):
-        """Sets the expected_amount_out of this QuoteSaverWithdrawResponse.
+    @inbound_confirmation_seconds.setter
+    def inbound_confirmation_seconds(self, inbound_confirmation_seconds):
+        """Sets the inbound_confirmation_seconds of this QuoteSaverWithdrawResponse.
 
-        the minimum amount of the target asset the user can expect to withdraw after fees in 1e8 decimals  # noqa: E501
+        the approximate seconds for block confirmations required before processing  # noqa: E501
 
-        :param expected_amount_out: The expected_amount_out of this QuoteSaverWithdrawResponse.  # noqa: E501
-        :type: str
+        :param inbound_confirmation_seconds: The inbound_confirmation_seconds of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :type: int
         """
-        if expected_amount_out is None:
-            raise ValueError("Invalid value for `expected_amount_out`, must not be `None`")  # noqa: E501
 
-        self._expected_amount_out = expected_amount_out
+        self._inbound_confirmation_seconds = inbound_confirmation_seconds
 
     @property
     def outbound_delay_blocks(self):
         """Gets the outbound_delay_blocks of this QuoteSaverWithdrawResponse.  # noqa: E501
 
-        the number of mayachain blocks the outbound will be delayed  # noqa: E501
+        the number of thorchain blocks the outbound will be delayed  # noqa: E501
 
         :return: The outbound_delay_blocks of this QuoteSaverWithdrawResponse.  # noqa: E501
         :rtype: int
         """
         return self._outbound_delay_blocks
 
     @outbound_delay_blocks.setter
     def outbound_delay_blocks(self, outbound_delay_blocks):
         """Sets the outbound_delay_blocks of this QuoteSaverWithdrawResponse.
 
-        the number of mayachain blocks the outbound will be delayed  # noqa: E501
+        the number of thorchain blocks the outbound will be delayed  # noqa: E501
 
         :param outbound_delay_blocks: The outbound_delay_blocks of this QuoteSaverWithdrawResponse.  # noqa: E501
         :type: int
         """
         if outbound_delay_blocks is None:
             raise ValueError("Invalid value for `outbound_delay_blocks`, must not be `None`")  # noqa: E501
 
@@ -242,35 +250,254 @@
 
         self._fees = fees
 
     @property
     def slippage_bps(self):
         """Gets the slippage_bps of this QuoteSaverWithdrawResponse.  # noqa: E501
 
-        the swap slippage in basis points  # noqa: E501
+        Deprecated - migrate to fees object.  # noqa: E501
 
         :return: The slippage_bps of this QuoteSaverWithdrawResponse.  # noqa: E501
         :rtype: int
         """
         return self._slippage_bps
 
     @slippage_bps.setter
     def slippage_bps(self, slippage_bps):
         """Sets the slippage_bps of this QuoteSaverWithdrawResponse.
 
-        the swap slippage in basis points  # noqa: E501
+        Deprecated - migrate to fees object.  # noqa: E501
 
         :param slippage_bps: The slippage_bps of this QuoteSaverWithdrawResponse.  # noqa: E501
         :type: int
         """
         if slippage_bps is None:
             raise ValueError("Invalid value for `slippage_bps`, must not be `None`")  # noqa: E501
 
         self._slippage_bps = slippage_bps
 
+    @property
+    def router(self):
+        """Gets the router of this QuoteSaverWithdrawResponse.  # noqa: E501
+
+        the EVM chain router contract address  # noqa: E501
+
+        :return: The router of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._router
+
+    @router.setter
+    def router(self, router):
+        """Sets the router of this QuoteSaverWithdrawResponse.
+
+        the EVM chain router contract address  # noqa: E501
+
+        :param router: The router of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :type: str
+        """
+
+        self._router = router
+
+    @property
+    def expiry(self):
+        """Gets the expiry of this QuoteSaverWithdrawResponse.  # noqa: E501
+
+        expiration timestamp in unix seconds  # noqa: E501
+
+        :return: The expiry of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :rtype: int
+        """
+        return self._expiry
+
+    @expiry.setter
+    def expiry(self, expiry):
+        """Sets the expiry of this QuoteSaverWithdrawResponse.
+
+        expiration timestamp in unix seconds  # noqa: E501
+
+        :param expiry: The expiry of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :type: int
+        """
+        if expiry is None:
+            raise ValueError("Invalid value for `expiry`, must not be `None`")  # noqa: E501
+
+        self._expiry = expiry
+
+    @property
+    def warning(self):
+        """Gets the warning of this QuoteSaverWithdrawResponse.  # noqa: E501
+
+        static warning message  # noqa: E501
+
+        :return: The warning of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._warning
+
+    @warning.setter
+    def warning(self, warning):
+        """Sets the warning of this QuoteSaverWithdrawResponse.
+
+        static warning message  # noqa: E501
+
+        :param warning: The warning of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :type: str
+        """
+        if warning is None:
+            raise ValueError("Invalid value for `warning`, must not be `None`")  # noqa: E501
+
+        self._warning = warning
+
+    @property
+    def notes(self):
+        """Gets the notes of this QuoteSaverWithdrawResponse.  # noqa: E501
+
+        chain specific quote notes  # noqa: E501
+
+        :return: The notes of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._notes
+
+    @notes.setter
+    def notes(self, notes):
+        """Sets the notes of this QuoteSaverWithdrawResponse.
+
+        chain specific quote notes  # noqa: E501
+
+        :param notes: The notes of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :type: str
+        """
+        if notes is None:
+            raise ValueError("Invalid value for `notes`, must not be `None`")  # noqa: E501
+
+        self._notes = notes
+
+    @property
+    def dust_threshold(self):
+        """Gets the dust_threshold of this QuoteSaverWithdrawResponse.  # noqa: E501
+
+        Defines the minimum transaction size for the chain in base units (sats, wei, uatom). Transactions with asset amounts lower than the dust_threshold are ignored.  # noqa: E501
+
+        :return: The dust_threshold of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._dust_threshold
+
+    @dust_threshold.setter
+    def dust_threshold(self, dust_threshold):
+        """Sets the dust_threshold of this QuoteSaverWithdrawResponse.
+
+        Defines the minimum transaction size for the chain in base units (sats, wei, uatom). Transactions with asset amounts lower than the dust_threshold are ignored.  # noqa: E501
+
+        :param dust_threshold: The dust_threshold of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :type: str
+        """
+
+        self._dust_threshold = dust_threshold
+
+    @property
+    def recommended_min_amount_in(self):
+        """Gets the recommended_min_amount_in of this QuoteSaverWithdrawResponse.  # noqa: E501
+
+        The recommended minimum inbound amount for this transaction type & inbound asset. Sending less than this amount could result in failed refunds.  # noqa: E501
+
+        :return: The recommended_min_amount_in of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._recommended_min_amount_in
+
+    @recommended_min_amount_in.setter
+    def recommended_min_amount_in(self, recommended_min_amount_in):
+        """Sets the recommended_min_amount_in of this QuoteSaverWithdrawResponse.
+
+        The recommended minimum inbound amount for this transaction type & inbound asset. Sending less than this amount could result in failed refunds.  # noqa: E501
+
+        :param recommended_min_amount_in: The recommended_min_amount_in of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :type: str
+        """
+
+        self._recommended_min_amount_in = recommended_min_amount_in
+
+    @property
+    def memo(self):
+        """Gets the memo of this QuoteSaverWithdrawResponse.  # noqa: E501
+
+        generated memo for the withdraw, the client can use this OR send the dust amount  # noqa: E501
+
+        :return: The memo of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._memo
+
+    @memo.setter
+    def memo(self, memo):
+        """Sets the memo of this QuoteSaverWithdrawResponse.
+
+        generated memo for the withdraw, the client can use this OR send the dust amount  # noqa: E501
+
+        :param memo: The memo of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :type: str
+        """
+        if memo is None:
+            raise ValueError("Invalid value for `memo`, must not be `None`")  # noqa: E501
+
+        self._memo = memo
+
+    @property
+    def dust_amount(self):
+        """Gets the dust_amount of this QuoteSaverWithdrawResponse.  # noqa: E501
+
+        the dust amount of the target asset the user should send to initialize the withdraw, the client can send this OR provide the memo  # noqa: E501
+
+        :return: The dust_amount of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._dust_amount
+
+    @dust_amount.setter
+    def dust_amount(self, dust_amount):
+        """Sets the dust_amount of this QuoteSaverWithdrawResponse.
+
+        the dust amount of the target asset the user should send to initialize the withdraw, the client can send this OR provide the memo  # noqa: E501
+
+        :param dust_amount: The dust_amount of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :type: str
+        """
+        if dust_amount is None:
+            raise ValueError("Invalid value for `dust_amount`, must not be `None`")  # noqa: E501
+
+        self._dust_amount = dust_amount
+
+    @property
+    def expected_amount_out(self):
+        """Gets the expected_amount_out of this QuoteSaverWithdrawResponse.  # noqa: E501
+
+        the amount of the target asset the user can expect to withdraw after fees in 1e8 decimals  # noqa: E501
+
+        :return: The expected_amount_out of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._expected_amount_out
+
+    @expected_amount_out.setter
+    def expected_amount_out(self, expected_amount_out):
+        """Sets the expected_amount_out of this QuoteSaverWithdrawResponse.
+
+        the amount of the target asset the user can expect to withdraw after fees in 1e8 decimals  # noqa: E501
+
+        :param expected_amount_out: The expected_amount_out of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :type: str
+        """
+        if expected_amount_out is None:
+            raise ValueError("Invalid value for `expected_amount_out`, must not be `None`")  # noqa: E501
+
+        self._expected_amount_out = expected_amount_out
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/saver.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/saver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/saver_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/saver_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/savers_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/nodes_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SaversResponse(object):
+class NodesResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """SaversResponse - a model defined in Swagger"""  # noqa: E501
+        """NodesResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(SaversResponse, dict):
+        if issubclass(NodesResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SaversResponse):
+        if not isinstance(other, NodesResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/scheduled_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/scheduled_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/tss_keysign_metric.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/tss_keysign_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/tss_metric.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/tss_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/tx.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/tx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/tx_out_item.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/tx_out_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/tx_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/tx_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/tx_signers_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/tx_signers_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/vault.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/vault_address.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/vault_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/vault_info.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/vault_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/vault_pubkeys_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/vault_pubkeys_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/vault_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/vault_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/vault_router.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/vault_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/vaults_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/pool_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class VaultsResponse(object):
+class PoolResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """VaultsResponse - a model defined in Swagger"""  # noqa: E501
+        """PoolResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(VaultsResponse, dict):
+        if issubclass(PoolResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, VaultsResponse):
+        if not isinstance(other, PoolResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/models/version_response.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/models/version_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode/rest.py` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Mayanode API
 
     Mayanode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.108.1
+    OpenAPI spec version: 1.109.0
     Contact: devs@mayachain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import io
 import json
 import logging
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode.egg-info/PKG-INFO` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2-mayanode
-Version: 1.108.1
+Version: 1.109.0
 Summary: Mayanode API
 Home-page: 
 Author-email: devs@mayachain.org
 Keywords: Swagger,Mayanode API
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urllib3>=1.15
@@ -14,16 +14,16 @@
 Requires-Dist: aiohttp
 
 # xchainpy2-mayanode
 Mayanode REST API.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.108.1
-- Package version: 1.107.3
+- API version: 1.109.0
+- Package version: 1.109.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -122,14 +122,22 @@
 *VaultsApi* | [**vault**](docs/VaultsApi.md#vault) | **GET** /mayachain/vaults/{pubkey} | 
 *VaultsApi* | [**vault_pubkeys**](docs/VaultsApi.md#vault_pubkeys) | **GET** /mayachain/vaults/pubkeys | 
 *VaultsApi* | [**yggdrasil**](docs/VaultsApi.md#yggdrasil) | **GET** /mayachain/vaults/yggdrasil | 
 
 ## Documentation For Models
 
  - [BanResponse](docs/BanResponse.md)
+ - [BaseQuoteResponse](docs/BaseQuoteResponse.md)
+ - [BlockResponse](docs/BlockResponse.md)
+ - [BlockResponseHeader](docs/BlockResponseHeader.md)
+ - [BlockResponseHeaderVersion](docs/BlockResponseHeaderVersion.md)
+ - [BlockResponseId](docs/BlockResponseId.md)
+ - [BlockResponseIdParts](docs/BlockResponseIdParts.md)
+ - [BlockTx](docs/BlockTx.md)
+ - [BlockTxResult](docs/BlockTxResult.md)
  - [ChainHeight](docs/ChainHeight.md)
  - [Coin](docs/Coin.md)
  - [ConstantsResponse](docs/ConstantsResponse.md)
  - [InboundAddress](docs/InboundAddress.md)
  - [InboundAddressesResponse](docs/InboundAddressesResponse.md)
  - [KeygenMetric](docs/KeygenMetric.md)
  - [KeygenMetric1](docs/KeygenMetric1.md)
```

### Comparing `xchainpy2-mayanode-1.108.1/xchainpy2_mayanode.egg-info/SOURCES.txt` & `xchainpy2_mayanode-1.109.0/xchainpy2_mayanode.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 LICENSE
 README.md
 setup.py
 test/__init__.py
 test/test_ban_response.py
+test/test_base_quote_response.py
+test/test_block_response.py
+test/test_block_response_header.py
+test/test_block_response_header_version.py
+test/test_block_response_id.py
+test/test_block_response_id_parts.py
+test/test_block_tx.py
+test/test_block_tx_result.py
 test/test_chain_height.py
 test/test_coin.py
 test/test_constants_response.py
 test/test_health_api.py
 test/test_inbound_address.py
 test/test_inbound_addresses_response.py
 test/test_keygen_metric.py
@@ -106,14 +114,22 @@
 xchainpy2_mayanode/api/quote_api.py
 xchainpy2_mayanode/api/savers_api.py
 xchainpy2_mayanode/api/transactions_api.py
 xchainpy2_mayanode/api/tss_api.py
 xchainpy2_mayanode/api/vaults_api.py
 xchainpy2_mayanode/models/__init__.py
 xchainpy2_mayanode/models/ban_response.py
+xchainpy2_mayanode/models/base_quote_response.py
+xchainpy2_mayanode/models/block_response.py
+xchainpy2_mayanode/models/block_response_header.py
+xchainpy2_mayanode/models/block_response_header_version.py
+xchainpy2_mayanode/models/block_response_id.py
+xchainpy2_mayanode/models/block_response_id_parts.py
+xchainpy2_mayanode/models/block_tx.py
+xchainpy2_mayanode/models/block_tx_result.py
 xchainpy2_mayanode/models/chain_height.py
 xchainpy2_mayanode/models/coin.py
 xchainpy2_mayanode/models/constants_response.py
 xchainpy2_mayanode/models/inbound_address.py
 xchainpy2_mayanode/models/inbound_addresses_response.py
 xchainpy2_mayanode/models/keygen_metric.py
 xchainpy2_mayanode/models/keygen_metric1.py
```

