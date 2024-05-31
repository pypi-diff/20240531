# Comparing `tmp/capdata-1.0.2.1.tar.gz` & `tmp/capdata-1.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capdata-1.0.2.1.tar", last modified: Wed May 29 06:24:15 2024, max compression
+gzip compressed data, was "capdata-1.0.3.1.tar", last modified: Fri May 31 03:24:26 2024, max compression
```

## Comparing `capdata-1.0.2.1.tar` & `capdata-1.0.3.1.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 06:24:15.639237 capdata-1.0.2.1/
--rw-rw-rw-   0        0        0      136 2024-05-29 06:24:15.639237 capdata-1.0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      504 2024-05-29 06:24:12.000000 capdata-1.0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 06:24:15.630239 capdata-1.0.2.1/capdata.egg-info/
--rw-rw-rw-   0        0        0      136 2024-05-29 06:24:15.000000 capdata-1.0.2.1/capdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2024-05-29 06:24:15.000000 capdata-1.0.2.1/capdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 06:24:15.000000 capdata-1.0.2.1/capdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-29 06:24:15.000000 capdata-1.0.2.1/capdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 06:24:15.000000 capdata-1.0.2.1/capdata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-29 06:24:15.634237 capdata-1.0.2.1/data/
--rw-rw-rw-   0        0        0       39 2022-07-29 01:19:04.000000 capdata-1.0.2.1/data/__init__.py
--rw-rw-rw-   0        0        0     1318 2024-05-28 09:44:12.000000 capdata-1.0.2.1/data/curve.py
--rw-rw-rw-   0        0        0     1341 2024-05-28 09:44:12.000000 capdata-1.0.2.1/data/market.py
--rw-rw-rw-   0        0        0     1982 2024-05-28 09:44:12.000000 capdata-1.0.2.1/data/pricing.py
--rw-rw-rw-   0        0        0      920 2024-05-28 09:44:12.000000 capdata-1.0.2.1/data/refer.py
--rw-rw-rw-   0        0        0     3550 2024-05-29 06:23:36.000000 capdata-1.0.2.1/data/risk.py
--rw-rw-rw-   0        0        0      225 2024-05-28 09:44:12.000000 capdata-1.0.2.1/data/token.py
-drwxrwxrwx   0        0        0        0 2024-05-29 06:24:15.635237 capdata-1.0.2.1/request/
--rw-rw-rw-   0        0        0       80 2024-05-27 10:19:49.000000 capdata-1.0.2.1/request/__init__.py
--rw-rw-rw-   0        0        0     1916 2024-05-29 02:26:32.000000 capdata-1.0.2.1/request/request.py
--rw-rw-rw-   0        0        0       42 2024-05-29 06:24:15.639237 capdata-1.0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      604 2024-05-29 06:24:12.000000 capdata-1.0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 06:24:15.638239 capdata-1.0.2.1/test/
--rw-rw-rw-   0        0        0      194 2024-05-29 02:27:37.000000 capdata-1.0.2.1/test/test_auth.py
--rw-rw-rw-   0        0        0     1036 2024-05-28 09:47:25.000000 capdata-1.0.2.1/test/test_curve.py
--rw-rw-rw-   0        0        0      691 2024-05-28 09:47:25.000000 capdata-1.0.2.1/test/test_market.py
--rw-rw-rw-   0        0        0      975 2024-05-28 09:47:25.000000 capdata-1.0.2.1/test/test_pricing.py
--rw-rw-rw-   0        0        0     1194 2024-05-28 09:47:25.000000 capdata-1.0.2.1/test/test_refer.py
--rw-rw-rw-   0        0        0     2098 2024-05-29 06:18:16.000000 capdata-1.0.2.1/test/test_risk.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:24:26.049296 capdata-1.0.3.1/
+-rw-rw-rw-   0        0        0      132 2024-05-31 03:24:26.049296 capdata-1.0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2024-05-31 03:23:46.000000 capdata-1.0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 03:24:26.038760 capdata-1.0.3.1/capdata.egg-info/
+-rw-rw-rw-   0        0        0      132 2024-05-31 03:24:25.000000 capdata-1.0.3.1/capdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      418 2024-05-31 03:24:25.000000 capdata-1.0.3.1/capdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 03:24:25.000000 capdata-1.0.3.1/capdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-31 03:24:25.000000 capdata-1.0.3.1/capdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 03:24:25.000000 capdata-1.0.3.1/capdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 03:24:26.042760 capdata-1.0.3.1/data/
+-rw-rw-rw-   0        0        0       39 2022-07-29 01:19:04.000000 capdata-1.0.3.1/data/__init__.py
+-rw-rw-rw-   0        0        0     1318 2024-05-31 02:50:56.000000 capdata-1.0.3.1/data/curve.py
+-rw-rw-rw-   0        0        0     1309 2024-05-31 02:55:42.000000 capdata-1.0.3.1/data/market.py
+-rw-rw-rw-   0        0        0     1941 2024-05-31 02:55:42.000000 capdata-1.0.3.1/data/pricing.py
+-rw-rw-rw-   0        0        0      920 2024-05-31 02:51:15.000000 capdata-1.0.3.1/data/refer.py
+-rw-rw-rw-   0        0        0     3541 2024-05-31 02:55:42.000000 capdata-1.0.3.1/data/risk.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:24:26.043762 capdata-1.0.3.1/request/
+-rw-rw-rw-   0        0        0       80 2024-05-27 10:19:49.000000 capdata-1.0.3.1/request/__init__.py
+-rw-rw-rw-   0        0        0     1916 2024-05-31 01:45:57.000000 capdata-1.0.3.1/request/request.py
+-rw-rw-rw-   0        0        0       42 2024-05-31 03:24:26.050303 capdata-1.0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-05-31 03:23:46.000000 capdata-1.0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:24:26.048760 capdata-1.0.3.1/test/
+-rw-rw-rw-   0        0        0     5712 2024-05-31 03:23:13.000000 capdata-1.0.3.1/test/test_capdata.py
+-rw-rw-rw-   0        0        0     1034 2024-05-31 02:42:04.000000 capdata-1.0.3.1/test/test_curve.py
+-rw-rw-rw-   0        0        0      691 2024-05-31 01:45:03.000000 capdata-1.0.3.1/test/test_market.py
+-rw-rw-rw-   0        0        0      975 2024-05-31 01:45:06.000000 capdata-1.0.3.1/test/test_pricing.py
+-rw-rw-rw-   0        0        0     1194 2024-05-31 01:44:25.000000 capdata-1.0.3.1/test/test_refer.py
+-rw-rw-rw-   0        0        0     2098 2024-05-31 01:41:43.000000 capdata-1.0.3.1/test/test_risk.py
```

### Comparing `capdata-1.0.2.1/data/curve.py` & `capdata-1.0.3.1/data/curve.py`

 * *Files identical despite different names*

### Comparing `capdata-1.0.2.1/data/market.py` & `capdata-1.0.3.1/data/market.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import request.request as rq
 
 """
 获取历史行情数据
 参数:
     inst -- 产品编码列表 ['200310.IB', '190008.IB']
-    
+
     start -- 开始时间  2024-05-09
-    
+
     end -- 结束时间  2024-05-10
-    
+
     fields -- 需要返回的字段(open、close、high、low、pre_adj_close、post_adj_close、volume、turnover、num_trades、settlement、
     open_interest、bid、ask、bid_size、ask_size、trade、trade_size、level1、level2、level2_5、level2_10、lix)  ['bid','ask']
-    
+
     freq  -- 频率( 1m, 1d, 1w)
-    
+
     window -- 时间窗口 ['10:00:00','10:30:00']
-    
+
     mkt -- 市场
 """
 
 
-def get_hist_mkt(inst, start, end, fields,   window=None, mkt=None, freq="1d"):
+def get_hist_mkt(inst, start, end, fields, window=None, mkt=None, freq="1d"):
     data_json = {'inst': inst, 'start': start, 'end': end, 'freq': freq, 'window': window, 'mkt': mkt,
                  'fields': fields}
     return rq.post_token("/capdata/get/hist/mkt", data_json)
 
 
 """
 获取日内实时行情数据
 参数:
   inst -- 产品编码列表 ['200310.IB', '190008.IB']
-  
+
   fields -- 需要返回的字段(bid、ask、level1、level2、level2_5、level2_10、lix)  ['bid','ask']
-  
+
   mkt -- 市场   
 """
 
 
-def get_live_mkt(inst, fields,   mkt=""):
+def get_live_mkt(inst, fields, mkt=""):
     data_json = {'inst': inst, 'mkt': mkt, 'fields': fields}
     return rq.post_token("/capdata/get/live/mkt", data_json)
```

### Comparing `capdata-1.0.2.1/data/pricing.py` & `capdata-1.0.3.1/data/pricing.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import request.request as rq
 
 """
 获取产品定价数据
 参数:
     inst -- 产品编码列表 ['2292030.IB', '2292012.IB']
-    
+
     start -- 开始时间  2024-05-26
-    
+
     end -- 结束时间  2024-05-29
-    
+
     fields -- 需要返回的字段(price、duration、modified_duration、macaulay_duration、convexity、z_spread、dv01、bucket_dv01、cs01、
     bucket_cs01、delta、gamma、vega、term_bucket_vega、term_strike_bucket_vega、volga、term_bucket_volga、term_strike_bucket_volga、
     vanna、term_bucket_vanna、term_strike_bucket_vanna、rho)  ['duration','modified_duration']
-    
+
     freq  -- 频率( 1m, 1d, 1w)
-    
+
     window -- 时间窗口 ['10:00:00','10:30:00']
 """
 
 
 def get_pricing(inst, start, end, fields, window=None, mkt=None, freq="1d"):
     data_json = {'inst': inst, 'start': start, 'end': end, 'freq': freq, 'window': window, 'mkt': mkt,
                  'fields': fields}
     return rq.post_token("/capdata/get/pricing", data_json)
 
 
 """
 获取产品估值数据
 参数:
     inst -- 产品编码列表 ['2292030.IB', '2292012.IB']
-    
+
     start -- 开始时间  2024-05-26
-    
+
     end -- 结束时间  2024-05-29
-    
+
     fields -- 需要返回的字段(present_value、dv01、bucket_dv01、frtb_bucket_dv01、cs01、bucket_cs01、frtb_bucket_cs01、delta、frtb_delta、
      gamma、frtb_curvature、vega、term_bucket_vega、term_strike_bucket_vega、frtb_vega、volga、term_bucket_volga、term_strike_bucket_volga、
      vanna、term_bucket_vanna、term_strike_bucket_vanna、rho)  ['dv01','cs01']
-     
+
     freq  -- 频率( 1m, 1d, 1w)
-    
+
     window -- 时间窗口 ['10:00:00','10:30:00']
 """
 
 
 def get_valuation(inst, start, end, fields, window=None, mkt=None, freq="1d"):
     data_json = {'inst': inst, 'start': start, 'end': end, 'freq': freq, 'window': window, 'mkt': mkt,
                  'fields': fields}
```

### Comparing `capdata-1.0.2.1/data/refer.py` & `capdata-1.0.3.1/data/refer.py`

 * *Files identical despite different names*

### Comparing `capdata-1.0.2.1/data/risk.py` & `capdata-1.0.3.1/data/risk.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   curve -- 曲线编码  CN_TREAS_STD
   sim_date -- 情景时间  2024-05-28
   num_sims -- 情景数   200
   base_date -- 基础时间 2024-05-27
 """
 
 
-def get_hist_sim_ir_curve(curve, sim_date, base_date,   num_sims=200):
+def get_hist_sim_ir_curve(curve, sim_date, base_date, num_sims=200):
     data_json = {'curve': curve, 'simDate': sim_date, 'baseDate': base_date, 'numSims': num_sims}
     return rq.post_token("/capdata/get/hist/sim/ir/curve", data_json)
 
 
 """
 获取历史模拟的信用利差曲线数据
 参数:
@@ -36,60 +36,60 @@
   curve -- 曲线编码  CN_TREAS_STD
   sim_date -- 情景时间  2024-05-28
   num_sims -- 情景数   200
   base_date -- 基础时间 2024-05-27
 """
 
 
-def get_hist_stressed_ir_curve(curve, sim_date, base_date,  num_sims=200):
+def get_hist_stressed_ir_curve(curve, sim_date, base_date, num_sims=200):
     data_json = {'curve': curve, 'simDate': sim_date, 'baseDate': base_date, 'numSims': num_sims}
     return rq.post_token("/capdata/get/hist/stressed/ir/curve", data_json)
 
 
 """
 获取历史压力情景下信用利差曲线数据
 参数:
   curve -- 曲线编码  CN_CORP_AAA_SPRD_STD
   sim_date -- 情景时间  2024-05-28
   num_sims -- 情景数   200
   base_date -- 基础时间 2024-05-27
 """
 
 
-def get_hist_stressed_credit_curve(curve, sim_date, base_date,   num_sims=200):
+def get_hist_stressed_credit_curve(curve, sim_date, base_date, num_sims=200):
     data_json = {'curve': curve, 'simDate': sim_date, 'baseDate': base_date, 'numSims': num_sims}
     return rq.post_token("/capdata/get/hist/stressed/credit/curve", data_json)
 
 
 """
 获取产品模拟情景下损益数据
 参数:
   inst -- 产品编码  ['2171035.IB','2105288.IB']
   sim_date -- 情景时间  2024-05-28
   num_sims -- 情景数   200
   base_date -- 基础时间 2024-05-27
 """
 
 
-def get_inst_sim_pnl(inst, sim_date, base_date,   num_sims=200):
+def get_inst_sim_pnl(inst, sim_date, base_date, num_sims=200):
     data_json = {'inst': inst, 'simDate': sim_date, 'baseDate': base_date, 'numSims': num_sims}
     return rq.post_token("/capdata/get/inst/sim/pnl", data_json)
 
 
 """
 获取产品压力情景下损益数据
 参数:
   inst -- 产品编码  ['2171035.IB','2105288.IB']
   sim_date -- 情景时间  2024-05-28
   num_sims -- 情景数   200
   base_date -- 基础时间 2024-05-27
 """
 
 
-def get_inst_stressed_pnl(inst, sim_date, base_date,   num_sims=200):
+def get_inst_stressed_pnl(inst, sim_date, base_date, num_sims=200):
     data_json = {'inst': inst, 'simDate': sim_date, 'baseDate': base_date, 'numSims': num_sims}
     return rq.post_token("/capdata/get/inst/stressed/pnl", data_json)
 
 
 """
 获取产品Value-at-Risk数据
 参数:
```

### Comparing `capdata-1.0.2.1/request/request.py` & `capdata-1.0.3.1/request/request.py`

 * *Files identical despite different names*

### Comparing `capdata-1.0.2.1/setup.py` & `capdata-1.0.3.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 
 from sys import version_info
 
 from setuptools import setup, find_packages
 
-__version__ = '1.0.2.1'  # 版本号
+__version__ = '1.0.3.1'  # 版本号
 requirements = open('requirements.txt').readlines()  # 依赖文件
 
 if version_info < (3, 8, 0):
     raise SystemExit('Sorry! capdata requires python 3.8.0 or later.')
 
 setup(
     name='capdata',
-    description='capdata data api',
+    description='capdata  api',
     long_description='',
     license='',
     version=__version__,
     author='zbz',
     url='',
     packages=find_packages(exclude=["test"]),
     python_requires='>= 3.8.0',
```

### Comparing `capdata-1.0.2.1/test/test_curve.py` & `capdata-1.0.3.1/test/test_curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import unittest
 
 import data.curve as curve
 
-
 class TestCurveFunctions(unittest.TestCase):
     def test_get_bond_curve(self):
         curve_data = curve.get_bond_curve("CN_TREAS_STD", '2024-05-27 00:00:00', '2024-05-27 18:00:00', '1m')
         if curve_data is not None:
             for data in curve_data:
                 print(data)
         else:
```

### Comparing `capdata-1.0.2.1/test/test_market.py` & `capdata-1.0.3.1/test/test_market.py`

 * *Files identical despite different names*

### Comparing `capdata-1.0.2.1/test/test_pricing.py` & `capdata-1.0.3.1/test/test_pricing.py`

 * *Files identical despite different names*

### Comparing `capdata-1.0.2.1/test/test_refer.py` & `capdata-1.0.3.1/test/test_refer.py`

 * *Files identical despite different names*

### Comparing `capdata-1.0.2.1/test/test_risk.py` & `capdata-1.0.3.1/test/test_risk.py`

 * *Files identical despite different names*

