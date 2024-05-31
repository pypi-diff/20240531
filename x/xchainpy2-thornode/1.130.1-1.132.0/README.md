# Comparing `tmp/xchainpy2-thornode-1.130.1.tar.gz` & `tmp/xchainpy2_thornode-1.132.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchainpy2-thornode-1.130.1.tar", last modified: Mon Apr  1 10:29:36 2024, max compression
+gzip compressed data, was "xchainpy2_thornode-1.132.0.tar", last modified: Fri May 31 12:55:40 2024, max compression
```

## Comparing `xchainpy2-thornode-1.130.1.tar` & `xchainpy2_thornode-1.132.0.tar`

### file list

```diff
@@ -1,279 +1,299 @@
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 10:29:36.057469 xchainpy2-thornode-1.130.1/
--rw-r--r--   0 tirinox    (501) staff       (20)     2124 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/LICENSE
--rw-r--r--   0 tirinox    (501) staff       (20)    13717 2024-04-01 10:29:36.056913 xchainpy2-thornode-1.130.1/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)    13361 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/README.md
--rw-r--r--   0 tirinox    (501) staff       (20)       38 2024-04-01 10:29:36.057510 xchainpy2-thornode-1.130.1/setup.cfg
--rw-r--r--   0 tirinox    (501) staff       (20)     1270 2024-04-01 10:24:14.000000 xchainpy2-thornode-1.130.1/setup.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 10:29:36.035430 xchainpy2-thornode-1.130.1/test/
--rw-r--r--   0 tirinox    (501) staff       (20)       15 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_ban_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_base_quote_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      730 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_block_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_block_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      937 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_block_response_header.py
--rw-r--r--   0 tirinox    (501) staff       (20)      995 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_block_response_header_version.py
--rw-r--r--   0 tirinox    (501) staff       (20)      905 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_block_response_id.py
--rw-r--r--   0 tirinox    (501) staff       (20)      947 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_block_response_id_parts.py
--rw-r--r--   0 tirinox    (501) staff       (20)      839 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_block_tx.py
--rw-r--r--   0 tirinox    (501) staff       (20)      889 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_block_tx_result.py
--rw-r--r--   0 tirinox    (501) staff       (20)      845 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_borrower.py
--rw-r--r--   0 tirinox    (501) staff       (20)      911 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_borrower_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      848 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_borrowers_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_borrowers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_chain_height.py
--rw-r--r--   0 tirinox    (501) staff       (20)      746 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_clout_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_coin.py
--rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_constants_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_derived_pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)      937 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_derived_pool_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      945 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_derived_pools_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      733 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_health_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_inbound_address.py
--rw-r--r--   0 tirinox    (501) staff       (20)      977 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_inbound_addresses_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_invariant_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      857 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_invariants_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      927 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_invariants_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_keygen_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)      953 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_keygen_metrics_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_keysign_info.py
--rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_keysign_metrics.py
--rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_keysign_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_last_block.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_last_block_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_liquidity_provider.py
--rw-r--r--   0 tirinox    (501) staff       (20)      985 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_liquidity_provider_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      977 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_liquidity_provider_summary.py
--rw-r--r--   0 tirinox    (501) staff       (20)      934 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_liquidity_providers_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      993 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_liquidity_providers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_metrics_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1296 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_mimir_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      929 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_mimir_nodes_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_mimir_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      931 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_mimir_v2_ids_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_mimir_vote.py
--rw-r--r--   0 tirinox    (501) staff       (20)      839 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_msg_swap.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1398 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_network_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_network_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_node.py
--rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_node_bond_provider.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_node_bond_providers.py
--rw-r--r--   0 tirinox    (501) staff       (20)      847 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_node_jail.py
--rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_node_keygen_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)      937 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_node_preflight_status.py
--rw-r--r--   0 tirinox    (501) staff       (20)      891 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_node_pub_key_set.py
--rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_node_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      812 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_nodes_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_nodes_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      863 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_observed_tx.py
--rw-r--r--   0 tirinox    (501) staff       (20)      911 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_outbound_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_ping.py
--rw-r--r--   0 tirinox    (501) staff       (20)      716 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_pol_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_pol_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_pool_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      982 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_pools_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_pools_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1030 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_queue_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_queue_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1158 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_quote_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_quote_fees.py
--rw-r--r--   0 tirinox    (501) staff       (20)      963 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_quote_loan_close_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      955 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_quote_loan_open_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      987 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_quote_saver_deposit_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      995 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_quote_saver_withdraw_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_quote_swap_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      821 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_saver.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_saver_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      821 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_savers_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_savers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_scheduled_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_streaming_swap.py
--rw-r--r--   0 tirinox    (501) staff       (20)      881 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_streaming_swap_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      953 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_streaming_swap_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      961 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_streaming_swaps_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_swap_queue_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      945 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_swapper_clout_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      845 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_thorname.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_thorname_alias.py
--rw-r--r--   0 tirinox    (501) staff       (20)      911 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_thorname_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      756 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_thornames_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      782 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_trade_account_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      945 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_trade_account_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      789 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_trade_accounts_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      953 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_trade_accounts_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      761 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_trade_unit_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_trade_unit_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      768 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_trade_units_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      929 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_trade_units_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1139 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_transactions_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1016 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_tss_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tss_keysign_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tss_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)      797 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_details_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      857 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_out_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)      863 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_signers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1127 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response_inbound_confirmation_counted.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1045 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response_inbound_finalised.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1037 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response_inbound_observed.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1021 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response_outbound_delay.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1029 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response_outbound_signed.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1021 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response_swap_finalised.py
--rw-r--r--   0 tirinox    (501) staff       (20)      997 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response_swap_status.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1071 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response_swap_status_streaming.py
--rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_status_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1023 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_status_response_planned_out_txs.py
--rw-r--r--   0 tirinox    (501) staff       (20)      821 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_vault.py
--rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_vault_address.py
--rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_vault_info.py
--rw-r--r--   0 tirinox    (501) staff       (20)      945 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_vault_pubkeys_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_vault_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_vault_router.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1013 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_vaults_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_vaults_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_version_response.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 10:29:36.036931 xchainpy2-thornode-1.130.1/xchainpy2_thornode/
--rw-r--r--   0 tirinox    (501) staff       (20)     9608 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 10:29:36.041879 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/
--rw-r--r--   0 tirinox    (501) staff       (20)     1467 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4010 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/block_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     8841 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/borrowers_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4618 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/clout_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3591 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/health_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7957 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/invariants_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     9207 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/liquidity_providers_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    25039 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/mimir_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    28645 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/network_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7800 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/nodes_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4014 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/pol_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14824 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/pools_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14025 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/queue_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    25292 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/quote_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     8757 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/savers_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7898 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/streaming_swap_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4563 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/thornames_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4646 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/trade_account_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4628 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/trade_accounts_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4575 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/trade_unit_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4139 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/trade_units_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    19756 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/transactions_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    16119 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/tss_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14407 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/vaults_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    25046 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api_client.py
--rw-r--r--   0 tirinox    (501) staff       (20)     8023 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/configuration.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 10:29:36.056402 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/
--rw-r--r--   0 tirinox    (501) staff       (20)     8068 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4499 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/ban_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    16196 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/base_quote_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6451 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14461 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response_header.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3874 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response_header_version.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3814 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response_id.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3823 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response_id_parts.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4358 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_tx.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7409 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_tx_result.py
--rw-r--r--   0 tirinox    (501) staff       (20)    10805 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/borrower.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2404 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/borrower_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2408 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/borrowers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3757 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/chain_height.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4298 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/coin.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4796 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/constants_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7204 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/derived_pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2416 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/derived_pool_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2420 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/derived_pools_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14332 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/inbound_address.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2436 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/inbound_addresses_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4957 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/invariant_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3149 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/invariants_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3950 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keygen_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2424 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keygen_metrics_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4071 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keysign_info.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3820 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keysign_metrics.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3760 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keysign_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5575 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/last_block.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2408 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/last_block_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    16304 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/liquidity_provider.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2440 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/liquidity_provider_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    11875 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/liquidity_provider_summary.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2444 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/liquidity_providers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3763 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/metrics_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3087 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/mimir_nodes_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2628 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/mimir_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5619 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/mimir_v2_ids_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4109 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/mimir_vote.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14536 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/msg_swap.py
--rw-r--r--   0 tirinox    (501) staff       (20)    20441 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/network_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    21507 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3748 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_bond_provider.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4111 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_bond_providers.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3732 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_jail.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3728 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_keygen_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4804 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_preflight_status.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3712 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_pub_key_set.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2388 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/nodes_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    12377 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/observed_tx.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2404 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/outbound_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2899 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/ping.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6975 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/pol_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    20318 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2388 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/pool_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/pools_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7066 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/queue_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     8184 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_fees.py
--rw-r--r--   0 tirinox    (501) staff       (20)    26967 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_loan_close_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    26986 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_loan_open_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    20465 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_saver_deposit_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    20804 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_saver_withdraw_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    24690 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_swap_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     8754 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/saver.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/saver_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2396 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/savers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2408 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/scheduled_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14192 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/streaming_swap.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2424 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/streaming_swap_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2428 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/streaming_swaps_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2408 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/swap_queue_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7826 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/swapper_clout_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7228 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/thorname.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3632 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/thorname_alias.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2404 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/thorname_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7043 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/trade_account_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2424 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/trade_accounts_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4831 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/trade_unit_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2412 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/trade_units_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3937 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tss_keysign_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3644 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tss_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6573 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx.py
--rw-r--r--   0 tirinox    (501) staff       (20)    10350 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_details_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     9938 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_out_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6805 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    10350 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_signers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     8982 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     9909 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_inbound_confirmation_counted.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3538 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_inbound_finalised.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6606 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_inbound_observed.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5854 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_outbound_delay.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5938 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_outbound_signed.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3604 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_swap_finalised.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4149 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_swap_status.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5297 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_swap_status_streaming.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5286 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_status_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5721 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_status_response_planned_out_txs.py
--rw-r--r--   0 tirinox    (501) staff       (20)    12716 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3620 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_address.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3838 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_info.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4833 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_pubkeys_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3588 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_router.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2396 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vaults_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5861 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/version_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    10622 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/rest.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 10:29:36.056629 xchainpy2-thornode-1.130.1/xchainpy2_thornode.egg-info/
--rw-r--r--   0 tirinox    (501) staff       (20)    13717 2024-04-01 10:29:36.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode.egg-info/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)    10309 2024-04-01 10:29:36.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode.egg-info/SOURCES.txt
--rw-r--r--   0 tirinox    (501) staff       (20)        1 2024-04-01 10:29:36.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode.egg-info/dependency_links.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       56 2024-04-01 10:29:36.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode.egg-info/requires.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       24 2024-04-01 10:29:36.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode.egg-info/top_level.txt
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 12:55:40.455415 xchainpy2_thornode-1.132.0/
+-rw-r--r--   0 tirinox    (501) staff       (20)     2124 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/LICENSE
+-rw-r--r--   0 tirinox    (501) staff       (20)    14419 2024-05-31 12:55:40.455157 xchainpy2_thornode-1.132.0/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)    14063 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/README.md
+-rw-r--r--   0 tirinox    (501) staff       (20)       38 2024-05-31 12:55:40.455450 xchainpy2_thornode-1.132.0/setup.cfg
+-rw-r--r--   0 tirinox    (501) staff       (20)     1270 2024-05-31 12:51:09.000000 xchainpy2_thornode-1.132.0/setup.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 12:55:40.416067 xchainpy2_thornode-1.132.0/test/
+-rw-r--r--   0 tirinox    (501) staff       (20)       15 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/test/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_ban_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_base_quote_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      730 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_block_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_block_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      937 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_block_response_header.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      995 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_block_response_header_version.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      905 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_block_response_id.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      947 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_block_response_id_parts.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      839 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_block_tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      889 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_block_tx_result.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      845 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_borrower.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      911 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_borrower_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      848 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_borrowers_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_borrowers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_chain_height.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      746 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_clout_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_coin.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_constants_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_derived_pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      937 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_derived_pool_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      945 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_derived_pools_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      733 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_health_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_inbound_address.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      977 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_inbound_addresses_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1035 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_inbound_confirmation_counted_stage.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      953 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_inbound_finalised_stage.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      945 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_inbound_observed_stage.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_inline_response200.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_invariant_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      857 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_invariants_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      927 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_invariants_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      829 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_keygen.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_keygen_block.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_keygen_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      953 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_keygen_metrics_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_keygen_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_keysign_info.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_keysign_metrics.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_keysign_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_last_block.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_last_block_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_liquidity_provider.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      985 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_liquidity_provider_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      977 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_liquidity_provider_summary.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      934 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_liquidity_providers_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      993 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_liquidity_providers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_metrics_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1296 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_mimir_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      929 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_mimir_nodes_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_mimir_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      931 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_mimir_v2_ids_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_mimir_vote.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      839 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_msg_swap.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1608 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_network_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_network_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_node.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_node_bond_provider.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_node_bond_providers.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      847 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_node_jail.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_node_keygen_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      937 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_node_preflight_status.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      891 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_node_pub_key_set.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_node_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      812 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_nodes_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_nodes_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      863 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_observed_tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      929 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_outbound_delay_stage.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_outbound_fee.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      945 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_outbound_fees_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      911 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_outbound_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      937 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_outbound_signed_stage.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_ping.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      881 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_planned_out_tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      716 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/test/test_pol_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_pol_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_pool_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      844 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/test/test_pool_slip_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_pool_slip_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      982 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/test/test_pools_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_pools_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1030 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/test/test_queue_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_queue_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1158 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/test/test_quote_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_quote_fees.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      963 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_quote_loan_close_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      955 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_quote_loan_open_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      987 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_quote_saver_deposit_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      995 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_quote_saver_withdraw_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_quote_swap_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      821 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_saver.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_saver_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      821 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/test/test_savers_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_savers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_scheduled_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_streaming_status.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_streaming_swap.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      881 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/test/test_streaming_swap_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      953 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_streaming_swap_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      961 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_streaming_swaps_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      929 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_swap_finalised_stage.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_swap_queue_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      863 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_swap_status.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      945 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_swapper_clout_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      845 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_thorname.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_thorname_alias.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      911 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_thorname_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      756 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/test/test_thornames_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      782 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/test/test_trade_account_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      945 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_trade_account_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      789 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/test/test_trade_accounts_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      953 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_trade_accounts_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      761 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/test/test_trade_unit_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_trade_unit_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      768 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/test/test_trade_units_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      929 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_trade_units_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1139 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/test/test_transactions_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1116 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/test/test_tss_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_tss_keysign_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_tss_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      797 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_tx_details_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      857 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_tx_out_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      863 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_tx_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_tx_signers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_tx_stages_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_tx_status_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      821 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_vault.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_vault_address.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_vault_info.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      945 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_vault_pubkeys_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_vault_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_vault_router.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1013 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/test/test_vaults_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_vaults_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_version_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_yggdrasil_vault.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      969 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/test/test_yggdrasil_vaults_response.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 12:55:40.417076 xchainpy2_thornode-1.132.0/xchainpy2_thornode/
+-rw-r--r--   0 tirinox    (501) staff       (20)    10044 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 12:55:40.425507 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/
+-rw-r--r--   0 tirinox    (501) staff       (20)     1528 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4010 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/block_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8841 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/borrowers_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4618 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/clout_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3591 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/health_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7957 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/invariants_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     9207 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/liquidity_providers_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    25039 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/mimir_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    35952 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/network_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7800 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/nodes_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4014 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/pol_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7979 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/pool_slip_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14824 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/pools_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14025 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/queue_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    25292 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/quote_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8757 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/savers_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7898 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/streaming_swap_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4563 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/thornames_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4646 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/trade_account_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4628 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/trade_accounts_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4575 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/trade_unit_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4139 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/trade_units_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    19756 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/transactions_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    20377 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/tss_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14434 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/vaults_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    25046 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/api_client.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8023 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/configuration.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 12:55:40.454571 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/
+-rw-r--r--   0 tirinox    (501) staff       (20)     8443 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4499 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/ban_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    18230 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/base_quote_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6451 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/block_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14461 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/block_response_header.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3874 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/block_response_header_version.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3814 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/block_response_id.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3823 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/block_response_id_parts.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4358 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/block_tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7409 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/block_tx_result.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    10805 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/borrower.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2404 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/borrower_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2408 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/borrowers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3757 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/chain_height.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4298 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/coin.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4796 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/constants_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7204 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/derived_pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2416 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/derived_pool_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2420 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/derived_pools_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14332 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/inbound_address.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2436 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/inbound_addresses_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     9601 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/inbound_confirmation_counted_stage.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3450 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/inbound_finalised_stage.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6476 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/inbound_observed_stage.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7936 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/inline_response200.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4957 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/invariant_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3149 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/invariants_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4059 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/keygen.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3847 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/keygen_block.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3950 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/keygen_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2424 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/keygen_metrics_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4027 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/keygen_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4071 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/keysign_info.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3820 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/keysign_metrics.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3934 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/keysign_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5575 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/last_block.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2408 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/last_block_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    15824 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/liquidity_provider.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2440 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/liquidity_provider_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    11875 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/liquidity_provider_summary.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2444 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/liquidity_providers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3763 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/metrics_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3087 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/mimir_nodes_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2628 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/mimir_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6751 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/mimir_v2_ids_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4109 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/mimir_vote.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14488 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/msg_swap.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    20441 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/network_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    21507 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/node.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3748 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/node_bond_provider.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4429 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/node_bond_providers.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3732 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/node_jail.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3728 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/node_keygen_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4804 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/node_preflight_status.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3712 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/node_pub_key_set.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2388 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/node_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/nodes_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    12377 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/observed_tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5678 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/outbound_delay_stage.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8507 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/outbound_fee.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2420 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/outbound_fees_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2404 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/outbound_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5762 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/outbound_signed_stage.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2899 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/ping.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5381 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/planned_out_tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6975 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/pol_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    20318 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2388 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/pool_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2404 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/pool_slip_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/pools_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7066 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/queue_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8184 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/quote_fees.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    29041 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/quote_loan_close_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    29244 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/quote_loan_open_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    22755 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/quote_saver_deposit_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    23102 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/quote_saver_withdraw_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    26724 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/quote_swap_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8754 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/saver.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/saver_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2396 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/savers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2408 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/scheduled_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4977 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/streaming_status.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14192 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/streaming_swap.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2424 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/streaming_swap_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2428 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/streaming_swaps_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3516 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/swap_finalised_stage.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2408 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/swap_queue_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3897 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/swap_status.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7826 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/swapper_clout_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7228 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/thorname.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3632 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/thorname_alias.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2404 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/thorname_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7043 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/trade_account_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2424 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/trade_accounts_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4831 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/trade_unit_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2412 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/trade_units_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3937 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tss_keysign_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3644 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tss_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6573 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    10350 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tx_details_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     9853 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tx_out_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6805 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tx_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    10350 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tx_signers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8736 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tx_stages_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5235 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tx_status_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    12716 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/vault.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3790 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/vault_address.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3838 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/vault_info.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4833 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/vault_pubkeys_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/vault_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3588 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/vault_router.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2396 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/vaults_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5861 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/version_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14292 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/yggdrasil_vault.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2432 2024-05-31 12:50:32.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/yggdrasil_vaults_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    10622 2024-05-31 12:50:33.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode/rest.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 12:55:40.454858 xchainpy2_thornode-1.132.0/xchainpy2_thornode.egg-info/
+-rw-r--r--   0 tirinox    (501) staff       (20)    14419 2024-05-31 12:55:40.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode.egg-info/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)    10776 2024-05-31 12:55:40.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode.egg-info/SOURCES.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)        1 2024-05-31 12:55:40.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode.egg-info/dependency_links.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       56 2024-05-31 12:55:40.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode.egg-info/requires.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       24 2024-05-31 12:55:40.000000 xchainpy2_thornode-1.132.0/xchainpy2_thornode.egg-info/top_level.txt
```

### Comparing `xchainpy2-thornode-1.130.1/LICENSE` & `xchainpy2_thornode-1.132.0/LICENSE`

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

### Comparing `xchainpy2-thornode-1.130.1/PKG-INFO` & `xchainpy2_thornode-1.132.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2-thornode
-Version: 1.130.1
+Version: 1.132.0
 Summary: Thornode API
 Home-page: 
 Author-email: devs@thorchain.org
 Keywords: Swagger,Thornode API
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urllib3>=1.15
@@ -14,16 +14,16 @@
 Requires-Dist: aiohttp
 
 # xchainpy2-thornode
 Thornode REST API.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.130.1
-- Package version: 1.130.1
+- API version: 1.132.0
+- Package version: 1.132.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -101,19 +101,23 @@
 *MimirApi* | [**mimir_v2_ids**](docs/MimirApi.md#mimir_v2_ids) | **GET** /thorchain/mimirV2/ids | 
 *NetworkApi* | [**ban**](docs/NetworkApi.md#ban) | **GET** /thorchain/ban/{address} | 
 *NetworkApi* | [**constants**](docs/NetworkApi.md#constants) | **GET** /thorchain/constants | 
 *NetworkApi* | [**inbound_addresses**](docs/NetworkApi.md#inbound_addresses) | **GET** /thorchain/inbound_addresses | 
 *NetworkApi* | [**lastblock**](docs/NetworkApi.md#lastblock) | **GET** /thorchain/lastblock | 
 *NetworkApi* | [**lastblock_chain**](docs/NetworkApi.md#lastblock_chain) | **GET** /thorchain/lastblock/{chain} | 
 *NetworkApi* | [**network**](docs/NetworkApi.md#network) | **GET** /thorchain/network | 
+*NetworkApi* | [**outbound_fee_asset**](docs/NetworkApi.md#outbound_fee_asset) | **GET** /thorchain/outbound_fee/{asset} | 
+*NetworkApi* | [**outbound_fees**](docs/NetworkApi.md#outbound_fees) | **GET** /thorchain/outbound_fees | 
 *NetworkApi* | [**ragnarok**](docs/NetworkApi.md#ragnarok) | **GET** /thorchain/ragnarok | 
 *NetworkApi* | [**version**](docs/NetworkApi.md#version) | **GET** /thorchain/version | 
 *NodesApi* | [**node**](docs/NodesApi.md#node) | **GET** /thorchain/node/{address} | 
 *NodesApi* | [**nodes**](docs/NodesApi.md#nodes) | **GET** /thorchain/nodes | 
 *POLApi* | [**pol**](docs/POLApi.md#pol) | **GET** /thorchain/pol | 
+*PoolSlipApi* | [**poolslip**](docs/PoolSlipApi.md#poolslip) | **GET** /thorchain/slip/{asset} | 
+*PoolSlipApi* | [**poolslips**](docs/PoolSlipApi.md#poolslips) | **GET** /thorchain/slips | 
 *PoolsApi* | [**dpool**](docs/PoolsApi.md#dpool) | **GET** /thorchain/dpool/{asset} | 
 *PoolsApi* | [**dpools**](docs/PoolsApi.md#dpools) | **GET** /thorchain/dpools | 
 *PoolsApi* | [**pool**](docs/PoolsApi.md#pool) | **GET** /thorchain/pool/{asset} | 
 *PoolsApi* | [**pools**](docs/PoolsApi.md#pools) | **GET** /thorchain/pools | 
 *QueueApi* | [**queue**](docs/QueueApi.md#queue) | **GET** /thorchain/queue | 
 *QueueApi* | [**queue_outbound**](docs/QueueApi.md#queue_outbound) | **GET** /thorchain/queue/outbound | 
 *QueueApi* | [**queue_scheduled**](docs/QueueApi.md#queue_scheduled) | **GET** /thorchain/queue/scheduled | 
@@ -123,14 +127,15 @@
 *QuoteApi* | [**quotesaverdeposit**](docs/QuoteApi.md#quotesaverdeposit) | **GET** /thorchain/quote/saver/deposit | 
 *QuoteApi* | [**quotesaverwithdraw**](docs/QuoteApi.md#quotesaverwithdraw) | **GET** /thorchain/quote/saver/withdraw | 
 *QuoteApi* | [**quoteswap**](docs/QuoteApi.md#quoteswap) | **GET** /thorchain/quote/swap | 
 *SaversApi* | [**saver**](docs/SaversApi.md#saver) | **GET** /thorchain/pool/{asset}/saver/{address} | 
 *SaversApi* | [**savers**](docs/SaversApi.md#savers) | **GET** /thorchain/pool/{asset}/savers | 
 *StreamingSwapApi* | [**stream_swap**](docs/StreamingSwapApi.md#stream_swap) | **GET** /thorchain/swap/streaming/{hash} | 
 *StreamingSwapApi* | [**stream_swaps**](docs/StreamingSwapApi.md#stream_swaps) | **GET** /thorchain/swaps/streaming | 
+*TSSApi* | [**keygen_pubkey**](docs/TSSApi.md#keygen_pubkey) | **GET** /thorchain/keygen/{height}/{pubkey} | 
 *TSSApi* | [**keysign**](docs/TSSApi.md#keysign) | **GET** /thorchain/keysign/{height} | 
 *TSSApi* | [**keysign_pubkey**](docs/TSSApi.md#keysign_pubkey) | **GET** /thorchain/keysign/{height}/{pubkey} | 
 *TSSApi* | [**metrics**](docs/TSSApi.md#metrics) | **GET** /thorchain/metrics | 
 *TSSApi* | [**metrics_keygen**](docs/TSSApi.md#metrics_keygen) | **GET** /thorchain/metric/keygen/{pubkey} | 
 *ThornamesApi* | [**thorname**](docs/ThornamesApi.md#thorname) | **GET** /thorchain/thorname/{name} | 
 *TradeAccountApi* | [**trade_account**](docs/TradeAccountApi.md#trade_account) | **GET** /thorchain/trade/account/{address} | 
 *TradeAccountsApi* | [**trade_accounts**](docs/TradeAccountsApi.md#trade_accounts) | **GET** /thorchain/trade/accounts/{asset} | 
@@ -164,18 +169,25 @@
  - [Coin](docs/Coin.md)
  - [ConstantsResponse](docs/ConstantsResponse.md)
  - [DerivedPool](docs/DerivedPool.md)
  - [DerivedPoolResponse](docs/DerivedPoolResponse.md)
  - [DerivedPoolsResponse](docs/DerivedPoolsResponse.md)
  - [InboundAddress](docs/InboundAddress.md)
  - [InboundAddressesResponse](docs/InboundAddressesResponse.md)
+ - [InboundConfirmationCountedStage](docs/InboundConfirmationCountedStage.md)
+ - [InboundFinalisedStage](docs/InboundFinalisedStage.md)
+ - [InboundObservedStage](docs/InboundObservedStage.md)
+ - [InlineResponse200](docs/InlineResponse200.md)
  - [InvariantResponse](docs/InvariantResponse.md)
  - [InvariantsResponse](docs/InvariantsResponse.md)
+ - [Keygen](docs/Keygen.md)
+ - [KeygenBlock](docs/KeygenBlock.md)
  - [KeygenMetric](docs/KeygenMetric.md)
  - [KeygenMetricsResponse](docs/KeygenMetricsResponse.md)
+ - [KeygenResponse](docs/KeygenResponse.md)
  - [KeysignInfo](docs/KeysignInfo.md)
  - [KeysignMetrics](docs/KeysignMetrics.md)
  - [KeysignResponse](docs/KeysignResponse.md)
  - [LastBlock](docs/LastBlock.md)
  - [LastBlockResponse](docs/LastBlockResponse.md)
  - [LiquidityProvider](docs/LiquidityProvider.md)
  - [LiquidityProviderResponse](docs/LiquidityProviderResponse.md)
@@ -194,35 +206,44 @@
  - [NodeJail](docs/NodeJail.md)
  - [NodeKeygenMetric](docs/NodeKeygenMetric.md)
  - [NodePreflightStatus](docs/NodePreflightStatus.md)
  - [NodePubKeySet](docs/NodePubKeySet.md)
  - [NodeResponse](docs/NodeResponse.md)
  - [NodesResponse](docs/NodesResponse.md)
  - [ObservedTx](docs/ObservedTx.md)
+ - [OutboundDelayStage](docs/OutboundDelayStage.md)
+ - [OutboundFee](docs/OutboundFee.md)
+ - [OutboundFeesResponse](docs/OutboundFeesResponse.md)
  - [OutboundResponse](docs/OutboundResponse.md)
+ - [OutboundSignedStage](docs/OutboundSignedStage.md)
  - [POLResponse](docs/POLResponse.md)
  - [Ping](docs/Ping.md)
+ - [PlannedOutTx](docs/PlannedOutTx.md)
  - [Pool](docs/Pool.md)
  - [PoolResponse](docs/PoolResponse.md)
+ - [PoolSlipResponse](docs/PoolSlipResponse.md)
  - [PoolsResponse](docs/PoolsResponse.md)
  - [QueueResponse](docs/QueueResponse.md)
  - [QuoteFees](docs/QuoteFees.md)
  - [QuoteLoanCloseResponse](docs/QuoteLoanCloseResponse.md)
  - [QuoteLoanOpenResponse](docs/QuoteLoanOpenResponse.md)
  - [QuoteSaverDepositResponse](docs/QuoteSaverDepositResponse.md)
  - [QuoteSaverWithdrawResponse](docs/QuoteSaverWithdrawResponse.md)
  - [QuoteSwapResponse](docs/QuoteSwapResponse.md)
  - [Saver](docs/Saver.md)
  - [SaverResponse](docs/SaverResponse.md)
  - [SaversResponse](docs/SaversResponse.md)
  - [ScheduledResponse](docs/ScheduledResponse.md)
+ - [StreamingStatus](docs/StreamingStatus.md)
  - [StreamingSwap](docs/StreamingSwap.md)
  - [StreamingSwapResponse](docs/StreamingSwapResponse.md)
  - [StreamingSwapsResponse](docs/StreamingSwapsResponse.md)
+ - [SwapFinalisedStage](docs/SwapFinalisedStage.md)
  - [SwapQueueResponse](docs/SwapQueueResponse.md)
+ - [SwapStatus](docs/SwapStatus.md)
  - [SwapperCloutResponse](docs/SwapperCloutResponse.md)
  - [Thorname](docs/Thorname.md)
  - [ThornameAlias](docs/ThornameAlias.md)
  - [ThornameResponse](docs/ThornameResponse.md)
  - [TradeAccountResponse](docs/TradeAccountResponse.md)
  - [TradeAccountsResponse](docs/TradeAccountsResponse.md)
  - [TradeUnitResponse](docs/TradeUnitResponse.md)
@@ -231,32 +252,25 @@
  - [TssMetric](docs/TssMetric.md)
  - [Tx](docs/Tx.md)
  - [TxDetailsResponse](docs/TxDetailsResponse.md)
  - [TxOutItem](docs/TxOutItem.md)
  - [TxResponse](docs/TxResponse.md)
  - [TxSignersResponse](docs/TxSignersResponse.md)
  - [TxStagesResponse](docs/TxStagesResponse.md)
- - [TxStagesResponseInboundConfirmationCounted](docs/TxStagesResponseInboundConfirmationCounted.md)
- - [TxStagesResponseInboundFinalised](docs/TxStagesResponseInboundFinalised.md)
- - [TxStagesResponseInboundObserved](docs/TxStagesResponseInboundObserved.md)
- - [TxStagesResponseOutboundDelay](docs/TxStagesResponseOutboundDelay.md)
- - [TxStagesResponseOutboundSigned](docs/TxStagesResponseOutboundSigned.md)
- - [TxStagesResponseSwapFinalised](docs/TxStagesResponseSwapFinalised.md)
- - [TxStagesResponseSwapStatus](docs/TxStagesResponseSwapStatus.md)
- - [TxStagesResponseSwapStatusStreaming](docs/TxStagesResponseSwapStatusStreaming.md)
  - [TxStatusResponse](docs/TxStatusResponse.md)
- - [TxStatusResponsePlannedOutTxs](docs/TxStatusResponsePlannedOutTxs.md)
  - [Vault](docs/Vault.md)
  - [VaultAddress](docs/VaultAddress.md)
  - [VaultInfo](docs/VaultInfo.md)
  - [VaultPubkeysResponse](docs/VaultPubkeysResponse.md)
  - [VaultResponse](docs/VaultResponse.md)
  - [VaultRouter](docs/VaultRouter.md)
  - [VaultsResponse](docs/VaultsResponse.md)
  - [VersionResponse](docs/VersionResponse.md)
+ - [YggdrasilVault](docs/YggdrasilVault.md)
+ - [YggdrasilVaultsResponse](docs/YggdrasilVaultsResponse.md)
 
 ## Documentation For Authorization
 
  All endpoints do not require authorization.
 
 
 ## Author
```

### Comparing `xchainpy2-thornode-1.130.1/README.md` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,29 @@
+Metadata-Version: 2.1
+Name: xchainpy2-thornode
+Version: 1.132.0
+Summary: Thornode API
+Home-page: 
+Author-email: devs@thorchain.org
+Keywords: Swagger,Thornode API
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: urllib3>=1.15
+Requires-Dist: six>=1.10
+Requires-Dist: certifi
+Requires-Dist: python-dateutil
+Requires-Dist: aiohttp
+
 # xchainpy2-thornode
 Thornode REST API.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.130.1
-- Package version: 1.130.1
+- API version: 1.132.0
+- Package version: 1.132.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -86,19 +101,23 @@
 *MimirApi* | [**mimir_v2_ids**](docs/MimirApi.md#mimir_v2_ids) | **GET** /thorchain/mimirV2/ids | 
 *NetworkApi* | [**ban**](docs/NetworkApi.md#ban) | **GET** /thorchain/ban/{address} | 
 *NetworkApi* | [**constants**](docs/NetworkApi.md#constants) | **GET** /thorchain/constants | 
 *NetworkApi* | [**inbound_addresses**](docs/NetworkApi.md#inbound_addresses) | **GET** /thorchain/inbound_addresses | 
 *NetworkApi* | [**lastblock**](docs/NetworkApi.md#lastblock) | **GET** /thorchain/lastblock | 
 *NetworkApi* | [**lastblock_chain**](docs/NetworkApi.md#lastblock_chain) | **GET** /thorchain/lastblock/{chain} | 
 *NetworkApi* | [**network**](docs/NetworkApi.md#network) | **GET** /thorchain/network | 
+*NetworkApi* | [**outbound_fee_asset**](docs/NetworkApi.md#outbound_fee_asset) | **GET** /thorchain/outbound_fee/{asset} | 
+*NetworkApi* | [**outbound_fees**](docs/NetworkApi.md#outbound_fees) | **GET** /thorchain/outbound_fees | 
 *NetworkApi* | [**ragnarok**](docs/NetworkApi.md#ragnarok) | **GET** /thorchain/ragnarok | 
 *NetworkApi* | [**version**](docs/NetworkApi.md#version) | **GET** /thorchain/version | 
 *NodesApi* | [**node**](docs/NodesApi.md#node) | **GET** /thorchain/node/{address} | 
 *NodesApi* | [**nodes**](docs/NodesApi.md#nodes) | **GET** /thorchain/nodes | 
 *POLApi* | [**pol**](docs/POLApi.md#pol) | **GET** /thorchain/pol | 
+*PoolSlipApi* | [**poolslip**](docs/PoolSlipApi.md#poolslip) | **GET** /thorchain/slip/{asset} | 
+*PoolSlipApi* | [**poolslips**](docs/PoolSlipApi.md#poolslips) | **GET** /thorchain/slips | 
 *PoolsApi* | [**dpool**](docs/PoolsApi.md#dpool) | **GET** /thorchain/dpool/{asset} | 
 *PoolsApi* | [**dpools**](docs/PoolsApi.md#dpools) | **GET** /thorchain/dpools | 
 *PoolsApi* | [**pool**](docs/PoolsApi.md#pool) | **GET** /thorchain/pool/{asset} | 
 *PoolsApi* | [**pools**](docs/PoolsApi.md#pools) | **GET** /thorchain/pools | 
 *QueueApi* | [**queue**](docs/QueueApi.md#queue) | **GET** /thorchain/queue | 
 *QueueApi* | [**queue_outbound**](docs/QueueApi.md#queue_outbound) | **GET** /thorchain/queue/outbound | 
 *QueueApi* | [**queue_scheduled**](docs/QueueApi.md#queue_scheduled) | **GET** /thorchain/queue/scheduled | 
@@ -108,14 +127,15 @@
 *QuoteApi* | [**quotesaverdeposit**](docs/QuoteApi.md#quotesaverdeposit) | **GET** /thorchain/quote/saver/deposit | 
 *QuoteApi* | [**quotesaverwithdraw**](docs/QuoteApi.md#quotesaverwithdraw) | **GET** /thorchain/quote/saver/withdraw | 
 *QuoteApi* | [**quoteswap**](docs/QuoteApi.md#quoteswap) | **GET** /thorchain/quote/swap | 
 *SaversApi* | [**saver**](docs/SaversApi.md#saver) | **GET** /thorchain/pool/{asset}/saver/{address} | 
 *SaversApi* | [**savers**](docs/SaversApi.md#savers) | **GET** /thorchain/pool/{asset}/savers | 
 *StreamingSwapApi* | [**stream_swap**](docs/StreamingSwapApi.md#stream_swap) | **GET** /thorchain/swap/streaming/{hash} | 
 *StreamingSwapApi* | [**stream_swaps**](docs/StreamingSwapApi.md#stream_swaps) | **GET** /thorchain/swaps/streaming | 
+*TSSApi* | [**keygen_pubkey**](docs/TSSApi.md#keygen_pubkey) | **GET** /thorchain/keygen/{height}/{pubkey} | 
 *TSSApi* | [**keysign**](docs/TSSApi.md#keysign) | **GET** /thorchain/keysign/{height} | 
 *TSSApi* | [**keysign_pubkey**](docs/TSSApi.md#keysign_pubkey) | **GET** /thorchain/keysign/{height}/{pubkey} | 
 *TSSApi* | [**metrics**](docs/TSSApi.md#metrics) | **GET** /thorchain/metrics | 
 *TSSApi* | [**metrics_keygen**](docs/TSSApi.md#metrics_keygen) | **GET** /thorchain/metric/keygen/{pubkey} | 
 *ThornamesApi* | [**thorname**](docs/ThornamesApi.md#thorname) | **GET** /thorchain/thorname/{name} | 
 *TradeAccountApi* | [**trade_account**](docs/TradeAccountApi.md#trade_account) | **GET** /thorchain/trade/account/{address} | 
 *TradeAccountsApi* | [**trade_accounts**](docs/TradeAccountsApi.md#trade_accounts) | **GET** /thorchain/trade/accounts/{asset} | 
@@ -149,18 +169,25 @@
  - [Coin](docs/Coin.md)
  - [ConstantsResponse](docs/ConstantsResponse.md)
  - [DerivedPool](docs/DerivedPool.md)
  - [DerivedPoolResponse](docs/DerivedPoolResponse.md)
  - [DerivedPoolsResponse](docs/DerivedPoolsResponse.md)
  - [InboundAddress](docs/InboundAddress.md)
  - [InboundAddressesResponse](docs/InboundAddressesResponse.md)
+ - [InboundConfirmationCountedStage](docs/InboundConfirmationCountedStage.md)
+ - [InboundFinalisedStage](docs/InboundFinalisedStage.md)
+ - [InboundObservedStage](docs/InboundObservedStage.md)
+ - [InlineResponse200](docs/InlineResponse200.md)
  - [InvariantResponse](docs/InvariantResponse.md)
  - [InvariantsResponse](docs/InvariantsResponse.md)
+ - [Keygen](docs/Keygen.md)
+ - [KeygenBlock](docs/KeygenBlock.md)
  - [KeygenMetric](docs/KeygenMetric.md)
  - [KeygenMetricsResponse](docs/KeygenMetricsResponse.md)
+ - [KeygenResponse](docs/KeygenResponse.md)
  - [KeysignInfo](docs/KeysignInfo.md)
  - [KeysignMetrics](docs/KeysignMetrics.md)
  - [KeysignResponse](docs/KeysignResponse.md)
  - [LastBlock](docs/LastBlock.md)
  - [LastBlockResponse](docs/LastBlockResponse.md)
  - [LiquidityProvider](docs/LiquidityProvider.md)
  - [LiquidityProviderResponse](docs/LiquidityProviderResponse.md)
@@ -179,35 +206,44 @@
  - [NodeJail](docs/NodeJail.md)
  - [NodeKeygenMetric](docs/NodeKeygenMetric.md)
  - [NodePreflightStatus](docs/NodePreflightStatus.md)
  - [NodePubKeySet](docs/NodePubKeySet.md)
  - [NodeResponse](docs/NodeResponse.md)
  - [NodesResponse](docs/NodesResponse.md)
  - [ObservedTx](docs/ObservedTx.md)
+ - [OutboundDelayStage](docs/OutboundDelayStage.md)
+ - [OutboundFee](docs/OutboundFee.md)
+ - [OutboundFeesResponse](docs/OutboundFeesResponse.md)
  - [OutboundResponse](docs/OutboundResponse.md)
+ - [OutboundSignedStage](docs/OutboundSignedStage.md)
  - [POLResponse](docs/POLResponse.md)
  - [Ping](docs/Ping.md)
+ - [PlannedOutTx](docs/PlannedOutTx.md)
  - [Pool](docs/Pool.md)
  - [PoolResponse](docs/PoolResponse.md)
+ - [PoolSlipResponse](docs/PoolSlipResponse.md)
  - [PoolsResponse](docs/PoolsResponse.md)
  - [QueueResponse](docs/QueueResponse.md)
  - [QuoteFees](docs/QuoteFees.md)
  - [QuoteLoanCloseResponse](docs/QuoteLoanCloseResponse.md)
  - [QuoteLoanOpenResponse](docs/QuoteLoanOpenResponse.md)
  - [QuoteSaverDepositResponse](docs/QuoteSaverDepositResponse.md)
  - [QuoteSaverWithdrawResponse](docs/QuoteSaverWithdrawResponse.md)
  - [QuoteSwapResponse](docs/QuoteSwapResponse.md)
  - [Saver](docs/Saver.md)
  - [SaverResponse](docs/SaverResponse.md)
  - [SaversResponse](docs/SaversResponse.md)
  - [ScheduledResponse](docs/ScheduledResponse.md)
+ - [StreamingStatus](docs/StreamingStatus.md)
  - [StreamingSwap](docs/StreamingSwap.md)
  - [StreamingSwapResponse](docs/StreamingSwapResponse.md)
  - [StreamingSwapsResponse](docs/StreamingSwapsResponse.md)
+ - [SwapFinalisedStage](docs/SwapFinalisedStage.md)
  - [SwapQueueResponse](docs/SwapQueueResponse.md)
+ - [SwapStatus](docs/SwapStatus.md)
  - [SwapperCloutResponse](docs/SwapperCloutResponse.md)
  - [Thorname](docs/Thorname.md)
  - [ThornameAlias](docs/ThornameAlias.md)
  - [ThornameResponse](docs/ThornameResponse.md)
  - [TradeAccountResponse](docs/TradeAccountResponse.md)
  - [TradeAccountsResponse](docs/TradeAccountsResponse.md)
  - [TradeUnitResponse](docs/TradeUnitResponse.md)
@@ -216,32 +252,25 @@
  - [TssMetric](docs/TssMetric.md)
  - [Tx](docs/Tx.md)
  - [TxDetailsResponse](docs/TxDetailsResponse.md)
  - [TxOutItem](docs/TxOutItem.md)
  - [TxResponse](docs/TxResponse.md)
  - [TxSignersResponse](docs/TxSignersResponse.md)
  - [TxStagesResponse](docs/TxStagesResponse.md)
- - [TxStagesResponseInboundConfirmationCounted](docs/TxStagesResponseInboundConfirmationCounted.md)
- - [TxStagesResponseInboundFinalised](docs/TxStagesResponseInboundFinalised.md)
- - [TxStagesResponseInboundObserved](docs/TxStagesResponseInboundObserved.md)
- - [TxStagesResponseOutboundDelay](docs/TxStagesResponseOutboundDelay.md)
- - [TxStagesResponseOutboundSigned](docs/TxStagesResponseOutboundSigned.md)
- - [TxStagesResponseSwapFinalised](docs/TxStagesResponseSwapFinalised.md)
- - [TxStagesResponseSwapStatus](docs/TxStagesResponseSwapStatus.md)
- - [TxStagesResponseSwapStatusStreaming](docs/TxStagesResponseSwapStatusStreaming.md)
  - [TxStatusResponse](docs/TxStatusResponse.md)
- - [TxStatusResponsePlannedOutTxs](docs/TxStatusResponsePlannedOutTxs.md)
  - [Vault](docs/Vault.md)
  - [VaultAddress](docs/VaultAddress.md)
  - [VaultInfo](docs/VaultInfo.md)
  - [VaultPubkeysResponse](docs/VaultPubkeysResponse.md)
  - [VaultResponse](docs/VaultResponse.md)
  - [VaultRouter](docs/VaultRouter.md)
  - [VaultsResponse](docs/VaultsResponse.md)
  - [VersionResponse](docs/VersionResponse.md)
+ - [YggdrasilVault](docs/YggdrasilVault.md)
+ - [YggdrasilVaultsResponse](docs/YggdrasilVaultsResponse.md)
 
 ## Documentation For Authorization
 
  All endpoints do not require authorization.
 
 
 ## Author
```

### Comparing `xchainpy2-thornode-1.130.1/setup.py` & `xchainpy2_thornode-1.132.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "xchainpy2-thornode"
-VERSION = "1.130.1"
+VERSION = "1.132.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_ban_response.py` & `xchainpy2_thornode-1.132.0/test/test_ban_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_base_quote_response.py` & `xchainpy2_thornode-1.132.0/test/test_base_quote_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_block_api.py` & `xchainpy2_thornode-1.132.0/test/test_block_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_block_response.py` & `xchainpy2_thornode-1.132.0/test/test_block_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_block_response_header.py` & `xchainpy2_thornode-1.132.0/test/test_block_response_header.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_block_response_header_version.py` & `xchainpy2_thornode-1.132.0/test/test_block_response_header_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_block_response_id.py` & `xchainpy2_thornode-1.132.0/test/test_block_response_id_parts.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.block_response_id import BlockResponseId  # noqa: E501
+from xchainpy2_thornode.models.block_response_id_parts import BlockResponseIdParts  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestBlockResponseId(unittest.TestCase):
-    """BlockResponseId unit test stubs"""
+class TestBlockResponseIdParts(unittest.TestCase):
+    """BlockResponseIdParts unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBlockResponseId(self):
-        """Test BlockResponseId"""
+    def testBlockResponseIdParts(self):
+        """Test BlockResponseIdParts"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.block_response_id.BlockResponseId()  # noqa: E501
+        # model = xchainpy2_thornode.models.block_response_id_parts.BlockResponseIdParts()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_block_response_id_parts.py` & `xchainpy2_thornode-1.132.0/test/test_block_response_id.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.block_response_id_parts import BlockResponseIdParts  # noqa: E501
+from xchainpy2_thornode.models.block_response_id import BlockResponseId  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestBlockResponseIdParts(unittest.TestCase):
-    """BlockResponseIdParts unit test stubs"""
+class TestBlockResponseId(unittest.TestCase):
+    """BlockResponseId unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBlockResponseIdParts(self):
-        """Test BlockResponseIdParts"""
+    def testBlockResponseId(self):
+        """Test BlockResponseId"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.block_response_id_parts.BlockResponseIdParts()  # noqa: E501
+        # model = xchainpy2_thornode.models.block_response_id.BlockResponseId()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_block_tx.py` & `xchainpy2_thornode-1.132.0/test/test_block_tx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_block_tx_result.py` & `xchainpy2_thornode-1.132.0/test/test_block_tx_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_borrower.py` & `xchainpy2_thornode-1.132.0/test/test_borrower.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_borrower_response.py` & `xchainpy2_thornode-1.132.0/test/test_borrower_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_borrowers_api.py` & `xchainpy2_thornode-1.132.0/test/test_borrowers_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_borrowers_response.py` & `xchainpy2_thornode-1.132.0/test/test_borrowers_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_chain_height.py` & `xchainpy2_thornode-1.132.0/test/test_chain_height.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_clout_api.py` & `xchainpy2_thornode-1.132.0/test/test_clout_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_coin.py` & `xchainpy2_thornode-1.132.0/test/test_coin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_constants_response.py` & `xchainpy2_thornode-1.132.0/test/test_constants_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_derived_pool.py` & `xchainpy2_thornode-1.132.0/test/test_derived_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_derived_pool_response.py` & `xchainpy2_thornode-1.132.0/test/test_derived_pool_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_derived_pools_response.py` & `xchainpy2_thornode-1.132.0/test/test_derived_pools_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_health_api.py` & `xchainpy2_thornode-1.132.0/test/test_health_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_inbound_address.py` & `xchainpy2_thornode-1.132.0/test/test_inbound_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_inbound_addresses_response.py` & `xchainpy2_thornode-1.132.0/test/test_inbound_addresses_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_invariant_response.py` & `xchainpy2_thornode-1.132.0/test/test_invariant_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_invariants_api.py` & `xchainpy2_thornode-1.132.0/test/test_invariants_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_invariants_response.py` & `xchainpy2_thornode-1.132.0/test/test_invariants_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_keygen_metric.py` & `xchainpy2_thornode-1.132.0/test/test_keygen_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_keygen_metrics_response.py` & `xchainpy2_thornode-1.132.0/test/test_keygen_metrics_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_keysign_info.py` & `xchainpy2_thornode-1.132.0/test/test_keysign_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_keysign_metrics.py` & `xchainpy2_thornode-1.132.0/test/test_keysign_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_keysign_response.py` & `xchainpy2_thornode-1.132.0/test/test_keysign_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_last_block.py` & `xchainpy2_thornode-1.132.0/test/test_last_block_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.last_block import LastBlock  # noqa: E501
+from xchainpy2_thornode.models.last_block_response import LastBlockResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestLastBlock(unittest.TestCase):
-    """LastBlock unit test stubs"""
+class TestLastBlockResponse(unittest.TestCase):
+    """LastBlockResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testLastBlock(self):
-        """Test LastBlock"""
+    def testLastBlockResponse(self):
+        """Test LastBlockResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.last_block.LastBlock()  # noqa: E501
+        # model = xchainpy2_thornode.models.last_block_response.LastBlockResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_last_block_response.py` & `xchainpy2_thornode-1.132.0/test/test_tx_details_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.last_block_response import LastBlockResponse  # noqa: E501
+from xchainpy2_thornode.models.tx_details_response import TxDetailsResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestLastBlockResponse(unittest.TestCase):
-    """LastBlockResponse unit test stubs"""
+class TestTxDetailsResponse(unittest.TestCase):
+    """TxDetailsResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testLastBlockResponse(self):
-        """Test LastBlockResponse"""
+    def testTxDetailsResponse(self):
+        """Test TxDetailsResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.last_block_response.LastBlockResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.tx_details_response.TxDetailsResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_liquidity_provider.py` & `xchainpy2_thornode-1.132.0/test/test_liquidity_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_liquidity_provider_response.py` & `xchainpy2_thornode-1.132.0/test/test_liquidity_provider_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_liquidity_provider_summary.py` & `xchainpy2_thornode-1.132.0/test/test_liquidity_provider_summary.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_liquidity_providers_api.py` & `xchainpy2_thornode-1.132.0/test/test_liquidity_providers_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_liquidity_providers_response.py` & `xchainpy2_thornode-1.132.0/test/test_liquidity_providers_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_metrics_response.py` & `xchainpy2_thornode-1.132.0/test/test_metrics_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_mimir_api.py` & `xchainpy2_thornode-1.132.0/test/test_mimir_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_mimir_nodes_response.py` & `xchainpy2_thornode-1.132.0/test/test_mimir_nodes_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_mimir_response.py` & `xchainpy2_thornode-1.132.0/test/test_mimir_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_mimir_v2_ids_response.py` & `xchainpy2_thornode-1.132.0/test/test_mimir_v2_ids_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_mimir_vote.py` & `xchainpy2_thornode-1.132.0/test/test_mimir_vote.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_msg_swap.py` & `xchainpy2_thornode-1.132.0/test/test_msg_swap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_network_api.py` & `xchainpy2_thornode-1.132.0/test/test_network_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
@@ -60,14 +60,26 @@
 
     def test_network(self):
         """Test case for network
 
         """
         pass
 
+    def test_outbound_fee_asset(self):
+        """Test case for outbound_fee_asset
+
+        """
+        pass
+
+    def test_outbound_fees(self):
+        """Test case for outbound_fees
+
+        """
+        pass
+
     def test_ragnarok(self):
         """Test case for ragnarok
 
         """
         pass
 
     def test_version(self):
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_network_response.py` & `xchainpy2_thornode-1.132.0/test/test_network_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_node.py` & `xchainpy2_thornode-1.132.0/test/test_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_node_bond_provider.py` & `xchainpy2_thornode-1.132.0/test/test_node_bond_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_node_bond_providers.py` & `xchainpy2_thornode-1.132.0/test/test_node_bond_providers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_node_jail.py` & `xchainpy2_thornode-1.132.0/test/test_node_jail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_node_keygen_metric.py` & `xchainpy2_thornode-1.132.0/test/test_keygen_block.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.node_keygen_metric import NodeKeygenMetric  # noqa: E501
+from xchainpy2_thornode.models.keygen_block import KeygenBlock  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestNodeKeygenMetric(unittest.TestCase):
-    """NodeKeygenMetric unit test stubs"""
+class TestKeygenBlock(unittest.TestCase):
+    """KeygenBlock unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testNodeKeygenMetric(self):
-        """Test NodeKeygenMetric"""
+    def testKeygenBlock(self):
+        """Test KeygenBlock"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.node_keygen_metric.NodeKeygenMetric()  # noqa: E501
+        # model = xchainpy2_thornode.models.keygen_block.KeygenBlock()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_node_preflight_status.py` & `xchainpy2_thornode-1.132.0/test/test_node_preflight_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_node_pub_key_set.py` & `xchainpy2_thornode-1.132.0/test/test_node_pub_key_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_node_response.py` & `xchainpy2_thornode-1.132.0/test/test_node_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_nodes_api.py` & `xchainpy2_thornode-1.132.0/test/test_nodes_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_nodes_response.py` & `xchainpy2_thornode-1.132.0/test/test_nodes_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_observed_tx.py` & `xchainpy2_thornode-1.132.0/test/test_observed_tx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_outbound_response.py` & `xchainpy2_thornode-1.132.0/test/test_outbound_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_ping.py` & `xchainpy2_thornode-1.132.0/test/test_ping.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_pol_api.py` & `xchainpy2_thornode-1.132.0/test/test_pol_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_pol_response.py` & `xchainpy2_thornode-1.132.0/test/test_pol_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_pool.py` & `xchainpy2_thornode-1.132.0/test/test_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_pool_response.py` & `xchainpy2_thornode-1.132.0/test/test_saver_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.pool_response import PoolResponse  # noqa: E501
+from xchainpy2_thornode.models.saver_response import SaverResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestPoolResponse(unittest.TestCase):
-    """PoolResponse unit test stubs"""
+class TestSaverResponse(unittest.TestCase):
+    """SaverResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPoolResponse(self):
-        """Test PoolResponse"""
+    def testSaverResponse(self):
+        """Test SaverResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.pool_response.PoolResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.saver_response.SaverResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_pools_api.py` & `xchainpy2_thornode-1.132.0/test/test_pools_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_pools_response.py` & `xchainpy2_thornode-1.132.0/test/test_pool_slip_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.pools_response import PoolsResponse  # noqa: E501
+from xchainpy2_thornode.models.pool_slip_response import PoolSlipResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestPoolsResponse(unittest.TestCase):
-    """PoolsResponse unit test stubs"""
+class TestPoolSlipResponse(unittest.TestCase):
+    """PoolSlipResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPoolsResponse(self):
-        """Test PoolsResponse"""
+    def testPoolSlipResponse(self):
+        """Test PoolSlipResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.pools_response.PoolsResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.pool_slip_response.PoolSlipResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_queue_api.py` & `xchainpy2_thornode-1.132.0/test/test_queue_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_queue_response.py` & `xchainpy2_thornode-1.132.0/test/test_queue_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_quote_api.py` & `xchainpy2_thornode-1.132.0/test/test_quote_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_quote_fees.py` & `xchainpy2_thornode-1.132.0/test/test_quote_fees.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_quote_loan_close_response.py` & `xchainpy2_thornode-1.132.0/test/test_quote_loan_close_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_quote_loan_open_response.py` & `xchainpy2_thornode-1.132.0/test/test_quote_loan_open_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_quote_saver_deposit_response.py` & `xchainpy2_thornode-1.132.0/test/test_quote_saver_deposit_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_quote_saver_withdraw_response.py` & `xchainpy2_thornode-1.132.0/test/test_quote_saver_withdraw_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_quote_swap_response.py` & `xchainpy2_thornode-1.132.0/test/test_quote_swap_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_saver.py` & `xchainpy2_thornode-1.132.0/test/test_saver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_saver_response.py` & `xchainpy2_thornode-1.132.0/test/test_savers_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.saver_response import SaverResponse  # noqa: E501
+from xchainpy2_thornode.models.savers_response import SaversResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestSaverResponse(unittest.TestCase):
-    """SaverResponse unit test stubs"""
+class TestSaversResponse(unittest.TestCase):
+    """SaversResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSaverResponse(self):
-        """Test SaverResponse"""
+    def testSaversResponse(self):
+        """Test SaversResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.saver_response.SaverResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.savers_response.SaversResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_savers_api.py` & `xchainpy2_thornode-1.132.0/test/test_savers_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_savers_response.py` & `xchainpy2_thornode-1.132.0/test/test_tx_signers_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.savers_response import SaversResponse  # noqa: E501
+from xchainpy2_thornode.models.tx_signers_response import TxSignersResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestSaversResponse(unittest.TestCase):
-    """SaversResponse unit test stubs"""
+class TestTxSignersResponse(unittest.TestCase):
+    """TxSignersResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSaversResponse(self):
-        """Test SaversResponse"""
+    def testTxSignersResponse(self):
+        """Test TxSignersResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.savers_response.SaversResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.tx_signers_response.TxSignersResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_scheduled_response.py` & `xchainpy2_thornode-1.132.0/test/test_scheduled_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_streaming_swap.py` & `xchainpy2_thornode-1.132.0/test/test_streaming_swap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_streaming_swap_api.py` & `xchainpy2_thornode-1.132.0/test/test_pool_slip_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.api.streaming_swap_api import StreamingSwapApi  # noqa: E501
+from xchainpy2_thornode.api.pool_slip_api import PoolSlipApi  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestStreamingSwapApi(unittest.TestCase):
-    """StreamingSwapApi unit test stubs"""
+class TestPoolSlipApi(unittest.TestCase):
+    """PoolSlipApi unit test stubs"""
 
     def setUp(self):
-        self.api = StreamingSwapApi()  # noqa: E501
+        self.api = PoolSlipApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_stream_swap(self):
-        """Test case for stream_swap
+    def test_poolslip(self):
+        """Test case for poolslip
 
         """
         pass
 
-    def test_stream_swaps(self):
-        """Test case for stream_swaps
+    def test_poolslips(self):
+        """Test case for poolslips
 
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_streaming_swap_response.py` & `xchainpy2_thornode-1.132.0/test/test_streaming_swap_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_streaming_swaps_response.py` & `xchainpy2_thornode-1.132.0/test/test_streaming_swaps_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_swap_queue_response.py` & `xchainpy2_thornode-1.132.0/test/test_tx_status_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.swap_queue_response import SwapQueueResponse  # noqa: E501
+from xchainpy2_thornode.models.tx_status_response import TxStatusResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestSwapQueueResponse(unittest.TestCase):
-    """SwapQueueResponse unit test stubs"""
+class TestTxStatusResponse(unittest.TestCase):
+    """TxStatusResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSwapQueueResponse(self):
-        """Test SwapQueueResponse"""
+    def testTxStatusResponse(self):
+        """Test TxStatusResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.swap_queue_response.SwapQueueResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.tx_status_response.TxStatusResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_swapper_clout_response.py` & `xchainpy2_thornode-1.132.0/test/test_swapper_clout_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_thorname.py` & `xchainpy2_thornode-1.132.0/test/test_thorname.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_thorname_alias.py` & `xchainpy2_thornode-1.132.0/test/test_thorname_alias.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_thorname_response.py` & `xchainpy2_thornode-1.132.0/test/test_thorname_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_thornames_api.py` & `xchainpy2_thornode-1.132.0/test/test_thornames_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_trade_account_api.py` & `xchainpy2_thornode-1.132.0/test/test_trade_account_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_trade_account_response.py` & `xchainpy2_thornode-1.132.0/test/test_trade_account_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_trade_accounts_api.py` & `xchainpy2_thornode-1.132.0/test/test_trade_accounts_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_trade_accounts_response.py` & `xchainpy2_thornode-1.132.0/test/test_trade_accounts_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_trade_unit_api.py` & `xchainpy2_thornode-1.132.0/test/test_trade_unit_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_trade_unit_response.py` & `xchainpy2_thornode-1.132.0/test/test_trade_unit_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_trade_units_api.py` & `xchainpy2_thornode-1.132.0/test/test_trade_units_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_trade_units_response.py` & `xchainpy2_thornode-1.132.0/test/test_trade_units_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_transactions_api.py` & `xchainpy2_thornode-1.132.0/test/test_transactions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_tss_api.py` & `xchainpy2_thornode-1.132.0/test/test_tss_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
@@ -24,14 +24,20 @@
 
     def setUp(self):
         self.api = TSSApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
+    def test_keygen_pubkey(self):
+        """Test case for keygen_pubkey
+
+        """
+        pass
+
     def test_keysign(self):
         """Test case for keysign
 
         """
         pass
 
     def test_keysign_pubkey(self):
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_tss_keysign_metric.py` & `xchainpy2_thornode-1.132.0/test/test_tss_keysign_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_tss_metric.py` & `xchainpy2_thornode-1.132.0/test/test_tss_metric.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_tx.py` & `xchainpy2_thornode-1.132.0/test/test_tx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_tx_details_response.py` & `xchainpy2_thornode-1.132.0/test/test_tx_out_item.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.tx_details_response import TxDetailsResponse  # noqa: E501
+from xchainpy2_thornode.models.tx_out_item import TxOutItem  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestTxDetailsResponse(unittest.TestCase):
-    """TxDetailsResponse unit test stubs"""
+class TestTxOutItem(unittest.TestCase):
+    """TxOutItem unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTxDetailsResponse(self):
-        """Test TxDetailsResponse"""
+    def testTxOutItem(self):
+        """Test TxOutItem"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.tx_details_response.TxDetailsResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.tx_out_item.TxOutItem()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_tx_out_item.py` & `xchainpy2_thornode-1.132.0/test/test_tx_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.tx_out_item import TxOutItem  # noqa: E501
+from xchainpy2_thornode.models.tx_response import TxResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestTxOutItem(unittest.TestCase):
-    """TxOutItem unit test stubs"""
+class TestTxResponse(unittest.TestCase):
+    """TxResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTxOutItem(self):
-        """Test TxOutItem"""
+    def testTxResponse(self):
+        """Test TxResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.tx_out_item.TxOutItem()  # noqa: E501
+        # model = xchainpy2_thornode.models.tx_response.TxResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_tx_response.py` & `xchainpy2_thornode-1.132.0/test/test_swap_queue_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.tx_response import TxResponse  # noqa: E501
+from xchainpy2_thornode.models.swap_queue_response import SwapQueueResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestTxResponse(unittest.TestCase):
-    """TxResponse unit test stubs"""
+class TestSwapQueueResponse(unittest.TestCase):
+    """SwapQueueResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTxResponse(self):
-        """Test TxResponse"""
+    def testSwapQueueResponse(self):
+        """Test SwapQueueResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.tx_response.TxResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.swap_queue_response.SwapQueueResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_tx_signers_response.py` & `xchainpy2_thornode-1.132.0/test/test_outbound_fees_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.tx_signers_response import TxSignersResponse  # noqa: E501
+from xchainpy2_thornode.models.outbound_fees_response import OutboundFeesResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestTxSignersResponse(unittest.TestCase):
-    """TxSignersResponse unit test stubs"""
+class TestOutboundFeesResponse(unittest.TestCase):
+    """OutboundFeesResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTxSignersResponse(self):
-        """Test TxSignersResponse"""
+    def testOutboundFeesResponse(self):
+        """Test OutboundFeesResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.tx_signers_response.TxSignersResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.outbound_fees_response.OutboundFeesResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_tx_stages_response.py` & `xchainpy2_thornode-1.132.0/test/test_tx_stages_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_tx_stages_response_inbound_confirmation_counted.py` & `xchainpy2_thornode-1.132.0/test/test_inbound_confirmation_counted_stage.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.tx_stages_response_inbound_confirmation_counted import TxStagesResponseInboundConfirmationCounted  # noqa: E501
+from xchainpy2_thornode.models.inbound_confirmation_counted_stage import InboundConfirmationCountedStage  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestTxStagesResponseInboundConfirmationCounted(unittest.TestCase):
-    """TxStagesResponseInboundConfirmationCounted unit test stubs"""
+class TestInboundConfirmationCountedStage(unittest.TestCase):
+    """InboundConfirmationCountedStage unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTxStagesResponseInboundConfirmationCounted(self):
-        """Test TxStagesResponseInboundConfirmationCounted"""
+    def testInboundConfirmationCountedStage(self):
+        """Test InboundConfirmationCountedStage"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.tx_stages_response_inbound_confirmation_counted.TxStagesResponseInboundConfirmationCounted()  # noqa: E501
+        # model = xchainpy2_thornode.models.inbound_confirmation_counted_stage.InboundConfirmationCountedStage()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_tx_stages_response_inbound_finalised.py` & `xchainpy2_thornode-1.132.0/test/test_inbound_finalised_stage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.tx_stages_response_inbound_finalised import TxStagesResponseInboundFinalised  # noqa: E501
+from xchainpy2_thornode.models.inbound_finalised_stage import InboundFinalisedStage  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestTxStagesResponseInboundFinalised(unittest.TestCase):
-    """TxStagesResponseInboundFinalised unit test stubs"""
+class TestInboundFinalisedStage(unittest.TestCase):
+    """InboundFinalisedStage unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTxStagesResponseInboundFinalised(self):
-        """Test TxStagesResponseInboundFinalised"""
+    def testInboundFinalisedStage(self):
+        """Test InboundFinalisedStage"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.tx_stages_response_inbound_finalised.TxStagesResponseInboundFinalised()  # noqa: E501
+        # model = xchainpy2_thornode.models.inbound_finalised_stage.InboundFinalisedStage()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_tx_stages_response_inbound_observed.py` & `xchainpy2_thornode-1.132.0/test/test_streaming_status.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.tx_stages_response_inbound_observed import TxStagesResponseInboundObserved  # noqa: E501
+from xchainpy2_thornode.models.streaming_status import StreamingStatus  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestTxStagesResponseInboundObserved(unittest.TestCase):
-    """TxStagesResponseInboundObserved unit test stubs"""
+class TestStreamingStatus(unittest.TestCase):
+    """StreamingStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTxStagesResponseInboundObserved(self):
-        """Test TxStagesResponseInboundObserved"""
+    def testStreamingStatus(self):
+        """Test StreamingStatus"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.tx_stages_response_inbound_observed.TxStagesResponseInboundObserved()  # noqa: E501
+        # model = xchainpy2_thornode.models.streaming_status.StreamingStatus()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_tx_stages_response_outbound_delay.py` & `xchainpy2_thornode-1.132.0/test/test_outbound_delay_stage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.tx_stages_response_outbound_delay import TxStagesResponseOutboundDelay  # noqa: E501
+from xchainpy2_thornode.models.outbound_delay_stage import OutboundDelayStage  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestTxStagesResponseOutboundDelay(unittest.TestCase):
-    """TxStagesResponseOutboundDelay unit test stubs"""
+class TestOutboundDelayStage(unittest.TestCase):
+    """OutboundDelayStage unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTxStagesResponseOutboundDelay(self):
-        """Test TxStagesResponseOutboundDelay"""
+    def testOutboundDelayStage(self):
+        """Test OutboundDelayStage"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.tx_stages_response_outbound_delay.TxStagesResponseOutboundDelay()  # noqa: E501
+        # model = xchainpy2_thornode.models.outbound_delay_stage.OutboundDelayStage()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_tx_stages_response_swap_finalised.py` & `xchainpy2_thornode-1.132.0/test/test_yggdrasil_vaults_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.tx_stages_response_swap_finalised import TxStagesResponseSwapFinalised  # noqa: E501
+from xchainpy2_thornode.models.yggdrasil_vaults_response import YggdrasilVaultsResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestTxStagesResponseSwapFinalised(unittest.TestCase):
-    """TxStagesResponseSwapFinalised unit test stubs"""
+class TestYggdrasilVaultsResponse(unittest.TestCase):
+    """YggdrasilVaultsResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTxStagesResponseSwapFinalised(self):
-        """Test TxStagesResponseSwapFinalised"""
+    def testYggdrasilVaultsResponse(self):
+        """Test YggdrasilVaultsResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.tx_stages_response_swap_finalised.TxStagesResponseSwapFinalised()  # noqa: E501
+        # model = xchainpy2_thornode.models.yggdrasil_vaults_response.YggdrasilVaultsResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_tx_stages_response_swap_status.py` & `xchainpy2_thornode-1.132.0/test/test_inline_response200.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.tx_stages_response_swap_status import TxStagesResponseSwapStatus  # noqa: E501
+from xchainpy2_thornode.models.inline_response200 import InlineResponse200  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestTxStagesResponseSwapStatus(unittest.TestCase):
-    """TxStagesResponseSwapStatus unit test stubs"""
+class TestInlineResponse200(unittest.TestCase):
+    """InlineResponse200 unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTxStagesResponseSwapStatus(self):
-        """Test TxStagesResponseSwapStatus"""
+    def testInlineResponse200(self):
+        """Test InlineResponse200"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.tx_stages_response_swap_status.TxStagesResponseSwapStatus()  # noqa: E501
+        # model = xchainpy2_thornode.models.inline_response200.InlineResponse200()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_tx_stages_response_swap_status_streaming.py` & `xchainpy2_thornode-1.132.0/test/test_vault_pubkeys_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.tx_stages_response_swap_status_streaming import TxStagesResponseSwapStatusStreaming  # noqa: E501
+from xchainpy2_thornode.models.vault_pubkeys_response import VaultPubkeysResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestTxStagesResponseSwapStatusStreaming(unittest.TestCase):
-    """TxStagesResponseSwapStatusStreaming unit test stubs"""
+class TestVaultPubkeysResponse(unittest.TestCase):
+    """VaultPubkeysResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTxStagesResponseSwapStatusStreaming(self):
-        """Test TxStagesResponseSwapStatusStreaming"""
+    def testVaultPubkeysResponse(self):
+        """Test VaultPubkeysResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.tx_stages_response_swap_status_streaming.TxStagesResponseSwapStatusStreaming()  # noqa: E501
+        # model = xchainpy2_thornode.models.vault_pubkeys_response.VaultPubkeysResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_tx_status_response.py` & `xchainpy2_thornode-1.132.0/test/test_vault_router.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.tx_status_response import TxStatusResponse  # noqa: E501
+from xchainpy2_thornode.models.vault_router import VaultRouter  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestTxStatusResponse(unittest.TestCase):
-    """TxStatusResponse unit test stubs"""
+class TestVaultRouter(unittest.TestCase):
+    """VaultRouter unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTxStatusResponse(self):
-        """Test TxStatusResponse"""
+    def testVaultRouter(self):
+        """Test VaultRouter"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.tx_status_response.TxStatusResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.vault_router.VaultRouter()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_vault.py` & `xchainpy2_thornode-1.132.0/test/test_vault.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_vault_address.py` & `xchainpy2_thornode-1.132.0/test/test_vault_address.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_vault_info.py` & `xchainpy2_thornode-1.132.0/test/test_vault_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_vault_pubkeys_response.py` & `xchainpy2_thornode-1.132.0/test/test_vaults_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.vault_pubkeys_response import VaultPubkeysResponse  # noqa: E501
+from xchainpy2_thornode.models.vaults_response import VaultsResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestVaultPubkeysResponse(unittest.TestCase):
-    """VaultPubkeysResponse unit test stubs"""
+class TestVaultsResponse(unittest.TestCase):
+    """VaultsResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testVaultPubkeysResponse(self):
-        """Test VaultPubkeysResponse"""
+    def testVaultsResponse(self):
+        """Test VaultsResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.vault_pubkeys_response.VaultPubkeysResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.vaults_response.VaultsResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_vault_response.py` & `xchainpy2_thornode-1.132.0/test/test_vault_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_vault_router.py` & `xchainpy2_thornode-1.132.0/test/test_yggdrasil_vault.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.vault_router import VaultRouter  # noqa: E501
+from xchainpy2_thornode.models.yggdrasil_vault import YggdrasilVault  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestVaultRouter(unittest.TestCase):
-    """VaultRouter unit test stubs"""
+class TestYggdrasilVault(unittest.TestCase):
+    """YggdrasilVault unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testVaultRouter(self):
-        """Test VaultRouter"""
+    def testYggdrasilVault(self):
+        """Test YggdrasilVault"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.vault_router.VaultRouter()  # noqa: E501
+        # model = xchainpy2_thornode.models.yggdrasil_vault.YggdrasilVault()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_vaults_api.py` & `xchainpy2_thornode-1.132.0/test/test_vaults_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_vaults_response.py` & `xchainpy2_thornode-1.132.0/test/test_outbound_fee.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.vaults_response import VaultsResponse  # noqa: E501
+from xchainpy2_thornode.models.outbound_fee import OutboundFee  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestVaultsResponse(unittest.TestCase):
-    """VaultsResponse unit test stubs"""
+class TestOutboundFee(unittest.TestCase):
+    """OutboundFee unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testVaultsResponse(self):
-        """Test VaultsResponse"""
+    def testOutboundFee(self):
+        """Test OutboundFee"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.vaults_response.VaultsResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.outbound_fee.OutboundFee()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.130.1/test/test_version_response.py` & `xchainpy2_thornode-1.132.0/test/test_version_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/__init__.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import apis into sdk package
@@ -21,14 +21,15 @@
 from xchainpy2_thornode.api.health_api import HealthApi
 from xchainpy2_thornode.api.invariants_api import InvariantsApi
 from xchainpy2_thornode.api.liquidity_providers_api import LiquidityProvidersApi
 from xchainpy2_thornode.api.mimir_api import MimirApi
 from xchainpy2_thornode.api.network_api import NetworkApi
 from xchainpy2_thornode.api.nodes_api import NodesApi
 from xchainpy2_thornode.api.pol_api import POLApi
+from xchainpy2_thornode.api.pool_slip_api import PoolSlipApi
 from xchainpy2_thornode.api.pools_api import PoolsApi
 from xchainpy2_thornode.api.queue_api import QueueApi
 from xchainpy2_thornode.api.quote_api import QuoteApi
 from xchainpy2_thornode.api.savers_api import SaversApi
 from xchainpy2_thornode.api.streaming_swap_api import StreamingSwapApi
 from xchainpy2_thornode.api.tss_api import TSSApi
 from xchainpy2_thornode.api.thornames_api import ThornamesApi
@@ -58,18 +59,25 @@
 from xchainpy2_thornode.models.coin import Coin
 from xchainpy2_thornode.models.constants_response import ConstantsResponse
 from xchainpy2_thornode.models.derived_pool import DerivedPool
 from xchainpy2_thornode.models.derived_pool_response import DerivedPoolResponse
 from xchainpy2_thornode.models.derived_pools_response import DerivedPoolsResponse
 from xchainpy2_thornode.models.inbound_address import InboundAddress
 from xchainpy2_thornode.models.inbound_addresses_response import InboundAddressesResponse
+from xchainpy2_thornode.models.inbound_confirmation_counted_stage import InboundConfirmationCountedStage
+from xchainpy2_thornode.models.inbound_finalised_stage import InboundFinalisedStage
+from xchainpy2_thornode.models.inbound_observed_stage import InboundObservedStage
+from xchainpy2_thornode.models.inline_response200 import InlineResponse200
 from xchainpy2_thornode.models.invariant_response import InvariantResponse
 from xchainpy2_thornode.models.invariants_response import InvariantsResponse
+from xchainpy2_thornode.models.keygen import Keygen
+from xchainpy2_thornode.models.keygen_block import KeygenBlock
 from xchainpy2_thornode.models.keygen_metric import KeygenMetric
 from xchainpy2_thornode.models.keygen_metrics_response import KeygenMetricsResponse
+from xchainpy2_thornode.models.keygen_response import KeygenResponse
 from xchainpy2_thornode.models.keysign_info import KeysignInfo
 from xchainpy2_thornode.models.keysign_metrics import KeysignMetrics
 from xchainpy2_thornode.models.keysign_response import KeysignResponse
 from xchainpy2_thornode.models.last_block import LastBlock
 from xchainpy2_thornode.models.last_block_response import LastBlockResponse
 from xchainpy2_thornode.models.liquidity_provider import LiquidityProvider
 from xchainpy2_thornode.models.liquidity_provider_response import LiquidityProviderResponse
@@ -88,35 +96,44 @@
 from xchainpy2_thornode.models.node_jail import NodeJail
 from xchainpy2_thornode.models.node_keygen_metric import NodeKeygenMetric
 from xchainpy2_thornode.models.node_preflight_status import NodePreflightStatus
 from xchainpy2_thornode.models.node_pub_key_set import NodePubKeySet
 from xchainpy2_thornode.models.node_response import NodeResponse
 from xchainpy2_thornode.models.nodes_response import NodesResponse
 from xchainpy2_thornode.models.observed_tx import ObservedTx
+from xchainpy2_thornode.models.outbound_delay_stage import OutboundDelayStage
+from xchainpy2_thornode.models.outbound_fee import OutboundFee
+from xchainpy2_thornode.models.outbound_fees_response import OutboundFeesResponse
 from xchainpy2_thornode.models.outbound_response import OutboundResponse
+from xchainpy2_thornode.models.outbound_signed_stage import OutboundSignedStage
 from xchainpy2_thornode.models.pol_response import POLResponse
 from xchainpy2_thornode.models.ping import Ping
+from xchainpy2_thornode.models.planned_out_tx import PlannedOutTx
 from xchainpy2_thornode.models.pool import Pool
 from xchainpy2_thornode.models.pool_response import PoolResponse
+from xchainpy2_thornode.models.pool_slip_response import PoolSlipResponse
 from xchainpy2_thornode.models.pools_response import PoolsResponse
 from xchainpy2_thornode.models.queue_response import QueueResponse
 from xchainpy2_thornode.models.quote_fees import QuoteFees
 from xchainpy2_thornode.models.quote_loan_close_response import QuoteLoanCloseResponse
 from xchainpy2_thornode.models.quote_loan_open_response import QuoteLoanOpenResponse
 from xchainpy2_thornode.models.quote_saver_deposit_response import QuoteSaverDepositResponse
 from xchainpy2_thornode.models.quote_saver_withdraw_response import QuoteSaverWithdrawResponse
 from xchainpy2_thornode.models.quote_swap_response import QuoteSwapResponse
 from xchainpy2_thornode.models.saver import Saver
 from xchainpy2_thornode.models.saver_response import SaverResponse
 from xchainpy2_thornode.models.savers_response import SaversResponse
 from xchainpy2_thornode.models.scheduled_response import ScheduledResponse
+from xchainpy2_thornode.models.streaming_status import StreamingStatus
 from xchainpy2_thornode.models.streaming_swap import StreamingSwap
 from xchainpy2_thornode.models.streaming_swap_response import StreamingSwapResponse
 from xchainpy2_thornode.models.streaming_swaps_response import StreamingSwapsResponse
+from xchainpy2_thornode.models.swap_finalised_stage import SwapFinalisedStage
 from xchainpy2_thornode.models.swap_queue_response import SwapQueueResponse
+from xchainpy2_thornode.models.swap_status import SwapStatus
 from xchainpy2_thornode.models.swapper_clout_response import SwapperCloutResponse
 from xchainpy2_thornode.models.thorname import Thorname
 from xchainpy2_thornode.models.thorname_alias import ThornameAlias
 from xchainpy2_thornode.models.thorname_response import ThornameResponse
 from xchainpy2_thornode.models.trade_account_response import TradeAccountResponse
 from xchainpy2_thornode.models.trade_accounts_response import TradeAccountsResponse
 from xchainpy2_thornode.models.trade_unit_response import TradeUnitResponse
@@ -125,25 +142,18 @@
 from xchainpy2_thornode.models.tss_metric import TssMetric
 from xchainpy2_thornode.models.tx import Tx
 from xchainpy2_thornode.models.tx_details_response import TxDetailsResponse
 from xchainpy2_thornode.models.tx_out_item import TxOutItem
 from xchainpy2_thornode.models.tx_response import TxResponse
 from xchainpy2_thornode.models.tx_signers_response import TxSignersResponse
 from xchainpy2_thornode.models.tx_stages_response import TxStagesResponse
-from xchainpy2_thornode.models.tx_stages_response_inbound_confirmation_counted import TxStagesResponseInboundConfirmationCounted
-from xchainpy2_thornode.models.tx_stages_response_inbound_finalised import TxStagesResponseInboundFinalised
-from xchainpy2_thornode.models.tx_stages_response_inbound_observed import TxStagesResponseInboundObserved
-from xchainpy2_thornode.models.tx_stages_response_outbound_delay import TxStagesResponseOutboundDelay
-from xchainpy2_thornode.models.tx_stages_response_outbound_signed import TxStagesResponseOutboundSigned
-from xchainpy2_thornode.models.tx_stages_response_swap_finalised import TxStagesResponseSwapFinalised
-from xchainpy2_thornode.models.tx_stages_response_swap_status import TxStagesResponseSwapStatus
-from xchainpy2_thornode.models.tx_stages_response_swap_status_streaming import TxStagesResponseSwapStatusStreaming
 from xchainpy2_thornode.models.tx_status_response import TxStatusResponse
-from xchainpy2_thornode.models.tx_status_response_planned_out_txs import TxStatusResponsePlannedOutTxs
 from xchainpy2_thornode.models.vault import Vault
 from xchainpy2_thornode.models.vault_address import VaultAddress
 from xchainpy2_thornode.models.vault_info import VaultInfo
 from xchainpy2_thornode.models.vault_pubkeys_response import VaultPubkeysResponse
 from xchainpy2_thornode.models.vault_response import VaultResponse
 from xchainpy2_thornode.models.vault_router import VaultRouter
 from xchainpy2_thornode.models.vaults_response import VaultsResponse
 from xchainpy2_thornode.models.version_response import VersionResponse
+from xchainpy2_thornode.models.yggdrasil_vault import YggdrasilVault
+from xchainpy2_thornode.models.yggdrasil_vaults_response import YggdrasilVaultsResponse
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/__init__.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from xchainpy2_thornode.api.health_api import HealthApi
 from xchainpy2_thornode.api.invariants_api import InvariantsApi
 from xchainpy2_thornode.api.liquidity_providers_api import LiquidityProvidersApi
 from xchainpy2_thornode.api.mimir_api import MimirApi
 from xchainpy2_thornode.api.network_api import NetworkApi
 from xchainpy2_thornode.api.nodes_api import NodesApi
 from xchainpy2_thornode.api.pol_api import POLApi
+from xchainpy2_thornode.api.pool_slip_api import PoolSlipApi
 from xchainpy2_thornode.api.pools_api import PoolsApi
 from xchainpy2_thornode.api.queue_api import QueueApi
 from xchainpy2_thornode.api.quote_api import QuoteApi
 from xchainpy2_thornode.api.savers_api import SaversApi
 from xchainpy2_thornode.api.streaming_swap_api import StreamingSwapApi
 from xchainpy2_thornode.api.tss_api import TSSApi
 from xchainpy2_thornode.api.thornames_api import ThornamesApi
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/block_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/block_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/borrowers_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/borrowers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/clout_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/clout_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/health_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/health_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/invariants_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/invariants_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/liquidity_providers_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/liquidity_providers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/mimir_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/mimir_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/network_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/network_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -590,14 +590,204 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def outbound_fee_asset(self, asset, **kwargs):  # noqa: E501
+        """outbound_fee_asset  # noqa: E501
+
+        Returns the outbound fee information for the provided asset.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.outbound_fee_asset(asset, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str asset: (required)
+        :param int height: optional block height, defaults to current tip
+        :return: list[OutboundFee]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.outbound_fee_asset_with_http_info(asset, **kwargs)  # noqa: E501
+        else:
+            (data) = self.outbound_fee_asset_with_http_info(asset, **kwargs)  # noqa: E501
+            return data
+
+    def outbound_fee_asset_with_http_info(self, asset, **kwargs):  # noqa: E501
+        """outbound_fee_asset  # noqa: E501
+
+        Returns the outbound fee information for the provided asset.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.outbound_fee_asset_with_http_info(asset, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str asset: (required)
+        :param int height: optional block height, defaults to current tip
+        :return: list[OutboundFee]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['asset', 'height']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method outbound_fee_asset" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'asset' is set
+        if ('asset' not in params or
+                params['asset'] is None):
+            raise ValueError("Missing the required parameter `asset` when calling `outbound_fee_asset`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'asset' in params:
+            path_params['asset'] = params['asset']  # noqa: E501
+
+        query_params = []
+        if 'height' in params:
+            query_params.append(('height', params['height']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = []  # noqa: E501
+
+        return self.api_client.call_api(
+            '/thorchain/outbound_fee/{asset}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[OutboundFee]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def outbound_fees(self, **kwargs):  # noqa: E501
+        """outbound_fees  # noqa: E501
+
+        Returns the last block information for all chains.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.outbound_fees(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param int height: optional block height, defaults to current tip
+        :return: list[OutboundFee]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.outbound_fees_with_http_info(**kwargs)  # noqa: E501
+        else:
+            (data) = self.outbound_fees_with_http_info(**kwargs)  # noqa: E501
+            return data
+
+    def outbound_fees_with_http_info(self, **kwargs):  # noqa: E501
+        """outbound_fees  # noqa: E501
+
+        Returns the last block information for all chains.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.outbound_fees_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param int height: optional block height, defaults to current tip
+        :return: list[OutboundFee]
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['height']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method outbound_fees" % key
+                )
+            params[key] = val
+        del params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'height' in params:
+            query_params.append(('height', params['height']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = []  # noqa: E501
+
+        return self.api_client.call_api(
+            '/thorchain/outbound_fees', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='list[OutboundFee]',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def ragnarok(self, **kwargs):  # noqa: E501
         """ragnarok  # noqa: E501
 
         Returns a boolean indicating whether the chain is in ragnarok.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.ragnarok(async_req=True)
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/nodes_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/nodes_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/pol_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/pol_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/pools_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/pools_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/queue_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/queue_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/quote_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/quote_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/savers_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/savers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/streaming_swap_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/streaming_swap_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/thornames_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/thornames_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/trade_account_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/trade_account_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/trade_accounts_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/trade_accounts_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/trade_unit_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/trade_unit_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/trade_units_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/trade_units_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/transactions_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/transactions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/tss_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/tss_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -28,14 +28,117 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
+    def keygen_pubkey(self, height, pubkey, **kwargs):  # noqa: E501
+        """keygen_pubkey  # noqa: E501
+
+        Returns keygen information for the provided height and pubkey - the pubkey being of one of the members of a keygen block for that height  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.keygen_pubkey(height, pubkey, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param int height: (required)
+        :param str pubkey: (required)
+        :return: KeygenResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.keygen_pubkey_with_http_info(height, pubkey, **kwargs)  # noqa: E501
+        else:
+            (data) = self.keygen_pubkey_with_http_info(height, pubkey, **kwargs)  # noqa: E501
+            return data
+
+    def keygen_pubkey_with_http_info(self, height, pubkey, **kwargs):  # noqa: E501
+        """keygen_pubkey  # noqa: E501
+
+        Returns keygen information for the provided height and pubkey - the pubkey being of one of the members of a keygen block for that height  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.keygen_pubkey_with_http_info(height, pubkey, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param int height: (required)
+        :param str pubkey: (required)
+        :return: KeygenResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['height', 'pubkey']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method keygen_pubkey" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'height' is set
+        if ('height' not in params or
+                params['height'] is None):
+            raise ValueError("Missing the required parameter `height` when calling `keygen_pubkey`")  # noqa: E501
+        # verify the required parameter 'pubkey' is set
+        if ('pubkey' not in params or
+                params['pubkey'] is None):
+            raise ValueError("Missing the required parameter `pubkey` when calling `keygen_pubkey`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'height' in params:
+            path_params['height'] = params['height']  # noqa: E501
+        if 'pubkey' in params:
+            path_params['pubkey'] = params['pubkey']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = []  # noqa: E501
+
+        return self.api_client.call_api(
+            '/thorchain/keygen/{height}/{pubkey}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='KeygenResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def keysign(self, height, **kwargs):  # noqa: E501
         """keysign  # noqa: E501
 
         Returns keysign information for the provided height - the height being the first block a tx out item appears in the signed-but-unobserved outbound queue.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.keysign(height, async_req=True)
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/vaults_api.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api/vaults_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -320,15 +320,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.yggdrasil(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int height: optional block height, defaults to current tip
-        :return: list[Vault]
+        :return: list[YggdrasilVault]
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.yggdrasil_with_http_info(**kwargs)  # noqa: E501
         else:
@@ -342,15 +342,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.yggdrasil_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int height: optional block height, defaults to current tip
-        :return: list[Vault]
+        :return: list[YggdrasilVault]
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['height']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -392,14 +392,14 @@
             '/thorchain/vaults/yggdrasil', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='list[Vault]',  # noqa: E501
+            response_type='list[YggdrasilVault]',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api_client.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
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
-        self.user_agent = 'Swagger-Codegen/1.130.1/python'
+        self.user_agent = 'Swagger-Codegen/1.132.0/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/configuration.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import copy
@@ -238,10 +238,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.130.1\n"\
-               "SDK Package Version: 1.130.1".\
+               "Version of the API: 1.132.0\n"\
+               "SDK Package Version: 1.132.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/__init__.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import models into model package
@@ -30,18 +30,25 @@
 from xchainpy2_thornode.models.coin import Coin
 from xchainpy2_thornode.models.constants_response import ConstantsResponse
 from xchainpy2_thornode.models.derived_pool import DerivedPool
 from xchainpy2_thornode.models.derived_pool_response import DerivedPoolResponse
 from xchainpy2_thornode.models.derived_pools_response import DerivedPoolsResponse
 from xchainpy2_thornode.models.inbound_address import InboundAddress
 from xchainpy2_thornode.models.inbound_addresses_response import InboundAddressesResponse
+from xchainpy2_thornode.models.inbound_confirmation_counted_stage import InboundConfirmationCountedStage
+from xchainpy2_thornode.models.inbound_finalised_stage import InboundFinalisedStage
+from xchainpy2_thornode.models.inbound_observed_stage import InboundObservedStage
+from xchainpy2_thornode.models.inline_response200 import InlineResponse200
 from xchainpy2_thornode.models.invariant_response import InvariantResponse
 from xchainpy2_thornode.models.invariants_response import InvariantsResponse
+from xchainpy2_thornode.models.keygen import Keygen
+from xchainpy2_thornode.models.keygen_block import KeygenBlock
 from xchainpy2_thornode.models.keygen_metric import KeygenMetric
 from xchainpy2_thornode.models.keygen_metrics_response import KeygenMetricsResponse
+from xchainpy2_thornode.models.keygen_response import KeygenResponse
 from xchainpy2_thornode.models.keysign_info import KeysignInfo
 from xchainpy2_thornode.models.keysign_metrics import KeysignMetrics
 from xchainpy2_thornode.models.keysign_response import KeysignResponse
 from xchainpy2_thornode.models.last_block import LastBlock
 from xchainpy2_thornode.models.last_block_response import LastBlockResponse
 from xchainpy2_thornode.models.liquidity_provider import LiquidityProvider
 from xchainpy2_thornode.models.liquidity_provider_response import LiquidityProviderResponse
@@ -60,35 +67,44 @@
 from xchainpy2_thornode.models.node_jail import NodeJail
 from xchainpy2_thornode.models.node_keygen_metric import NodeKeygenMetric
 from xchainpy2_thornode.models.node_preflight_status import NodePreflightStatus
 from xchainpy2_thornode.models.node_pub_key_set import NodePubKeySet
 from xchainpy2_thornode.models.node_response import NodeResponse
 from xchainpy2_thornode.models.nodes_response import NodesResponse
 from xchainpy2_thornode.models.observed_tx import ObservedTx
+from xchainpy2_thornode.models.outbound_delay_stage import OutboundDelayStage
+from xchainpy2_thornode.models.outbound_fee import OutboundFee
+from xchainpy2_thornode.models.outbound_fees_response import OutboundFeesResponse
 from xchainpy2_thornode.models.outbound_response import OutboundResponse
+from xchainpy2_thornode.models.outbound_signed_stage import OutboundSignedStage
 from xchainpy2_thornode.models.pol_response import POLResponse
 from xchainpy2_thornode.models.ping import Ping
+from xchainpy2_thornode.models.planned_out_tx import PlannedOutTx
 from xchainpy2_thornode.models.pool import Pool
 from xchainpy2_thornode.models.pool_response import PoolResponse
+from xchainpy2_thornode.models.pool_slip_response import PoolSlipResponse
 from xchainpy2_thornode.models.pools_response import PoolsResponse
 from xchainpy2_thornode.models.queue_response import QueueResponse
 from xchainpy2_thornode.models.quote_fees import QuoteFees
 from xchainpy2_thornode.models.quote_loan_close_response import QuoteLoanCloseResponse
 from xchainpy2_thornode.models.quote_loan_open_response import QuoteLoanOpenResponse
 from xchainpy2_thornode.models.quote_saver_deposit_response import QuoteSaverDepositResponse
 from xchainpy2_thornode.models.quote_saver_withdraw_response import QuoteSaverWithdrawResponse
 from xchainpy2_thornode.models.quote_swap_response import QuoteSwapResponse
 from xchainpy2_thornode.models.saver import Saver
 from xchainpy2_thornode.models.saver_response import SaverResponse
 from xchainpy2_thornode.models.savers_response import SaversResponse
 from xchainpy2_thornode.models.scheduled_response import ScheduledResponse
+from xchainpy2_thornode.models.streaming_status import StreamingStatus
 from xchainpy2_thornode.models.streaming_swap import StreamingSwap
 from xchainpy2_thornode.models.streaming_swap_response import StreamingSwapResponse
 from xchainpy2_thornode.models.streaming_swaps_response import StreamingSwapsResponse
+from xchainpy2_thornode.models.swap_finalised_stage import SwapFinalisedStage
 from xchainpy2_thornode.models.swap_queue_response import SwapQueueResponse
+from xchainpy2_thornode.models.swap_status import SwapStatus
 from xchainpy2_thornode.models.swapper_clout_response import SwapperCloutResponse
 from xchainpy2_thornode.models.thorname import Thorname
 from xchainpy2_thornode.models.thorname_alias import ThornameAlias
 from xchainpy2_thornode.models.thorname_response import ThornameResponse
 from xchainpy2_thornode.models.trade_account_response import TradeAccountResponse
 from xchainpy2_thornode.models.trade_accounts_response import TradeAccountsResponse
 from xchainpy2_thornode.models.trade_unit_response import TradeUnitResponse
@@ -97,25 +113,18 @@
 from xchainpy2_thornode.models.tss_metric import TssMetric
 from xchainpy2_thornode.models.tx import Tx
 from xchainpy2_thornode.models.tx_details_response import TxDetailsResponse
 from xchainpy2_thornode.models.tx_out_item import TxOutItem
 from xchainpy2_thornode.models.tx_response import TxResponse
 from xchainpy2_thornode.models.tx_signers_response import TxSignersResponse
 from xchainpy2_thornode.models.tx_stages_response import TxStagesResponse
-from xchainpy2_thornode.models.tx_stages_response_inbound_confirmation_counted import TxStagesResponseInboundConfirmationCounted
-from xchainpy2_thornode.models.tx_stages_response_inbound_finalised import TxStagesResponseInboundFinalised
-from xchainpy2_thornode.models.tx_stages_response_inbound_observed import TxStagesResponseInboundObserved
-from xchainpy2_thornode.models.tx_stages_response_outbound_delay import TxStagesResponseOutboundDelay
-from xchainpy2_thornode.models.tx_stages_response_outbound_signed import TxStagesResponseOutboundSigned
-from xchainpy2_thornode.models.tx_stages_response_swap_finalised import TxStagesResponseSwapFinalised
-from xchainpy2_thornode.models.tx_stages_response_swap_status import TxStagesResponseSwapStatus
-from xchainpy2_thornode.models.tx_stages_response_swap_status_streaming import TxStagesResponseSwapStatusStreaming
 from xchainpy2_thornode.models.tx_status_response import TxStatusResponse
-from xchainpy2_thornode.models.tx_status_response_planned_out_txs import TxStatusResponsePlannedOutTxs
 from xchainpy2_thornode.models.vault import Vault
 from xchainpy2_thornode.models.vault_address import VaultAddress
 from xchainpy2_thornode.models.vault_info import VaultInfo
 from xchainpy2_thornode.models.vault_pubkeys_response import VaultPubkeysResponse
 from xchainpy2_thornode.models.vault_response import VaultResponse
 from xchainpy2_thornode.models.vault_router import VaultRouter
 from xchainpy2_thornode.models.vaults_response import VaultsResponse
 from xchainpy2_thornode.models.version_response import VersionResponse
+from xchainpy2_thornode.models.yggdrasil_vault import YggdrasilVault
+from xchainpy2_thornode.models.yggdrasil_vaults_response import YggdrasilVaultsResponse
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/ban_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/ban_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/base_quote_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/base_quote_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -37,15 +37,17 @@
         'slippage_bps': 'int',
         'streaming_slippage_bps': 'int',
         'router': 'str',
         'expiry': 'int',
         'warning': 'str',
         'notes': 'str',
         'dust_threshold': 'str',
-        'recommended_min_amount_in': 'str'
+        'recommended_min_amount_in': 'str',
+        'recommended_gas_rate': 'str',
+        'gas_rate_units': 'str'
     }
 
     attribute_map = {
         'inbound_address': 'inbound_address',
         'inbound_confirmation_blocks': 'inbound_confirmation_blocks',
         'inbound_confirmation_seconds': 'inbound_confirmation_seconds',
         'outbound_delay_blocks': 'outbound_delay_blocks',
@@ -54,18 +56,20 @@
         'slippage_bps': 'slippage_bps',
         'streaming_slippage_bps': 'streaming_slippage_bps',
         'router': 'router',
         'expiry': 'expiry',
         'warning': 'warning',
         'notes': 'notes',
         'dust_threshold': 'dust_threshold',
-        'recommended_min_amount_in': 'recommended_min_amount_in'
+        'recommended_min_amount_in': 'recommended_min_amount_in',
+        'recommended_gas_rate': 'recommended_gas_rate',
+        'gas_rate_units': 'gas_rate_units'
     }
 
-    def __init__(self, inbound_address=None, inbound_confirmation_blocks=None, inbound_confirmation_seconds=None, outbound_delay_blocks=None, outbound_delay_seconds=None, fees=None, slippage_bps=None, streaming_slippage_bps=None, router=None, expiry=None, warning=None, notes=None, dust_threshold=None, recommended_min_amount_in=None):  # noqa: E501
+    def __init__(self, inbound_address=None, inbound_confirmation_blocks=None, inbound_confirmation_seconds=None, outbound_delay_blocks=None, outbound_delay_seconds=None, fees=None, slippage_bps=None, streaming_slippage_bps=None, router=None, expiry=None, warning=None, notes=None, dust_threshold=None, recommended_min_amount_in=None, recommended_gas_rate=None, gas_rate_units=None):  # noqa: E501
         """BaseQuoteResponse - a model defined in Swagger"""  # noqa: E501
         self._inbound_address = None
         self._inbound_confirmation_blocks = None
         self._inbound_confirmation_seconds = None
         self._outbound_delay_blocks = None
         self._outbound_delay_seconds = None
         self._fees = None
@@ -73,14 +77,16 @@
         self._streaming_slippage_bps = None
         self._router = None
         self._expiry = None
         self._warning = None
         self._notes = None
         self._dust_threshold = None
         self._recommended_min_amount_in = None
+        self._recommended_gas_rate = None
+        self._gas_rate_units = None
         self.discriminator = None
         if inbound_address is not None:
             self.inbound_address = inbound_address
         if inbound_confirmation_blocks is not None:
             self.inbound_confirmation_blocks = inbound_confirmation_blocks
         if inbound_confirmation_seconds is not None:
             self.inbound_confirmation_seconds = inbound_confirmation_seconds
@@ -102,14 +108,18 @@
             self.warning = warning
         if notes is not None:
             self.notes = notes
         if dust_threshold is not None:
             self.dust_threshold = dust_threshold
         if recommended_min_amount_in is not None:
             self.recommended_min_amount_in = recommended_min_amount_in
+        if recommended_gas_rate is not None:
+            self.recommended_gas_rate = recommended_gas_rate
+        if gas_rate_units is not None:
+            self.gas_rate_units = gas_rate_units
 
     @property
     def inbound_address(self):
         """Gets the inbound_address of this BaseQuoteResponse.  # noqa: E501
 
         the inbound address for the transaction on the source chain  # noqa: E501
 
@@ -423,14 +433,60 @@
 
         :param recommended_min_amount_in: The recommended_min_amount_in of this BaseQuoteResponse.  # noqa: E501
         :type: str
         """
 
         self._recommended_min_amount_in = recommended_min_amount_in
 
+    @property
+    def recommended_gas_rate(self):
+        """Gets the recommended_gas_rate of this BaseQuoteResponse.  # noqa: E501
+
+        the recommended gas rate to use for the inbound to ensure timely confirmation  # noqa: E501
+
+        :return: The recommended_gas_rate of this BaseQuoteResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._recommended_gas_rate
+
+    @recommended_gas_rate.setter
+    def recommended_gas_rate(self, recommended_gas_rate):
+        """Sets the recommended_gas_rate of this BaseQuoteResponse.
+
+        the recommended gas rate to use for the inbound to ensure timely confirmation  # noqa: E501
+
+        :param recommended_gas_rate: The recommended_gas_rate of this BaseQuoteResponse.  # noqa: E501
+        :type: str
+        """
+
+        self._recommended_gas_rate = recommended_gas_rate
+
+    @property
+    def gas_rate_units(self):
+        """Gets the gas_rate_units of this BaseQuoteResponse.  # noqa: E501
+
+        the units of the recommended gas rate  # noqa: E501
+
+        :return: The gas_rate_units of this BaseQuoteResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._gas_rate_units
+
+    @gas_rate_units.setter
+    def gas_rate_units(self, gas_rate_units):
+        """Sets the gas_rate_units of this BaseQuoteResponse.
+
+        the units of the recommended gas rate  # noqa: E501
+
+        :param gas_rate_units: The gas_rate_units of this BaseQuoteResponse.  # noqa: E501
+        :type: str
+        """
+
+        self._gas_rate_units = gas_rate_units
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/block_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response_header.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/block_response_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response_header_version.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/block_response_header_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response_id.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/block_response_id.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response_id_parts.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/block_response_id_parts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_tx.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/block_tx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_tx_result.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/block_tx_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/borrower.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/borrower.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/borrower_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/borrower_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/borrowers_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/borrowers_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/chain_height.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/chain_height.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/coin.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/coin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/constants_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/constants_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/derived_pool.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/derived_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/derived_pool_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/derived_pool_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/derived_pools_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/derived_pools_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/inbound_address.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/inbound_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/inbound_addresses_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/inbound_addresses_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/invariant_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/invariant_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/invariants_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/invariants_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keygen_metric.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/keygen_metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keygen_metrics_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/keygen_metrics_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keysign_info.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/keysign_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keysign_metrics.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/keysign_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keysign_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/keysign_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -38,18 +38,16 @@
     }
 
     def __init__(self, keysign=None, signature=None):  # noqa: E501
         """KeysignResponse - a model defined in Swagger"""  # noqa: E501
         self._keysign = None
         self._signature = None
         self.discriminator = None
-        if keysign is not None:
-            self.keysign = keysign
-        if signature is not None:
-            self.signature = signature
+        self.keysign = keysign
+        self.signature = signature
 
     @property
     def keysign(self):
         """Gets the keysign of this KeysignResponse.  # noqa: E501
 
 
         :return: The keysign of this KeysignResponse.  # noqa: E501
@@ -61,14 +59,16 @@
     def keysign(self, keysign):
         """Sets the keysign of this KeysignResponse.
 
 
         :param keysign: The keysign of this KeysignResponse.  # noqa: E501
         :type: KeysignInfo
         """
+        if keysign is None:
+            raise ValueError("Invalid value for `keysign`, must not be `None`")  # noqa: E501
 
         self._keysign = keysign
 
     @property
     def signature(self):
         """Gets the signature of this KeysignResponse.  # noqa: E501
 
@@ -82,14 +82,16 @@
     def signature(self, signature):
         """Sets the signature of this KeysignResponse.
 
 
         :param signature: The signature of this KeysignResponse.  # noqa: E501
         :type: str
         """
+        if signature is None:
+            raise ValueError("Invalid value for `signature`, must not be `None`")  # noqa: E501
 
         self._signature = signature
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/last_block.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/last_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/last_block_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/last_block_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/liquidity_provider.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/liquidity_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -96,19 +96,24 @@
         self.units = units
         self.pending_rune = pending_rune
         self.pending_asset = pending_asset
         if pending_tx_id is not None:
             self.pending_tx_id = pending_tx_id
         self.rune_deposit_value = rune_deposit_value
         self.asset_deposit_value = asset_deposit_value
-        self.rune_redeem_value = rune_redeem_value
-        self.asset_redeem_value = asset_redeem_value
-        self.luvi_deposit_value = luvi_deposit_value
-        self.luvi_redeem_value = luvi_redeem_value
-        self.luvi_growth_pct = luvi_growth_pct
+        if rune_redeem_value is not None:
+            self.rune_redeem_value = rune_redeem_value
+        if asset_redeem_value is not None:
+            self.asset_redeem_value = asset_redeem_value
+        if luvi_deposit_value is not None:
+            self.luvi_deposit_value = luvi_deposit_value
+        if luvi_redeem_value is not None:
+            self.luvi_redeem_value = luvi_redeem_value
+        if luvi_growth_pct is not None:
+            self.luvi_growth_pct = luvi_growth_pct
 
     @property
     def asset(self):
         """Gets the asset of this LiquidityProvider.  # noqa: E501
 
 
         :return: The asset of this LiquidityProvider.  # noqa: E501
@@ -363,16 +368,14 @@
     def rune_redeem_value(self, rune_redeem_value):
         """Sets the rune_redeem_value of this LiquidityProvider.
 
 
         :param rune_redeem_value: The rune_redeem_value of this LiquidityProvider.  # noqa: E501
         :type: str
         """
-        if rune_redeem_value is None:
-            raise ValueError("Invalid value for `rune_redeem_value`, must not be `None`")  # noqa: E501
 
         self._rune_redeem_value = rune_redeem_value
 
     @property
     def asset_redeem_value(self):
         """Gets the asset_redeem_value of this LiquidityProvider.  # noqa: E501
 
@@ -386,16 +389,14 @@
     def asset_redeem_value(self, asset_redeem_value):
         """Sets the asset_redeem_value of this LiquidityProvider.
 
 
         :param asset_redeem_value: The asset_redeem_value of this LiquidityProvider.  # noqa: E501
         :type: str
         """
-        if asset_redeem_value is None:
-            raise ValueError("Invalid value for `asset_redeem_value`, must not be `None`")  # noqa: E501
 
         self._asset_redeem_value = asset_redeem_value
 
     @property
     def luvi_deposit_value(self):
         """Gets the luvi_deposit_value of this LiquidityProvider.  # noqa: E501
 
@@ -409,16 +410,14 @@
     def luvi_deposit_value(self, luvi_deposit_value):
         """Sets the luvi_deposit_value of this LiquidityProvider.
 
 
         :param luvi_deposit_value: The luvi_deposit_value of this LiquidityProvider.  # noqa: E501
         :type: str
         """
-        if luvi_deposit_value is None:
-            raise ValueError("Invalid value for `luvi_deposit_value`, must not be `None`")  # noqa: E501
 
         self._luvi_deposit_value = luvi_deposit_value
 
     @property
     def luvi_redeem_value(self):
         """Gets the luvi_redeem_value of this LiquidityProvider.  # noqa: E501
 
@@ -432,16 +431,14 @@
     def luvi_redeem_value(self, luvi_redeem_value):
         """Sets the luvi_redeem_value of this LiquidityProvider.
 
 
         :param luvi_redeem_value: The luvi_redeem_value of this LiquidityProvider.  # noqa: E501
         :type: str
         """
-        if luvi_redeem_value is None:
-            raise ValueError("Invalid value for `luvi_redeem_value`, must not be `None`")  # noqa: E501
 
         self._luvi_redeem_value = luvi_redeem_value
 
     @property
     def luvi_growth_pct(self):
         """Gets the luvi_growth_pct of this LiquidityProvider.  # noqa: E501
 
@@ -455,16 +452,14 @@
     def luvi_growth_pct(self, luvi_growth_pct):
         """Sets the luvi_growth_pct of this LiquidityProvider.
 
 
         :param luvi_growth_pct: The luvi_growth_pct of this LiquidityProvider.  # noqa: E501
         :type: str
         """
-        if luvi_growth_pct is None:
-            raise ValueError("Invalid value for `luvi_growth_pct`, must not be `None`")  # noqa: E501
 
         self._luvi_growth_pct = luvi_growth_pct
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/liquidity_provider_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/liquidity_provider_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/liquidity_provider_summary.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/liquidity_provider_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/liquidity_providers_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/liquidity_providers_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/metrics_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/metrics_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/mimir_nodes_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/mimir_nodes_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/mimir_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/mimir_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/mimir_v2_ids_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/mimir_v2_ids_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -26,45 +26,44 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'id': 'ModelInt',
         'name': 'str',
-        'legacy_key': 'str',
         'vote_key': 'str',
-        'votes': 'object'
+        'legacy_key': 'str',
+        'type': 'str',
+        'votes': 'dict(str, int)'
     }
 
     attribute_map = {
         'id': 'id',
         'name': 'name',
-        'legacy_key': 'legacy_key',
         'vote_key': 'vote_key',
+        'legacy_key': 'legacy_key',
+        'type': 'type',
         'votes': 'votes'
     }
 
-    def __init__(self, id=None, name=None, legacy_key=None, vote_key=None, votes=None):  # noqa: E501
+    def __init__(self, id=None, name=None, vote_key=None, legacy_key=None, type=None, votes=None):  # noqa: E501
         """MimirV2IDsResponse - a model defined in Swagger"""  # noqa: E501
         self._id = None
         self._name = None
-        self._legacy_key = None
         self._vote_key = None
+        self._legacy_key = None
+        self._type = None
         self._votes = None
         self.discriminator = None
-        if id is not None:
-            self.id = id
-        if name is not None:
-            self.name = name
-        if legacy_key is not None:
-            self.legacy_key = legacy_key
-        if vote_key is not None:
-            self.vote_key = vote_key
-        if votes is not None:
-            self.votes = votes
+        self.id = id
+        self.name = name
+        self.vote_key = vote_key
+        self.legacy_key = legacy_key
+        self.type = type
+        self.votes = votes
 
     @property
     def id(self):
         """Gets the id of this MimirV2IDsResponse.  # noqa: E501
 
 
         :return: The id of this MimirV2IDsResponse.  # noqa: E501
@@ -76,14 +75,16 @@
     def id(self, id):
         """Sets the id of this MimirV2IDsResponse.
 
 
         :param id: The id of this MimirV2IDsResponse.  # noqa: E501
         :type: ModelInt
         """
+        if id is None:
+            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
         self._id = id
 
     @property
     def name(self):
         """Gets the name of this MimirV2IDsResponse.  # noqa: E501
 
@@ -97,18 +98,43 @@
     def name(self, name):
         """Sets the name of this MimirV2IDsResponse.
 
 
         :param name: The name of this MimirV2IDsResponse.  # noqa: E501
         :type: str
         """
+        if name is None:
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
+    def vote_key(self):
+        """Gets the vote_key of this MimirV2IDsResponse.  # noqa: E501
+
+
+        :return: The vote_key of this MimirV2IDsResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._vote_key
+
+    @vote_key.setter
+    def vote_key(self, vote_key):
+        """Sets the vote_key of this MimirV2IDsResponse.
+
+
+        :param vote_key: The vote_key of this MimirV2IDsResponse.  # noqa: E501
+        :type: str
+        """
+        if vote_key is None:
+            raise ValueError("Invalid value for `vote_key`, must not be `None`")  # noqa: E501
+
+        self._vote_key = vote_key
+
+    @property
     def legacy_key(self):
         """Gets the legacy_key of this MimirV2IDsResponse.  # noqa: E501
 
 
         :return: The legacy_key of this MimirV2IDsResponse.  # noqa: E501
         :rtype: str
         """
@@ -118,56 +144,62 @@
     def legacy_key(self, legacy_key):
         """Sets the legacy_key of this MimirV2IDsResponse.
 
 
         :param legacy_key: The legacy_key of this MimirV2IDsResponse.  # noqa: E501
         :type: str
         """
+        if legacy_key is None:
+            raise ValueError("Invalid value for `legacy_key`, must not be `None`")  # noqa: E501
 
         self._legacy_key = legacy_key
 
     @property
-    def vote_key(self):
-        """Gets the vote_key of this MimirV2IDsResponse.  # noqa: E501
+    def type(self):
+        """Gets the type of this MimirV2IDsResponse.  # noqa: E501
 
 
-        :return: The vote_key of this MimirV2IDsResponse.  # noqa: E501
+        :return: The type of this MimirV2IDsResponse.  # noqa: E501
         :rtype: str
         """
-        return self._vote_key
+        return self._type
 
-    @vote_key.setter
-    def vote_key(self, vote_key):
-        """Sets the vote_key of this MimirV2IDsResponse.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this MimirV2IDsResponse.
 
 
-        :param vote_key: The vote_key of this MimirV2IDsResponse.  # noqa: E501
+        :param type: The type of this MimirV2IDsResponse.  # noqa: E501
         :type: str
         """
+        if type is None:
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
 
-        self._vote_key = vote_key
+        self._type = type
 
     @property
     def votes(self):
         """Gets the votes of this MimirV2IDsResponse.  # noqa: E501
 
 
         :return: The votes of this MimirV2IDsResponse.  # noqa: E501
-        :rtype: object
+        :rtype: dict(str, int)
         """
         return self._votes
 
     @votes.setter
     def votes(self, votes):
         """Sets the votes of this MimirV2IDsResponse.
 
 
         :param votes: The votes of this MimirV2IDsResponse.  # noqa: E501
-        :type: object
+        :type: dict(str, int)
         """
+        if votes is None:
+            raise ValueError("Invalid value for `votes`, must not be `None`")  # noqa: E501
 
         self._votes = votes
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/mimir_vote.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/mimir_vote.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/msg_swap.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/msg_swap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -34,15 +34,15 @@
         'trade_target': 'str',
         'affiliate_address': 'str',
         'affiliate_basis_points': 'str',
         'signer': 'str',
         'aggregator': 'str',
         'aggregator_target_address': 'str',
         'aggregator_target_limit': 'str',
-        'order_type': 'int',
+        'order_type': 'str',
         'stream_quantity': 'int',
         'stream_interval': 'int'
     }
 
     attribute_map = {
         'tx': 'tx',
         'target_asset': 'target_asset',
@@ -334,29 +334,29 @@
 
         self._aggregator_target_limit = aggregator_target_limit
 
     @property
     def order_type(self):
         """Gets the order_type of this MsgSwap.  # noqa: E501
 
-        0 if a market order (immediately completed or refunded), 1 if a limit order (held until fulfillable)  # noqa: E501
+        market if immediately completed or refunded, limit if held until fulfillable  # noqa: E501
 
         :return: The order_type of this MsgSwap.  # noqa: E501
-        :rtype: int
+        :rtype: str
         """
         return self._order_type
 
     @order_type.setter
     def order_type(self, order_type):
         """Sets the order_type of this MsgSwap.
 
-        0 if a market order (immediately completed or refunded), 1 if a limit order (held until fulfillable)  # noqa: E501
+        market if immediately completed or refunded, limit if held until fulfillable  # noqa: E501
 
         :param order_type: The order_type of this MsgSwap.  # noqa: E501
-        :type: int
+        :type: str
         """
 
         self._order_type = order_type
 
     @property
     def stream_quantity(self):
         """Gets the stream_quantity of this MsgSwap.  # noqa: E501
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/network_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/network_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_bond_provider.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/node_bond_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_bond_providers.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/node_bond_providers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -25,31 +25,29 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'node_operator_fee': 'str',
-        'providers': 'NodeBondProvider'
+        'providers': 'list[NodeBondProvider]'
     }
 
     attribute_map = {
         'node_operator_fee': 'node_operator_fee',
         'providers': 'providers'
     }
 
     def __init__(self, node_operator_fee=None, providers=None):  # noqa: E501
         """NodeBondProviders - a model defined in Swagger"""  # noqa: E501
         self._node_operator_fee = None
         self._providers = None
         self.discriminator = None
-        if node_operator_fee is not None:
-            self.node_operator_fee = node_operator_fee
-        if providers is not None:
-            self.providers = providers
+        self.node_operator_fee = node_operator_fee
+        self.providers = providers
 
     @property
     def node_operator_fee(self):
         """Gets the node_operator_fee of this NodeBondProviders.  # noqa: E501
 
         node operator fee in basis points  # noqa: E501
 
@@ -63,35 +61,41 @@
         """Sets the node_operator_fee of this NodeBondProviders.
 
         node operator fee in basis points  # noqa: E501
 
         :param node_operator_fee: The node_operator_fee of this NodeBondProviders.  # noqa: E501
         :type: str
         """
+        if node_operator_fee is None:
+            raise ValueError("Invalid value for `node_operator_fee`, must not be `None`")  # noqa: E501
 
         self._node_operator_fee = node_operator_fee
 
     @property
     def providers(self):
         """Gets the providers of this NodeBondProviders.  # noqa: E501
 
+        all the bond providers for the node  # noqa: E501
 
         :return: The providers of this NodeBondProviders.  # noqa: E501
-        :rtype: NodeBondProvider
+        :rtype: list[NodeBondProvider]
         """
         return self._providers
 
     @providers.setter
     def providers(self, providers):
         """Sets the providers of this NodeBondProviders.
 
+        all the bond providers for the node  # noqa: E501
 
         :param providers: The providers of this NodeBondProviders.  # noqa: E501
-        :type: NodeBondProvider
+        :type: list[NodeBondProvider]
         """
+        if providers is None:
+            raise ValueError("Invalid value for `providers`, must not be `None`")  # noqa: E501
 
         self._providers = providers
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_jail.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/node_jail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_keygen_metric.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/node_keygen_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_preflight_status.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/node_preflight_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_pub_key_set.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/node_pub_key_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/pool_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class NodeResponse(object):
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
-        """NodeResponse - a model defined in Swagger"""  # noqa: E501
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
-        if issubclass(NodeResponse, dict):
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
-        if not isinstance(other, NodeResponse):
+        if not isinstance(other, PoolResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/nodes_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/nodes_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/observed_tx.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/observed_tx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/outbound_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/outbound_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/ping.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/ping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/pol_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/pol_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/pool.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/pool_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/pools_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class PoolResponse(object):
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
-        """PoolResponse - a model defined in Swagger"""  # noqa: E501
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
-        if issubclass(PoolResponse, dict):
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
-        if not isinstance(other, PoolResponse):
+        if not isinstance(other, PoolsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/pools_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/streaming_swaps_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class PoolsResponse(object):
+class StreamingSwapsResponse(object):
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
+        """StreamingSwapsResponse - a model defined in Swagger"""  # noqa: E501
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
+        if issubclass(StreamingSwapsResponse, dict):
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
+        if not isinstance(other, StreamingSwapsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/queue_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/queue_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_fees.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/quote_fees.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_loan_close_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/quote_loan_close_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -38,14 +38,16 @@
         'streaming_slippage_bps': 'int',
         'router': 'str',
         'expiry': 'int',
         'warning': 'str',
         'notes': 'str',
         'dust_threshold': 'str',
         'recommended_min_amount_in': 'str',
+        'recommended_gas_rate': 'str',
+        'gas_rate_units': 'str',
         'memo': 'str',
         'expected_amount_out': 'str',
         'expected_amount_in': 'str',
         'expected_collateral_withdrawn': 'str',
         'expected_debt_repaid': 'str',
         'streaming_swap_blocks': 'int',
         'streaming_swap_seconds': 'int',
@@ -63,25 +65,27 @@
         'streaming_slippage_bps': 'streaming_slippage_bps',
         'router': 'router',
         'expiry': 'expiry',
         'warning': 'warning',
         'notes': 'notes',
         'dust_threshold': 'dust_threshold',
         'recommended_min_amount_in': 'recommended_min_amount_in',
+        'recommended_gas_rate': 'recommended_gas_rate',
+        'gas_rate_units': 'gas_rate_units',
         'memo': 'memo',
         'expected_amount_out': 'expected_amount_out',
         'expected_amount_in': 'expected_amount_in',
         'expected_collateral_withdrawn': 'expected_collateral_withdrawn',
         'expected_debt_repaid': 'expected_debt_repaid',
         'streaming_swap_blocks': 'streaming_swap_blocks',
         'streaming_swap_seconds': 'streaming_swap_seconds',
         'total_repay_seconds': 'total_repay_seconds'
     }
 
-    def __init__(self, inbound_address=None, inbound_confirmation_blocks=None, inbound_confirmation_seconds=None, outbound_delay_blocks=None, outbound_delay_seconds=None, fees=None, slippage_bps=None, streaming_slippage_bps=None, router=None, expiry=None, warning=None, notes=None, dust_threshold=None, recommended_min_amount_in=None, memo=None, expected_amount_out=None, expected_amount_in=None, expected_collateral_withdrawn=None, expected_debt_repaid=None, streaming_swap_blocks=None, streaming_swap_seconds=None, total_repay_seconds=None):  # noqa: E501
+    def __init__(self, inbound_address=None, inbound_confirmation_blocks=None, inbound_confirmation_seconds=None, outbound_delay_blocks=None, outbound_delay_seconds=None, fees=None, slippage_bps=None, streaming_slippage_bps=None, router=None, expiry=None, warning=None, notes=None, dust_threshold=None, recommended_min_amount_in=None, recommended_gas_rate=None, gas_rate_units=None, memo=None, expected_amount_out=None, expected_amount_in=None, expected_collateral_withdrawn=None, expected_debt_repaid=None, streaming_swap_blocks=None, streaming_swap_seconds=None, total_repay_seconds=None):  # noqa: E501
         """QuoteLoanCloseResponse - a model defined in Swagger"""  # noqa: E501
         self._inbound_address = None
         self._inbound_confirmation_blocks = None
         self._inbound_confirmation_seconds = None
         self._outbound_delay_blocks = None
         self._outbound_delay_seconds = None
         self._fees = None
@@ -89,14 +93,16 @@
         self._streaming_slippage_bps = None
         self._router = None
         self._expiry = None
         self._warning = None
         self._notes = None
         self._dust_threshold = None
         self._recommended_min_amount_in = None
+        self._recommended_gas_rate = None
+        self._gas_rate_units = None
         self._memo = None
         self._expected_amount_out = None
         self._expected_amount_in = None
         self._expected_collateral_withdrawn = None
         self._expected_debt_repaid = None
         self._streaming_swap_blocks = None
         self._streaming_swap_seconds = None
@@ -120,14 +126,18 @@
         self.expiry = expiry
         self.warning = warning
         self.notes = notes
         if dust_threshold is not None:
             self.dust_threshold = dust_threshold
         if recommended_min_amount_in is not None:
             self.recommended_min_amount_in = recommended_min_amount_in
+        if recommended_gas_rate is not None:
+            self.recommended_gas_rate = recommended_gas_rate
+        if gas_rate_units is not None:
+            self.gas_rate_units = gas_rate_units
         self.memo = memo
         self.expected_amount_out = expected_amount_out
         self.expected_amount_in = expected_amount_in
         self.expected_collateral_withdrawn = expected_collateral_withdrawn
         self.expected_debt_repaid = expected_debt_repaid
         self.streaming_swap_blocks = streaming_swap_blocks
         self.streaming_swap_seconds = streaming_swap_seconds
@@ -462,14 +472,60 @@
         :param recommended_min_amount_in: The recommended_min_amount_in of this QuoteLoanCloseResponse.  # noqa: E501
         :type: str
         """
 
         self._recommended_min_amount_in = recommended_min_amount_in
 
     @property
+    def recommended_gas_rate(self):
+        """Gets the recommended_gas_rate of this QuoteLoanCloseResponse.  # noqa: E501
+
+        the recommended gas rate to use for the inbound to ensure timely confirmation  # noqa: E501
+
+        :return: The recommended_gas_rate of this QuoteLoanCloseResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._recommended_gas_rate
+
+    @recommended_gas_rate.setter
+    def recommended_gas_rate(self, recommended_gas_rate):
+        """Sets the recommended_gas_rate of this QuoteLoanCloseResponse.
+
+        the recommended gas rate to use for the inbound to ensure timely confirmation  # noqa: E501
+
+        :param recommended_gas_rate: The recommended_gas_rate of this QuoteLoanCloseResponse.  # noqa: E501
+        :type: str
+        """
+
+        self._recommended_gas_rate = recommended_gas_rate
+
+    @property
+    def gas_rate_units(self):
+        """Gets the gas_rate_units of this QuoteLoanCloseResponse.  # noqa: E501
+
+        the units of the recommended gas rate  # noqa: E501
+
+        :return: The gas_rate_units of this QuoteLoanCloseResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._gas_rate_units
+
+    @gas_rate_units.setter
+    def gas_rate_units(self, gas_rate_units):
+        """Sets the gas_rate_units of this QuoteLoanCloseResponse.
+
+        the units of the recommended gas rate  # noqa: E501
+
+        :param gas_rate_units: The gas_rate_units of this QuoteLoanCloseResponse.  # noqa: E501
+        :type: str
+        """
+
+        self._gas_rate_units = gas_rate_units
+
+    @property
     def memo(self):
         """Gets the memo of this QuoteLoanCloseResponse.  # noqa: E501
 
         generated memo for the loan close  # noqa: E501
 
         :return: The memo of this QuoteLoanCloseResponse.  # noqa: E501
         :rtype: str
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_loan_open_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/quote_loan_open_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -38,14 +38,16 @@
         'streaming_slippage_bps': 'int',
         'router': 'str',
         'expiry': 'int',
         'warning': 'str',
         'notes': 'str',
         'dust_threshold': 'str',
         'recommended_min_amount_in': 'str',
+        'recommended_gas_rate': 'str',
+        'gas_rate_units': 'str',
         'memo': 'str',
         'expected_amount_out': 'str',
         'expected_collateralization_ratio': 'str',
         'expected_collateral_deposited': 'str',
         'expected_debt_issued': 'str',
         'streaming_swap_blocks': 'int',
         'streaming_swap_seconds': 'int',
@@ -63,25 +65,27 @@
         'streaming_slippage_bps': 'streaming_slippage_bps',
         'router': 'router',
         'expiry': 'expiry',
         'warning': 'warning',
         'notes': 'notes',
         'dust_threshold': 'dust_threshold',
         'recommended_min_amount_in': 'recommended_min_amount_in',
+        'recommended_gas_rate': 'recommended_gas_rate',
+        'gas_rate_units': 'gas_rate_units',
         'memo': 'memo',
         'expected_amount_out': 'expected_amount_out',
         'expected_collateralization_ratio': 'expected_collateralization_ratio',
         'expected_collateral_deposited': 'expected_collateral_deposited',
         'expected_debt_issued': 'expected_debt_issued',
         'streaming_swap_blocks': 'streaming_swap_blocks',
         'streaming_swap_seconds': 'streaming_swap_seconds',
         'total_open_loan_seconds': 'total_open_loan_seconds'
     }
 
-    def __init__(self, inbound_address=None, inbound_confirmation_blocks=None, inbound_confirmation_seconds=None, outbound_delay_blocks=None, outbound_delay_seconds=None, fees=None, slippage_bps=None, streaming_slippage_bps=None, router=None, expiry=None, warning=None, notes=None, dust_threshold=None, recommended_min_amount_in=None, memo=None, expected_amount_out=None, expected_collateralization_ratio=None, expected_collateral_deposited=None, expected_debt_issued=None, streaming_swap_blocks=None, streaming_swap_seconds=None, total_open_loan_seconds=None):  # noqa: E501
+    def __init__(self, inbound_address=None, inbound_confirmation_blocks=None, inbound_confirmation_seconds=None, outbound_delay_blocks=None, outbound_delay_seconds=None, fees=None, slippage_bps=None, streaming_slippage_bps=None, router=None, expiry=None, warning=None, notes=None, dust_threshold=None, recommended_min_amount_in=None, recommended_gas_rate=None, gas_rate_units=None, memo=None, expected_amount_out=None, expected_collateralization_ratio=None, expected_collateral_deposited=None, expected_debt_issued=None, streaming_swap_blocks=None, streaming_swap_seconds=None, total_open_loan_seconds=None):  # noqa: E501
         """QuoteLoanOpenResponse - a model defined in Swagger"""  # noqa: E501
         self._inbound_address = None
         self._inbound_confirmation_blocks = None
         self._inbound_confirmation_seconds = None
         self._outbound_delay_blocks = None
         self._outbound_delay_seconds = None
         self._fees = None
@@ -89,14 +93,16 @@
         self._streaming_slippage_bps = None
         self._router = None
         self._expiry = None
         self._warning = None
         self._notes = None
         self._dust_threshold = None
         self._recommended_min_amount_in = None
+        self._recommended_gas_rate = None
+        self._gas_rate_units = None
         self._memo = None
         self._expected_amount_out = None
         self._expected_collateralization_ratio = None
         self._expected_collateral_deposited = None
         self._expected_debt_issued = None
         self._streaming_swap_blocks = None
         self._streaming_swap_seconds = None
@@ -120,14 +126,16 @@
         self.expiry = expiry
         self.warning = warning
         self.notes = notes
         if dust_threshold is not None:
             self.dust_threshold = dust_threshold
         if recommended_min_amount_in is not None:
             self.recommended_min_amount_in = recommended_min_amount_in
+        self.recommended_gas_rate = recommended_gas_rate
+        self.gas_rate_units = gas_rate_units
         if memo is not None:
             self.memo = memo
         self.expected_amount_out = expected_amount_out
         self.expected_collateralization_ratio = expected_collateralization_ratio
         self.expected_collateral_deposited = expected_collateral_deposited
         self.expected_debt_issued = expected_debt_issued
         self.streaming_swap_blocks = streaming_swap_blocks
@@ -463,14 +471,64 @@
         :param recommended_min_amount_in: The recommended_min_amount_in of this QuoteLoanOpenResponse.  # noqa: E501
         :type: str
         """
 
         self._recommended_min_amount_in = recommended_min_amount_in
 
     @property
+    def recommended_gas_rate(self):
+        """Gets the recommended_gas_rate of this QuoteLoanOpenResponse.  # noqa: E501
+
+        the recommended gas rate to use for the inbound to ensure timely confirmation  # noqa: E501
+
+        :return: The recommended_gas_rate of this QuoteLoanOpenResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._recommended_gas_rate
+
+    @recommended_gas_rate.setter
+    def recommended_gas_rate(self, recommended_gas_rate):
+        """Sets the recommended_gas_rate of this QuoteLoanOpenResponse.
+
+        the recommended gas rate to use for the inbound to ensure timely confirmation  # noqa: E501
+
+        :param recommended_gas_rate: The recommended_gas_rate of this QuoteLoanOpenResponse.  # noqa: E501
+        :type: str
+        """
+        if recommended_gas_rate is None:
+            raise ValueError("Invalid value for `recommended_gas_rate`, must not be `None`")  # noqa: E501
+
+        self._recommended_gas_rate = recommended_gas_rate
+
+    @property
+    def gas_rate_units(self):
+        """Gets the gas_rate_units of this QuoteLoanOpenResponse.  # noqa: E501
+
+        the units of the recommended gas rate  # noqa: E501
+
+        :return: The gas_rate_units of this QuoteLoanOpenResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._gas_rate_units
+
+    @gas_rate_units.setter
+    def gas_rate_units(self, gas_rate_units):
+        """Sets the gas_rate_units of this QuoteLoanOpenResponse.
+
+        the units of the recommended gas rate  # noqa: E501
+
+        :param gas_rate_units: The gas_rate_units of this QuoteLoanOpenResponse.  # noqa: E501
+        :type: str
+        """
+        if gas_rate_units is None:
+            raise ValueError("Invalid value for `gas_rate_units`, must not be `None`")  # noqa: E501
+
+        self._gas_rate_units = gas_rate_units
+
+    @property
     def memo(self):
         """Gets the memo of this QuoteLoanOpenResponse.  # noqa: E501
 
         generated memo for the loan open  # noqa: E501
 
         :return: The memo of this QuoteLoanOpenResponse.  # noqa: E501
         :rtype: str
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_saver_deposit_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/quote_saver_deposit_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -38,14 +38,16 @@
         'streaming_slippage_bps': 'int',
         'router': 'str',
         'expiry': 'int',
         'warning': 'str',
         'notes': 'str',
         'dust_threshold': 'str',
         'recommended_min_amount_in': 'str',
+        'recommended_gas_rate': 'str',
+        'gas_rate_units': 'str',
         'memo': 'str',
         'expected_amount_out': 'str',
         'expected_amount_deposit': 'str'
     }
 
     attribute_map = {
         'inbound_address': 'inbound_address',
@@ -58,20 +60,22 @@
         'streaming_slippage_bps': 'streaming_slippage_bps',
         'router': 'router',
         'expiry': 'expiry',
         'warning': 'warning',
         'notes': 'notes',
         'dust_threshold': 'dust_threshold',
         'recommended_min_amount_in': 'recommended_min_amount_in',
+        'recommended_gas_rate': 'recommended_gas_rate',
+        'gas_rate_units': 'gas_rate_units',
         'memo': 'memo',
         'expected_amount_out': 'expected_amount_out',
         'expected_amount_deposit': 'expected_amount_deposit'
     }
 
-    def __init__(self, inbound_address=None, inbound_confirmation_blocks=None, inbound_confirmation_seconds=None, outbound_delay_blocks=None, outbound_delay_seconds=None, fees=None, slippage_bps=None, streaming_slippage_bps=None, router=None, expiry=None, warning=None, notes=None, dust_threshold=None, recommended_min_amount_in=None, memo=None, expected_amount_out=None, expected_amount_deposit=None):  # noqa: E501
+    def __init__(self, inbound_address=None, inbound_confirmation_blocks=None, inbound_confirmation_seconds=None, outbound_delay_blocks=None, outbound_delay_seconds=None, fees=None, slippage_bps=None, streaming_slippage_bps=None, router=None, expiry=None, warning=None, notes=None, dust_threshold=None, recommended_min_amount_in=None, recommended_gas_rate=None, gas_rate_units=None, memo=None, expected_amount_out=None, expected_amount_deposit=None):  # noqa: E501
         """QuoteSaverDepositResponse - a model defined in Swagger"""  # noqa: E501
         self._inbound_address = None
         self._inbound_confirmation_blocks = None
         self._inbound_confirmation_seconds = None
         self._outbound_delay_blocks = None
         self._outbound_delay_seconds = None
         self._fees = None
@@ -79,14 +83,16 @@
         self._streaming_slippage_bps = None
         self._router = None
         self._expiry = None
         self._warning = None
         self._notes = None
         self._dust_threshold = None
         self._recommended_min_amount_in = None
+        self._recommended_gas_rate = None
+        self._gas_rate_units = None
         self._memo = None
         self._expected_amount_out = None
         self._expected_amount_deposit = None
         self.discriminator = None
         self.inbound_address = inbound_address
         if inbound_confirmation_blocks is not None:
             self.inbound_confirmation_blocks = inbound_confirmation_blocks
@@ -105,14 +111,16 @@
         self.expiry = expiry
         self.warning = warning
         self.notes = notes
         if dust_threshold is not None:
             self.dust_threshold = dust_threshold
         if recommended_min_amount_in is not None:
             self.recommended_min_amount_in = recommended_min_amount_in
+        self.recommended_gas_rate = recommended_gas_rate
+        self.gas_rate_units = gas_rate_units
         self.memo = memo
         if expected_amount_out is not None:
             self.expected_amount_out = expected_amount_out
         self.expected_amount_deposit = expected_amount_deposit
 
     @property
     def inbound_address(self):
@@ -443,14 +451,64 @@
         :param recommended_min_amount_in: The recommended_min_amount_in of this QuoteSaverDepositResponse.  # noqa: E501
         :type: str
         """
 
         self._recommended_min_amount_in = recommended_min_amount_in
 
     @property
+    def recommended_gas_rate(self):
+        """Gets the recommended_gas_rate of this QuoteSaverDepositResponse.  # noqa: E501
+
+        the recommended gas rate to use for the inbound to ensure timely confirmation  # noqa: E501
+
+        :return: The recommended_gas_rate of this QuoteSaverDepositResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._recommended_gas_rate
+
+    @recommended_gas_rate.setter
+    def recommended_gas_rate(self, recommended_gas_rate):
+        """Sets the recommended_gas_rate of this QuoteSaverDepositResponse.
+
+        the recommended gas rate to use for the inbound to ensure timely confirmation  # noqa: E501
+
+        :param recommended_gas_rate: The recommended_gas_rate of this QuoteSaverDepositResponse.  # noqa: E501
+        :type: str
+        """
+        if recommended_gas_rate is None:
+            raise ValueError("Invalid value for `recommended_gas_rate`, must not be `None`")  # noqa: E501
+
+        self._recommended_gas_rate = recommended_gas_rate
+
+    @property
+    def gas_rate_units(self):
+        """Gets the gas_rate_units of this QuoteSaverDepositResponse.  # noqa: E501
+
+        the units of the recommended gas rate  # noqa: E501
+
+        :return: The gas_rate_units of this QuoteSaverDepositResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._gas_rate_units
+
+    @gas_rate_units.setter
+    def gas_rate_units(self, gas_rate_units):
+        """Sets the gas_rate_units of this QuoteSaverDepositResponse.
+
+        the units of the recommended gas rate  # noqa: E501
+
+        :param gas_rate_units: The gas_rate_units of this QuoteSaverDepositResponse.  # noqa: E501
+        :type: str
+        """
+        if gas_rate_units is None:
+            raise ValueError("Invalid value for `gas_rate_units`, must not be `None`")  # noqa: E501
+
+        self._gas_rate_units = gas_rate_units
+
+    @property
     def memo(self):
         """Gets the memo of this QuoteSaverDepositResponse.  # noqa: E501
 
         generated memo for the deposit  # noqa: E501
 
         :return: The memo of this QuoteSaverDepositResponse.  # noqa: E501
         :rtype: str
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_saver_withdraw_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/quote_saver_withdraw_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -38,14 +38,16 @@
         'streaming_slippage_bps': 'int',
         'router': 'str',
         'expiry': 'int',
         'warning': 'str',
         'notes': 'str',
         'dust_threshold': 'str',
         'recommended_min_amount_in': 'str',
+        'recommended_gas_rate': 'str',
+        'gas_rate_units': 'str',
         'memo': 'str',
         'dust_amount': 'str',
         'expected_amount_out': 'str'
     }
 
     attribute_map = {
         'inbound_address': 'inbound_address',
@@ -58,20 +60,22 @@
         'streaming_slippage_bps': 'streaming_slippage_bps',
         'router': 'router',
         'expiry': 'expiry',
         'warning': 'warning',
         'notes': 'notes',
         'dust_threshold': 'dust_threshold',
         'recommended_min_amount_in': 'recommended_min_amount_in',
+        'recommended_gas_rate': 'recommended_gas_rate',
+        'gas_rate_units': 'gas_rate_units',
         'memo': 'memo',
         'dust_amount': 'dust_amount',
         'expected_amount_out': 'expected_amount_out'
     }
 
-    def __init__(self, inbound_address=None, inbound_confirmation_blocks=None, inbound_confirmation_seconds=None, outbound_delay_blocks=None, outbound_delay_seconds=None, fees=None, slippage_bps=None, streaming_slippage_bps=None, router=None, expiry=None, warning=None, notes=None, dust_threshold=None, recommended_min_amount_in=None, memo=None, dust_amount=None, expected_amount_out=None):  # noqa: E501
+    def __init__(self, inbound_address=None, inbound_confirmation_blocks=None, inbound_confirmation_seconds=None, outbound_delay_blocks=None, outbound_delay_seconds=None, fees=None, slippage_bps=None, streaming_slippage_bps=None, router=None, expiry=None, warning=None, notes=None, dust_threshold=None, recommended_min_amount_in=None, recommended_gas_rate=None, gas_rate_units=None, memo=None, dust_amount=None, expected_amount_out=None):  # noqa: E501
         """QuoteSaverWithdrawResponse - a model defined in Swagger"""  # noqa: E501
         self._inbound_address = None
         self._inbound_confirmation_blocks = None
         self._inbound_confirmation_seconds = None
         self._outbound_delay_blocks = None
         self._outbound_delay_seconds = None
         self._fees = None
@@ -79,14 +83,16 @@
         self._streaming_slippage_bps = None
         self._router = None
         self._expiry = None
         self._warning = None
         self._notes = None
         self._dust_threshold = None
         self._recommended_min_amount_in = None
+        self._recommended_gas_rate = None
+        self._gas_rate_units = None
         self._memo = None
         self._dust_amount = None
         self._expected_amount_out = None
         self.discriminator = None
         self.inbound_address = inbound_address
         if inbound_confirmation_blocks is not None:
             self.inbound_confirmation_blocks = inbound_confirmation_blocks
@@ -103,14 +109,16 @@
         self.expiry = expiry
         self.warning = warning
         self.notes = notes
         if dust_threshold is not None:
             self.dust_threshold = dust_threshold
         if recommended_min_amount_in is not None:
             self.recommended_min_amount_in = recommended_min_amount_in
+        self.recommended_gas_rate = recommended_gas_rate
+        self.gas_rate_units = gas_rate_units
         self.memo = memo
         self.dust_amount = dust_amount
         self.expected_amount_out = expected_amount_out
 
     @property
     def inbound_address(self):
         """Gets the inbound_address of this QuoteSaverWithdrawResponse.  # noqa: E501
@@ -444,14 +452,64 @@
         :param recommended_min_amount_in: The recommended_min_amount_in of this QuoteSaverWithdrawResponse.  # noqa: E501
         :type: str
         """
 
         self._recommended_min_amount_in = recommended_min_amount_in
 
     @property
+    def recommended_gas_rate(self):
+        """Gets the recommended_gas_rate of this QuoteSaverWithdrawResponse.  # noqa: E501
+
+        the recommended gas rate to use for the inbound to ensure timely confirmation  # noqa: E501
+
+        :return: The recommended_gas_rate of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._recommended_gas_rate
+
+    @recommended_gas_rate.setter
+    def recommended_gas_rate(self, recommended_gas_rate):
+        """Sets the recommended_gas_rate of this QuoteSaverWithdrawResponse.
+
+        the recommended gas rate to use for the inbound to ensure timely confirmation  # noqa: E501
+
+        :param recommended_gas_rate: The recommended_gas_rate of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :type: str
+        """
+        if recommended_gas_rate is None:
+            raise ValueError("Invalid value for `recommended_gas_rate`, must not be `None`")  # noqa: E501
+
+        self._recommended_gas_rate = recommended_gas_rate
+
+    @property
+    def gas_rate_units(self):
+        """Gets the gas_rate_units of this QuoteSaverWithdrawResponse.  # noqa: E501
+
+        the units of the recommended gas rate  # noqa: E501
+
+        :return: The gas_rate_units of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._gas_rate_units
+
+    @gas_rate_units.setter
+    def gas_rate_units(self, gas_rate_units):
+        """Sets the gas_rate_units of this QuoteSaverWithdrawResponse.
+
+        the units of the recommended gas rate  # noqa: E501
+
+        :param gas_rate_units: The gas_rate_units of this QuoteSaverWithdrawResponse.  # noqa: E501
+        :type: str
+        """
+        if gas_rate_units is None:
+            raise ValueError("Invalid value for `gas_rate_units`, must not be `None`")  # noqa: E501
+
+        self._gas_rate_units = gas_rate_units
+
+    @property
     def memo(self):
         """Gets the memo of this QuoteSaverWithdrawResponse.  # noqa: E501
 
         generated memo for the withdraw, the client can use this OR send the dust amount  # noqa: E501
 
         :return: The memo of this QuoteSaverWithdrawResponse.  # noqa: E501
         :rtype: str
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_swap_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/quote_swap_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -38,14 +38,16 @@
         'streaming_slippage_bps': 'int',
         'router': 'str',
         'expiry': 'int',
         'warning': 'str',
         'notes': 'str',
         'dust_threshold': 'str',
         'recommended_min_amount_in': 'str',
+        'recommended_gas_rate': 'str',
+        'gas_rate_units': 'str',
         'memo': 'str',
         'expected_amount_out': 'str',
         'expected_amount_out_streaming': 'str',
         'max_streaming_quantity': 'int',
         'streaming_swap_blocks': 'int',
         'streaming_swap_seconds': 'int',
         'total_swap_seconds': 'int'
@@ -62,24 +64,26 @@
         'streaming_slippage_bps': 'streaming_slippage_bps',
         'router': 'router',
         'expiry': 'expiry',
         'warning': 'warning',
         'notes': 'notes',
         'dust_threshold': 'dust_threshold',
         'recommended_min_amount_in': 'recommended_min_amount_in',
+        'recommended_gas_rate': 'recommended_gas_rate',
+        'gas_rate_units': 'gas_rate_units',
         'memo': 'memo',
         'expected_amount_out': 'expected_amount_out',
         'expected_amount_out_streaming': 'expected_amount_out_streaming',
         'max_streaming_quantity': 'max_streaming_quantity',
         'streaming_swap_blocks': 'streaming_swap_blocks',
         'streaming_swap_seconds': 'streaming_swap_seconds',
         'total_swap_seconds': 'total_swap_seconds'
     }
 
-    def __init__(self, inbound_address=None, inbound_confirmation_blocks=None, inbound_confirmation_seconds=None, outbound_delay_blocks=None, outbound_delay_seconds=None, fees=None, slippage_bps=None, streaming_slippage_bps=None, router=None, expiry=None, warning=None, notes=None, dust_threshold=None, recommended_min_amount_in=None, memo=None, expected_amount_out=None, expected_amount_out_streaming=None, max_streaming_quantity=None, streaming_swap_blocks=None, streaming_swap_seconds=None, total_swap_seconds=None):  # noqa: E501
+    def __init__(self, inbound_address=None, inbound_confirmation_blocks=None, inbound_confirmation_seconds=None, outbound_delay_blocks=None, outbound_delay_seconds=None, fees=None, slippage_bps=None, streaming_slippage_bps=None, router=None, expiry=None, warning=None, notes=None, dust_threshold=None, recommended_min_amount_in=None, recommended_gas_rate=None, gas_rate_units=None, memo=None, expected_amount_out=None, expected_amount_out_streaming=None, max_streaming_quantity=None, streaming_swap_blocks=None, streaming_swap_seconds=None, total_swap_seconds=None):  # noqa: E501
         """QuoteSwapResponse - a model defined in Swagger"""  # noqa: E501
         self._inbound_address = None
         self._inbound_confirmation_blocks = None
         self._inbound_confirmation_seconds = None
         self._outbound_delay_blocks = None
         self._outbound_delay_seconds = None
         self._fees = None
@@ -87,14 +91,16 @@
         self._streaming_slippage_bps = None
         self._router = None
         self._expiry = None
         self._warning = None
         self._notes = None
         self._dust_threshold = None
         self._recommended_min_amount_in = None
+        self._recommended_gas_rate = None
+        self._gas_rate_units = None
         self._memo = None
         self._expected_amount_out = None
         self._expected_amount_out_streaming = None
         self._max_streaming_quantity = None
         self._streaming_swap_blocks = None
         self._streaming_swap_seconds = None
         self._total_swap_seconds = None
@@ -115,14 +121,18 @@
         self.expiry = expiry
         self.warning = warning
         self.notes = notes
         if dust_threshold is not None:
             self.dust_threshold = dust_threshold
         if recommended_min_amount_in is not None:
             self.recommended_min_amount_in = recommended_min_amount_in
+        if recommended_gas_rate is not None:
+            self.recommended_gas_rate = recommended_gas_rate
+        if gas_rate_units is not None:
+            self.gas_rate_units = gas_rate_units
         if memo is not None:
             self.memo = memo
         self.expected_amount_out = expected_amount_out
         self.expected_amount_out_streaming = expected_amount_out_streaming
         if max_streaming_quantity is not None:
             self.max_streaming_quantity = max_streaming_quantity
         if streaming_swap_blocks is not None:
@@ -465,14 +475,60 @@
         :param recommended_min_amount_in: The recommended_min_amount_in of this QuoteSwapResponse.  # noqa: E501
         :type: str
         """
 
         self._recommended_min_amount_in = recommended_min_amount_in
 
     @property
+    def recommended_gas_rate(self):
+        """Gets the recommended_gas_rate of this QuoteSwapResponse.  # noqa: E501
+
+        the recommended gas rate to use for the inbound to ensure timely confirmation  # noqa: E501
+
+        :return: The recommended_gas_rate of this QuoteSwapResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._recommended_gas_rate
+
+    @recommended_gas_rate.setter
+    def recommended_gas_rate(self, recommended_gas_rate):
+        """Sets the recommended_gas_rate of this QuoteSwapResponse.
+
+        the recommended gas rate to use for the inbound to ensure timely confirmation  # noqa: E501
+
+        :param recommended_gas_rate: The recommended_gas_rate of this QuoteSwapResponse.  # noqa: E501
+        :type: str
+        """
+
+        self._recommended_gas_rate = recommended_gas_rate
+
+    @property
+    def gas_rate_units(self):
+        """Gets the gas_rate_units of this QuoteSwapResponse.  # noqa: E501
+
+        the units of the recommended gas rate  # noqa: E501
+
+        :return: The gas_rate_units of this QuoteSwapResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._gas_rate_units
+
+    @gas_rate_units.setter
+    def gas_rate_units(self, gas_rate_units):
+        """Sets the gas_rate_units of this QuoteSwapResponse.
+
+        the units of the recommended gas rate  # noqa: E501
+
+        :param gas_rate_units: The gas_rate_units of this QuoteSwapResponse.  # noqa: E501
+        :type: str
+        """
+
+        self._gas_rate_units = gas_rate_units
+
+    @property
     def memo(self):
         """Gets the memo of this QuoteSwapResponse.  # noqa: E501
 
         generated memo for the swap  # noqa: E501
 
         :return: The memo of this QuoteSwapResponse.  # noqa: E501
         :rtype: str
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/saver.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/saver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/saver_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/saver_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/savers_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/savers_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/scheduled_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/scheduled_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/streaming_swap.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/streaming_swap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/streaming_swap_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/streaming_swap_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/streaming_swaps_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/node_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class StreamingSwapsResponse(object):
+class NodeResponse(object):
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
-        """StreamingSwapsResponse - a model defined in Swagger"""  # noqa: E501
+        """NodeResponse - a model defined in Swagger"""  # noqa: E501
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
-        if issubclass(StreamingSwapsResponse, dict):
+        if issubclass(NodeResponse, dict):
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
-        if not isinstance(other, StreamingSwapsResponse):
+        if not isinstance(other, NodeResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/swap_queue_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/swap_queue_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/swapper_clout_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/swapper_clout_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/thorname.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/thorname.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/thorname_alias.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/thorname_alias.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/thorname_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/thorname_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/trade_account_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/trade_account_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/trade_accounts_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/trade_accounts_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/trade_unit_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/trade_unit_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/trade_units_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/trade_units_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tss_keysign_metric.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tss_keysign_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tss_metric.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tss_metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_details_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tx_details_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_out_item.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tx_out_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -79,15 +79,16 @@
         self.max_gas = max_gas
         if gas_rate is not None:
             self.gas_rate = gas_rate
         if in_hash is not None:
             self.in_hash = in_hash
         if out_hash is not None:
             self.out_hash = out_hash
-        self.height = height
+        if height is not None:
+            self.height = height
         if clout_spent is not None:
             self.clout_spent = clout_spent
 
     @property
     def chain(self):
         """Gets the chain of this TxOutItem.  # noqa: E501
 
@@ -298,16 +299,14 @@
     def height(self, height):
         """Sets the height of this TxOutItem.
 
 
         :param height: The height of this TxOutItem.  # noqa: E501
         :type: int
         """
-        if height is None:
-            raise ValueError("Invalid value for `height`, must not be `None`")  # noqa: E501
 
         self._height = height
 
     @property
     def clout_spent(self):
         """Gets the clout_spent of this TxOutItem.  # noqa: E501
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tx_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_signers_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tx_signers_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tx_stages_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -24,21 +24,21 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'inbound_observed': 'TxStagesResponseInboundObserved',
-        'inbound_confirmation_counted': 'TxStagesResponseInboundConfirmationCounted',
-        'inbound_finalised': 'TxStagesResponseInboundFinalised',
-        'swap_status': 'TxStagesResponseSwapStatus',
-        'swap_finalised': 'TxStagesResponseSwapFinalised',
-        'outbound_delay': 'TxStagesResponseOutboundDelay',
-        'outbound_signed': 'TxStagesResponseOutboundSigned'
+        'inbound_observed': 'InboundObservedStage',
+        'inbound_confirmation_counted': 'InboundConfirmationCountedStage',
+        'inbound_finalised': 'InboundFinalisedStage',
+        'swap_status': 'SwapStatus',
+        'swap_finalised': 'SwapFinalisedStage',
+        'outbound_delay': 'OutboundDelayStage',
+        'outbound_signed': 'OutboundSignedStage'
     }
 
     attribute_map = {
         'inbound_observed': 'inbound_observed',
         'inbound_confirmation_counted': 'inbound_confirmation_counted',
         'inbound_finalised': 'inbound_finalised',
         'swap_status': 'swap_status',
@@ -73,153 +73,153 @@
 
     @property
     def inbound_observed(self):
         """Gets the inbound_observed of this TxStagesResponse.  # noqa: E501
 
 
         :return: The inbound_observed of this TxStagesResponse.  # noqa: E501
-        :rtype: TxStagesResponseInboundObserved
+        :rtype: InboundObservedStage
         """
         return self._inbound_observed
 
     @inbound_observed.setter
     def inbound_observed(self, inbound_observed):
         """Sets the inbound_observed of this TxStagesResponse.
 
 
         :param inbound_observed: The inbound_observed of this TxStagesResponse.  # noqa: E501
-        :type: TxStagesResponseInboundObserved
+        :type: InboundObservedStage
         """
         if inbound_observed is None:
             raise ValueError("Invalid value for `inbound_observed`, must not be `None`")  # noqa: E501
 
         self._inbound_observed = inbound_observed
 
     @property
     def inbound_confirmation_counted(self):
         """Gets the inbound_confirmation_counted of this TxStagesResponse.  # noqa: E501
 
 
         :return: The inbound_confirmation_counted of this TxStagesResponse.  # noqa: E501
-        :rtype: TxStagesResponseInboundConfirmationCounted
+        :rtype: InboundConfirmationCountedStage
         """
         return self._inbound_confirmation_counted
 
     @inbound_confirmation_counted.setter
     def inbound_confirmation_counted(self, inbound_confirmation_counted):
         """Sets the inbound_confirmation_counted of this TxStagesResponse.
 
 
         :param inbound_confirmation_counted: The inbound_confirmation_counted of this TxStagesResponse.  # noqa: E501
-        :type: TxStagesResponseInboundConfirmationCounted
+        :type: InboundConfirmationCountedStage
         """
 
         self._inbound_confirmation_counted = inbound_confirmation_counted
 
     @property
     def inbound_finalised(self):
         """Gets the inbound_finalised of this TxStagesResponse.  # noqa: E501
 
 
         :return: The inbound_finalised of this TxStagesResponse.  # noqa: E501
-        :rtype: TxStagesResponseInboundFinalised
+        :rtype: InboundFinalisedStage
         """
         return self._inbound_finalised
 
     @inbound_finalised.setter
     def inbound_finalised(self, inbound_finalised):
         """Sets the inbound_finalised of this TxStagesResponse.
 
 
         :param inbound_finalised: The inbound_finalised of this TxStagesResponse.  # noqa: E501
-        :type: TxStagesResponseInboundFinalised
+        :type: InboundFinalisedStage
         """
 
         self._inbound_finalised = inbound_finalised
 
     @property
     def swap_status(self):
         """Gets the swap_status of this TxStagesResponse.  # noqa: E501
 
 
         :return: The swap_status of this TxStagesResponse.  # noqa: E501
-        :rtype: TxStagesResponseSwapStatus
+        :rtype: SwapStatus
         """
         return self._swap_status
 
     @swap_status.setter
     def swap_status(self, swap_status):
         """Sets the swap_status of this TxStagesResponse.
 
 
         :param swap_status: The swap_status of this TxStagesResponse.  # noqa: E501
-        :type: TxStagesResponseSwapStatus
+        :type: SwapStatus
         """
 
         self._swap_status = swap_status
 
     @property
     def swap_finalised(self):
         """Gets the swap_finalised of this TxStagesResponse.  # noqa: E501
 
 
         :return: The swap_finalised of this TxStagesResponse.  # noqa: E501
-        :rtype: TxStagesResponseSwapFinalised
+        :rtype: SwapFinalisedStage
         """
         return self._swap_finalised
 
     @swap_finalised.setter
     def swap_finalised(self, swap_finalised):
         """Sets the swap_finalised of this TxStagesResponse.
 
 
         :param swap_finalised: The swap_finalised of this TxStagesResponse.  # noqa: E501
-        :type: TxStagesResponseSwapFinalised
+        :type: SwapFinalisedStage
         """
 
         self._swap_finalised = swap_finalised
 
     @property
     def outbound_delay(self):
         """Gets the outbound_delay of this TxStagesResponse.  # noqa: E501
 
 
         :return: The outbound_delay of this TxStagesResponse.  # noqa: E501
-        :rtype: TxStagesResponseOutboundDelay
+        :rtype: OutboundDelayStage
         """
         return self._outbound_delay
 
     @outbound_delay.setter
     def outbound_delay(self, outbound_delay):
         """Sets the outbound_delay of this TxStagesResponse.
 
 
         :param outbound_delay: The outbound_delay of this TxStagesResponse.  # noqa: E501
-        :type: TxStagesResponseOutboundDelay
+        :type: OutboundDelayStage
         """
 
         self._outbound_delay = outbound_delay
 
     @property
     def outbound_signed(self):
         """Gets the outbound_signed of this TxStagesResponse.  # noqa: E501
 
 
         :return: The outbound_signed of this TxStagesResponse.  # noqa: E501
-        :rtype: TxStagesResponseOutboundSigned
+        :rtype: OutboundSignedStage
         """
         return self._outbound_signed
 
     @outbound_signed.setter
     def outbound_signed(self, outbound_signed):
         """Sets the outbound_signed of this TxStagesResponse.
 
 
         :param outbound_signed: The outbound_signed of this TxStagesResponse.  # noqa: E501
-        :type: TxStagesResponseOutboundSigned
+        :type: OutboundSignedStage
         """
 
         self._outbound_signed = outbound_signed
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_inbound_confirmation_counted.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/inbound_confirmation_counted_stage.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TxStagesResponseInboundConfirmationCounted(object):
+class InboundConfirmationCountedStage(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -42,15 +42,15 @@
         'external_observed_height': 'external_observed_height',
         'external_confirmation_delay_height': 'external_confirmation_delay_height',
         'remaining_confirmation_seconds': 'remaining_confirmation_seconds',
         'completed': 'completed'
     }
 
     def __init__(self, counting_start_height=None, chain=None, external_observed_height=None, external_confirmation_delay_height=None, remaining_confirmation_seconds=None, completed=None):  # noqa: E501
-        """TxStagesResponseInboundConfirmationCounted - a model defined in Swagger"""  # noqa: E501
+        """InboundConfirmationCountedStage - a model defined in Swagger"""  # noqa: E501
         self._counting_start_height = None
         self._chain = None
         self._external_observed_height = None
         self._external_confirmation_delay_height = None
         self._remaining_confirmation_seconds = None
         self._completed = None
         self.discriminator = None
@@ -64,145 +64,145 @@
             self.external_confirmation_delay_height = external_confirmation_delay_height
         if remaining_confirmation_seconds is not None:
             self.remaining_confirmation_seconds = remaining_confirmation_seconds
         self.completed = completed
 
     @property
     def counting_start_height(self):
-        """Gets the counting_start_height of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        """Gets the counting_start_height of this InboundConfirmationCountedStage.  # noqa: E501
 
         the THORChain block height when confirmation counting began  # noqa: E501
 
-        :return: The counting_start_height of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        :return: The counting_start_height of this InboundConfirmationCountedStage.  # noqa: E501
         :rtype: int
         """
         return self._counting_start_height
 
     @counting_start_height.setter
     def counting_start_height(self, counting_start_height):
-        """Sets the counting_start_height of this TxStagesResponseInboundConfirmationCounted.
+        """Sets the counting_start_height of this InboundConfirmationCountedStage.
 
         the THORChain block height when confirmation counting began  # noqa: E501
 
-        :param counting_start_height: The counting_start_height of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        :param counting_start_height: The counting_start_height of this InboundConfirmationCountedStage.  # noqa: E501
         :type: int
         """
 
         self._counting_start_height = counting_start_height
 
     @property
     def chain(self):
-        """Gets the chain of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        """Gets the chain of this InboundConfirmationCountedStage.  # noqa: E501
 
         the external source chain for which confirmation counting takes place  # noqa: E501
 
-        :return: The chain of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        :return: The chain of this InboundConfirmationCountedStage.  # noqa: E501
         :rtype: str
         """
         return self._chain
 
     @chain.setter
     def chain(self, chain):
-        """Sets the chain of this TxStagesResponseInboundConfirmationCounted.
+        """Sets the chain of this InboundConfirmationCountedStage.
 
         the external source chain for which confirmation counting takes place  # noqa: E501
 
-        :param chain: The chain of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        :param chain: The chain of this InboundConfirmationCountedStage.  # noqa: E501
         :type: str
         """
 
         self._chain = chain
 
     @property
     def external_observed_height(self):
-        """Gets the external_observed_height of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        """Gets the external_observed_height of this InboundConfirmationCountedStage.  # noqa: E501
 
         the block height on the external source chain when the transaction was observed  # noqa: E501
 
-        :return: The external_observed_height of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        :return: The external_observed_height of this InboundConfirmationCountedStage.  # noqa: E501
         :rtype: int
         """
         return self._external_observed_height
 
     @external_observed_height.setter
     def external_observed_height(self, external_observed_height):
-        """Sets the external_observed_height of this TxStagesResponseInboundConfirmationCounted.
+        """Sets the external_observed_height of this InboundConfirmationCountedStage.
 
         the block height on the external source chain when the transaction was observed  # noqa: E501
 
-        :param external_observed_height: The external_observed_height of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        :param external_observed_height: The external_observed_height of this InboundConfirmationCountedStage.  # noqa: E501
         :type: int
         """
 
         self._external_observed_height = external_observed_height
 
     @property
     def external_confirmation_delay_height(self):
-        """Gets the external_confirmation_delay_height of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        """Gets the external_confirmation_delay_height of this InboundConfirmationCountedStage.  # noqa: E501
 
         the block height on the external source chain when confirmation counting will be complete  # noqa: E501
 
-        :return: The external_confirmation_delay_height of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        :return: The external_confirmation_delay_height of this InboundConfirmationCountedStage.  # noqa: E501
         :rtype: int
         """
         return self._external_confirmation_delay_height
 
     @external_confirmation_delay_height.setter
     def external_confirmation_delay_height(self, external_confirmation_delay_height):
-        """Sets the external_confirmation_delay_height of this TxStagesResponseInboundConfirmationCounted.
+        """Sets the external_confirmation_delay_height of this InboundConfirmationCountedStage.
 
         the block height on the external source chain when confirmation counting will be complete  # noqa: E501
 
-        :param external_confirmation_delay_height: The external_confirmation_delay_height of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        :param external_confirmation_delay_height: The external_confirmation_delay_height of this InboundConfirmationCountedStage.  # noqa: E501
         :type: int
         """
 
         self._external_confirmation_delay_height = external_confirmation_delay_height
 
     @property
     def remaining_confirmation_seconds(self):
-        """Gets the remaining_confirmation_seconds of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        """Gets the remaining_confirmation_seconds of this InboundConfirmationCountedStage.  # noqa: E501
 
         the estimated remaining seconds before confirmation counting completes  # noqa: E501
 
-        :return: The remaining_confirmation_seconds of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        :return: The remaining_confirmation_seconds of this InboundConfirmationCountedStage.  # noqa: E501
         :rtype: int
         """
         return self._remaining_confirmation_seconds
 
     @remaining_confirmation_seconds.setter
     def remaining_confirmation_seconds(self, remaining_confirmation_seconds):
-        """Sets the remaining_confirmation_seconds of this TxStagesResponseInboundConfirmationCounted.
+        """Sets the remaining_confirmation_seconds of this InboundConfirmationCountedStage.
 
         the estimated remaining seconds before confirmation counting completes  # noqa: E501
 
-        :param remaining_confirmation_seconds: The remaining_confirmation_seconds of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        :param remaining_confirmation_seconds: The remaining_confirmation_seconds of this InboundConfirmationCountedStage.  # noqa: E501
         :type: int
         """
 
         self._remaining_confirmation_seconds = remaining_confirmation_seconds
 
     @property
     def completed(self):
-        """Gets the completed of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        """Gets the completed of this InboundConfirmationCountedStage.  # noqa: E501
 
         returns true if no transaction confirmation counting remains to be done  # noqa: E501
 
-        :return: The completed of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        :return: The completed of this InboundConfirmationCountedStage.  # noqa: E501
         :rtype: bool
         """
         return self._completed
 
     @completed.setter
     def completed(self, completed):
-        """Sets the completed of this TxStagesResponseInboundConfirmationCounted.
+        """Sets the completed of this InboundConfirmationCountedStage.
 
         returns true if no transaction confirmation counting remains to be done  # noqa: E501
 
-        :param completed: The completed of this TxStagesResponseInboundConfirmationCounted.  # noqa: E501
+        :param completed: The completed of this InboundConfirmationCountedStage.  # noqa: E501
         :type: bool
         """
         if completed is None:
             raise ValueError("Invalid value for `completed`, must not be `None`")  # noqa: E501
 
         self._completed = completed
 
@@ -223,15 +223,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TxStagesResponseInboundConfirmationCounted, dict):
+        if issubclass(InboundConfirmationCountedStage, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -239,15 +239,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TxStagesResponseInboundConfirmationCounted):
+        if not isinstance(other, InboundConfirmationCountedStage):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_inbound_finalised.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/inbound_finalised_stage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TxStagesResponseInboundFinalised(object):
+class InboundFinalisedStage(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,37 +32,37 @@
     }
 
     attribute_map = {
         'completed': 'completed'
     }
 
     def __init__(self, completed=None):  # noqa: E501
-        """TxStagesResponseInboundFinalised - a model defined in Swagger"""  # noqa: E501
+        """InboundFinalisedStage - a model defined in Swagger"""  # noqa: E501
         self._completed = None
         self.discriminator = None
         self.completed = completed
 
     @property
     def completed(self):
-        """Gets the completed of this TxStagesResponseInboundFinalised.  # noqa: E501
+        """Gets the completed of this InboundFinalisedStage.  # noqa: E501
 
         returns true if the inbound transaction has been finalised (THORChain agreeing it exists)  # noqa: E501
 
-        :return: The completed of this TxStagesResponseInboundFinalised.  # noqa: E501
+        :return: The completed of this InboundFinalisedStage.  # noqa: E501
         :rtype: bool
         """
         return self._completed
 
     @completed.setter
     def completed(self, completed):
-        """Sets the completed of this TxStagesResponseInboundFinalised.
+        """Sets the completed of this InboundFinalisedStage.
 
         returns true if the inbound transaction has been finalised (THORChain agreeing it exists)  # noqa: E501
 
-        :param completed: The completed of this TxStagesResponseInboundFinalised.  # noqa: E501
+        :param completed: The completed of this InboundFinalisedStage.  # noqa: E501
         :type: bool
         """
         if completed is None:
             raise ValueError("Invalid value for `completed`, must not be `None`")  # noqa: E501
 
         self._completed = completed
 
@@ -83,15 +83,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TxStagesResponseInboundFinalised, dict):
+        if issubclass(InboundFinalisedStage, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -99,15 +99,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TxStagesResponseInboundFinalised):
+        if not isinstance(other, InboundFinalisedStage):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_inbound_observed.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/inbound_observed_stage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TxStagesResponseInboundObserved(object):
+class InboundObservedStage(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -38,115 +38,116 @@
         'started': 'started',
         'pre_confirmation_count': 'pre_confirmation_count',
         'final_count': 'final_count',
         'completed': 'completed'
     }
 
     def __init__(self, started=None, pre_confirmation_count=None, final_count=None, completed=None):  # noqa: E501
-        """TxStagesResponseInboundObserved - a model defined in Swagger"""  # noqa: E501
+        """InboundObservedStage - a model defined in Swagger"""  # noqa: E501
         self._started = None
         self._pre_confirmation_count = None
         self._final_count = None
         self._completed = None
         self.discriminator = None
         if started is not None:
             self.started = started
         if pre_confirmation_count is not None:
             self.pre_confirmation_count = pre_confirmation_count
-        if final_count is not None:
-            self.final_count = final_count
+        self.final_count = final_count
         self.completed = completed
 
     @property
     def started(self):
-        """Gets the started of this TxStagesResponseInboundObserved.  # noqa: E501
+        """Gets the started of this InboundObservedStage.  # noqa: E501
 
         returns true if any nodes have observed the transaction (to be deprecated in favour of counts)  # noqa: E501
 
-        :return: The started of this TxStagesResponseInboundObserved.  # noqa: E501
+        :return: The started of this InboundObservedStage.  # noqa: E501
         :rtype: bool
         """
         return self._started
 
     @started.setter
     def started(self, started):
-        """Sets the started of this TxStagesResponseInboundObserved.
+        """Sets the started of this InboundObservedStage.
 
         returns true if any nodes have observed the transaction (to be deprecated in favour of counts)  # noqa: E501
 
-        :param started: The started of this TxStagesResponseInboundObserved.  # noqa: E501
+        :param started: The started of this InboundObservedStage.  # noqa: E501
         :type: bool
         """
 
         self._started = started
 
     @property
     def pre_confirmation_count(self):
-        """Gets the pre_confirmation_count of this TxStagesResponseInboundObserved.  # noqa: E501
+        """Gets the pre_confirmation_count of this InboundObservedStage.  # noqa: E501
 
         number of signers for pre-confirmation-counting observations  # noqa: E501
 
-        :return: The pre_confirmation_count of this TxStagesResponseInboundObserved.  # noqa: E501
+        :return: The pre_confirmation_count of this InboundObservedStage.  # noqa: E501
         :rtype: int
         """
         return self._pre_confirmation_count
 
     @pre_confirmation_count.setter
     def pre_confirmation_count(self, pre_confirmation_count):
-        """Sets the pre_confirmation_count of this TxStagesResponseInboundObserved.
+        """Sets the pre_confirmation_count of this InboundObservedStage.
 
         number of signers for pre-confirmation-counting observations  # noqa: E501
 
-        :param pre_confirmation_count: The pre_confirmation_count of this TxStagesResponseInboundObserved.  # noqa: E501
+        :param pre_confirmation_count: The pre_confirmation_count of this InboundObservedStage.  # noqa: E501
         :type: int
         """
 
         self._pre_confirmation_count = pre_confirmation_count
 
     @property
     def final_count(self):
-        """Gets the final_count of this TxStagesResponseInboundObserved.  # noqa: E501
+        """Gets the final_count of this InboundObservedStage.  # noqa: E501
 
         number of signers for final observations, after any confirmation counting complete  # noqa: E501
 
-        :return: The final_count of this TxStagesResponseInboundObserved.  # noqa: E501
+        :return: The final_count of this InboundObservedStage.  # noqa: E501
         :rtype: int
         """
         return self._final_count
 
     @final_count.setter
     def final_count(self, final_count):
-        """Sets the final_count of this TxStagesResponseInboundObserved.
+        """Sets the final_count of this InboundObservedStage.
 
         number of signers for final observations, after any confirmation counting complete  # noqa: E501
 
-        :param final_count: The final_count of this TxStagesResponseInboundObserved.  # noqa: E501
+        :param final_count: The final_count of this InboundObservedStage.  # noqa: E501
         :type: int
         """
+        if final_count is None:
+            raise ValueError("Invalid value for `final_count`, must not be `None`")  # noqa: E501
 
         self._final_count = final_count
 
     @property
     def completed(self):
-        """Gets the completed of this TxStagesResponseInboundObserved.  # noqa: E501
+        """Gets the completed of this InboundObservedStage.  # noqa: E501
 
         returns true if no transaction observation remains to be done  # noqa: E501
 
-        :return: The completed of this TxStagesResponseInboundObserved.  # noqa: E501
+        :return: The completed of this InboundObservedStage.  # noqa: E501
         :rtype: bool
         """
         return self._completed
 
     @completed.setter
     def completed(self, completed):
-        """Sets the completed of this TxStagesResponseInboundObserved.
+        """Sets the completed of this InboundObservedStage.
 
         returns true if no transaction observation remains to be done  # noqa: E501
 
-        :param completed: The completed of this TxStagesResponseInboundObserved.  # noqa: E501
+        :param completed: The completed of this InboundObservedStage.  # noqa: E501
         :type: bool
         """
         if completed is None:
             raise ValueError("Invalid value for `completed`, must not be `None`")  # noqa: E501
 
         self._completed = completed
 
@@ -167,15 +168,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TxStagesResponseInboundObserved, dict):
+        if issubclass(InboundObservedStage, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -183,15 +184,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TxStagesResponseInboundObserved):
+        if not isinstance(other, InboundObservedStage):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_outbound_delay.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/outbound_delay_stage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TxStagesResponseOutboundDelay(object):
+class OutboundDelayStage(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -36,89 +36,89 @@
     attribute_map = {
         'remaining_delay_blocks': 'remaining_delay_blocks',
         'remaining_delay_seconds': 'remaining_delay_seconds',
         'completed': 'completed'
     }
 
     def __init__(self, remaining_delay_blocks=None, remaining_delay_seconds=None, completed=None):  # noqa: E501
-        """TxStagesResponseOutboundDelay - a model defined in Swagger"""  # noqa: E501
+        """OutboundDelayStage - a model defined in Swagger"""  # noqa: E501
         self._remaining_delay_blocks = None
         self._remaining_delay_seconds = None
         self._completed = None
         self.discriminator = None
         if remaining_delay_blocks is not None:
             self.remaining_delay_blocks = remaining_delay_blocks
         if remaining_delay_seconds is not None:
             self.remaining_delay_seconds = remaining_delay_seconds
         self.completed = completed
 
     @property
     def remaining_delay_blocks(self):
-        """Gets the remaining_delay_blocks of this TxStagesResponseOutboundDelay.  # noqa: E501
+        """Gets the remaining_delay_blocks of this OutboundDelayStage.  # noqa: E501
 
         the number of remaining THORChain blocks the outbound will be delayed  # noqa: E501
 
-        :return: The remaining_delay_blocks of this TxStagesResponseOutboundDelay.  # noqa: E501
+        :return: The remaining_delay_blocks of this OutboundDelayStage.  # noqa: E501
         :rtype: int
         """
         return self._remaining_delay_blocks
 
     @remaining_delay_blocks.setter
     def remaining_delay_blocks(self, remaining_delay_blocks):
-        """Sets the remaining_delay_blocks of this TxStagesResponseOutboundDelay.
+        """Sets the remaining_delay_blocks of this OutboundDelayStage.
 
         the number of remaining THORChain blocks the outbound will be delayed  # noqa: E501
 
-        :param remaining_delay_blocks: The remaining_delay_blocks of this TxStagesResponseOutboundDelay.  # noqa: E501
+        :param remaining_delay_blocks: The remaining_delay_blocks of this OutboundDelayStage.  # noqa: E501
         :type: int
         """
 
         self._remaining_delay_blocks = remaining_delay_blocks
 
     @property
     def remaining_delay_seconds(self):
-        """Gets the remaining_delay_seconds of this TxStagesResponseOutboundDelay.  # noqa: E501
+        """Gets the remaining_delay_seconds of this OutboundDelayStage.  # noqa: E501
 
         the estimated remaining seconds of the outbound delay before it will be sent  # noqa: E501
 
-        :return: The remaining_delay_seconds of this TxStagesResponseOutboundDelay.  # noqa: E501
+        :return: The remaining_delay_seconds of this OutboundDelayStage.  # noqa: E501
         :rtype: int
         """
         return self._remaining_delay_seconds
 
     @remaining_delay_seconds.setter
     def remaining_delay_seconds(self, remaining_delay_seconds):
-        """Sets the remaining_delay_seconds of this TxStagesResponseOutboundDelay.
+        """Sets the remaining_delay_seconds of this OutboundDelayStage.
 
         the estimated remaining seconds of the outbound delay before it will be sent  # noqa: E501
 
-        :param remaining_delay_seconds: The remaining_delay_seconds of this TxStagesResponseOutboundDelay.  # noqa: E501
+        :param remaining_delay_seconds: The remaining_delay_seconds of this OutboundDelayStage.  # noqa: E501
         :type: int
         """
 
         self._remaining_delay_seconds = remaining_delay_seconds
 
     @property
     def completed(self):
-        """Gets the completed of this TxStagesResponseOutboundDelay.  # noqa: E501
+        """Gets the completed of this OutboundDelayStage.  # noqa: E501
 
         returns true if no transaction outbound delay remains  # noqa: E501
 
-        :return: The completed of this TxStagesResponseOutboundDelay.  # noqa: E501
+        :return: The completed of this OutboundDelayStage.  # noqa: E501
         :rtype: bool
         """
         return self._completed
 
     @completed.setter
     def completed(self, completed):
-        """Sets the completed of this TxStagesResponseOutboundDelay.
+        """Sets the completed of this OutboundDelayStage.
 
         returns true if no transaction outbound delay remains  # noqa: E501
 
-        :param completed: The completed of this TxStagesResponseOutboundDelay.  # noqa: E501
+        :param completed: The completed of this OutboundDelayStage.  # noqa: E501
         :type: bool
         """
         if completed is None:
             raise ValueError("Invalid value for `completed`, must not be `None`")  # noqa: E501
 
         self._completed = completed
 
@@ -139,15 +139,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TxStagesResponseOutboundDelay, dict):
+        if issubclass(OutboundDelayStage, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -155,15 +155,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TxStagesResponseOutboundDelay):
+        if not isinstance(other, OutboundDelayStage):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_outbound_signed.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/outbound_signed_stage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TxStagesResponseOutboundSigned(object):
+class OutboundSignedStage(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -36,89 +36,89 @@
     attribute_map = {
         'scheduled_outbound_height': 'scheduled_outbound_height',
         'blocks_since_scheduled': 'blocks_since_scheduled',
         'completed': 'completed'
     }
 
     def __init__(self, scheduled_outbound_height=None, blocks_since_scheduled=None, completed=None):  # noqa: E501
-        """TxStagesResponseOutboundSigned - a model defined in Swagger"""  # noqa: E501
+        """OutboundSignedStage - a model defined in Swagger"""  # noqa: E501
         self._scheduled_outbound_height = None
         self._blocks_since_scheduled = None
         self._completed = None
         self.discriminator = None
         if scheduled_outbound_height is not None:
             self.scheduled_outbound_height = scheduled_outbound_height
         if blocks_since_scheduled is not None:
             self.blocks_since_scheduled = blocks_since_scheduled
         self.completed = completed
 
     @property
     def scheduled_outbound_height(self):
-        """Gets the scheduled_outbound_height of this TxStagesResponseOutboundSigned.  # noqa: E501
+        """Gets the scheduled_outbound_height of this OutboundSignedStage.  # noqa: E501
 
         THORChain height for which the external outbound is scheduled  # noqa: E501
 
-        :return: The scheduled_outbound_height of this TxStagesResponseOutboundSigned.  # noqa: E501
+        :return: The scheduled_outbound_height of this OutboundSignedStage.  # noqa: E501
         :rtype: int
         """
         return self._scheduled_outbound_height
 
     @scheduled_outbound_height.setter
     def scheduled_outbound_height(self, scheduled_outbound_height):
-        """Sets the scheduled_outbound_height of this TxStagesResponseOutboundSigned.
+        """Sets the scheduled_outbound_height of this OutboundSignedStage.
 
         THORChain height for which the external outbound is scheduled  # noqa: E501
 
-        :param scheduled_outbound_height: The scheduled_outbound_height of this TxStagesResponseOutboundSigned.  # noqa: E501
+        :param scheduled_outbound_height: The scheduled_outbound_height of this OutboundSignedStage.  # noqa: E501
         :type: int
         """
 
         self._scheduled_outbound_height = scheduled_outbound_height
 
     @property
     def blocks_since_scheduled(self):
-        """Gets the blocks_since_scheduled of this TxStagesResponseOutboundSigned.  # noqa: E501
+        """Gets the blocks_since_scheduled of this OutboundSignedStage.  # noqa: E501
 
         THORChain blocks since the scheduled outbound height  # noqa: E501
 
-        :return: The blocks_since_scheduled of this TxStagesResponseOutboundSigned.  # noqa: E501
+        :return: The blocks_since_scheduled of this OutboundSignedStage.  # noqa: E501
         :rtype: int
         """
         return self._blocks_since_scheduled
 
     @blocks_since_scheduled.setter
     def blocks_since_scheduled(self, blocks_since_scheduled):
-        """Sets the blocks_since_scheduled of this TxStagesResponseOutboundSigned.
+        """Sets the blocks_since_scheduled of this OutboundSignedStage.
 
         THORChain blocks since the scheduled outbound height  # noqa: E501
 
-        :param blocks_since_scheduled: The blocks_since_scheduled of this TxStagesResponseOutboundSigned.  # noqa: E501
+        :param blocks_since_scheduled: The blocks_since_scheduled of this OutboundSignedStage.  # noqa: E501
         :type: int
         """
 
         self._blocks_since_scheduled = blocks_since_scheduled
 
     @property
     def completed(self):
-        """Gets the completed of this TxStagesResponseOutboundSigned.  # noqa: E501
+        """Gets the completed of this OutboundSignedStage.  # noqa: E501
 
         returns true if an external transaction has been signed and broadcast (and observed in its mempool)  # noqa: E501
 
-        :return: The completed of this TxStagesResponseOutboundSigned.  # noqa: E501
+        :return: The completed of this OutboundSignedStage.  # noqa: E501
         :rtype: bool
         """
         return self._completed
 
     @completed.setter
     def completed(self, completed):
-        """Sets the completed of this TxStagesResponseOutboundSigned.
+        """Sets the completed of this OutboundSignedStage.
 
         returns true if an external transaction has been signed and broadcast (and observed in its mempool)  # noqa: E501
 
-        :param completed: The completed of this TxStagesResponseOutboundSigned.  # noqa: E501
+        :param completed: The completed of this OutboundSignedStage.  # noqa: E501
         :type: bool
         """
         if completed is None:
             raise ValueError("Invalid value for `completed`, must not be `None`")  # noqa: E501
 
         self._completed = completed
 
@@ -139,15 +139,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TxStagesResponseOutboundSigned, dict):
+        if issubclass(OutboundSignedStage, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -155,15 +155,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TxStagesResponseOutboundSigned):
+        if not isinstance(other, OutboundSignedStage):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_swap_finalised.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/swap_finalised_stage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TxStagesResponseSwapFinalised(object):
+class SwapFinalisedStage(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,37 +32,37 @@
     }
 
     attribute_map = {
         'completed': 'completed'
     }
 
     def __init__(self, completed=None):  # noqa: E501
-        """TxStagesResponseSwapFinalised - a model defined in Swagger"""  # noqa: E501
+        """SwapFinalisedStage - a model defined in Swagger"""  # noqa: E501
         self._completed = None
         self.discriminator = None
         self.completed = completed
 
     @property
     def completed(self):
-        """Gets the completed of this TxStagesResponseSwapFinalised.  # noqa: E501
+        """Gets the completed of this SwapFinalisedStage.  # noqa: E501
 
         (to be deprecated in favor of swap_status) returns true if an inbound transaction's swap (successful or refunded) is no longer pending  # noqa: E501
 
-        :return: The completed of this TxStagesResponseSwapFinalised.  # noqa: E501
+        :return: The completed of this SwapFinalisedStage.  # noqa: E501
         :rtype: bool
         """
         return self._completed
 
     @completed.setter
     def completed(self, completed):
-        """Sets the completed of this TxStagesResponseSwapFinalised.
+        """Sets the completed of this SwapFinalisedStage.
 
         (to be deprecated in favor of swap_status) returns true if an inbound transaction's swap (successful or refunded) is no longer pending  # noqa: E501
 
-        :param completed: The completed of this TxStagesResponseSwapFinalised.  # noqa: E501
+        :param completed: The completed of this SwapFinalisedStage.  # noqa: E501
         :type: bool
         """
         if completed is None:
             raise ValueError("Invalid value for `completed`, must not be `None`")  # noqa: E501
 
         self._completed = completed
 
@@ -83,15 +83,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TxStagesResponseSwapFinalised, dict):
+        if issubclass(SwapFinalisedStage, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -99,15 +99,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TxStagesResponseSwapFinalised):
+        if not isinstance(other, SwapFinalisedStage):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_swap_status.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/vault_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,100 +1,99 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TxStagesResponseSwapStatus(object):
+class VaultInfo(object):
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
-        'pending': 'bool',
-        'streaming': 'TxStagesResponseSwapStatusStreaming'
+        'pub_key': 'str',
+        'routers': 'list[VaultRouter]'
     }
 
     attribute_map = {
-        'pending': 'pending',
-        'streaming': 'streaming'
+        'pub_key': 'pub_key',
+        'routers': 'routers'
     }
 
-    def __init__(self, pending=None, streaming=None):  # noqa: E501
-        """TxStagesResponseSwapStatus - a model defined in Swagger"""  # noqa: E501
-        self._pending = None
-        self._streaming = None
+    def __init__(self, pub_key=None, routers=None):  # noqa: E501
+        """VaultInfo - a model defined in Swagger"""  # noqa: E501
+        self._pub_key = None
+        self._routers = None
         self.discriminator = None
-        self.pending = pending
-        if streaming is not None:
-            self.streaming = streaming
+        self.pub_key = pub_key
+        self.routers = routers
 
     @property
-    def pending(self):
-        """Gets the pending of this TxStagesResponseSwapStatus.  # noqa: E501
+    def pub_key(self):
+        """Gets the pub_key of this VaultInfo.  # noqa: E501
 
-        true when awaiting a swap  # noqa: E501
 
-        :return: The pending of this TxStagesResponseSwapStatus.  # noqa: E501
-        :rtype: bool
+        :return: The pub_key of this VaultInfo.  # noqa: E501
+        :rtype: str
         """
-        return self._pending
+        return self._pub_key
 
-    @pending.setter
-    def pending(self, pending):
-        """Sets the pending of this TxStagesResponseSwapStatus.
+    @pub_key.setter
+    def pub_key(self, pub_key):
+        """Sets the pub_key of this VaultInfo.
 
-        true when awaiting a swap  # noqa: E501
 
-        :param pending: The pending of this TxStagesResponseSwapStatus.  # noqa: E501
-        :type: bool
+        :param pub_key: The pub_key of this VaultInfo.  # noqa: E501
+        :type: str
         """
-        if pending is None:
-            raise ValueError("Invalid value for `pending`, must not be `None`")  # noqa: E501
+        if pub_key is None:
+            raise ValueError("Invalid value for `pub_key`, must not be `None`")  # noqa: E501
 
-        self._pending = pending
+        self._pub_key = pub_key
 
     @property
-    def streaming(self):
-        """Gets the streaming of this TxStagesResponseSwapStatus.  # noqa: E501
+    def routers(self):
+        """Gets the routers of this VaultInfo.  # noqa: E501
 
 
-        :return: The streaming of this TxStagesResponseSwapStatus.  # noqa: E501
-        :rtype: TxStagesResponseSwapStatusStreaming
+        :return: The routers of this VaultInfo.  # noqa: E501
+        :rtype: list[VaultRouter]
         """
-        return self._streaming
+        return self._routers
 
-    @streaming.setter
-    def streaming(self, streaming):
-        """Sets the streaming of this TxStagesResponseSwapStatus.
+    @routers.setter
+    def routers(self, routers):
+        """Sets the routers of this VaultInfo.
 
 
-        :param streaming: The streaming of this TxStagesResponseSwapStatus.  # noqa: E501
-        :type: TxStagesResponseSwapStatusStreaming
+        :param routers: The routers of this VaultInfo.  # noqa: E501
+        :type: list[VaultRouter]
         """
+        if routers is None:
+            raise ValueError("Invalid value for `routers`, must not be `None`")  # noqa: E501
 
-        self._streaming = streaming
+        self._routers = routers
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -109,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TxStagesResponseSwapStatus, dict):
+        if issubclass(VaultInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -125,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TxStagesResponseSwapStatus):
+        if not isinstance(other, VaultInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_swap_status_streaming.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/streaming_status.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TxStagesResponseSwapStatusStreaming(object):
+class StreamingStatus(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -36,91 +36,91 @@
     attribute_map = {
         'interval': 'interval',
         'quantity': 'quantity',
         'count': 'count'
     }
 
     def __init__(self, interval=None, quantity=None, count=None):  # noqa: E501
-        """TxStagesResponseSwapStatusStreaming - a model defined in Swagger"""  # noqa: E501
+        """StreamingStatus - a model defined in Swagger"""  # noqa: E501
         self._interval = None
         self._quantity = None
         self._count = None
         self.discriminator = None
         self.interval = interval
         self.quantity = quantity
         self.count = count
 
     @property
     def interval(self):
-        """Gets the interval of this TxStagesResponseSwapStatusStreaming.  # noqa: E501
+        """Gets the interval of this StreamingStatus.  # noqa: E501
 
         how often each swap is made, in blocks  # noqa: E501
 
-        :return: The interval of this TxStagesResponseSwapStatusStreaming.  # noqa: E501
+        :return: The interval of this StreamingStatus.  # noqa: E501
         :rtype: int
         """
         return self._interval
 
     @interval.setter
     def interval(self, interval):
-        """Sets the interval of this TxStagesResponseSwapStatusStreaming.
+        """Sets the interval of this StreamingStatus.
 
         how often each swap is made, in blocks  # noqa: E501
 
-        :param interval: The interval of this TxStagesResponseSwapStatusStreaming.  # noqa: E501
+        :param interval: The interval of this StreamingStatus.  # noqa: E501
         :type: int
         """
         if interval is None:
             raise ValueError("Invalid value for `interval`, must not be `None`")  # noqa: E501
 
         self._interval = interval
 
     @property
     def quantity(self):
-        """Gets the quantity of this TxStagesResponseSwapStatusStreaming.  # noqa: E501
+        """Gets the quantity of this StreamingStatus.  # noqa: E501
 
         the total number of swaps in a streaming swaps  # noqa: E501
 
-        :return: The quantity of this TxStagesResponseSwapStatusStreaming.  # noqa: E501
+        :return: The quantity of this StreamingStatus.  # noqa: E501
         :rtype: int
         """
         return self._quantity
 
     @quantity.setter
     def quantity(self, quantity):
-        """Sets the quantity of this TxStagesResponseSwapStatusStreaming.
+        """Sets the quantity of this StreamingStatus.
 
         the total number of swaps in a streaming swaps  # noqa: E501
 
-        :param quantity: The quantity of this TxStagesResponseSwapStatusStreaming.  # noqa: E501
+        :param quantity: The quantity of this StreamingStatus.  # noqa: E501
         :type: int
         """
         if quantity is None:
             raise ValueError("Invalid value for `quantity`, must not be `None`")  # noqa: E501
 
         self._quantity = quantity
 
     @property
     def count(self):
-        """Gets the count of this TxStagesResponseSwapStatusStreaming.  # noqa: E501
+        """Gets the count of this StreamingStatus.  # noqa: E501
 
         the amount of swap attempts so far  # noqa: E501
 
-        :return: The count of this TxStagesResponseSwapStatusStreaming.  # noqa: E501
+        :return: The count of this StreamingStatus.  # noqa: E501
         :rtype: int
         """
         return self._count
 
     @count.setter
     def count(self, count):
-        """Sets the count of this TxStagesResponseSwapStatusStreaming.
+        """Sets the count of this StreamingStatus.
 
         the amount of swap attempts so far  # noqa: E501
 
-        :param count: The count of this TxStagesResponseSwapStatusStreaming.  # noqa: E501
+        :param count: The count of this StreamingStatus.  # noqa: E501
         :type: int
         """
         if count is None:
             raise ValueError("Invalid value for `count`, must not be `None`")  # noqa: E501
 
         self._count = count
 
@@ -141,15 +141,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TxStagesResponseSwapStatusStreaming, dict):
+        if issubclass(StreamingStatus, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -157,15 +157,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TxStagesResponseSwapStatusStreaming):
+        if not isinstance(other, StreamingStatus):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_status_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/tx_status_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -25,15 +25,15 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'tx': 'Tx',
-        'planned_out_txs': 'list[TxStatusResponsePlannedOutTxs]',
+        'planned_out_txs': 'list[PlannedOutTx]',
         'out_txs': 'list[Tx]',
         'stages': 'TxStagesResponse'
     }
 
     attribute_map = {
         'tx': 'tx',
         'planned_out_txs': 'planned_out_txs',
@@ -79,25 +79,25 @@
 
     @property
     def planned_out_txs(self):
         """Gets the planned_out_txs of this TxStatusResponse.  # noqa: E501
 
 
         :return: The planned_out_txs of this TxStatusResponse.  # noqa: E501
-        :rtype: list[TxStatusResponsePlannedOutTxs]
+        :rtype: list[PlannedOutTx]
         """
         return self._planned_out_txs
 
     @planned_out_txs.setter
     def planned_out_txs(self, planned_out_txs):
         """Sets the planned_out_txs of this TxStatusResponse.
 
 
         :param planned_out_txs: The planned_out_txs of this TxStatusResponse.  # noqa: E501
-        :type: list[TxStatusResponsePlannedOutTxs]
+        :type: list[PlannedOutTx]
         """
 
         self._planned_out_txs = planned_out_txs
 
     @property
     def out_txs(self):
         """Gets the out_txs of this TxStatusResponse.  # noqa: E501
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_status_response_planned_out_txs.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/planned_out_tx.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TxStatusResponsePlannedOutTxs(object):
+class PlannedOutTx(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -38,112 +38,112 @@
         'chain': 'chain',
         'to_address': 'to_address',
         'coin': 'coin',
         'refund': 'refund'
     }
 
     def __init__(self, chain=None, to_address=None, coin=None, refund=None):  # noqa: E501
-        """TxStatusResponsePlannedOutTxs - a model defined in Swagger"""  # noqa: E501
+        """PlannedOutTx - a model defined in Swagger"""  # noqa: E501
         self._chain = None
         self._to_address = None
         self._coin = None
         self._refund = None
         self.discriminator = None
         self.chain = chain
         self.to_address = to_address
         self.coin = coin
         self.refund = refund
 
     @property
     def chain(self):
-        """Gets the chain of this TxStatusResponsePlannedOutTxs.  # noqa: E501
+        """Gets the chain of this PlannedOutTx.  # noqa: E501
 
 
-        :return: The chain of this TxStatusResponsePlannedOutTxs.  # noqa: E501
+        :return: The chain of this PlannedOutTx.  # noqa: E501
         :rtype: str
         """
         return self._chain
 
     @chain.setter
     def chain(self, chain):
-        """Sets the chain of this TxStatusResponsePlannedOutTxs.
+        """Sets the chain of this PlannedOutTx.
 
 
-        :param chain: The chain of this TxStatusResponsePlannedOutTxs.  # noqa: E501
+        :param chain: The chain of this PlannedOutTx.  # noqa: E501
         :type: str
         """
         if chain is None:
             raise ValueError("Invalid value for `chain`, must not be `None`")  # noqa: E501
 
         self._chain = chain
 
     @property
     def to_address(self):
-        """Gets the to_address of this TxStatusResponsePlannedOutTxs.  # noqa: E501
+        """Gets the to_address of this PlannedOutTx.  # noqa: E501
 
 
-        :return: The to_address of this TxStatusResponsePlannedOutTxs.  # noqa: E501
+        :return: The to_address of this PlannedOutTx.  # noqa: E501
         :rtype: str
         """
         return self._to_address
 
     @to_address.setter
     def to_address(self, to_address):
-        """Sets the to_address of this TxStatusResponsePlannedOutTxs.
+        """Sets the to_address of this PlannedOutTx.
 
 
-        :param to_address: The to_address of this TxStatusResponsePlannedOutTxs.  # noqa: E501
+        :param to_address: The to_address of this PlannedOutTx.  # noqa: E501
         :type: str
         """
         if to_address is None:
             raise ValueError("Invalid value for `to_address`, must not be `None`")  # noqa: E501
 
         self._to_address = to_address
 
     @property
     def coin(self):
-        """Gets the coin of this TxStatusResponsePlannedOutTxs.  # noqa: E501
+        """Gets the coin of this PlannedOutTx.  # noqa: E501
 
 
-        :return: The coin of this TxStatusResponsePlannedOutTxs.  # noqa: E501
+        :return: The coin of this PlannedOutTx.  # noqa: E501
         :rtype: Coin
         """
         return self._coin
 
     @coin.setter
     def coin(self, coin):
-        """Sets the coin of this TxStatusResponsePlannedOutTxs.
+        """Sets the coin of this PlannedOutTx.
 
 
-        :param coin: The coin of this TxStatusResponsePlannedOutTxs.  # noqa: E501
+        :param coin: The coin of this PlannedOutTx.  # noqa: E501
         :type: Coin
         """
         if coin is None:
             raise ValueError("Invalid value for `coin`, must not be `None`")  # noqa: E501
 
         self._coin = coin
 
     @property
     def refund(self):
-        """Gets the refund of this TxStatusResponsePlannedOutTxs.  # noqa: E501
+        """Gets the refund of this PlannedOutTx.  # noqa: E501
 
         returns true if the planned transaction has a refund memo  # noqa: E501
 
-        :return: The refund of this TxStatusResponsePlannedOutTxs.  # noqa: E501
+        :return: The refund of this PlannedOutTx.  # noqa: E501
         :rtype: bool
         """
         return self._refund
 
     @refund.setter
     def refund(self, refund):
-        """Sets the refund of this TxStatusResponsePlannedOutTxs.
+        """Sets the refund of this PlannedOutTx.
 
         returns true if the planned transaction has a refund memo  # noqa: E501
 
-        :param refund: The refund of this TxStatusResponsePlannedOutTxs.  # noqa: E501
+        :param refund: The refund of this PlannedOutTx.  # noqa: E501
         :type: bool
         """
         if refund is None:
             raise ValueError("Invalid value for `refund`, must not be `None`")  # noqa: E501
 
         self._refund = refund
 
@@ -164,15 +164,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TxStatusResponsePlannedOutTxs, dict):
+        if issubclass(PlannedOutTx, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -180,15 +180,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TxStatusResponsePlannedOutTxs):
+        if not isinstance(other, PlannedOutTx):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_address.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/vault_address.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -38,18 +38,16 @@
     }
 
     def __init__(self, chain=None, address=None):  # noqa: E501
         """VaultAddress - a model defined in Swagger"""  # noqa: E501
         self._chain = None
         self._address = None
         self.discriminator = None
-        if chain is not None:
-            self.chain = chain
-        if address is not None:
-            self.address = address
+        self.chain = chain
+        self.address = address
 
     @property
     def chain(self):
         """Gets the chain of this VaultAddress.  # noqa: E501
 
 
         :return: The chain of this VaultAddress.  # noqa: E501
@@ -61,14 +59,16 @@
     def chain(self, chain):
         """Sets the chain of this VaultAddress.
 
 
         :param chain: The chain of this VaultAddress.  # noqa: E501
         :type: str
         """
+        if chain is None:
+            raise ValueError("Invalid value for `chain`, must not be `None`")  # noqa: E501
 
         self._chain = chain
 
     @property
     def address(self):
         """Gets the address of this VaultAddress.  # noqa: E501
 
@@ -82,14 +82,16 @@
     def address(self, address):
         """Sets the address of this VaultAddress.
 
 
         :param address: The address of this VaultAddress.  # noqa: E501
         :type: str
         """
+        if address is None:
+            raise ValueError("Invalid value for `address`, must not be `None`")  # noqa: E501
 
         self._address = address
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_info.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/keygen.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,99 +1,123 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class VaultInfo(object):
+class Keygen(object):
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
-        'pub_key': 'str',
-        'routers': 'list[VaultRouter]'
+        'id': 'str',
+        'type': 'str',
+        'members': 'list[str]'
     }
 
     attribute_map = {
-        'pub_key': 'pub_key',
-        'routers': 'routers'
+        'id': 'id',
+        'type': 'type',
+        'members': 'members'
     }
 
-    def __init__(self, pub_key=None, routers=None):  # noqa: E501
-        """VaultInfo - a model defined in Swagger"""  # noqa: E501
-        self._pub_key = None
-        self._routers = None
+    def __init__(self, id=None, type=None, members=None):  # noqa: E501
+        """Keygen - a model defined in Swagger"""  # noqa: E501
+        self._id = None
+        self._type = None
+        self._members = None
         self.discriminator = None
-        self.pub_key = pub_key
-        self.routers = routers
+        if id is not None:
+            self.id = id
+        if type is not None:
+            self.type = type
+        if members is not None:
+            self.members = members
 
     @property
-    def pub_key(self):
-        """Gets the pub_key of this VaultInfo.  # noqa: E501
+    def id(self):
+        """Gets the id of this Keygen.  # noqa: E501
 
 
-        :return: The pub_key of this VaultInfo.  # noqa: E501
+        :return: The id of this Keygen.  # noqa: E501
         :rtype: str
         """
-        return self._pub_key
+        return self._id
 
-    @pub_key.setter
-    def pub_key(self, pub_key):
-        """Sets the pub_key of this VaultInfo.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this Keygen.
 
 
-        :param pub_key: The pub_key of this VaultInfo.  # noqa: E501
+        :param id: The id of this Keygen.  # noqa: E501
         :type: str
         """
-        if pub_key is None:
-            raise ValueError("Invalid value for `pub_key`, must not be `None`")  # noqa: E501
 
-        self._pub_key = pub_key
+        self._id = id
 
     @property
-    def routers(self):
-        """Gets the routers of this VaultInfo.  # noqa: E501
+    def type(self):
+        """Gets the type of this Keygen.  # noqa: E501
 
 
-        :return: The routers of this VaultInfo.  # noqa: E501
-        :rtype: list[VaultRouter]
+        :return: The type of this Keygen.  # noqa: E501
+        :rtype: str
+        """
+        return self._type
+
+    @type.setter
+    def type(self, type):
+        """Sets the type of this Keygen.
+
+
+        :param type: The type of this Keygen.  # noqa: E501
+        :type: str
+        """
+
+        self._type = type
+
+    @property
+    def members(self):
+        """Gets the members of this Keygen.  # noqa: E501
+
+
+        :return: The members of this Keygen.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._routers
+        return self._members
 
-    @routers.setter
-    def routers(self, routers):
-        """Sets the routers of this VaultInfo.
+    @members.setter
+    def members(self, members):
+        """Sets the members of this Keygen.
 
 
-        :param routers: The routers of this VaultInfo.  # noqa: E501
-        :type: list[VaultRouter]
+        :param members: The members of this Keygen.  # noqa: E501
+        :type: list[str]
         """
-        if routers is None:
-            raise ValueError("Invalid value for `routers`, must not be `None`")  # noqa: E501
 
-        self._routers = routers
+        self._members = members
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -108,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(VaultInfo, dict):
+        if issubclass(Keygen, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -124,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, VaultInfo):
+        if not isinstance(other, Keygen):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_pubkeys_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/vault_pubkeys_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/vault_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_router.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/vault_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vaults_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/vaults_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/version_response.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/models/version_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode/rest.py` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.130.1
+    OpenAPI spec version: 1.132.0
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import io
 import json
 import logging
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode.egg-info/PKG-INFO` & `xchainpy2_thornode-1.132.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,14 @@
-Metadata-Version: 2.1
-Name: xchainpy2-thornode
-Version: 1.130.1
-Summary: Thornode API
-Home-page: 
-Author-email: devs@thorchain.org
-Keywords: Swagger,Thornode API
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: urllib3>=1.15
-Requires-Dist: six>=1.10
-Requires-Dist: certifi
-Requires-Dist: python-dateutil
-Requires-Dist: aiohttp
-
 # xchainpy2-thornode
 Thornode REST API.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.130.1
-- Package version: 1.130.1
+- API version: 1.132.0
+- Package version: 1.132.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -101,19 +86,23 @@
 *MimirApi* | [**mimir_v2_ids**](docs/MimirApi.md#mimir_v2_ids) | **GET** /thorchain/mimirV2/ids | 
 *NetworkApi* | [**ban**](docs/NetworkApi.md#ban) | **GET** /thorchain/ban/{address} | 
 *NetworkApi* | [**constants**](docs/NetworkApi.md#constants) | **GET** /thorchain/constants | 
 *NetworkApi* | [**inbound_addresses**](docs/NetworkApi.md#inbound_addresses) | **GET** /thorchain/inbound_addresses | 
 *NetworkApi* | [**lastblock**](docs/NetworkApi.md#lastblock) | **GET** /thorchain/lastblock | 
 *NetworkApi* | [**lastblock_chain**](docs/NetworkApi.md#lastblock_chain) | **GET** /thorchain/lastblock/{chain} | 
 *NetworkApi* | [**network**](docs/NetworkApi.md#network) | **GET** /thorchain/network | 
+*NetworkApi* | [**outbound_fee_asset**](docs/NetworkApi.md#outbound_fee_asset) | **GET** /thorchain/outbound_fee/{asset} | 
+*NetworkApi* | [**outbound_fees**](docs/NetworkApi.md#outbound_fees) | **GET** /thorchain/outbound_fees | 
 *NetworkApi* | [**ragnarok**](docs/NetworkApi.md#ragnarok) | **GET** /thorchain/ragnarok | 
 *NetworkApi* | [**version**](docs/NetworkApi.md#version) | **GET** /thorchain/version | 
 *NodesApi* | [**node**](docs/NodesApi.md#node) | **GET** /thorchain/node/{address} | 
 *NodesApi* | [**nodes**](docs/NodesApi.md#nodes) | **GET** /thorchain/nodes | 
 *POLApi* | [**pol**](docs/POLApi.md#pol) | **GET** /thorchain/pol | 
+*PoolSlipApi* | [**poolslip**](docs/PoolSlipApi.md#poolslip) | **GET** /thorchain/slip/{asset} | 
+*PoolSlipApi* | [**poolslips**](docs/PoolSlipApi.md#poolslips) | **GET** /thorchain/slips | 
 *PoolsApi* | [**dpool**](docs/PoolsApi.md#dpool) | **GET** /thorchain/dpool/{asset} | 
 *PoolsApi* | [**dpools**](docs/PoolsApi.md#dpools) | **GET** /thorchain/dpools | 
 *PoolsApi* | [**pool**](docs/PoolsApi.md#pool) | **GET** /thorchain/pool/{asset} | 
 *PoolsApi* | [**pools**](docs/PoolsApi.md#pools) | **GET** /thorchain/pools | 
 *QueueApi* | [**queue**](docs/QueueApi.md#queue) | **GET** /thorchain/queue | 
 *QueueApi* | [**queue_outbound**](docs/QueueApi.md#queue_outbound) | **GET** /thorchain/queue/outbound | 
 *QueueApi* | [**queue_scheduled**](docs/QueueApi.md#queue_scheduled) | **GET** /thorchain/queue/scheduled | 
@@ -123,14 +112,15 @@
 *QuoteApi* | [**quotesaverdeposit**](docs/QuoteApi.md#quotesaverdeposit) | **GET** /thorchain/quote/saver/deposit | 
 *QuoteApi* | [**quotesaverwithdraw**](docs/QuoteApi.md#quotesaverwithdraw) | **GET** /thorchain/quote/saver/withdraw | 
 *QuoteApi* | [**quoteswap**](docs/QuoteApi.md#quoteswap) | **GET** /thorchain/quote/swap | 
 *SaversApi* | [**saver**](docs/SaversApi.md#saver) | **GET** /thorchain/pool/{asset}/saver/{address} | 
 *SaversApi* | [**savers**](docs/SaversApi.md#savers) | **GET** /thorchain/pool/{asset}/savers | 
 *StreamingSwapApi* | [**stream_swap**](docs/StreamingSwapApi.md#stream_swap) | **GET** /thorchain/swap/streaming/{hash} | 
 *StreamingSwapApi* | [**stream_swaps**](docs/StreamingSwapApi.md#stream_swaps) | **GET** /thorchain/swaps/streaming | 
+*TSSApi* | [**keygen_pubkey**](docs/TSSApi.md#keygen_pubkey) | **GET** /thorchain/keygen/{height}/{pubkey} | 
 *TSSApi* | [**keysign**](docs/TSSApi.md#keysign) | **GET** /thorchain/keysign/{height} | 
 *TSSApi* | [**keysign_pubkey**](docs/TSSApi.md#keysign_pubkey) | **GET** /thorchain/keysign/{height}/{pubkey} | 
 *TSSApi* | [**metrics**](docs/TSSApi.md#metrics) | **GET** /thorchain/metrics | 
 *TSSApi* | [**metrics_keygen**](docs/TSSApi.md#metrics_keygen) | **GET** /thorchain/metric/keygen/{pubkey} | 
 *ThornamesApi* | [**thorname**](docs/ThornamesApi.md#thorname) | **GET** /thorchain/thorname/{name} | 
 *TradeAccountApi* | [**trade_account**](docs/TradeAccountApi.md#trade_account) | **GET** /thorchain/trade/account/{address} | 
 *TradeAccountsApi* | [**trade_accounts**](docs/TradeAccountsApi.md#trade_accounts) | **GET** /thorchain/trade/accounts/{asset} | 
@@ -164,18 +154,25 @@
  - [Coin](docs/Coin.md)
  - [ConstantsResponse](docs/ConstantsResponse.md)
  - [DerivedPool](docs/DerivedPool.md)
  - [DerivedPoolResponse](docs/DerivedPoolResponse.md)
  - [DerivedPoolsResponse](docs/DerivedPoolsResponse.md)
  - [InboundAddress](docs/InboundAddress.md)
  - [InboundAddressesResponse](docs/InboundAddressesResponse.md)
+ - [InboundConfirmationCountedStage](docs/InboundConfirmationCountedStage.md)
+ - [InboundFinalisedStage](docs/InboundFinalisedStage.md)
+ - [InboundObservedStage](docs/InboundObservedStage.md)
+ - [InlineResponse200](docs/InlineResponse200.md)
  - [InvariantResponse](docs/InvariantResponse.md)
  - [InvariantsResponse](docs/InvariantsResponse.md)
+ - [Keygen](docs/Keygen.md)
+ - [KeygenBlock](docs/KeygenBlock.md)
  - [KeygenMetric](docs/KeygenMetric.md)
  - [KeygenMetricsResponse](docs/KeygenMetricsResponse.md)
+ - [KeygenResponse](docs/KeygenResponse.md)
  - [KeysignInfo](docs/KeysignInfo.md)
  - [KeysignMetrics](docs/KeysignMetrics.md)
  - [KeysignResponse](docs/KeysignResponse.md)
  - [LastBlock](docs/LastBlock.md)
  - [LastBlockResponse](docs/LastBlockResponse.md)
  - [LiquidityProvider](docs/LiquidityProvider.md)
  - [LiquidityProviderResponse](docs/LiquidityProviderResponse.md)
@@ -194,35 +191,44 @@
  - [NodeJail](docs/NodeJail.md)
  - [NodeKeygenMetric](docs/NodeKeygenMetric.md)
  - [NodePreflightStatus](docs/NodePreflightStatus.md)
  - [NodePubKeySet](docs/NodePubKeySet.md)
  - [NodeResponse](docs/NodeResponse.md)
  - [NodesResponse](docs/NodesResponse.md)
  - [ObservedTx](docs/ObservedTx.md)
+ - [OutboundDelayStage](docs/OutboundDelayStage.md)
+ - [OutboundFee](docs/OutboundFee.md)
+ - [OutboundFeesResponse](docs/OutboundFeesResponse.md)
  - [OutboundResponse](docs/OutboundResponse.md)
+ - [OutboundSignedStage](docs/OutboundSignedStage.md)
  - [POLResponse](docs/POLResponse.md)
  - [Ping](docs/Ping.md)
+ - [PlannedOutTx](docs/PlannedOutTx.md)
  - [Pool](docs/Pool.md)
  - [PoolResponse](docs/PoolResponse.md)
+ - [PoolSlipResponse](docs/PoolSlipResponse.md)
  - [PoolsResponse](docs/PoolsResponse.md)
  - [QueueResponse](docs/QueueResponse.md)
  - [QuoteFees](docs/QuoteFees.md)
  - [QuoteLoanCloseResponse](docs/QuoteLoanCloseResponse.md)
  - [QuoteLoanOpenResponse](docs/QuoteLoanOpenResponse.md)
  - [QuoteSaverDepositResponse](docs/QuoteSaverDepositResponse.md)
  - [QuoteSaverWithdrawResponse](docs/QuoteSaverWithdrawResponse.md)
  - [QuoteSwapResponse](docs/QuoteSwapResponse.md)
  - [Saver](docs/Saver.md)
  - [SaverResponse](docs/SaverResponse.md)
  - [SaversResponse](docs/SaversResponse.md)
  - [ScheduledResponse](docs/ScheduledResponse.md)
+ - [StreamingStatus](docs/StreamingStatus.md)
  - [StreamingSwap](docs/StreamingSwap.md)
  - [StreamingSwapResponse](docs/StreamingSwapResponse.md)
  - [StreamingSwapsResponse](docs/StreamingSwapsResponse.md)
+ - [SwapFinalisedStage](docs/SwapFinalisedStage.md)
  - [SwapQueueResponse](docs/SwapQueueResponse.md)
+ - [SwapStatus](docs/SwapStatus.md)
  - [SwapperCloutResponse](docs/SwapperCloutResponse.md)
  - [Thorname](docs/Thorname.md)
  - [ThornameAlias](docs/ThornameAlias.md)
  - [ThornameResponse](docs/ThornameResponse.md)
  - [TradeAccountResponse](docs/TradeAccountResponse.md)
  - [TradeAccountsResponse](docs/TradeAccountsResponse.md)
  - [TradeUnitResponse](docs/TradeUnitResponse.md)
@@ -231,32 +237,25 @@
  - [TssMetric](docs/TssMetric.md)
  - [Tx](docs/Tx.md)
  - [TxDetailsResponse](docs/TxDetailsResponse.md)
  - [TxOutItem](docs/TxOutItem.md)
  - [TxResponse](docs/TxResponse.md)
  - [TxSignersResponse](docs/TxSignersResponse.md)
  - [TxStagesResponse](docs/TxStagesResponse.md)
- - [TxStagesResponseInboundConfirmationCounted](docs/TxStagesResponseInboundConfirmationCounted.md)
- - [TxStagesResponseInboundFinalised](docs/TxStagesResponseInboundFinalised.md)
- - [TxStagesResponseInboundObserved](docs/TxStagesResponseInboundObserved.md)
- - [TxStagesResponseOutboundDelay](docs/TxStagesResponseOutboundDelay.md)
- - [TxStagesResponseOutboundSigned](docs/TxStagesResponseOutboundSigned.md)
- - [TxStagesResponseSwapFinalised](docs/TxStagesResponseSwapFinalised.md)
- - [TxStagesResponseSwapStatus](docs/TxStagesResponseSwapStatus.md)
- - [TxStagesResponseSwapStatusStreaming](docs/TxStagesResponseSwapStatusStreaming.md)
  - [TxStatusResponse](docs/TxStatusResponse.md)
- - [TxStatusResponsePlannedOutTxs](docs/TxStatusResponsePlannedOutTxs.md)
  - [Vault](docs/Vault.md)
  - [VaultAddress](docs/VaultAddress.md)
  - [VaultInfo](docs/VaultInfo.md)
  - [VaultPubkeysResponse](docs/VaultPubkeysResponse.md)
  - [VaultResponse](docs/VaultResponse.md)
  - [VaultRouter](docs/VaultRouter.md)
  - [VaultsResponse](docs/VaultsResponse.md)
  - [VersionResponse](docs/VersionResponse.md)
+ - [YggdrasilVault](docs/YggdrasilVault.md)
+ - [YggdrasilVaultsResponse](docs/YggdrasilVaultsResponse.md)
 
 ## Documentation For Authorization
 
  All endpoints do not require authorization.
 
 
 ## Author
```

### Comparing `xchainpy2-thornode-1.130.1/xchainpy2_thornode.egg-info/SOURCES.txt` & `xchainpy2_thornode-1.132.0/xchainpy2_thornode.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -22,19 +22,26 @@
 test/test_constants_response.py
 test/test_derived_pool.py
 test/test_derived_pool_response.py
 test/test_derived_pools_response.py
 test/test_health_api.py
 test/test_inbound_address.py
 test/test_inbound_addresses_response.py
+test/test_inbound_confirmation_counted_stage.py
+test/test_inbound_finalised_stage.py
+test/test_inbound_observed_stage.py
+test/test_inline_response200.py
 test/test_invariant_response.py
 test/test_invariants_api.py
 test/test_invariants_response.py
+test/test_keygen.py
+test/test_keygen_block.py
 test/test_keygen_metric.py
 test/test_keygen_metrics_response.py
+test/test_keygen_response.py
 test/test_keysign_info.py
 test/test_keysign_metrics.py
 test/test_keysign_response.py
 test/test_last_block.py
 test/test_last_block_response.py
 test/test_liquidity_provider.py
 test/test_liquidity_provider_response.py
@@ -57,20 +64,27 @@
 test/test_node_keygen_metric.py
 test/test_node_preflight_status.py
 test/test_node_pub_key_set.py
 test/test_node_response.py
 test/test_nodes_api.py
 test/test_nodes_response.py
 test/test_observed_tx.py
+test/test_outbound_delay_stage.py
+test/test_outbound_fee.py
+test/test_outbound_fees_response.py
 test/test_outbound_response.py
+test/test_outbound_signed_stage.py
 test/test_ping.py
+test/test_planned_out_tx.py
 test/test_pol_api.py
 test/test_pol_response.py
 test/test_pool.py
 test/test_pool_response.py
+test/test_pool_slip_api.py
+test/test_pool_slip_response.py
 test/test_pools_api.py
 test/test_pools_response.py
 test/test_queue_api.py
 test/test_queue_response.py
 test/test_quote_api.py
 test/test_quote_fees.py
 test/test_quote_loan_close_response.py
@@ -79,19 +93,22 @@
 test/test_quote_saver_withdraw_response.py
 test/test_quote_swap_response.py
 test/test_saver.py
 test/test_saver_response.py
 test/test_savers_api.py
 test/test_savers_response.py
 test/test_scheduled_response.py
+test/test_streaming_status.py
 test/test_streaming_swap.py
 test/test_streaming_swap_api.py
 test/test_streaming_swap_response.py
 test/test_streaming_swaps_response.py
+test/test_swap_finalised_stage.py
 test/test_swap_queue_response.py
+test/test_swap_status.py
 test/test_swapper_clout_response.py
 test/test_thorname.py
 test/test_thorname_alias.py
 test/test_thorname_response.py
 test/test_thornames_api.py
 test/test_trade_account_api.py
 test/test_trade_account_response.py
@@ -107,33 +124,26 @@
 test/test_tss_metric.py
 test/test_tx.py
 test/test_tx_details_response.py
 test/test_tx_out_item.py
 test/test_tx_response.py
 test/test_tx_signers_response.py
 test/test_tx_stages_response.py
-test/test_tx_stages_response_inbound_confirmation_counted.py
-test/test_tx_stages_response_inbound_finalised.py
-test/test_tx_stages_response_inbound_observed.py
-test/test_tx_stages_response_outbound_delay.py
-test/test_tx_stages_response_outbound_signed.py
-test/test_tx_stages_response_swap_finalised.py
-test/test_tx_stages_response_swap_status.py
-test/test_tx_stages_response_swap_status_streaming.py
 test/test_tx_status_response.py
-test/test_tx_status_response_planned_out_txs.py
 test/test_vault.py
 test/test_vault_address.py
 test/test_vault_info.py
 test/test_vault_pubkeys_response.py
 test/test_vault_response.py
 test/test_vault_router.py
 test/test_vaults_api.py
 test/test_vaults_response.py
 test/test_version_response.py
+test/test_yggdrasil_vault.py
+test/test_yggdrasil_vaults_response.py
 xchainpy2_thornode/__init__.py
 xchainpy2_thornode/api_client.py
 xchainpy2_thornode/configuration.py
 xchainpy2_thornode/rest.py
 xchainpy2_thornode.egg-info/PKG-INFO
 xchainpy2_thornode.egg-info/SOURCES.txt
 xchainpy2_thornode.egg-info/dependency_links.txt
@@ -146,14 +156,15 @@
 xchainpy2_thornode/api/health_api.py
 xchainpy2_thornode/api/invariants_api.py
 xchainpy2_thornode/api/liquidity_providers_api.py
 xchainpy2_thornode/api/mimir_api.py
 xchainpy2_thornode/api/network_api.py
 xchainpy2_thornode/api/nodes_api.py
 xchainpy2_thornode/api/pol_api.py
+xchainpy2_thornode/api/pool_slip_api.py
 xchainpy2_thornode/api/pools_api.py
 xchainpy2_thornode/api/queue_api.py
 xchainpy2_thornode/api/quote_api.py
 xchainpy2_thornode/api/savers_api.py
 xchainpy2_thornode/api/streaming_swap_api.py
 xchainpy2_thornode/api/thornames_api.py
 xchainpy2_thornode/api/trade_account_api.py
@@ -180,18 +191,25 @@
 xchainpy2_thornode/models/coin.py
 xchainpy2_thornode/models/constants_response.py
 xchainpy2_thornode/models/derived_pool.py
 xchainpy2_thornode/models/derived_pool_response.py
 xchainpy2_thornode/models/derived_pools_response.py
 xchainpy2_thornode/models/inbound_address.py
 xchainpy2_thornode/models/inbound_addresses_response.py
+xchainpy2_thornode/models/inbound_confirmation_counted_stage.py
+xchainpy2_thornode/models/inbound_finalised_stage.py
+xchainpy2_thornode/models/inbound_observed_stage.py
+xchainpy2_thornode/models/inline_response200.py
 xchainpy2_thornode/models/invariant_response.py
 xchainpy2_thornode/models/invariants_response.py
+xchainpy2_thornode/models/keygen.py
+xchainpy2_thornode/models/keygen_block.py
 xchainpy2_thornode/models/keygen_metric.py
 xchainpy2_thornode/models/keygen_metrics_response.py
+xchainpy2_thornode/models/keygen_response.py
 xchainpy2_thornode/models/keysign_info.py
 xchainpy2_thornode/models/keysign_metrics.py
 xchainpy2_thornode/models/keysign_response.py
 xchainpy2_thornode/models/last_block.py
 xchainpy2_thornode/models/last_block_response.py
 xchainpy2_thornode/models/liquidity_provider.py
 xchainpy2_thornode/models/liquidity_provider_response.py
@@ -210,35 +228,44 @@
 xchainpy2_thornode/models/node_jail.py
 xchainpy2_thornode/models/node_keygen_metric.py
 xchainpy2_thornode/models/node_preflight_status.py
 xchainpy2_thornode/models/node_pub_key_set.py
 xchainpy2_thornode/models/node_response.py
 xchainpy2_thornode/models/nodes_response.py
 xchainpy2_thornode/models/observed_tx.py
+xchainpy2_thornode/models/outbound_delay_stage.py
+xchainpy2_thornode/models/outbound_fee.py
+xchainpy2_thornode/models/outbound_fees_response.py
 xchainpy2_thornode/models/outbound_response.py
+xchainpy2_thornode/models/outbound_signed_stage.py
 xchainpy2_thornode/models/ping.py
+xchainpy2_thornode/models/planned_out_tx.py
 xchainpy2_thornode/models/pol_response.py
 xchainpy2_thornode/models/pool.py
 xchainpy2_thornode/models/pool_response.py
+xchainpy2_thornode/models/pool_slip_response.py
 xchainpy2_thornode/models/pools_response.py
 xchainpy2_thornode/models/queue_response.py
 xchainpy2_thornode/models/quote_fees.py
 xchainpy2_thornode/models/quote_loan_close_response.py
 xchainpy2_thornode/models/quote_loan_open_response.py
 xchainpy2_thornode/models/quote_saver_deposit_response.py
 xchainpy2_thornode/models/quote_saver_withdraw_response.py
 xchainpy2_thornode/models/quote_swap_response.py
 xchainpy2_thornode/models/saver.py
 xchainpy2_thornode/models/saver_response.py
 xchainpy2_thornode/models/savers_response.py
 xchainpy2_thornode/models/scheduled_response.py
+xchainpy2_thornode/models/streaming_status.py
 xchainpy2_thornode/models/streaming_swap.py
 xchainpy2_thornode/models/streaming_swap_response.py
 xchainpy2_thornode/models/streaming_swaps_response.py
+xchainpy2_thornode/models/swap_finalised_stage.py
 xchainpy2_thornode/models/swap_queue_response.py
+xchainpy2_thornode/models/swap_status.py
 xchainpy2_thornode/models/swapper_clout_response.py
 xchainpy2_thornode/models/thorname.py
 xchainpy2_thornode/models/thorname_alias.py
 xchainpy2_thornode/models/thorname_response.py
 xchainpy2_thornode/models/trade_account_response.py
 xchainpy2_thornode/models/trade_accounts_response.py
 xchainpy2_thornode/models/trade_unit_response.py
@@ -247,25 +274,18 @@
 xchainpy2_thornode/models/tss_metric.py
 xchainpy2_thornode/models/tx.py
 xchainpy2_thornode/models/tx_details_response.py
 xchainpy2_thornode/models/tx_out_item.py
 xchainpy2_thornode/models/tx_response.py
 xchainpy2_thornode/models/tx_signers_response.py
 xchainpy2_thornode/models/tx_stages_response.py
-xchainpy2_thornode/models/tx_stages_response_inbound_confirmation_counted.py
-xchainpy2_thornode/models/tx_stages_response_inbound_finalised.py
-xchainpy2_thornode/models/tx_stages_response_inbound_observed.py
-xchainpy2_thornode/models/tx_stages_response_outbound_delay.py
-xchainpy2_thornode/models/tx_stages_response_outbound_signed.py
-xchainpy2_thornode/models/tx_stages_response_swap_finalised.py
-xchainpy2_thornode/models/tx_stages_response_swap_status.py
-xchainpy2_thornode/models/tx_stages_response_swap_status_streaming.py
 xchainpy2_thornode/models/tx_status_response.py
-xchainpy2_thornode/models/tx_status_response_planned_out_txs.py
 xchainpy2_thornode/models/vault.py
 xchainpy2_thornode/models/vault_address.py
 xchainpy2_thornode/models/vault_info.py
 xchainpy2_thornode/models/vault_pubkeys_response.py
 xchainpy2_thornode/models/vault_response.py
 xchainpy2_thornode/models/vault_router.py
 xchainpy2_thornode/models/vaults_response.py
-xchainpy2_thornode/models/version_response.py
+xchainpy2_thornode/models/version_response.py
+xchainpy2_thornode/models/yggdrasil_vault.py
+xchainpy2_thornode/models/yggdrasil_vaults_response.py
```

