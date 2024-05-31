# Comparing `tmp/baostock-0.8.8.tar.gz` & `tmp/baostock-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\baostock-0.8.8.tar", last modified: Fri Jan 25 10:00:32 2019, max compression
+gzip compressed data, was "dist\baostock-0.8.9.tar", last modified: Fri May 31 02:50:15 2024, max compression
```

## Comparing `baostock-0.8.8.tar` & `baostock-0.8.9.tar`

### file list

```diff
@@ -1,82 +1,72 @@
-drwxrwxrwx   0        0        0        0 2019-01-25 10:00:32.000000 baostock-0.8.8/
-drwxrwxrwx   0        0        0        0 2019-01-25 10:00:31.000000 baostock-0.8.8/baostock/
-drwxrwxrwx   0        0        0        0 2019-01-25 10:00:31.000000 baostock-0.8.8/baostock/common/
--rw-rw-rw-   0        0        0    11538 2019-01-24 15:33:05.000000 baostock-0.8.8/baostock/common/contants.py
--rw-rw-rw-   0        0        0       43 2019-01-22 02:25:13.000000 baostock-0.8.8/baostock/common/context.py
--rw-rw-rw-   0        0        0        0 2019-01-22 02:25:13.000000 baostock-0.8.8/baostock/common/__init__.py
-drwxrwxrwx   0        0        0        0 2019-01-25 10:00:31.000000 baostock-0.8.8/baostock/corpreport/
--rw-rw-rw-   0        0        0     8289 2019-01-22 02:25:13.000000 baostock-0.8.8/baostock/corpreport/corp_performance.py
--rw-rw-rw-   0        0        0        0 2019-01-22 02:25:13.000000 baostock-0.8.8/baostock/corpreport/__init__.py
-drwxrwxrwx   0        0        0        0 2019-01-25 10:00:31.000000 baostock-0.8.8/baostock/data/
--rw-rw-rw-   0        0        0      489 2019-01-22 02:25:14.000000 baostock-0.8.8/baostock/data/messageheader.py
--rw-rw-rw-   0        0        0      567 2019-01-22 02:25:14.000000 baostock-0.8.8/baostock/data/msg.py
--rw-rw-rw-   0        0        0     6986 2019-01-22 02:25:14.000000 baostock-0.8.8/baostock/data/resultset.py
--rw-rw-rw-   0        0        0        0 2019-01-22 02:25:14.000000 baostock-0.8.8/baostock/data/__init__.py
-drwxrwxrwx   0        0        0        0 2019-01-25 10:00:31.000000 baostock-0.8.8/baostock/evaluation/
--rw-rw-rw-   0        0        0    28149 2019-01-22 02:25:13.000000 baostock-0.8.8/baostock/evaluation/season_index.py
--rw-rw-rw-   0        0        0        0 2019-01-22 02:25:13.000000 baostock-0.8.8/baostock/evaluation/__init__.py
-drwxrwxrwx   0        0        0        0 2019-01-25 10:00:31.000000 baostock-0.8.8/baostock/login/
--rw-rw-rw-   0        0        0     8595 2019-01-22 02:25:14.000000 baostock-0.8.8/baostock/login/loginout.py
--rw-rw-rw-   0        0        0        0 2019-01-22 02:25:14.000000 baostock-0.8.8/baostock/login/__init__.py
-drwxrwxrwx   0        0        0        0 2019-01-25 10:00:31.000000 baostock-0.8.8/baostock/macroscopic/
--rw-rw-rw-   0        0        0    30440 2019-01-22 02:25:13.000000 baostock-0.8.8/baostock/macroscopic/economic_data.py
--rw-rw-rw-   0        0        0        0 2019-01-22 02:25:13.000000 baostock-0.8.8/baostock/macroscopic/__init__.py
-drwxrwxrwx   0        0        0        0 2019-01-25 10:00:31.000000 baostock-0.8.8/baostock/metadata/
--rw-rw-rw-   0        0        0     7237 2019-01-22 02:25:13.000000 baostock-0.8.8/baostock/metadata/stock_metadata.py
--rw-rw-rw-   0        0        0        0 2019-01-22 02:25:13.000000 baostock-0.8.8/baostock/metadata/__init__.py
-drwxrwxrwx   0        0        0        0 2019-01-25 10:00:31.000000 baostock-0.8.8/baostock/realtime/
--rw-rw-rw-   0        0        0     5436 2019-01-22 02:25:13.000000 baostock-0.8.8/baostock/realtime/subscibe.py
--rw-rw-rw-   0        0        0        0 2019-01-22 02:25:13.000000 baostock-0.8.8/baostock/realtime/__init__.py
-drwxrwxrwx   0        0        0        0 2019-01-25 10:00:31.000000 baostock-0.8.8/baostock/security/
--rw-rw-rw-   0        0        0    10681 2019-01-22 03:33:25.000000 baostock-0.8.8/baostock/security/history.py
--rw-rw-rw-   0        0        0    36261 2019-01-22 02:25:13.000000 baostock-0.8.8/baostock/security/sectorinfo.py
--rw-rw-rw-   0        0        0        0 2019-01-22 02:25:13.000000 baostock-0.8.8/baostock/security/__init__.py
-drwxrwxrwx   0        0        0        0 2019-01-25 10:00:31.000000 baostock-0.8.8/baostock/util/
--rw-rw-rw-   0        0        0    15426 2019-01-22 02:25:14.000000 baostock-0.8.8/baostock/util/socketutil.py
--rw-rw-rw-   0        0        0     2207 2019-01-22 02:25:14.000000 baostock-0.8.8/baostock/util/stringutil.py
--rw-rw-rw-   0        0        0        0 2019-01-22 02:25:14.000000 baostock-0.8.8/baostock/util/__init__.py
--rw-rw-rw-   0        0        0     1692 2019-01-24 15:34:53.000000 baostock-0.8.8/baostock/__init__.py
-drwxrwxrwx   0        0        0        0 2019-01-25 10:00:31.000000 baostock-0.8.8/baostock.egg-info/
--rw-rw-rw-   0        0        0        1 2019-01-25 10:00:30.000000 baostock-0.8.8/baostock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     4050 2019-01-25 10:00:30.000000 baostock-0.8.8/baostock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       15 2019-01-25 10:00:30.000000 baostock-0.8.8/baostock.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1898 2019-01-25 10:00:31.000000 baostock-0.8.8/baostock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       14 2019-01-25 10:00:30.000000 baostock-0.8.8/baostock.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2019-01-25 10:00:32.000000 baostock-0.8.8/demo/
--rw-rw-rw-   0        0        0      711 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_Adjust_factor_data.py
--rw-rw-rw-   0        0        0      806 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_AllStock.py
--rw-rw-rw-   0        0        0     1162 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_A_stock_k_data.py
--rw-rw-rw-   0        0        0      679 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_Balance_data.py
--rw-rw-rw-   0        0        0      711 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_CashFlow_data.py
--rw-rw-rw-   0        0        0      817 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_depositRate_data.py
--rw-rw-rw-   0        0        0     1309 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_Dividend_data.py
--rw-rw-rw-   0        0        0      710 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_Dupont_data.py
--rw-rw-rw-   0        0        0      956 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_Forecast_report.py
--rw-rw-rw-   0        0        0      666 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_Growth_data.py
--rw-rw-rw-   0        0        0      741 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_hs300_stocks.py
--rw-rw-rw-   0        0        0     1810 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_Index_k_data.py
--rw-rw-rw-   0        0        0      805 2019-01-22 02:25:12.000000 baostock-0.8.8/demo/demo_loanRate_data.py
--rw-rw-rw-   0        0        0      843 2019-01-22 02:25:12.000000 baostock-0.8.8/demo/demo_moneySupplyDataMonth_data.py
--rw-rw-rw-   0        0        0      847 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_moneySupplyDataYear_data.py
--rw-rw-rw-   0        0        0      705 2019-01-22 02:25:12.000000 baostock-0.8.8/demo/demo_Operation_data.py
--rw-rw-rw-   0        0        0      897 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_PerformanceExpress_report.py
--rw-rw-rw-   0        0        0      690 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_Profit_data.py
--rw-rw-rw-   0        0        0      834 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_RealTime.py
--rw-rw-rw-   0        0        0      863 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_requiredReserveRatio_data.py
--rw-rw-rw-   0        0        0      813 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_shibor_data.py
--rw-rw-rw-   0        0        0      748 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_startst_stocks.py
--rw-rw-rw-   0        0        0      829 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_stockBasic_data.py
--rw-rw-rw-   0        0        0      799 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_stock_industry.py
--rw-rw-rw-   0        0        0     9645 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_stock_k_data_test.py
--rw-rw-rw-   0        0        0     1114 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_stock_Valuation_indicator_data.py
--rw-rw-rw-   0        0        0      720 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_st_stocks.py
--rw-rw-rw-   0        0        0      769 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_suspended_stocks.py
--rw-rw-rw-   0        0        0      750 2019-01-22 02:25:12.000000 baostock-0.8.8/demo/demo_sz50stocks.py
--rw-rw-rw-   0        0        0      794 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_terminated_stocks.py
--rw-rw-rw-   0        0        0      847 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_TradeDates.py
--rw-rw-rw-   0        0        0      741 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/demo_zz500_stock.py
--rw-rw-rw-   0        0        0     1100 2019-01-22 02:25:13.000000 baostock-0.8.8/demo/helloWorld.py
--rw-rw-rw-   0        0        0        0 2019-01-22 02:25:12.000000 baostock-0.8.8/demo/__init__.py
--rw-rw-rw-   0        0        0     4050 2019-01-25 10:00:32.000000 baostock-0.8.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2019-01-25 10:00:32.000000 baostock-0.8.8/setup.cfg
--rw-rw-rw-   0        0        0     3759 2019-01-22 02:25:14.000000 baostock-0.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:50:15.000000 baostock-0.8.9/
+drwxrwxrwx   0        0        0        0 2024-05-31 02:50:15.000000 baostock-0.8.9/baostock/
+drwxrwxrwx   0        0        0        0 2024-05-31 02:50:15.000000 baostock-0.8.9/baostock/common/
+-rw-rw-rw-   0        0        0    11369 2024-05-30 08:33:08.000000 baostock-0.8.9/baostock/common/contants.py
+-rw-rw-rw-   0        0        0       43 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/common/context.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:50:15.000000 baostock-0.8.9/baostock/corpreport/
+-rw-rw-rw-   0        0        0     8289 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/corpreport/corp_performance.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/corpreport/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:50:15.000000 baostock-0.8.9/baostock/data/
+-rw-rw-rw-   0        0        0      489 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/data/messageheader.py
+-rw-rw-rw-   0        0        0      567 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/data/msg.py
+-rw-rw-rw-   0        0        0     6986 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/data/resultset.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:50:15.000000 baostock-0.8.9/baostock/demo/
+-rw-rw-rw-   0        0        0      711 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_Adjust_factor_data.py
+-rw-rw-rw-   0        0        0      806 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_AllStock.py
+-rw-rw-rw-   0        0        0      705 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_assignDayData.py
+-rw-rw-rw-   0        0        0     1177 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_A_stock_k_data.py
+-rw-rw-rw-   0        0        0      679 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_Balance_data.py
+-rw-rw-rw-   0        0        0      711 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_CashFlow_data.py
+-rw-rw-rw-   0        0        0      817 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_depositRate_data.py
+-rw-rw-rw-   0        0        0     1309 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_Dividend_data.py
+-rw-rw-rw-   0        0        0      710 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_Dupont_data.py
+-rw-rw-rw-   0        0        0      956 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_Forecast_report.py
+-rw-rw-rw-   0        0        0      666 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_Growth_data.py
+-rw-rw-rw-   0        0        0      741 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_hs300_stocks.py
+-rw-rw-rw-   0        0        0     1825 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_Index_k_data.py
+-rw-rw-rw-   0        0        0      805 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_loanRate_data.py
+-rw-rw-rw-   0        0        0      843 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_moneySupplyDataMonth_data.py
+-rw-rw-rw-   0        0        0      847 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_moneySupplyDataYear_data.py
+-rw-rw-rw-   0        0        0      705 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_Operation_data.py
+-rw-rw-rw-   0        0        0      897 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_PerformanceExpress_report.py
+-rw-rw-rw-   0        0        0      690 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_Profit_data.py
+-rw-rw-rw-   0        0        0      863 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_requiredReserveRatio_data.py
+-rw-rw-rw-   0        0        0      829 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_stockBasic_data.py
+-rw-rw-rw-   0        0        0      799 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_stock_industry.py
+-rw-rw-rw-   0        0        0     1129 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_stock_Valuation_indicator_data.py
+-rw-rw-rw-   0        0        0      750 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_sz50stocks.py
+-rw-rw-rw-   0        0        0      847 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_TradeDates.py
+-rw-rw-rw-   0        0        0      741 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/demo_zz500_stock.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 03:19:50.000000 baostock-0.8.9/baostock/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:50:15.000000 baostock-0.8.9/baostock/evaluation/
+-rw-rw-rw-   0        0        0    28149 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/evaluation/season_index.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/evaluation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:50:15.000000 baostock-0.8.9/baostock/login/
+-rw-rw-rw-   0        0        0     4347 2024-05-30 06:47:22.000000 baostock-0.8.9/baostock/login/loginout.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/login/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:50:15.000000 baostock-0.8.9/baostock/macroscopic/
+-rw-rw-rw-   0        0        0    27189 2024-05-30 06:38:04.000000 baostock-0.8.9/baostock/macroscopic/economic_data.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/macroscopic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:50:15.000000 baostock-0.8.9/baostock/metadata/
+-rw-rw-rw-   0        0        0     7237 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/metadata/stock_metadata.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/metadata/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:50:15.000000 baostock-0.8.9/baostock/security/
+-rw-rw-rw-   0        0        0     5577 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/security/history.py
+-rw-rw-rw-   0        0        0    36261 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/security/sectorinfo.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/security/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:50:15.000000 baostock-0.8.9/baostock/util/
+-rw-rw-rw-   0        0        0     3551 2024-05-30 03:39:25.000000 baostock-0.8.9/baostock/util/socketutil.py
+-rw-rw-rw-   0        0        0     2207 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/util/stringutil.py
+-rw-rw-rw-   0        0        0        0 2024-05-30 02:31:10.000000 baostock-0.8.9/baostock/util/__init__.py
+-rw-rw-rw-   0        0        0     1651 2024-05-30 06:38:12.000000 baostock-0.8.9/baostock/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:50:15.000000 baostock-0.8.9/baostock.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-31 02:50:14.000000 baostock-0.8.9/baostock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     4055 2024-05-31 02:50:14.000000 baostock-0.8.9/baostock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2024-05-31 02:50:14.000000 baostock-0.8.9/baostock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1899 2024-05-31 02:50:14.000000 baostock-0.8.9/baostock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 02:50:14.000000 baostock-0.8.9/baostock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4055 2024-05-31 02:50:15.000000 baostock-0.8.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-31 02:50:15.000000 baostock-0.8.9/setup.cfg
+-rw-rw-rw-   0        0        0     3764 2024-05-30 02:33:57.000000 baostock-0.8.9/setup.py
```

### Comparing `baostock-0.8.8/baostock/common/contants.py` & `baostock-0.8.9/baostock/common/contants.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 """
 常量类
 @author: baostock.com
 @group : baostock.com
 @contact: baostock@163.com
 """
 # 版本信息
-BAOSTOCK_CLIENT_VERSION = "00.8.80"
+BAOSTOCK_CLIENT_VERSION = "00.8.90"
 BAOSTOCK_AUTHOR = "baostock.com"
 BAOSTOCK_SERVER_IP = "www.baostock.com"  # localhost  www.baostock.com  10.25.7.4
 BAOSTOCK_SERVER_PORT = 10030
 
-BAOSTOCK_SERVER_REAL_TIME_IP = "www.baostock.com"  # 实时行情服务地址 localhost  www.baostock.com
-BAOSTOCK_SERVER_REAL_TIME_PORT = 10032  # 实时行情端口
 
 BAOSTOCK_PER_PAGE_COUNT = 10000  # 默认每页查询条数
 
 STOCK_CODE_LENGTH = 9  # 证券代码的长度
 MESSAGE_SPLIT = "\1"  # 消息内部的分隔符
 
 DELIMITER = "\n"  # 分隔符号,消息与消息之间的分隔符
```

### Comparing `baostock-0.8.8/baostock/corpreport/corp_performance.py` & `baostock-0.8.9/baostock/corpreport/corp_performance.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/baostock/data/msg.py` & `baostock-0.8.9/baostock/data/msg.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/baostock/data/resultset.py` & `baostock-0.8.9/baostock/data/resultset.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/baostock/evaluation/season_index.py` & `baostock-0.8.9/baostock/evaluation/season_index.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/baostock/login/loginout.py` & `baostock-0.8.9/baostock/metadata/stock_metadata.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,283 +1,207 @@
 # -*- coding:utf-8 -*-
 """
-登录登出
-@author: baostock.com
-@group : baostock.com
-@contact: baostock@163.com
+    证券系统元方法，如获取交易日等
 """
+import time
 import zlib
-import baostock.util.socketutil as sock
 import baostock.data.resultset as rs
 import baostock.common.contants as cons
-import baostock.data.messageheader as msgheader
-import datetime
+import baostock.util.stringutil as strUtil
 import baostock.common.context as conx
+import baostock.util.socketutil as sock
+import baostock.data.messageheader as msgheader
 
 
-def login(user_id='anonymous', password='123456', options=0):
-    """登录系统
-    :param user_id:用户ID
-    :param password:密码
-    :param options:可选项，00.5.00版本暂未使用
-    :return: ResultData()
-    """
+def query_trade_dates(start_date=None, end_date=None):
+    """查询出给定范围的交易日信息
 
+    @param start_date: 起始日期，默认2015-01-01
+    @param end_date: 终止日期，默认当前日期
+    @return: calendar_date 日期；is_trading_day，是否交易日，0:非交易日;1:交易日
+    """
     data = rs.ResultData()
-    if user_id is None or user_id == "":
-        print("用户ID不能为空。")
-        data.error_msg = "用户ID不能为空。"
-        data.error_code = cons.BSERR_USERNAME_EMPTY
-        return data
 
-    setattr(conx, "user_id", user_id)
+    if start_date is None or start_date == "":
+        start_date = cons.DEFAULT_START_DATE
+    if end_date is None or end_date == "":
+        end_date = time.strftime("%Y-%m-%d", time.localtime())
 
-    if password is None or password == "":
-        print("密码不能为空。")
-        data.error_msg = "密码不能为空。"
-        data.error_code = cons.BSERR_PASSWORD_EMPTY
+    user_id = ""
+    try:
+        user_id = getattr(conx, "user_id")
+    except Exception:
+        print("you don't login.")
+        data.error_code = cons.BSERR_NO_LOGIN
+        data.error_msg = "you don't login."
         return data
 
-    # 组织体信息
-    msg_body = "login" + cons.MESSAGE_SPLIT + user_id + cons.MESSAGE_SPLIT + \
-        password + cons.MESSAGE_SPLIT + str(options)
+    param = "%s,%s,%s,%s,%s,%s" % (
+        "query_trade_dates", user_id, "1",
+        cons.BAOSTOCK_PER_PAGE_COUNT, start_date, end_date)
 
-    # 组织头信息
+    msg_body = strUtil.organize_msg_body(param)
     msg_header = msgheader.to_message_header(
-        cons.MESSAGE_TYPE_LOGIN_REQUEST, len(msg_body))
-    head_body = msg_header + msg_body
-
-    crc32str = zlib.crc32(bytes(head_body, encoding='utf-8'))
+        cons.MESSAGE_TYPE_QUERYTRADEDATES_REQUEST, len(msg_body))
 
-    # 发送并接收消息
-    mySocketUtil = sock.SocketUtil()
-    # 创建连接
-    mySocketUtil.connect()
+    data.msg_type = cons.MESSAGE_TYPE_QUERYTRADEDATES_REQUEST
+    data.msg_body = msg_body
 
-    receive_data = sock.send_msg(
-        head_body + cons.MESSAGE_SPLIT + str(crc32str))
+    head_body = msg_header + msg_body
+    crc32str = zlib.crc32(bytes(head_body, encoding='utf-8'))
+    receive_data = sock.send_msg(head_body + cons.MESSAGE_SPLIT + str(crc32str))
 
     if receive_data is None or receive_data.strip() == "":
         data.error_code = cons.BSERR_RECVSOCK_FAIL
         data.error_msg = "网络接收错误。"
         return data
 
     msg_header = receive_data[0:cons.MESSAGE_HEADER_LENGTH]
     msg_body = receive_data[cons.MESSAGE_HEADER_LENGTH:-1]
-
     header_arr = msg_header.split(cons.MESSAGE_SPLIT)
     body_arr = msg_body.split(cons.MESSAGE_SPLIT)
-
-    data.msg_type = header_arr[1]
     data.msg_body_length = header_arr[2]
-
     data.error_code = body_arr[0]
     data.error_msg = body_arr[1]
 
     if cons.BSERR_SUCCESS == data.error_code:
-        print("login success!")
         data.method = body_arr[2]
         data.user_id = body_arr[3]
-    else:
-        print("login failed!")
+        data.cur_page_num = body_arr[4]
+        data.per_page_count = body_arr[5]
+        data.setData(body_arr[6])
+        data.start_date = body_arr[7]
+        data.end_date = body_arr[8]
+        data.setFields(body_arr[9])
 
     return data
 
 
-def logout(user_id='anonymous'):
-    """登出系统，默认用户ID：anonymous
-    :param user_id:用户ID
-    :return:ResultData()
+def query_all_stock(day=None):
+    """查询给定日期的所有证券信息，
+
+    @param day: 默认当前日期
     """
+    data = rs.ResultData()
 
-    now_time = datetime.datetime.now().strftime('%Y%m%d%H%M%S')
+    if day is None or day == "":
+        day = time.strftime("%Y-%m-%d", time.localtime())
 
-    if hasattr(conx, "user_id"):
+    user_id = ""
+    try:
         user_id = getattr(conx, "user_id")
-        if user_id is None or user_id == "":
-            print("you don't login, logout failed!")
-            return
-
-    # 组织体信息
-    msg_body = "logout" + cons.MESSAGE_SPLIT + \
-        user_id + cons.MESSAGE_SPLIT + now_time
+    except Exception:
+        print("you don't login.")
+        data.error_code = cons.BSERR_NO_LOGIN
+        data.error_msg = "you don't login."
+        return data
 
-    # 组织头信息
+    param = "%s,%s,%s,%s,%s" % (
+        "query_all_stock", user_id, "1",
+        cons.BAOSTOCK_PER_PAGE_COUNT, day)
+
+    msg_body = strUtil.organize_msg_body(param)
     msg_header = msgheader.to_message_header(
-        cons.MESSAGE_TYPE_LOGOUT_REQUEST, len(msg_body))
+        cons.MESSAGE_TYPE_QUERYALLSTOCK_REQUEST, len(msg_body))
 
-    head_body = msg_header + msg_body
+    data.msg_type = cons.MESSAGE_TYPE_QUERYALLSTOCK_REQUEST
+    data.msg_body = msg_body
 
+    head_body = msg_header + msg_body
     crc32str = zlib.crc32(bytes(head_body, encoding='utf-8'))
-
-    # 发送并接收消息
-    receive_data = sock.send_msg(
-        head_body + cons.MESSAGE_SPLIT + str(crc32str))
-
-    data = rs.ResultData()
+    receive_data = sock.send_msg(head_body + cons.MESSAGE_SPLIT + str(crc32str))
 
     if receive_data is None or receive_data.strip() == "":
         data.error_code = cons.BSERR_RECVSOCK_FAIL
         data.error_msg = "网络接收错误。"
         return data
 
     msg_header = receive_data[0:cons.MESSAGE_HEADER_LENGTH]
     msg_body = receive_data[cons.MESSAGE_HEADER_LENGTH:-1]
-
     header_arr = msg_header.split(cons.MESSAGE_SPLIT)
     body_arr = msg_body.split(cons.MESSAGE_SPLIT)
-
-    data.msg_type = header_arr[1]
     data.msg_body_length = header_arr[2]
-
     data.error_code = body_arr[0]
     data.error_msg = body_arr[1]
 
     if cons.BSERR_SUCCESS == data.error_code:
-        print("logout success!")
         data.method = body_arr[2]
         data.user_id = body_arr[3]
-    else:
-        print("logout failed!")
-
-    if hasattr(conx, "defallt_socket"):
-        if getattr(conx, "default_socket") is not None:
-            getattr(conx, "default_socket").close()
+        data.cur_page_num = body_arr[4]
+        data.per_page_count = body_arr[5]
+        data.setData(body_arr[6])
+        data.day = body_arr[7]
+        data.setFields(body_arr[8])
 
     return data
 
 
-def login_real_time(user_id='anonymous', password='123456', options=0):
-    """登录实时订阅系统系统
-    :param user_id:用户ID
-    :param password:密码
-    :param options:可选项，00.5.00版本暂未使用
-    :return: ResultData()
+def query_stock_basic(code="", code_name=""):
+    """A股证券基本资料
+    @param code: 证券代码，可为空
+    @param code_name: 证券名称，可为空，支持模糊查询
     """
-
     data = rs.ResultData()
-    if user_id is None or user_id == "":
-        print("用户ID不能为空。")
-        data.error_msg = "用户ID不能为空。"
-        data.error_code = cons.BSERR_USERNAME_EMPTY
-        return data
 
-    setattr(conx, "user_id", user_id)
+    if code is None or code == "":
+        code = ""
+    if code != "" and code is not None:
+        if len(code) != cons.STOCK_CODE_LENGTH:
+            print("股票代码应为" + str(cons.STOCK_CODE_LENGTH) + "位，请检查。格式示例：sh.600000。")
+            data.error_msg = "股票代码应为" + str(cons.STOCK_CODE_LENGTH) + "位，请检查。格式示例：sh.600000。"
+            data.error_code = cons.BSERR_PARAM_ERR
+            return data
+        code = code.lower()
+        if (code.endswith("sh") or code.endswith("sz")):
+            code = code[7:9].lower() + "." + code[0:6]
+
+    if code_name is None or code_name == "":
+        code_name = ""
 
-    if password is None or password == "":
-        print("密码不能为空。")
-        data.error_msg = "密码不能为空。"
-        data.error_code = cons.BSERR_PASSWORD_EMPTY
+    user_id = ""
+    try:
+        user_id = getattr(conx, "user_id")
+    except Exception:
+        print("you don't login.")
+        data.error_code = cons.BSERR_NO_LOGIN
+        data.error_msg = "you don't login."
         return data
 
-    # 组织体信息
-    msg_body = "login_real_time" + cons.MESSAGE_SPLIT + user_id + cons.MESSAGE_SPLIT + \
-        password + cons.MESSAGE_SPLIT + str(options)
+    param = "query_stock_basic," + str(user_id) + ",1," + \
+        str(cons.BAOSTOCK_PER_PAGE_COUNT) + \
+        "," + str(code) + "," + str(code_name)
 
-    # 组织头信息
+    msg_body = strUtil.organize_msg_body(param)
     msg_header = msgheader.to_message_header(
-        cons.MESSAGE_TYPE_LOGIN_REAL_TIME_REQUEST, len(msg_body))
-    head_body = msg_header + msg_body
+        cons.MESSAGE_TYPE_QUERYSTOCKBASIC_REQUEST, len(msg_body))
 
-    crc32str = zlib.crc32(bytes(head_body, encoding='utf-8'))
-
-    # 发送并接收消息
-    mySocketUtil = sock.SocketRealTimeUtil()
-    # 创建连接
-    mySocketUtil.connect()
+    data.msg_type = cons.MESSAGE_TYPE_QUERYSTOCKBASIC_REQUEST
+    data.msg_body = msg_body
 
-    receive_data = sock.send_real_time_msg(
-        head_body + cons.MESSAGE_SPLIT + str(crc32str))
+    head_body = msg_header + msg_body
+    crc32str = zlib.crc32(bytes(head_body, encoding='utf-8'))
+    receive_data = sock.send_msg(head_body + cons.MESSAGE_SPLIT + str(crc32str))
 
     if receive_data is None or receive_data.strip() == "":
         data.error_code = cons.BSERR_RECVSOCK_FAIL
         data.error_msg = "网络接收错误。"
         return data
 
     msg_header = receive_data[0:cons.MESSAGE_HEADER_LENGTH]
     msg_body = receive_data[cons.MESSAGE_HEADER_LENGTH:-1]
-
     header_arr = msg_header.split(cons.MESSAGE_SPLIT)
     body_arr = msg_body.split(cons.MESSAGE_SPLIT)
-
-    data.msg_type = header_arr[1]
     data.msg_body_length = header_arr[2]
-
     data.error_code = body_arr[0]
     data.error_msg = body_arr[1]
 
     if cons.BSERR_SUCCESS == data.error_code:
-        print("login success!")
         data.method = body_arr[2]
         data.user_id = body_arr[3]
-    else:
-        print("login failed!")
-        delattr(conx, "user_id")
-
-    return data
-
-
-def logout_real_time(user_id='anonymous'):
-    """登出系统，默认用户ID：anonymous
-    :param user_id:用户ID
-    :return:ResultData()
-    """
-
-    now_time = datetime.datetime.now().strftime('%Y%m%d%H%M%S')
-
-    if hasattr(conx, "user_id"):
-        user_id = getattr(conx, "user_id")
-        if user_id is None or user_id == "":
-            print("you don't login, logout failed!")
-            return
-
-    # 组织体信息
-    msg_body = "logout_real_time" + cons.MESSAGE_SPLIT + \
-        user_id + cons.MESSAGE_SPLIT + now_time
-
-    # 组织头信息
-    msg_header = msgheader.to_message_header(
-        cons.MESSAGE_TYPE_LOGOUT_REAL_TIME_REQUEST, len(msg_body))
-
-    head_body = msg_header + msg_body
-
-    crc32str = zlib.crc32(bytes(head_body, encoding='utf-8'))
-
-    # 发送并接收消息
-    receive_data = sock.send_real_time_msg(
-        head_body + cons.MESSAGE_SPLIT + str(crc32str))
-
-    data = rs.ResultData()
-
-#     if receive_data is None or receive_data.strip() == "":
-#         data.error_code = cons.BSERR_RECVSOCK_FAIL
-#         data.error_msg = "网络接收错误。"
-#         return data
-# 
-#     msg_header = receive_data[0:cons.MESSAGE_HEADER_LENGTH]
-#     msg_body = receive_data[cons.MESSAGE_HEADER_LENGTH:-1]
-# 
-#     header_arr = msg_header.split(cons.MESSAGE_SPLIT)
-#     body_arr = msg_body.split(cons.MESSAGE_SPLIT)
-# 
-#     data.msg_type = header_arr[1]
-#     data.msg_body_length = header_arr[2]
-# 
-#     data.error_code = body_arr[0]
-#     data.error_msg = body_arr[1]
-# 
-#     if cons.BSERR_SUCCESS == data.error_code:
-#         print("logout success!")
-#         data.method = body_arr[2]
-#         data.user_id = body_arr[3]
-#     else:
-#         print("logout failed!")
-
-    data.error_code = cons.BSERR_SUCCESS
-    data.error_msg = "SUCCESS"
-
-    if hasattr(conx, "socket_real_time"):
-        if getattr(conx, "socket_real_time") is not None:
-            getattr(conx, "socket_real_time").close()
+        data.cur_page_num = body_arr[4]
+        data.per_page_count = body_arr[5]
+        data.setData(body_arr[6])
+        data.code = body_arr[7]
+        data.code_name = body_arr[8]
+        data.setFields(body_arr[9])
 
     return data
-
```

### Comparing `baostock-0.8.8/baostock/macroscopic/economic_data.py` & `baostock-0.8.9/baostock/macroscopic/economic_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -454,99 +454,15 @@
         data.start_date = body_arr[7]
         data.end_date = body_arr[8]
         data.setFields(body_arr[9])
 
     return data
 
 
-def query_shibor_data(start_date="", end_date=""):
-    """银行间同业拆放利率
-    @param sart_date: 起始日期，包含次此日期，可为空
-    @param end_date: 结束日期，包含次此日期，可为空
-    """
-    data = rs.ResultData()
-
-    if start_date is None or start_date == "":
-        start_date = ""
-    else:
-        if strUtil.is_valid_date(start_date):
-            pass
-        else:
-            print("起始日期格式不正确，请修改。")
-            data.error_code = cons.BSERR_DATE_ERR
-            data.error_msg = "起始日期格式不正确，请修改。"
-            return data
-    if end_date is None or end_date == "":
-        end_date = ""
-    else:
-        if strUtil.is_valid_date(end_date):
-            pass
-        else:
-            print("结束日期格式不正确，请修改。")
-            data.error_code = cons.BSERR_DATE_ERR
-            data.error_msg = "结束日期格式不正确，请修改。"
-            return data
-    if start_date != "" and end_date != "":
-        start_date_time = datetime.datetime.strptime(
-            start_date, '%Y-%m-%d')
-        end_date_time = datetime.datetime.strptime(end_date, '%Y-%m-%d')
-        if end_date_time < start_date_time:
-            print("起始日期大于结束日期，请修改。")
-            data.error_code = cons.BSERR_START_BIGTHAN_END
-            data.error_msg = "起始日期大于结束日期，请修改。"
-            return data
-
-    user_id = ""
-    try:
-        user_id = getattr(conx, "user_id")
-    except Exception:
-        print("you don't login.")
-        data.error_code = cons.BSERR_NO_LOGIN
-        data.error_msg = "you don't login."
-        return data
-
-    param = "query_shibor_data," + str(user_id) + ",1," + \
-        str(cons.BAOSTOCK_PER_PAGE_COUNT) + \
-        "," + str(start_date) + "," + str(end_date)
-
-    msg_body = strUtil.organize_msg_body(param)
-    msg_header = msgheader.to_message_header(
-        cons.MESSAGE_TYPE_QUERYSHIBORDATA_REQUEST, len(msg_body))
-
-    data.msg_type = cons.MESSAGE_TYPE_QUERYSHIBORDATA_REQUEST
-    data.msg_body = msg_body
-
-    head_body = msg_header + msg_body
-    crc32str = zlib.crc32(bytes(head_body, encoding='utf-8'))
-    receive_data = sock.send_msg(head_body + cons.MESSAGE_SPLIT + str(crc32str))
-
-    if receive_data is None or receive_data.strip() == "":
-        data.error_code = cons.BSERR_RECVSOCK_FAIL
-        data.error_msg = "网络接收错误。"
-        return data
-
-    msg_header = receive_data[0:cons.MESSAGE_HEADER_LENGTH]
-    msg_body = receive_data[cons.MESSAGE_HEADER_LENGTH:-1]
-    header_arr = msg_header.split(cons.MESSAGE_SPLIT)
-    body_arr = msg_body.split(cons.MESSAGE_SPLIT)
-    data.msg_body_length = header_arr[2]
-    data.error_code = body_arr[0]
-    data.error_msg = body_arr[1]
-
-    if cons.BSERR_SUCCESS == data.error_code:
-        data.method = body_arr[2]
-        data.user_id = body_arr[3]
-        data.cur_page_num = body_arr[4]
-        data.per_page_count = body_arr[5]
-        data.setData(body_arr[6])
-        data.start_date = body_arr[7]
-        data.end_date = body_arr[8]
-        data.setFields(body_arr[9])
 
-    return data
 
 
 def query_cpi_data(start_date="", end_date=""):
     """居民价格消费指数
     @param sart_date: 起始日期，包含次此日期，可为空
     @param end_date: 结束日期，包含次此日期，可为空
     """
```

### Comparing `baostock-0.8.8/baostock/metadata/stock_metadata.py` & `baostock-0.8.9/baostock/login/loginout.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,207 +1,148 @@
 # -*- coding:utf-8 -*-
 """
-    证券系统元方法，如获取交易日等
+登录登出
+@author: baostock.com
+@group : baostock.com
+@contact: baostock@163.com
 """
-import time
 import zlib
+import baostock.util.socketutil as sock
 import baostock.data.resultset as rs
 import baostock.common.contants as cons
-import baostock.util.stringutil as strUtil
-import baostock.common.context as conx
-import baostock.util.socketutil as sock
 import baostock.data.messageheader as msgheader
+import datetime
+import baostock.common.context as conx
 
 
-def query_trade_dates(start_date=None, end_date=None):
-    """查询出给定范围的交易日信息
-
-    @param start_date: 起始日期，默认2015-01-01
-    @param end_date: 终止日期，默认当前日期
-    @return: calendar_date 日期；is_trading_day，是否交易日，0:非交易日;1:交易日
+def login(user_id='anonymous', password='123456', options=0):
+    """登录系统
+    :param user_id:用户ID
+    :param password:密码
+    :param options:可选项，00.5.00版本暂未使用
+    :return: ResultData()
     """
+
     data = rs.ResultData()
+    if user_id is None or user_id == "":
+        print("用户ID不能为空。")
+        data.error_msg = "用户ID不能为空。"
+        data.error_code = cons.BSERR_USERNAME_EMPTY
+        return data
 
-    if start_date is None or start_date == "":
-        start_date = cons.DEFAULT_START_DATE
-    if end_date is None or end_date == "":
-        end_date = time.strftime("%Y-%m-%d", time.localtime())
+    setattr(conx, "user_id", user_id)
 
-    user_id = ""
-    try:
-        user_id = getattr(conx, "user_id")
-    except Exception:
-        print("you don't login.")
-        data.error_code = cons.BSERR_NO_LOGIN
-        data.error_msg = "you don't login."
+    if password is None or password == "":
+        print("密码不能为空。")
+        data.error_msg = "密码不能为空。"
+        data.error_code = cons.BSERR_PASSWORD_EMPTY
         return data
 
-    param = "%s,%s,%s,%s,%s,%s" % (
-        "query_trade_dates", user_id, "1",
-        cons.BAOSTOCK_PER_PAGE_COUNT, start_date, end_date)
+    # 组织体信息
+    msg_body = "login" + cons.MESSAGE_SPLIT + user_id + cons.MESSAGE_SPLIT + \
+        password + cons.MESSAGE_SPLIT + str(options)
 
-    msg_body = strUtil.organize_msg_body(param)
+    # 组织头信息
     msg_header = msgheader.to_message_header(
-        cons.MESSAGE_TYPE_QUERYTRADEDATES_REQUEST, len(msg_body))
-
-    data.msg_type = cons.MESSAGE_TYPE_QUERYTRADEDATES_REQUEST
-    data.msg_body = msg_body
-
+        cons.MESSAGE_TYPE_LOGIN_REQUEST, len(msg_body))
     head_body = msg_header + msg_body
+
     crc32str = zlib.crc32(bytes(head_body, encoding='utf-8'))
-    receive_data = sock.send_msg(head_body + cons.MESSAGE_SPLIT + str(crc32str))
+
+    # 发送并接收消息
+    mySocketUtil = sock.SocketUtil()
+    # 创建连接
+    mySocketUtil.connect()
+
+    receive_data = sock.send_msg(
+        head_body + cons.MESSAGE_SPLIT + str(crc32str))
 
     if receive_data is None or receive_data.strip() == "":
         data.error_code = cons.BSERR_RECVSOCK_FAIL
         data.error_msg = "网络接收错误。"
         return data
 
     msg_header = receive_data[0:cons.MESSAGE_HEADER_LENGTH]
     msg_body = receive_data[cons.MESSAGE_HEADER_LENGTH:-1]
+
     header_arr = msg_header.split(cons.MESSAGE_SPLIT)
     body_arr = msg_body.split(cons.MESSAGE_SPLIT)
+
+    data.msg_type = header_arr[1]
     data.msg_body_length = header_arr[2]
+
     data.error_code = body_arr[0]
     data.error_msg = body_arr[1]
 
     if cons.BSERR_SUCCESS == data.error_code:
+        print("login success!")
         data.method = body_arr[2]
         data.user_id = body_arr[3]
-        data.cur_page_num = body_arr[4]
-        data.per_page_count = body_arr[5]
-        data.setData(body_arr[6])
-        data.start_date = body_arr[7]
-        data.end_date = body_arr[8]
-        data.setFields(body_arr[9])
+    else:
+        print("login failed!")
 
     return data
 
 
-def query_all_stock(day=None):
-    """查询给定日期的所有证券信息，
-
-    @param day: 默认当前日期
+def logout(user_id='anonymous'):
+    """登出系统，默认用户ID：anonymous
+    :param user_id:用户ID
+    :return:ResultData()
     """
-    data = rs.ResultData()
 
-    if day is None or day == "":
-        day = time.strftime("%Y-%m-%d", time.localtime())
+    now_time = datetime.datetime.now().strftime('%Y%m%d%H%M%S')
 
-    user_id = ""
-    try:
+    if hasattr(conx, "user_id"):
         user_id = getattr(conx, "user_id")
-    except Exception:
-        print("you don't login.")
-        data.error_code = cons.BSERR_NO_LOGIN
-        data.error_msg = "you don't login."
-        return data
+        if user_id is None or user_id == "":
+            print("you don't login, logout failed!")
+            return
+
+    # 组织体信息
+    msg_body = "logout" + cons.MESSAGE_SPLIT + \
+        user_id + cons.MESSAGE_SPLIT + now_time
 
-    param = "%s,%s,%s,%s,%s" % (
-        "query_all_stock", user_id, "1",
-        cons.BAOSTOCK_PER_PAGE_COUNT, day)
-
-    msg_body = strUtil.organize_msg_body(param)
+    # 组织头信息
     msg_header = msgheader.to_message_header(
-        cons.MESSAGE_TYPE_QUERYALLSTOCK_REQUEST, len(msg_body))
-
-    data.msg_type = cons.MESSAGE_TYPE_QUERYALLSTOCK_REQUEST
-    data.msg_body = msg_body
+        cons.MESSAGE_TYPE_LOGOUT_REQUEST, len(msg_body))
 
     head_body = msg_header + msg_body
-    crc32str = zlib.crc32(bytes(head_body, encoding='utf-8'))
-    receive_data = sock.send_msg(head_body + cons.MESSAGE_SPLIT + str(crc32str))
-
-    if receive_data is None or receive_data.strip() == "":
-        data.error_code = cons.BSERR_RECVSOCK_FAIL
-        data.error_msg = "网络接收错误。"
-        return data
-
-    msg_header = receive_data[0:cons.MESSAGE_HEADER_LENGTH]
-    msg_body = receive_data[cons.MESSAGE_HEADER_LENGTH:-1]
-    header_arr = msg_header.split(cons.MESSAGE_SPLIT)
-    body_arr = msg_body.split(cons.MESSAGE_SPLIT)
-    data.msg_body_length = header_arr[2]
-    data.error_code = body_arr[0]
-    data.error_msg = body_arr[1]
 
-    if cons.BSERR_SUCCESS == data.error_code:
-        data.method = body_arr[2]
-        data.user_id = body_arr[3]
-        data.cur_page_num = body_arr[4]
-        data.per_page_count = body_arr[5]
-        data.setData(body_arr[6])
-        data.day = body_arr[7]
-        data.setFields(body_arr[8])
-
-    return data
+    crc32str = zlib.crc32(bytes(head_body, encoding='utf-8'))
 
+    # 发送并接收消息
+    receive_data = sock.send_msg(
+        head_body + cons.MESSAGE_SPLIT + str(crc32str))
 
-def query_stock_basic(code="", code_name=""):
-    """A股证券基本资料
-    @param code: 证券代码，可为空
-    @param code_name: 证券名称，可为空，支持模糊查询
-    """
     data = rs.ResultData()
 
-    if code is None or code == "":
-        code = ""
-    if code != "" and code is not None:
-        if len(code) != cons.STOCK_CODE_LENGTH:
-            print("股票代码应为" + str(cons.STOCK_CODE_LENGTH) + "位，请检查。格式示例：sh.600000。")
-            data.error_msg = "股票代码应为" + str(cons.STOCK_CODE_LENGTH) + "位，请检查。格式示例：sh.600000。"
-            data.error_code = cons.BSERR_PARAM_ERR
-            return data
-        code = code.lower()
-        if (code.endswith("sh") or code.endswith("sz")):
-            code = code[7:9].lower() + "." + code[0:6]
-
-    if code_name is None or code_name == "":
-        code_name = ""
-
-    user_id = ""
-    try:
-        user_id = getattr(conx, "user_id")
-    except Exception:
-        print("you don't login.")
-        data.error_code = cons.BSERR_NO_LOGIN
-        data.error_msg = "you don't login."
-        return data
-
-    param = "query_stock_basic," + str(user_id) + ",1," + \
-        str(cons.BAOSTOCK_PER_PAGE_COUNT) + \
-        "," + str(code) + "," + str(code_name)
-
-    msg_body = strUtil.organize_msg_body(param)
-    msg_header = msgheader.to_message_header(
-        cons.MESSAGE_TYPE_QUERYSTOCKBASIC_REQUEST, len(msg_body))
-
-    data.msg_type = cons.MESSAGE_TYPE_QUERYSTOCKBASIC_REQUEST
-    data.msg_body = msg_body
-
-    head_body = msg_header + msg_body
-    crc32str = zlib.crc32(bytes(head_body, encoding='utf-8'))
-    receive_data = sock.send_msg(head_body + cons.MESSAGE_SPLIT + str(crc32str))
-
     if receive_data is None or receive_data.strip() == "":
         data.error_code = cons.BSERR_RECVSOCK_FAIL
         data.error_msg = "网络接收错误。"
         return data
 
     msg_header = receive_data[0:cons.MESSAGE_HEADER_LENGTH]
     msg_body = receive_data[cons.MESSAGE_HEADER_LENGTH:-1]
+
     header_arr = msg_header.split(cons.MESSAGE_SPLIT)
     body_arr = msg_body.split(cons.MESSAGE_SPLIT)
+
+    data.msg_type = header_arr[1]
     data.msg_body_length = header_arr[2]
+
     data.error_code = body_arr[0]
     data.error_msg = body_arr[1]
 
     if cons.BSERR_SUCCESS == data.error_code:
+        print("logout success!")
         data.method = body_arr[2]
         data.user_id = body_arr[3]
-        data.cur_page_num = body_arr[4]
-        data.per_page_count = body_arr[5]
-        data.setData(body_arr[6])
-        data.code = body_arr[7]
-        data.code_name = body_arr[8]
-        data.setFields(body_arr[9])
+    else:
+        print("logout failed!")
+
+    if hasattr(conx, "default_socket"):
+        if getattr(conx, "default_socket") is not None:
+            getattr(conx, "default_socket").close()
 
     return data
+
+
```

### Comparing `baostock-0.8.8/baostock/realtime/subscibe.py` & `baostock-0.8.9/baostock/security/history.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,157 +1,137 @@
 # -*- coding:utf-8 -*-
+"""
+获取历史行情
+@author: baostock.com
+@group : baostock.com
+@contact: baostock@163.com
+"""
+import datetime
 import time
 import zlib
-import ctypes
-import inspect
-import baostock.data.resultset as rs
+
 import baostock.common.contants as cons
-import baostock.util.stringutil as strUtil
 import baostock.common.context as conx
-import baostock.util.socketutil as sock
 import baostock.data.messageheader as msgheader
+import baostock.data.resultset as rs
+import baostock.util.socketutil as sock
+import baostock.util.stringutil as strUtil
 
 
-def subscribe_by_code(code_list, subscribe_type=0, fncallback=None, options="", user_params=None):
-    """订阅实时行情
-    @param code_list: 每只证券代码之间用“英文逗号分隔符”，结尾不存在“英文逗号分隔符”；证券代码格式：sh.600000，前两位为证券市场：“sz”深圳、“sh”上海
-    @param subscribe_type: 订阅方式 0：按证券代码订阅， 1：按行情数据类型订阅。0.7.5版本只支持按证券代码订阅；
-    @param fncallback: 自定义回调方法
-    @param options: 预留参数
-    @param user_params: 用户参数，回调时原样返回
-    """
-    data = rs.SubscibeData()
-    data.method = "subscribe_by_code"
-    data.options = options
-    data.user_params = user_params
-
-    if code_list is None or code_list == "":
-        data.error_code = cons.BSERR_CODE_INVALIED
-        data.error_msg = "证券代码不正确"
-        return data
-
-    # 判断code_list，如果大于限制，则进行截取
-    if len(code_list.split(cons.ATTRIBUTE_SPLIT)) > cons.BAOSTOCK_REALTIME_LIMIT_COUNT:
-        code_list = cons.ATTRIBUTE_SPLIT.join(code_list.split(cons.ATTRIBUTE_SPLIT)[0:cons.BAOSTOCK_REALTIME_LIMIT_COUNT])
-
-    data.code_list = code_list.lower()
-
-    # 设置订阅方式 默认为0
-    # if subscribe_type == 0 or subscribe_type == 1:
-    if subscribe_type == 0:
-        pass
-    else:
-        subscribe_type = 0
-    data.subscribe_type = subscribe_type
-
-    if not callable(fncallback):
-        fncallback = DemoCallback
-    data.fncallback = fncallback
-    user_id = ""
-    try:
-        user_id = getattr(conx, "user_id")
-    except Exception:
-        print("you don't login.")
-        data.error_code = cons.BSERR_NO_LOGIN
-        data.error_msg = "you don't login."
-        return data
-
-    data.user_id = user_id
-    param = "%s\1%s\1%s\1%s\1%s\1%s\1%s" % (
-        "subscribe_by_code", user_id, subscribe_type,
-        code_list, fncallback, options, user_params)
-    msg_body = strUtil.organize_realtime_msg_body(param)
-    msg_header = msgheader.to_message_header(
-        cons.MESSAGE_TYPE_SUBSCRIPTIONS_BY_SECURITYID_REQUEST, len(msg_body))
-    data.msg_type = cons.MESSAGE_TYPE_SUBSCRIPTIONS_BY_SECURITYID_REQUEST
-    data.msg_body = msg_body
-
-    head_body = msg_header + msg_body
-    crc32str = zlib.crc32(bytes(head_body, encoding='utf-8'))
-
-    sock.send_real_time_subscibe(head_body + cons.MESSAGE_SPLIT + str(crc32str), data)
-
-    return data
+def query_history_k_data_plus(code, fields, start_date=None, end_date=None,
+                              frequency='d', adjustflag='3'):
+    """获取历史K线plus"""
+    return __query_history_k_data_plus_page(1, cons.BAOSTOCK_PER_PAGE_COUNT, code, fields, start_date,
+                                            end_date, frequency, adjustflag)
 
 
-def cancel_subscribe(ident):
-    """取消实时行情
-    @param thread: 实时行情的线程；
-    """
-    data = rs.SubscibeData()
+def __query_history_k_data_plus_page(cur_page_num, per_page_count, code, fields,
+                                     start_date, end_date, frequency, adjustflag):
+    """获取历史K线，私有方法"""
+    data = rs.ResultData()
+    if code is None or code == "":
+        print("股票代码不能为空，请检查。")
+        data.error_msg = "股票代码不能为空，请检查。"
+        data.error_code = cons.BSERR_PARAM_ERR
+        return data
+    if len(code) != cons.STOCK_CODE_LENGTH:
+        print("股票代码应为" + str(cons.STOCK_CODE_LENGTH) + "位，请检查。格式示例：sh.600000。")
+        data.error_msg = "股票代码应为" + str(cons.STOCK_CODE_LENGTH) + "位，请检查。格式示例：sh.600000。"
+        data.error_code = cons.BSERR_PARAM_ERR
+        return data
+    code = code.lower()
+    if (code.endswith("sh") or code.endswith("sz")):
+        code = code[7:9].lower() + "." + code[0:6]
+    if fields is None or fields == "":
+        data.error_msg = "指示简称不能为空，请检查。"
+        data.error_code = cons.BSERR_PARAM_ERR
+        print("指示简称不能为空，请检查。")
+        return data
 
-    # 取订阅的子循环
-    try:
-        _async_raise(ident, SystemExit)
-    except (ValueError, TypeError):
+    if start_date is None or start_date == "":
+        start_date = cons.DEFAULT_START_DATE
+    if end_date is None or end_date == "":
+        end_date = time.strftime("%Y-%m-%d", time.localtime())
+
+    if start_date != "" and end_date != "":
+        if strUtil.is_valid_date(start_date) and strUtil.is_valid_date(end_date):
+            start_date_time = datetime.datetime.strptime(
+                start_date, '%Y-%m-%d')
+            end_date_time = datetime.datetime.strptime(end_date, '%Y-%m-%d')
+            if end_date_time < start_date_time:
+                print("起始日期大于终止日期，请修改。")
+                data.error_code = cons.BSERR_START_BIGTHAN_END
+                data.error_msg = "起始日期大于终止日期，请修改。"
+                return data
+        else:
+            print("日期格式不正确，请修改。")
+            return
+
+    if frequency is None or frequency == "":
+        print("数据类型（frequency）不可为空，请检查。")
+        data.error_msg = "数据类型（frequency）不可为空，请检查"
+        data.error_code = cons.BSERR_PARAM_ERR
+        return data
+    if adjustflag is None or adjustflag == "":
+        print("复权类型（adjustflag）不可为空，请检查。")
+        data.error_msg = "复权类型（adjustflag）不可为空，请检查。"
         data.error_code = cons.BSERR_PARAM_ERR
-        data.error_msg = "取消订阅失败"
         return data
 
-    # 封装待发出的消息
     user_id = ""
     try:
         user_id = getattr(conx, "user_id")
     except Exception:
         print("you don't login.")
         data.error_code = cons.BSERR_NO_LOGIN
         data.error_msg = "you don't login."
         return data
 
-    data.user_id = user_id
-
-    # 组织体信息
-    msg_body = "cancel_subscribe" + cons.MESSAGE_SPLIT + user_id
+    msg_body = "query_history_k_data_plus" + cons.MESSAGE_SPLIT + user_id + cons.MESSAGE_SPLIT \
+               + str(cur_page_num) + cons.MESSAGE_SPLIT + str(per_page_count) + cons.MESSAGE_SPLIT + code \
+               + cons.MESSAGE_SPLIT + fields + cons.MESSAGE_SPLIT + start_date \
+               + cons.MESSAGE_SPLIT + end_date + cons.MESSAGE_SPLIT + frequency \
+               + cons.MESSAGE_SPLIT + adjustflag
 
-    # 组织头信息
     msg_header = msgheader.to_message_header(
-        cons.MESSAGE_TYPE_CANCEL_SUBSCRIBE_REQUEST, len(msg_body))
-    head_body = msg_header + msg_body
+        cons.MESSAGE_TYPE_GETKDATAPLUS_REQUEST, len(msg_body))
+
+    data.msg_type = cons.MESSAGE_TYPE_GETKDATAPLUS_REQUEST
+    data.msg_body = msg_body
 
+    head_body = msg_header + msg_body
     crc32str = zlib.crc32(bytes(head_body, encoding='utf-8'))
 
-    # 向服务器发送取消订阅
-    sock.send_cancel_real_time_msg(head_body + cons.MESSAGE_SPLIT + str(crc32str))
+    receive_data = sock.send_msg(head_body + cons.MESSAGE_SPLIT + str(crc32str))
 
-    data.error_code = cons.BSERR_SUCCESS
-    data.error_msg = "success"
+    if receive_data is None or receive_data.strip() == "":
+        data.error_code = cons.BSERR_RECVSOCK_FAIL
+        data.error_msg = "网络接收错误。"
+        return data
 
-#     if receive_data is None or receive_data.strip() == "":
-#         data.error_code = cons.BSERR_RECVSOCK_FAIL
-#         data.error_msg = "网络接收错误。"
-#         return data
-# 
-#     msg_header = receive_data[0:cons.MESSAGE_HEADER_LENGTH]
-#     msg_body = receive_data[cons.MESSAGE_HEADER_LENGTH:-1]
-# 
-#     header_arr = msg_header.split(cons.MESSAGE_SPLIT)
-#     body_arr = msg_body.split(cons.MESSAGE_SPLIT)
-# 
-#     data.msg_type = header_arr[1]
-#     data.msg_body_length = header_arr[2]
-# 
-#     data.error_code = body_arr[0]
-#     data.error_msg = body_arr[1]
+    msg_header = receive_data[0:cons.MESSAGE_HEADER_LENGTH]
+    msg_body = receive_data[cons.MESSAGE_HEADER_LENGTH:-1]
 
-    return data
+    header_arr = msg_header.split(cons.MESSAGE_SPLIT)
+    body_arr = msg_body.split(cons.MESSAGE_SPLIT)
 
+    # data.version = header_arr[0]
+    # data.msg_type = header_arr[1]
+    data.msg_body_length = header_arr[2]
+
+    data.error_code = body_arr[0]
+    data.error_msg = body_arr[1]
+
+    if cons.BSERR_SUCCESS == data.error_code:
+        data.method = body_arr[2]
+        data.user_id = body_arr[3]
+        data.cur_page_num = body_arr[4]
+        data.per_page_count = body_arr[5]
+        data.setData(body_arr[6])
+        data.code = body_arr[7]
+        data.setFields(body_arr[8])
+        data.start_date = body_arr[9]
+        data.end_date = body_arr[10]
+        data.frequency = body_arr[11]
+        data.adjustflag = body_arr[12]
 
-def _async_raise(tid, exctype):
-    """raises the exception, performs cleanup if needed"""
-    tid = ctypes.c_long(tid)
-    if not inspect.isclass(exctype):
-        exctype = type(exctype)
-    res = ctypes.pythonapi.PyThreadState_SetAsyncExc(tid, ctypes.py_object(exctype))
-    if res == 0:
-        raise ValueError("invalid thread id")
-    elif res != 1:
-        ctypes.pythonapi.PyThreadState_SetAsyncExc(tid, None)
-        raise SystemError("PyThreadState_SetAsyncExc failed")
-
-
-def DemoCallback(quantdata):
-    """
-    DemoCallback 是订阅时提供的回调函数模板。该函数只有一个为ResultData类型的参数quantdata
-    :param quantdata:ResultData
-    :return:
-    """
-    print(quantdata.data)
+    return data
```

### Comparing `baostock-0.8.8/baostock/security/sectorinfo.py` & `baostock-0.8.9/baostock/security/sectorinfo.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/baostock/util/stringutil.py` & `baostock-0.8.9/baostock/util/stringutil.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/baostock/__init__.py` & `baostock-0.8.9/baostock/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 __version__ = cons.BAOSTOCK_CLIENT_VERSION
 __author__ = cons.BAOSTOCK_AUTHOR
 
 # login/logout
 from baostock.login.loginout import (login, logout)
 
 # history data
-from baostock.security.history import (query_history_k_data, query_history_k_data_plus)
+from baostock.security.history import (query_history_k_data_plus)
 
 # sector info
 from baostock.security.sectorinfo import (query_stock_industry,
                                           query_hs300_stocks,
                                           query_sz50_stocks,
                                           query_zz500_stocks)
 
@@ -34,8 +34,8 @@
 # metadata
 from baostock.metadata.stock_metadata import (query_trade_dates, query_all_stock,
                                               query_stock_basic)
 
 # macroscopic
 from baostock.macroscopic.economic_data import (query_deposit_rate_data, query_loan_rate_data,
                                                 query_required_reserve_ratio_data, query_money_supply_data_month,
-                                                query_money_supply_data_year, query_shibor_data)
+                                                query_money_supply_data_year)
```

### Comparing `baostock-0.8.8/baostock.egg-info/PKG-INFO` & `baostock-0.8.9/baostock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: baostock
-Version: 0.8.8
+Version: 0.8.9
 Summary: A tool for obtaining historical data of China stock market
 Home-page: http://www.baostock.com
 Author: baostock
 Author-email: baostock@163.com
 License: BSD License
 Description: 
         BaoStock
@@ -42,15 +42,15 @@
         
             # 登陆系统
             lg = bs.login()
             # 显示登陆返回信息
             print(lg.error_code)
             print(lg.error_msg)
             # 详细指标参数，参见“历史行情指标参数”章节
-            rs = bs.query_history_k_data("sh.601398",
+            rs = bs.query_history_k_data_plus("sh.601398",
                 "date,code,open,high,low,close,volume,amount,adjustflag",
                 start_date='2017-01-01', end_date='2017-01-31',
                 frequency="d", adjustflag="3")
             print(rs.error_code)
             print(rs.error_msg)
             # 获取具体的信息
             result_list = []
```

### Comparing `baostock-0.8.8/demo/demo_Adjust_factor_data.py` & `baostock-0.8.9/baostock/demo/demo_Adjust_factor_data.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_AllStock.py` & `baostock-0.8.9/baostock/demo/demo_AllStock.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_A_stock_k_data.py` & `baostock-0.8.9/baostock/demo/demo_A_stock_k_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 lg = bs.login()
 # 显示登陆返回信息
 print('login respond error_code:'+lg.error_code)
 print('login respond  error_msg:'+lg.error_msg)
 
 #### 获取历史K线数据 ####
 # 详细指标参数，参见“历史行情指标参数”章节
-rs = bs.query_history_k_data("sh.600000",
+rs = bs.query_history_k_data_plus("sh.600000",
     "date,code,open,high,low,close,preclose,volume,amount,adjustflag,turn,tradestatus,pctChg,peTTM,pbMRQ,psTTM,pcfNcfTTM,isST",
     start_date='2017-06-01', end_date='2017-12-31', 
     frequency="d", adjustflag="3") #frequency="d"取日k线，adjustflag="3"默认不复权
 
-print('query_history_k_data respond error_code:'+rs.error_code)
-print('query_history_k_data respond  error_msg:'+rs.error_msg)
+print('query_history_k_data_plus respond error_code:'+rs.error_code)
+print('query_history_k_data_plus respond  error_msg:'+rs.error_msg)
 
 #### 打印结果集 ####
 data_list = []
 while (rs.error_code == '0') & rs.next():
     # 获取一条记录，将记录合并在一起
     data_list.append(rs.get_row_data())
 result = pd.DataFrame(data_list, columns=rs.fields)
```

### Comparing `baostock-0.8.8/demo/demo_Balance_data.py` & `baostock-0.8.9/baostock/demo/demo_Balance_data.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_CashFlow_data.py` & `baostock-0.8.9/baostock/demo/demo_CashFlow_data.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_depositRate_data.py` & `baostock-0.8.9/baostock/demo/demo_depositRate_data.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_Dividend_data.py` & `baostock-0.8.9/baostock/demo/demo_Dividend_data.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_Dupont_data.py` & `baostock-0.8.9/baostock/demo/demo_Dupont_data.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_Forecast_report.py` & `baostock-0.8.9/baostock/demo/demo_Forecast_report.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_Growth_data.py` & `baostock-0.8.9/baostock/demo/demo_Growth_data.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_hs300_stocks.py` & `baostock-0.8.9/baostock/demo/demo_hs300_stocks.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_Index_k_data.py` & `baostock-0.8.9/baostock/demo/demo_Index_k_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 ##二级行业指数，例如：sh.000952 300地产，sz.399951 300银行 等；
 ##策略指数，例如：sh.000050 50等权，sh.000982 500等权 等；
 ##成长指数，例如：sz.399376 小盘成长 等；
 ##价值指数，例如：sh.000029 180价值 等；
 ##主题指数，例如：sh.000015 红利指数，sh.000063 上证周期 等；
 
 # 详细指标参数，参见“历史行情指标参数”章节
-rs = bs.query_history_k_data("sh.600000",
+rs = bs.query_history_k_data_plus("sh.600000",
     "date,code,open,high,low,close,preclose,volume,amount,pctChg",
     start_date='2017-01-01', end_date='2017-06-30', 
     frequency="d", adjustflag="3")
-print('query_history_k_data respond error_code:'+rs.error_code)
-print('query_history_k_data respond  error_msg:'+rs.error_msg)
+print('query_history_k_data_plus respond error_code:'+rs.error_code)
+print('query_history_k_data_plus respond  error_msg:'+rs.error_msg)
 
 #### 打印结果集 ####
 data_list = []
 while (rs.error_code == '0') & rs.next():
     # 获取一条记录，将记录合并在一起
     data_list.append(rs.get_row_data())
 result = pd.DataFrame(data_list, columns=rs.fields)
```

### Comparing `baostock-0.8.8/demo/demo_loanRate_data.py` & `baostock-0.8.9/baostock/demo/demo_loanRate_data.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_moneySupplyDataMonth_data.py` & `baostock-0.8.9/baostock/demo/demo_moneySupplyDataMonth_data.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_moneySupplyDataYear_data.py` & `baostock-0.8.9/baostock/demo/demo_moneySupplyDataYear_data.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_Operation_data.py` & `baostock-0.8.9/baostock/demo/demo_Operation_data.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_PerformanceExpress_report.py` & `baostock-0.8.9/baostock/demo/demo_PerformanceExpress_report.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_Profit_data.py` & `baostock-0.8.9/baostock/demo/demo_Profit_data.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_requiredReserveRatio_data.py` & `baostock-0.8.9/baostock/demo/demo_requiredReserveRatio_data.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_startst_stocks.py` & `baostock-0.8.9/baostock/demo/demo_zz500_stock.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 # 登陆系统
 lg = bs.login()
 # 显示登陆返回信息
 print('login respond error_code:'+lg.error_code)
 print('login respond  error_msg:'+lg.error_msg)
 
-# 获取证券基本资料
-rs = bs.query_starst_stocks()
-print('query_starst error_code:'+rs.error_code)
-print('query_starst  error_msg:'+rs.error_msg)
+# 获取中证500成分股
+rs = bs.query_zz500_stocks()
+print('query_zz500 error_code:'+rs.error_code)
+print('query_zz500  error_msg:'+rs.error_msg)
 
 # 打印结果集
-starst_stocks = []
+zz500_stocks = []
 while (rs.error_code == '0') & rs.next():
     # 获取一条记录，将记录合并在一起
-    starst_stocks.append(rs.get_row_data())
-result = pd.DataFrame(starst_stocks, columns=rs.fields)
+    zz500_stocks.append(rs.get_row_data())
+result = pd.DataFrame(zz500_stocks, columns=rs.fields)
 # 结果集输出到csv文件
-result.to_csv("D:/starst_stocks.csv", encoding="gbk", index=False)
+result.to_csv("D:/zz500_stocks.csv", encoding="gbk", index=False)
 print(result)
 
 # 登出系统
 bs.logout()
```

### Comparing `baostock-0.8.8/demo/demo_stockBasic_data.py` & `baostock-0.8.9/baostock/demo/demo_stockBasic_data.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_stock_industry.py` & `baostock-0.8.9/baostock/demo/demo_stock_industry.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/demo/demo_stock_Valuation_indicator_data.py` & `baostock-0.8.9/baostock/demo/demo_stock_Valuation_indicator_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 print('login respond  error_msg:'+lg.error_msg)
 
 #### 获取沪深A股估值指标(日频)数据 ####
 # peTTM    动态市盈率
 # psTTM    市销率
 # pcfNcfTTM    市现率
 # pbMRQ    市净率
-rs = bs.query_history_k_data("sh.600000",
+rs = bs.query_history_k_data_plus("sh.600000",
     "date,code,close,peTTM,pbMRQ,psTTM,pcfNcfTTM",
     start_date='2015-01-01', end_date='2017-12-31', 
     frequency="d", adjustflag="3")
-print('query_history_k_data respond error_code:'+rs.error_code)
-print('query_history_k_data respond  error_msg:'+rs.error_msg)
+print('query_history_k_data_plus respond error_code:'+rs.error_code)
+print('query_history_k_data_plus respond  error_msg:'+rs.error_msg)
 
 #### 打印结果集 ####
 result_list = []
 while (rs.error_code == '0') & rs.next():
     # 获取一条记录，将记录合并在一起
     result_list.append(rs.get_row_data())
 result = pd.DataFrame(result_list, columns=rs.fields)
```

### Comparing `baostock-0.8.8/demo/demo_suspended_stocks.py` & `baostock-0.8.9/baostock/demo/demo_sz50stocks.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 # 登陆系统
 lg = bs.login()
 # 显示登陆返回信息
 print('login respond error_code:'+lg.error_code)
 print('login respond  error_msg:'+lg.error_msg)
 
-# 获取暂停上市股票
-rs = bs.query_suspended_stocks()
-print('query_suspended error_code:'+rs.error_code)
-print('query_suspended  error_msg:'+rs.error_msg)
+# 获取上证50成分股
+rs = bs.query_sz50_stocks(date="2018-08-10")
+print('query_sz50 error_code:'+rs.error_code)
+print('query_sz50  error_msg:'+rs.error_msg)
 
 # 打印结果集
-suspended_stocks = []
+sz50_stocks = []
 while (rs.error_code == '0') & rs.next():
     # 获取一条记录，将记录合并在一起
-    suspended_stocks.append(rs.get_row_data())
-result = pd.DataFrame(suspended_stocks, columns=rs.fields)
+    sz50_stocks.append(rs.get_row_data())
+result = pd.DataFrame(sz50_stocks, columns=rs.fields)
 # 结果集输出到csv文件
-result.to_csv("D:/suspended_stocks.csv", encoding="gbk", index=False)
+result.to_csv("D:/sz50_stocks.csv", encoding="gbk", index=False)
 print(result)
 
 # 登出系统
 bs.logout()
```

### Comparing `baostock-0.8.8/demo/demo_TradeDates.py` & `baostock-0.8.9/baostock/demo/demo_TradeDates.py`

 * *Files identical despite different names*

### Comparing `baostock-0.8.8/PKG-INFO` & `baostock-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: baostock
-Version: 0.8.8
+Version: 0.8.9
 Summary: A tool for obtaining historical data of China stock market
 Home-page: http://www.baostock.com
 Author: baostock
 Author-email: baostock@163.com
 License: BSD License
 Description: 
         BaoStock
@@ -42,15 +42,15 @@
         
             # 登陆系统
             lg = bs.login()
             # 显示登陆返回信息
             print(lg.error_code)
             print(lg.error_msg)
             # 详细指标参数，参见“历史行情指标参数”章节
-            rs = bs.query_history_k_data("sh.601398",
+            rs = bs.query_history_k_data_plus("sh.601398",
                 "date,code,open,high,low,close,volume,amount,adjustflag",
                 start_date='2017-01-01', end_date='2017-01-31',
                 frequency="d", adjustflag="3")
             print(rs.error_code)
             print(rs.error_msg)
             # 获取具体的信息
             result_list = []
```

### Comparing `baostock-0.8.8/setup.py` & `baostock-0.8.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     # 登陆系统
     lg = bs.login()
     # 显示登陆返回信息
     print(lg.error_code)
     print(lg.error_msg)
     # 详细指标参数，参见“历史行情指标参数”章节
-    rs = bs.query_history_k_data("sh.601398",
+    rs = bs.query_history_k_data_plus("sh.601398",
         "date,code,open,high,low,close,volume,amount,adjustflag",
         start_date='2017-01-01', end_date='2017-01-31',
         frequency="d", adjustflag="3")
     print(rs.error_code)
     print(rs.error_msg)
     # 获取具体的信息
     result_list = []
@@ -81,15 +81,15 @@
     7    277258304.0000          3  0.023058           1  
 
 """
 
 
 setup(
     name='baostock',
-    version='0.8.8',
+    version='0.8.9',
     description=(
         'A tool for obtaining historical data of China stock market'
     ),
     long_description=long_desc,
     author='baostock',
     author_email='baostock@163.com',
     license='BSD License',
```

