# Comparing `tmp/mns_common-1.1.3.4.tar.gz` & `tmp/mns_common-1.1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns_common-1.1.3.4.tar", last modified: Fri May 31 08:29:36 2024, max compression
+gzip compressed data, was "mns_common-1.1.3.5.tar", last modified: Fri May 31 09:02:27 2024, max compression
```

## Comparing `mns_common-1.1.3.4.tar` & `mns_common-1.1.3.5.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.946356 mns_common-1.1.3.4/
--rw-rw-rw-   0        0        0       59 2024-05-31 08:29:36.945358 mns_common-1.1.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.1.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.903470 mns_common-1.1.3.4/mns_common/
--rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.1.3.4/mns_common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.905465 mns_common-1.1.3.4/mns_common/api/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.3.4/mns_common/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.908457 mns_common-1.1.3.4/mns_common/api/akshare/
--rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.1.3.4/mns_common/api/akshare/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.1.3.4/mns_common/api/akshare/k_line_api.py
--rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.1.3.4/mns_common/api/akshare/stock_bid_ask_api.py
--rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.1.3.4/mns_common/api/akshare/stock_dt_pool.py
--rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.1.3.4/mns_common/api/akshare/stock_zb_pool.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.1.3.4/mns_common/api/akshare/stock_zt_pool_api.py
--rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.1.3.4/mns_common/api/akshare/yjyg_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.911449 mns_common-1.1.3.4/mns_common/api/em/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.3.4/mns_common/api/em/__init__.py
--rw-rw-rw-   0        0        0     8352 2024-05-10 13:01:52.000000 mns_common-1.1.3.4/mns_common/api/em/east_money_stock_api.py
--rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.1.3.4/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
--rw-rw-rw-   0        0        0     4371 2024-05-17 04:06:34.000000 mns_common-1.1.3.4/mns_common/api/em/east_money_stock_hk_api.py
--rw-rw-rw-   0        0        0    14960 2024-05-10 12:40:48.000000 mns_common-1.1.3.4/mns_common/api/em/east_money_stock_v2_api.py
--rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.1.3.4/mns_common/api/em/em_concept_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.912447 mns_common-1.1.3.4/mns_common/api/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.4/mns_common/api/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.913444 mns_common-1.1.3.4/mns_common/api/kpl/common/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.3.4/mns_common/api/kpl/common/__init__.py
--rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.1.3.4/mns_common/api/kpl/common/kpl_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.914441 mns_common-1.1.3.4/mns_common/api/kpl/concept/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.3.4/mns_common/api/kpl/concept/__init__.py
--rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.1.3.4/mns_common/api/kpl/concept/kpl_concept_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.915439 mns_common-1.1.3.4/mns_common/api/kpl/constant/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.3.4/mns_common/api/kpl/constant/__init__.py
--rw-rw-rw-   0        0        0      235 2024-05-24 10:14:14.000000 mns_common-1.1.3.4/mns_common/api/kpl/constant/kpl_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.915439 mns_common-1.1.3.4/mns_common/api/kpl/industry/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.3.4/mns_common/api/kpl/industry/__init__.py
--rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.1.3.4/mns_common/api/kpl/industry/kpl_industry_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.916436 mns_common-1.1.3.4/mns_common/api/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.3.4/mns_common/api/kpl/selection/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 13:55:26.000000 mns_common-1.1.3.4/mns_common/api/kpl/selection/kpl_selection_plate_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.918430 mns_common-1.1.3.4/mns_common/api/kpl/symbol/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.3.4/mns_common/api/kpl/symbol/__init__.py
--rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.1.3.4/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
--rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.1.3.4/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
--rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.1.3.4/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.919428 mns_common-1.1.3.4/mns_common/api/msg/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.3.4/mns_common/api/msg/__init__.py
--rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.1.3.4/mns_common/api/msg/push_msg_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.921426 mns_common-1.1.3.4/mns_common/api/ths/
--rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.1.3.4/mns_common/api/ths/__init__.py
--rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.1.3.4/mns_common/api/ths/ths_big_deal_api.py
--rw-rw-rw-   0        0        0    40309 2024-05-14 08:22:47.000000 mns_common-1.1.3.4/mns_common/api/ths/ths_stock_api.py
--rw-rw-rw-   0        0        0     6648 2024-05-20 06:35:22.000000 mns_common-1.1.3.4/mns_common/api/ths/ths_stock_zt_pool_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.922421 mns_common-1.1.3.4/mns_common/component/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.1.3.4/mns_common/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.923419 mns_common-1.1.3.4/mns_common/component/cache/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.3.4/mns_common/component/cache/__init__.py
--rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.1.3.4/mns_common/component/cache/cache_service.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.925418 mns_common-1.1.3.4/mns_common/component/classify/
--rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.1.3.4/mns_common/component/classify/__init__.py
--rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.1.3.4/mns_common/component/classify/classify_constant.py
--rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.1.3.4/mns_common/component/classify/symbol_classify_api.py
--rw-rw-rw-   0        0        0     4896 2024-05-22 14:19:44.000000 mns_common-1.1.3.4/mns_common/component/common_service_fun_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.926409 mns_common-1.1.3.4/mns_common/component/company/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.4/mns_common/component/company/__init__.py
--rw-rw-rw-   0        0        0     7992 2024-05-25 06:17:07.000000 mns_common-1.1.3.4/mns_common/component/company/company_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.927406 mns_common-1.1.3.4/mns_common/component/concept/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.4/mns_common/component/concept/__init__.py
--rw-rw-rw-   0        0        0     3235 2024-05-09 14:23:16.000000 mns_common-1.1.3.4/mns_common/component/concept/kpl_concept_common_service_api.py
--rw-rw-rw-   0        0        0     9682 2024-05-31 08:28:58.000000 mns_common-1.1.3.4/mns_common/component/concept/ths_concept_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.928404 mns_common-1.1.3.4/mns_common/component/data/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.3.4/mns_common/component/data/__init__.py
--rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.1.3.4/mns_common/component/data/data_init_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.929401 mns_common-1.1.3.4/mns_common/component/industry/
--rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.1.3.4/mns_common/component/industry/__init__.py
--rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.1.3.4/mns_common/component/industry/ths_industry_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.930399 mns_common-1.1.3.4/mns_common/component/k_line/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.4/mns_common/component/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.931396 mns_common-1.1.3.4/mns_common/component/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.1.3.4/mns_common/component/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.1.3.4/mns_common/component/k_line/clean/k_line_param.py
--rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.1.3.4/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.932393 mns_common-1.1.3.4/mns_common/component/k_line/common/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.1.3.4/mns_common/component/k_line/common/__init__.py
--rw-rw-rw-   0        0        0     4770 2024-05-20 14:28:57.000000 mns_common-1.1.3.4/mns_common/component/k_line/common/k_line_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.933390 mns_common-1.1.3.4/mns_common/component/k_line/patterns/
--rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.1.3.4/mns_common/component/k_line/patterns/__init__.py
--rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.1.3.4/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
--rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.1.3.4/mns_common/component/k_line/patterns/pattern_Enum.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.934388 mns_common-1.1.3.4/mns_common/component/qmt/
--rw-rw-rw-   0        0        0      163 2024-05-23 13:30:35.000000 mns_common-1.1.3.4/mns_common/component/qmt/__init__.py
--rw-rw-rw-   0        0        0     7540 2024-05-23 14:38:14.000000 mns_common-1.1.3.4/mns_common/component/qmt/qmt_buy_service.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.935385 mns_common-1.1.3.4/mns_common/component/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.4/mns_common/component/real_time/__init__.py
--rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.1.3.4/mns_common/component/real_time/real_time_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.937379 mns_common-1.1.3.4/mns_common/component/self_choose/
--rw-rw-rw-   0        0        0      163 2024-05-14 15:36:27.000000 mns_common-1.1.3.4/mns_common/component/self_choose/__init__.py
--rw-rw-rw-   0        0        0     2232 2024-05-16 05:56:38.000000 mns_common-1.1.3.4/mns_common/component/self_choose/black_list_service_api.py
--rw-rw-rw-   0        0        0      519 2024-05-18 07:01:06.000000 mns_common-1.1.3.4/mns_common/component/self_choose/self_choose_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.937379 mns_common-1.1.3.4/mns_common/component/trade/
--rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.1.3.4/mns_common/component/trade/__init__.py
--rw-rw-rw-   0        0        0     3120 2024-05-08 07:34:38.000000 mns_common-1.1.3.4/mns_common/component/trade/trade_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.938377 mns_common-1.1.3.4/mns_common/component/trade_date/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.4/mns_common/component/trade_date/__init__.py
--rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.1.3.4/mns_common/component/trade_date/trade_date_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.939375 mns_common-1.1.3.4/mns_common/component/zt/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.4/mns_common/component/zt/__init__.py
--rw-rw-rw-   0        0        0     9927 2024-05-22 08:23:47.000000 mns_common-1.1.3.4/mns_common/component/zt/zt_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.941369 mns_common-1.1.3.4/mns_common/constant/
--rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.1.3.4/mns_common/constant/__init__.py
--rw-rw-rw-   0        0        0     2283 2024-05-24 22:26:12.000000 mns_common-1.1.3.4/mns_common/constant/db_name_constant.py
--rw-rw-rw-   0        0        0      492 2024-05-24 09:42:58.000000 mns_common-1.1.3.4/mns_common/constant/self_choose_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.942367 mns_common-1.1.3.4/mns_common/db/
--rw-rw-rw-   0        0        0    11520 2024-05-27 11:15:24.000000 mns_common-1.1.3.4/mns_common/db/MongodbUtil.py
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.3.4/mns_common/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.944361 mns_common-1.1.3.4/mns_common/utils/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.3.4/mns_common/utils/__init__.py
--rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.1.3.4/mns_common/utils/async_fun.py
--rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.1.3.4/mns_common/utils/data_frame_util.py
--rw-rw-rw-   0        0        0     7379 2024-05-29 15:15:49.000000 mns_common-1.1.3.4/mns_common/utils/date_handle_util.py
--rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.1.3.4/mns_common/utils/ip_util.py
-drwxrwxrwx   0        0        0        0 2024-05-31 08:29:36.945358 mns_common-1.1.3.4/mns_common.egg-info/
--rw-rw-rw-   0        0        0       59 2024-05-31 08:29:36.000000 mns_common-1.1.3.4/mns_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3843 2024-05-31 08:29:36.000000 mns_common-1.1.3.4/mns_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 08:29:36.000000 mns_common-1.1.3.4/mns_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-31 08:29:36.000000 mns_common-1.1.3.4/mns_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 08:29:36.946356 mns_common-1.1.3.4/setup.cfg
--rw-rw-rw-   0        0        0      466 2024-05-31 08:29:13.000000 mns_common-1.1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.537982 mns_common-1.1.3.5/
+-rw-rw-rw-   0        0        0       59 2024-05-31 09:02:27.536985 mns_common-1.1.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.1.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.500083 mns_common-1.1.3.5/mns_common/
+-rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.1.3.5/mns_common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.502078 mns_common-1.1.3.5/mns_common/api/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.3.5/mns_common/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.505070 mns_common-1.1.3.5/mns_common/api/akshare/
+-rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.1.3.5/mns_common/api/akshare/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.1.3.5/mns_common/api/akshare/k_line_api.py
+-rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.1.3.5/mns_common/api/akshare/stock_bid_ask_api.py
+-rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.1.3.5/mns_common/api/akshare/stock_dt_pool.py
+-rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.1.3.5/mns_common/api/akshare/stock_zb_pool.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.1.3.5/mns_common/api/akshare/stock_zt_pool_api.py
+-rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.1.3.5/mns_common/api/akshare/yjyg_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.507064 mns_common-1.1.3.5/mns_common/api/em/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.3.5/mns_common/api/em/__init__.py
+-rw-rw-rw-   0        0        0     8352 2024-05-10 13:01:52.000000 mns_common-1.1.3.5/mns_common/api/em/east_money_stock_api.py
+-rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.1.3.5/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
+-rw-rw-rw-   0        0        0     4371 2024-05-17 04:06:34.000000 mns_common-1.1.3.5/mns_common/api/em/east_money_stock_hk_api.py
+-rw-rw-rw-   0        0        0    14960 2024-05-10 12:40:48.000000 mns_common-1.1.3.5/mns_common/api/em/east_money_stock_v2_api.py
+-rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.1.3.5/mns_common/api/em/em_concept_index_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.508062 mns_common-1.1.3.5/mns_common/api/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.5/mns_common/api/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.509059 mns_common-1.1.3.5/mns_common/api/kpl/common/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.3.5/mns_common/api/kpl/common/__init__.py
+-rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.1.3.5/mns_common/api/kpl/common/kpl_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.509059 mns_common-1.1.3.5/mns_common/api/kpl/concept/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.3.5/mns_common/api/kpl/concept/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.1.3.5/mns_common/api/kpl/concept/kpl_concept_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.510056 mns_common-1.1.3.5/mns_common/api/kpl/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.3.5/mns_common/api/kpl/constant/__init__.py
+-rw-rw-rw-   0        0        0      235 2024-05-24 10:14:14.000000 mns_common-1.1.3.5/mns_common/api/kpl/constant/kpl_constant.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.511053 mns_common-1.1.3.5/mns_common/api/kpl/industry/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.3.5/mns_common/api/kpl/industry/__init__.py
+-rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.1.3.5/mns_common/api/kpl/industry/kpl_industry_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.512051 mns_common-1.1.3.5/mns_common/api/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.3.5/mns_common/api/kpl/selection/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 13:55:26.000000 mns_common-1.1.3.5/mns_common/api/kpl/selection/kpl_selection_plate_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.514045 mns_common-1.1.3.5/mns_common/api/kpl/symbol/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.3.5/mns_common/api/kpl/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.1.3.5/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
+-rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.1.3.5/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
+-rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.1.3.5/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.514045 mns_common-1.1.3.5/mns_common/api/msg/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.3.5/mns_common/api/msg/__init__.py
+-rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.1.3.5/mns_common/api/msg/push_msg_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.516040 mns_common-1.1.3.5/mns_common/api/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.1.3.5/mns_common/api/ths/__init__.py
+-rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.1.3.5/mns_common/api/ths/ths_big_deal_api.py
+-rw-rw-rw-   0        0        0    40309 2024-05-14 08:22:47.000000 mns_common-1.1.3.5/mns_common/api/ths/ths_stock_api.py
+-rw-rw-rw-   0        0        0     6648 2024-05-20 06:35:22.000000 mns_common-1.1.3.5/mns_common/api/ths/ths_stock_zt_pool_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.517038 mns_common-1.1.3.5/mns_common/component/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.1.3.5/mns_common/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.518035 mns_common-1.1.3.5/mns_common/component/cache/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.3.5/mns_common/component/cache/__init__.py
+-rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.1.3.5/mns_common/component/cache/cache_service.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.519032 mns_common-1.1.3.5/mns_common/component/classify/
+-rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.1.3.5/mns_common/component/classify/__init__.py
+-rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.1.3.5/mns_common/component/classify/classify_constant.py
+-rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.1.3.5/mns_common/component/classify/symbol_classify_api.py
+-rw-rw-rw-   0        0        0     4896 2024-05-22 14:19:44.000000 mns_common-1.1.3.5/mns_common/component/common_service_fun_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.520030 mns_common-1.1.3.5/mns_common/component/company/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.5/mns_common/component/company/__init__.py
+-rw-rw-rw-   0        0        0     7992 2024-05-25 06:17:07.000000 mns_common-1.1.3.5/mns_common/component/company/company_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.521027 mns_common-1.1.3.5/mns_common/component/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.5/mns_common/component/concept/__init__.py
+-rw-rw-rw-   0        0        0     3235 2024-05-09 14:23:16.000000 mns_common-1.1.3.5/mns_common/component/concept/kpl_concept_common_service_api.py
+-rw-rw-rw-   0        0        0     9682 2024-05-31 08:28:58.000000 mns_common-1.1.3.5/mns_common/component/concept/ths_concept_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.522024 mns_common-1.1.3.5/mns_common/component/data/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.3.5/mns_common/component/data/__init__.py
+-rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.1.3.5/mns_common/component/data/data_init_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.523022 mns_common-1.1.3.5/mns_common/component/industry/
+-rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.1.3.5/mns_common/component/industry/__init__.py
+-rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.1.3.5/mns_common/component/industry/ths_industry_index_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.523022 mns_common-1.1.3.5/mns_common/component/k_line/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.5/mns_common/component/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.524019 mns_common-1.1.3.5/mns_common/component/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.1.3.5/mns_common/component/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.1.3.5/mns_common/component/k_line/clean/k_line_param.py
+-rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.1.3.5/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.525016 mns_common-1.1.3.5/mns_common/component/k_line/common/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.1.3.5/mns_common/component/k_line/common/__init__.py
+-rw-rw-rw-   0        0        0     4770 2024-05-20 14:28:57.000000 mns_common-1.1.3.5/mns_common/component/k_line/common/k_line_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.527010 mns_common-1.1.3.5/mns_common/component/k_line/patterns/
+-rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.1.3.5/mns_common/component/k_line/patterns/__init__.py
+-rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.1.3.5/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
+-rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.1.3.5/mns_common/component/k_line/patterns/pattern_Enum.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.527010 mns_common-1.1.3.5/mns_common/component/qmt/
+-rw-rw-rw-   0        0        0      163 2024-05-23 13:30:35.000000 mns_common-1.1.3.5/mns_common/component/qmt/__init__.py
+-rw-rw-rw-   0        0        0     7540 2024-05-23 14:38:14.000000 mns_common-1.1.3.5/mns_common/component/qmt/qmt_buy_service.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.528008 mns_common-1.1.3.5/mns_common/component/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.5/mns_common/component/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.1.3.5/mns_common/component/real_time/real_time_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.530003 mns_common-1.1.3.5/mns_common/component/self_choose/
+-rw-rw-rw-   0        0        0      163 2024-05-14 15:36:27.000000 mns_common-1.1.3.5/mns_common/component/self_choose/__init__.py
+-rw-rw-rw-   0        0        0     2232 2024-05-16 05:56:38.000000 mns_common-1.1.3.5/mns_common/component/self_choose/black_list_service_api.py
+-rw-rw-rw-   0        0        0      519 2024-05-18 07:01:06.000000 mns_common-1.1.3.5/mns_common/component/self_choose/self_choose_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.530003 mns_common-1.1.3.5/mns_common/component/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.1.3.5/mns_common/component/trade/__init__.py
+-rw-rw-rw-   0        0        0     3120 2024-05-08 07:34:38.000000 mns_common-1.1.3.5/mns_common/component/trade/trade_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.531000 mns_common-1.1.3.5/mns_common/component/trade_date/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.5/mns_common/component/trade_date/__init__.py
+-rw-rw-rw-   0        0        0     3032 2024-05-31 09:01:38.000000 mns_common-1.1.3.5/mns_common/component/trade_date/trade_date_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.531997 mns_common-1.1.3.5/mns_common/component/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.3.5/mns_common/component/zt/__init__.py
+-rw-rw-rw-   0        0        0     9927 2024-05-22 08:23:47.000000 mns_common-1.1.3.5/mns_common/component/zt/zt_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.532995 mns_common-1.1.3.5/mns_common/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.1.3.5/mns_common/constant/__init__.py
+-rw-rw-rw-   0        0        0     2283 2024-05-24 22:26:12.000000 mns_common-1.1.3.5/mns_common/constant/db_name_constant.py
+-rw-rw-rw-   0        0        0      492 2024-05-24 09:42:58.000000 mns_common-1.1.3.5/mns_common/constant/self_choose_constant.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.533993 mns_common-1.1.3.5/mns_common/db/
+-rw-rw-rw-   0        0        0    11520 2024-05-27 11:15:24.000000 mns_common-1.1.3.5/mns_common/db/MongodbUtil.py
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.3.5/mns_common/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.535987 mns_common-1.1.3.5/mns_common/utils/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.3.5/mns_common/utils/__init__.py
+-rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.1.3.5/mns_common/utils/async_fun.py
+-rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.1.3.5/mns_common/utils/data_frame_util.py
+-rw-rw-rw-   0        0        0     7379 2024-05-29 15:15:49.000000 mns_common-1.1.3.5/mns_common/utils/date_handle_util.py
+-rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.1.3.5/mns_common/utils/ip_util.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:02:27.536985 mns_common-1.1.3.5/mns_common.egg-info/
+-rw-rw-rw-   0        0        0       59 2024-05-31 09:02:27.000000 mns_common-1.1.3.5/mns_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3843 2024-05-31 09:02:27.000000 mns_common-1.1.3.5/mns_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 09:02:27.000000 mns_common-1.1.3.5/mns_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-31 09:02:27.000000 mns_common-1.1.3.5/mns_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 09:02:27.537982 mns_common-1.1.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      466 2024-05-31 09:01:44.000000 mns_common-1.1.3.5/setup.py
```

### Comparing `mns_common-1.1.3.4/README.md` & `mns_common-1.1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/akshare/k_line_api.py` & `mns_common-1.1.3.5/mns_common/api/akshare/k_line_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/akshare/stock_bid_ask_api.py` & `mns_common-1.1.3.5/mns_common/api/akshare/stock_bid_ask_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/akshare/stock_dt_pool.py` & `mns_common-1.1.3.5/mns_common/api/akshare/stock_dt_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/akshare/stock_zb_pool.py` & `mns_common-1.1.3.5/mns_common/api/akshare/stock_zb_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/akshare/stock_zt_pool_api.py` & `mns_common-1.1.3.5/mns_common/api/akshare/stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/akshare/yjyg_sync_api.py` & `mns_common-1.1.3.5/mns_common/api/akshare/yjyg_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/em/east_money_stock_api.py` & `mns_common-1.1.3.5/mns_common/api/em/east_money_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py` & `mns_common-1.1.3.5/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/em/east_money_stock_hk_api.py` & `mns_common-1.1.3.5/mns_common/api/em/east_money_stock_hk_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/em/east_money_stock_v2_api.py` & `mns_common-1.1.3.5/mns_common/api/em/east_money_stock_v2_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/em/em_concept_index_api.py` & `mns_common-1.1.3.5/mns_common/api/em/em_concept_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/kpl/common/kpl_common_api.py` & `mns_common-1.1.3.5/mns_common/api/kpl/common/kpl_common_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/kpl/concept/kpl_concept_api.py` & `mns_common-1.1.3.5/mns_common/api/kpl/concept/kpl_concept_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/kpl/industry/kpl_industry_api.py` & `mns_common-1.1.3.5/mns_common/api/kpl/industry/kpl_industry_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/kpl/selection/kpl_selection_plate_api.py` & `mns_common-1.1.3.5/mns_common/api/kpl/selection/kpl_selection_plate_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py` & `mns_common-1.1.3.5/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py` & `mns_common-1.1.3.5/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/kpl/symbol/symbol_his_quotes_api.py` & `mns_common-1.1.3.5/mns_common/api/kpl/symbol/symbol_his_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/msg/push_msg_api.py` & `mns_common-1.1.3.5/mns_common/api/msg/push_msg_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/ths/ths_big_deal_api.py` & `mns_common-1.1.3.5/mns_common/api/ths/ths_big_deal_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/ths/ths_stock_api.py` & `mns_common-1.1.3.5/mns_common/api/ths/ths_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/api/ths/ths_stock_zt_pool_api.py` & `mns_common-1.1.3.5/mns_common/api/ths/ths_stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/cache/cache_service.py` & `mns_common-1.1.3.5/mns_common/component/cache/cache_service.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/classify/classify_constant.py` & `mns_common-1.1.3.5/mns_common/component/classify/classify_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/classify/symbol_classify_api.py` & `mns_common-1.1.3.5/mns_common/component/classify/symbol_classify_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/common_service_fun_api.py` & `mns_common-1.1.3.5/mns_common/component/common_service_fun_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/company/company_common_service_api.py` & `mns_common-1.1.3.5/mns_common/component/company/company_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/concept/kpl_concept_common_service_api.py` & `mns_common-1.1.3.5/mns_common/component/concept/kpl_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/concept/ths_concept_common_service_api.py` & `mns_common-1.1.3.5/mns_common/component/concept/ths_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/data/data_init_api.py` & `mns_common-1.1.3.5/mns_common/component/data/data_init_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/industry/ths_industry_index_api.py` & `mns_common-1.1.3.5/mns_common/component/industry/ths_industry_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py` & `mns_common-1.1.3.5/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/k_line/common/k_line_common_service_api.py` & `mns_common-1.1.3.5/mns_common/component/k_line/common/k_line_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/k_line/patterns/k_line_patterns_service_api.py` & `mns_common-1.1.3.5/mns_common/component/k_line/patterns/k_line_patterns_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/qmt/qmt_buy_service.py` & `mns_common-1.1.3.5/mns_common/component/qmt/qmt_buy_service.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/real_time/real_time_common_service_api.py` & `mns_common-1.1.3.5/mns_common/component/real_time/real_time_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/self_choose/black_list_service_api.py` & `mns_common-1.1.3.5/mns_common/component/self_choose/black_list_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/self_choose/self_choose_service_api.py` & `mns_common-1.1.3.5/mns_common/component/self_choose/self_choose_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/trade/trade_service_api.py` & `mns_common-1.1.3.5/mns_common/component/trade/trade_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/component/trade_date/trade_date_common_service_api.py` & `mns_common-1.1.3.5/mns_common/component/trade_date/trade_date_common_service_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,10 +62,16 @@
 
 
 def is_trade_day(str_day):
     query = {"trade_date": str_day}
     return mongodb_util.exist_data_query("trade_date_list", query)
 
 
-if __name__ == '__main__':
+# 计算两个交易日直接的天数
+@lru_cache(maxsize=None)
+def calculate_two_date_days(begin_day, end_day):
+    query = {"$and": [{"_id": {'$gte': begin_day}}, {"_id": {'$lt': end_day}}]}
+    return mongodb_util.count(query, "trade_date_list")
+
 
+if __name__ == '__main__':
     get_further_trade_date('2023-12-15', 5)
```

### Comparing `mns_common-1.1.3.4/mns_common/component/zt/zt_common_service_api.py` & `mns_common-1.1.3.5/mns_common/component/zt/zt_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/constant/db_name_constant.py` & `mns_common-1.1.3.5/mns_common/constant/db_name_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/db/MongodbUtil.py` & `mns_common-1.1.3.5/mns_common/db/MongodbUtil.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/utils/data_frame_util.py` & `mns_common-1.1.3.5/mns_common/utils/data_frame_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common/utils/date_handle_util.py` & `mns_common-1.1.3.5/mns_common/utils/date_handle_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.3.4/mns_common.egg-info/SOURCES.txt` & `mns_common-1.1.3.5/mns_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

