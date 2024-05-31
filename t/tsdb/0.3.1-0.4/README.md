# Comparing `tmp/tsdb-0.3.1.tar.gz` & `tmp/tsdb-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsdb-0.3.1.tar", last modified: Tue Jan 16 01:20:14 2024, max compression
+gzip compressed data, was "tsdb-0.4.tar", last modified: Fri May 31 03:49:02 2024, max compression
```

## Comparing `tsdb-0.3.1.tar` & `tsdb-0.4.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 01:20:14.976464 tsdb-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-01-16 01:19:51.000000 tsdb-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-16 01:19:51.000000 tsdb-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-01-16 01:20:14.976464 tsdb-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-01-16 01:19:51.000000 tsdb-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-16 01:20:14.976464 tsdb-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-01-16 01:19:51.000000 tsdb-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 01:20:14.976464 tsdb-0.3.1/tsdb/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-01-16 01:19:51.000000 tsdb-0.3.1/tsdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-16 01:19:51.000000 tsdb-0.3.1/tsdb/config.ini
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-01-16 01:19:51.000000 tsdb-0.3.1/tsdb/data_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-01-16 01:19:51.000000 tsdb-0.3.1/tsdb/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 01:20:14.976464 tsdb-0.3.1/tsdb/loading_funcs/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-01-16 01:19:51.000000 tsdb-0.3.1/tsdb/loading_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-01-16 01:19:51.000000 tsdb-0.3.1/tsdb/loading_funcs/beijing_multisite_air_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-01-16 01:19:51.000000 tsdb-0.3.1/tsdb/loading_funcs/electricity_load_diagrams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-01-16 01:19:51.000000 tsdb-0.3.1/tsdb/loading_funcs/electricity_transformer_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-01-16 01:19:51.000000 tsdb-0.3.1/tsdb/loading_funcs/physionet_2012.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-01-16 01:19:51.000000 tsdb-0.3.1/tsdb/loading_funcs/physionet_2019.py
--rw-r--r--   0 runner    (1001) docker     (127)     9280 2024-01-16 01:19:51.000000 tsdb-0.3.1/tsdb/loading_funcs/ucr_uea_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-01-16 01:19:51.000000 tsdb-0.3.1/tsdb/loading_funcs/vessel_ais.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 01:20:14.976464 tsdb-0.3.1/tsdb/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-16 01:19:51.000000 tsdb-0.3.1/tsdb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-01-16 01:19:51.000000 tsdb-0.3.1/tsdb/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-01-16 01:19:51.000000 tsdb-0.3.1/tsdb/utils/downloading.py
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-01-16 01:19:51.000000 tsdb-0.3.1/tsdb/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-01-16 01:19:51.000000 tsdb-0.3.1/tsdb/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 01:20:14.976464 tsdb-0.3.1/tsdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-01-16 01:20:14.000000 tsdb-0.3.1/tsdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-01-16 01:20:14.000000 tsdb-0.3.1/tsdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 01:20:14.000000 tsdb-0.3.1/tsdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-16 01:20:14.000000 tsdb-0.3.1/tsdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-16 01:20:14.000000 tsdb-0.3.1/tsdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:49:02.639728 tsdb-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-31 03:48:40.000000 tsdb-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-31 03:48:40.000000 tsdb-0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-05-31 03:49:02.639728 tsdb-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-05-31 03:48:40.000000 tsdb-0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-31 03:49:02.639728 tsdb-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-31 03:48:40.000000 tsdb-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:49:02.635728 tsdb-0.4/tsdb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/data_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:49:02.635728 tsdb-0.4/tsdb/loading_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/loading_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/loading_funcs/beijing_multisite_air_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/loading_funcs/electricity_load_diagrams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/loading_funcs/electricity_transformer_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/loading_funcs/italy_air_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/loading_funcs/physionet_2012.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/loading_funcs/physionet_2019.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9280 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/loading_funcs/ucr_uea_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/loading_funcs/vessel_ais.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:49:02.639728 tsdb-0.4/tsdb/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/utils/downloading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-31 03:48:40.000000 tsdb-0.4/tsdb/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:49:02.635728 tsdb-0.4/tsdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10373 2024-05-31 03:49:02.000000 tsdb-0.4/tsdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-31 03:49:02.000000 tsdb-0.4/tsdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 03:49:02.000000 tsdb-0.4/tsdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-31 03:49:02.000000 tsdb-0.4/tsdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 03:49:02.000000 tsdb-0.4/tsdb.egg-info/top_level.txt
```

### Comparing `tsdb-0.3.1/LICENSE` & `tsdb-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tsdb-0.3.1/PKG-INFO` & `tsdb-0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsdb
-Version: 0.3.1
+Version: 0.4
 Summary: TSDB (Time Series Data Beans): a Python toolbox helping load open-source time-series datasets
 Home-page: https://github.com/WenjieDu/TSDB
 Author: Wenjie Du
 Author-email: wenjay.du@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://tsdb.readthedocs.io/
 Project-URL: Source, https://github.com/WenjieDu/TSDB/
@@ -21,15 +21,15 @@
 Classifier: Topic :: Database
 Description-Content-Type: text/markdown
 Provides-Extra: basic
 License-File: LICENSE
 
 <a href='https://github.com/WenjieDu/TSDB'><img src="https://pypots.com/figs/pypots_logos/TSDB/logo_FFBG.svg" align='right' width='200'/></a>
 
-<h2 align="center">Welcome to TSDB</h2>
+<h3 align="center">Welcome to TSDB</h3>
 
 *<p align='center'>a Python toolbox to ease loading public time-series datasets</p>*
 
 <p align='center'>
     <a href='https://github.com/WenjieDu/TSDB'>
         <img alt='Python version' src='https://img.shields.io/badge/python-v3-E97040?logo=python&logoColor=white'>
     </a>
@@ -45,15 +45,15 @@
     <a href="https://github.com/WenjieDu/TSDB/graphs/contributors">
         <img alt="GitHub contributors" src="https://img.shields.io/github/contributors/wenjiedu/tsdb?color=D8E699&label=Contributors&logo=GitHub">
     </a>
     <a href="https://star-history.com/#wenjiedu/tsdb">
         <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/wenjiedu/tsdb?logo=None&color=6BB392&label=%E2%98%85%20Stars">
     </a>
     <a href="https://github.com/WenjieDu/TSDB/network/members">
-        <img alt="GitHub Repo forks" src="https://img.shields.io/github/forks/wenjiedu/pygrinder?logo=forgejo&logoColor=black&label=Forks">
+        <img alt="GitHub Repo forks" src="https://img.shields.io/github/forks/wenjiedu/tsdb?logo=forgejo&logoColor=black&label=Forks">
     </a>
     <a href="https://codeclimate.com/github/WenjieDu/TSDB">
         <img alt="Code Climate maintainability" src="https://img.shields.io/codeclimate/maintainability-percentage/WenjieDu/TSDB?color=3C7699&label=Maintainability&logo=codeclimate">
     </a>
     <a href='https://coveralls.io/github/WenjieDu/TSDB'>
         <img alt='Coveralls report' src='https://img.shields.io/coverallsCoverage/github/WenjieDu/TSDB?branch=main&logo=coveralls&color=75C1C4&label=Coverage'>
     </a>
@@ -67,15 +67,15 @@
         <img alt="Conda downloads" src="https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/conda_tsdb_downloads.json">
     </a>
     <a href='https://pepy.tech/project/tsdb'>
         <img alt='PyPI downloads' src='https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/pypi_tsdb_downloads.json'>
     </a>
 </p>
 
-> 📣 TSDB now supports a total of 1️⃣6️⃣9️⃣ time-series datasets ‼️
+> 📣 TSDB now supports a total of 1️⃣7️⃣0️⃣ time-series datasets ‼️
 
 <a href='https://github.com/WenjieDu/PyPOTS'><img src='https://pypots.com/figs/pypots_logos/PyPOTS/logo_FFBG.svg' width='160' align='left' /></a>
 TSDB is a part of
 <a href="https://github.com/WenjieDu/PyPOTS">
 PyPOTS <img align="center" src="https://img.shields.io/github/stars/WenjieDu/PyPOTS?style=social">
 </a>
 (a Python toolbox for data mining on Partially-Observed Time Series), and was separated from PyPOTS for decoupling datasets from learning algorithms.
@@ -92,25 +92,25 @@
 
 
 ## ❖ Usage Examples
 TSDB now is available on <a alt='Anaconda' href='https://anaconda.org/conda-forge/tsdb'><img align='center' src='https://img.shields.io/badge/Anaconda--lightgreen?style=social&logo=anaconda'></a>❗️
 
 Install it with `conda install tsdb `, you may need to specify the channel with option `-c conda-forge`
 
-or install from PyPI:
+or install via PyPI:
 > pip install tsdb
 
 or install from source code:
 > pip install `https://github.com/WenjieDu/TSDB/archive/main.zip`
 
 ```python
 import tsdb
 
 # list all available datasets in TSDB
-tsdb.list_available_datasets()
+tsdb.list()
 # select the dataset you need and load it, TSDB will download, extract, and process it automatically
 data = tsdb.load('physionet_2012')
 # if you need the raw data, use download_and_extract()
 tsdb.download_and_extract('physionet_2012', './save_it_here')
 # datasets you once loaded are cached, and you can check them with list_cached_data()
 tsdb.list_cache()
 # you can delete only one specific dataset and preserve others
@@ -129,28 +129,35 @@
 ## ❖ List of Available Datasets
 
 | Name                                                                                              | Main Tasks                              |
 |---------------------------------------------------------------------------------------------------|-----------------------------------------|
 | [PhysioNet Challenge 2012](dataset_profiles/physionet_2012)                                       | Forecasting, Imputation, Classification |
 | [PhysioNet Challenge 2019](dataset_profiles/physionet_2019)                                       | Forecasting, Imputation, Classification |
 | [Beijing Multi-Site Air-Quality](dataset_profiles/beijing_multisite_air_quality)                  | Forecasting, Imputation                 |
+| [Italy Air Quality](dataset_profiles/italy_air_quality)                                           | Forecasting, Imputation                 |
 | [Electricity Load Diagrams](dataset_profiles/electricity_load_diagrams)                           | Forecasting, Imputation                 |
 | [Electricity Transformer Temperature (ETT)](dataset_profiles/electricity_transformer_temperature) | Forecasting, Imputation                 |
 | [Vessel AIS](dataset_profiles/vessel_ais)                                                         | Forecasting, Imputation, Classification |
 | [UCR & UEA Datasets](dataset_profiles/ucr_uea_datasets) (all 163 datasets)                        | Classification                          |
 
 
 ## ❖ Citing TSDB/PyPOTS
 The paper introducing PyPOTS project is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
 and we are pursuing to publish it in prestigious academic venues, e.g. JMLR (track for
 [Machine Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use TSDB in your work,
 please cite PyPOTS project as below and 🌟star this repository to make others notice this library. 🤗 Thank you!
 
+<p align="center">
+<a href="https://github.com/WenjieDu/PyPOTS">
+    <img src="https://pypots.com/figs/pypots_logos/Ecosystem/PyPOTS_Ecosystem_Pipeline.png" width="95%"/>
+</a>
+</p>
+
 ``` bibtex
-@article{du2023PyPOTS,
+@article{du2023pypots,
 title={{PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series}},
 author={Wenjie Du},
 year={2023},
 eprint={2305.18811},
 archivePrefix={arXiv},
 primaryClass={cs.LG},
 url={https://arxiv.org/abs/2305.18811},
@@ -158,28 +165,13 @@
 }
 ```
 
 > Wenjie Du. (2023).
 > PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series.
 > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811
 
-or
-
-``` bibtex
-@inproceedings{du2023PyPOTS,
-title={{PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series}},
-booktitle={9th SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)},
-author={Wenjie Du},
-year={2023},
-url={https://arxiv.org/abs/2305.18811},
-}
-```
-
-> Wenjie Du. (2023).
-> PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series.
-> In *9th SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)*. https://arxiv.org/abs/2305.18811
 
 
 <details>
 <summary>🏠 Visits</summary>
 <img align='left' src='https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FWenjieDu%2FTime_Series_Database&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+April+2022&edge_flat=false'>
 </details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsdb Version: 0.3.1 Summary: TSDB (Time Series Data
+Metadata-Version: 2.1 Name: tsdb Version: 0.4 Summary: TSDB (Time Series Data
 Beans): a Python toolbox helping load open-source time-series datasets Home-
 page: https://github.com/WenjieDu/TSDB Author: Wenjie Du Author-email:
 wenjay.du@gmail.com License: BSD-3-Clause Project-URL: Documentation, https://
 tsdb.readthedocs.io/ Project-URL: Source, https://github.com/WenjieDu/TSDB/
 Project-URL: Tracker, https://github.com/WenjieDu/TSDB/issues/ Project-URL:
 Download, https://github.com/WenjieDu/TSDB/archive/main.zip Keywords: data
 mining,time series,time-series analysis,time-series database,time-series
@@ -13,23 +13,23 @@
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: BSD License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Topic :: Database Description-Content-Type: text/markdown
 Provides-Extra: basic License-File: LICENSE_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/
 _p_y_p_o_t_s___l_o_g_o_s_/_T_S_D_B_/_l_o_g_o___F_F_B_G_._s_v_g_]
-                          ********** WWeellccoommee ttoo TTSSDDBB **********
+                           ******** WWeellccoommee ttoo TTSSDDBB ********
 *
          a Python toolbox to ease loading public time-series datasets
 *
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_t_h_e_ _l_a_t_e_s_t_ _r_e_l_e_a_s_e_ _v_e_r_s_i_o_n_]_[_B_S_D_-_3_ _l_i_c_e_n_s_e_]_[_C_o_m_m_u_n_i_t_y_]_[_G_i_t_H_u_b
        _c_o_n_t_r_i_b_u_t_o_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _f_o_r_k_s_]_[_C_o_d_e_ _C_l_i_m_a_t_e
 _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_C_o_v_e_r_a_l_l_s_ _r_e_p_o_r_t_]_[_G_i_t_H_u_b_ _T_e_s_t_i_n_g_]_[_a_r_X_i_v_ _D_O_I_]_[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]
                                _[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]
-> ð£ TSDB now supports a total of 1ï¸â£6ï¸â£9ï¸â£ time-series datasets
+> ð£ TSDB now supports a total of 1ï¸â£7ï¸â£0ï¸â£ time-series datasets
 â¼ï¸ _[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]TSDB is a
 part of _P_y_P_O_T_S_ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_W_e_n_j_i_e_D_u_/
 _P_y_P_O_T_S_?_s_t_y_l_e_=_s_o_c_i_a_l_](a Python toolbox for data mining on Partially-Observed
 Time Series), and was separated from PyPOTS for decoupling datasets from
 learning algorithms. TSDB is created to help researchers and engineers get rid
 of data collecting and downloading, and focus back on data processing details.
 TSDB provides all-in-one-stop convenience for downloading and loading open-
@@ -47,54 +47,49 @@
 notice TSDB if you think it is a useful toolkit. **Please** properly [cite TSDB
 and PyPOTS](https://github.com/WenjieDu/TSDB#-citing-tsdbpypots) in your
 publications if it helps with your research. This really means a lot to our
 open-source research. Thank you! ## â Usage Examples TSDB now is available on
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_n_a_c_o_n_d_a_-_-
 _l_i_g_h_t_g_r_e_e_n_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_o_g_o_=_a_n_a_c_o_n_d_a_]âï¸ Install it with `conda install
 tsdb `, you may need to specify the channel with option `-c conda-forge` or
-install from PyPI: > pip install tsdb or install from source code: > pip
-install `https://github.com/WenjieDu/TSDB/archive/main.zip` ```python import
-tsdb # list all available datasets in TSDB tsdb.list_available_datasets() #
-select the dataset you need and load it, TSDB will download, extract, and
-process it automatically data = tsdb.load('physionet_2012') # if you need the
-raw data, use download_and_extract() tsdb.download_and_extract
-('physionet_2012', './save_it_here') # datasets you once loaded are cached, and
-you can check them with list_cached_data() tsdb.list_cache() # you can delete
-only one specific dataset and preserve others tsdb.delete_cache
-(dataset_name='physionet_2012') # or you can delete all cache with
-delete_cached_data() to free disk space tsdb.delete_cache() # to avoid taking
-up too much space if downloading many datasets, # TSDB cache directory can be
-migrated to an external disk tsdb.migrate_cache("/mnt/external_disk/
-TSDB_cache") ``` That's all. Simple and efficient. Enjoy it! ð ## â List
-of Available Datasets | Name | Main Tasks | |----------------------------------
------------------------------------------------------------------|-------------
-----------------------------| | [PhysioNet Challenge 2012](dataset_profiles/
-physionet_2012) | Forecasting, Imputation, Classification | | [PhysioNet
-Challenge 2019](dataset_profiles/physionet_2019) | Forecasting, Imputation,
-Classification | | [Beijing Multi-Site Air-Quality](dataset_profiles/
-beijing_multisite_air_quality) | Forecasting, Imputation | | [Electricity Load
-Diagrams](dataset_profiles/electricity_load_diagrams) | Forecasting, Imputation
-| | [Electricity Transformer Temperature (ETT)](dataset_profiles/
+install via PyPI: > pip install tsdb or install from source code: > pip install
+`https://github.com/WenjieDu/TSDB/archive/main.zip` ```python import tsdb #
+list all available datasets in TSDB tsdb.list() # select the dataset you need
+and load it, TSDB will download, extract, and process it automatically data =
+tsdb.load('physionet_2012') # if you need the raw data, use
+download_and_extract() tsdb.download_and_extract('physionet_2012', './
+save_it_here') # datasets you once loaded are cached, and you can check them
+with list_cached_data() tsdb.list_cache() # you can delete only one specific
+dataset and preserve others tsdb.delete_cache(dataset_name='physionet_2012') #
+or you can delete all cache with delete_cached_data() to free disk space
+tsdb.delete_cache() # to avoid taking up too much space if downloading many
+datasets, # TSDB cache directory can be migrated to an external disk
+tsdb.migrate_cache("/mnt/external_disk/TSDB_cache") ``` That's all. Simple and
+efficient. Enjoy it! ð ## â List of Available Datasets | Name | Main Tasks
+| |----------------------------------------------------------------------------
+-----------------------|-----------------------------------------| | [PhysioNet
+Challenge 2012](dataset_profiles/physionet_2012) | Forecasting, Imputation,
+Classification | | [PhysioNet Challenge 2019](dataset_profiles/physionet_2019)
+| Forecasting, Imputation, Classification | | [Beijing Multi-Site Air-Quality]
+(dataset_profiles/beijing_multisite_air_quality) | Forecasting, Imputation | |
+[Italy Air Quality](dataset_profiles/italy_air_quality) | Forecasting,
+Imputation | | [Electricity Load Diagrams](dataset_profiles/
+electricity_load_diagrams) | Forecasting, Imputation | | [Electricity
+Transformer Temperature (ETT)](dataset_profiles/
 electricity_transformer_temperature) | Forecasting, Imputation | | [Vessel AIS]
 (dataset_profiles/vessel_ais) | Forecasting, Imputation, Classification | |
 [UCR & UEA Datasets](dataset_profiles/ucr_uea_datasets) (all 163 datasets) |
 Classification | ## â Citing TSDB/PyPOTS The paper introducing PyPOTS project
 is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811), and we
 are pursuing to publish it in prestigious academic venues, e.g. JMLR (track for
 [Machine Learning Open Source Software](https://www.jmlr.org/mloss/)). If you
 use TSDB in your work, please cite PyPOTS project as below and ðstar this
-repository to make others notice this library. ð¤ Thank you! ``` bibtex
-@article{du2023PyPOTS, title={{PyPOTS: a Python toolbox for data mining on
-Partially-Observed Time Series}}, author={Wenjie Du}, year={2023}, eprint=
-{2305.18811}, archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://
+repository to make others notice this library. ð¤ Thank you!
+_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_E_c_o_s_y_s_t_e_m_/_P_y_P_O_T_S___E_c_o_s_y_s_t_e_m___P_i_p_e_l_i_n_e_._p_n_g_]
+``` bibtex @article{du2023pypots, title={{PyPOTS: a Python toolbox for data
+mining on Partially-Observed Time Series}}, author={Wenjie Du}, year={2023},
+eprint={2305.18811}, archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://
 arxiv.org/abs/2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` > Wenjie Du.
 (2023). > PyPOTS: a Python toolbox for data mining on Partially-Observed Time
-Series. > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 or ``` bibtex
-@inproceedings{du2023PyPOTS, title={{PyPOTS: a Python toolbox for data mining
-on Partially-Observed Time Series}}, booktitle={9th SIGKDD workshop on Mining
-and Learning from Time Series (MiLeTS'23)}, author={Wenjie Du}, year={2023},
-url={https://arxiv.org/abs/2305.18811}, } ``` > Wenjie Du. (2023). > PyPOTS: a
-Python toolbox for data mining on Partially-Observed Time Series. > In *9th
-SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)*. https://
-arxiv.org/abs/2305.18811 ð  Visits[https://hits.seeyoufarm.com/api/count/
-incr/
+Series. > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 ð  Visits
+[https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FWenjieDu%2FTime_Series_Database&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+April+2022&edge_flat=false]
```

### Comparing `tsdb-0.3.1/README.md` & `tsdb-0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <a href='https://github.com/WenjieDu/TSDB'><img src="https://pypots.com/figs/pypots_logos/TSDB/logo_FFBG.svg" align='right' width='200'/></a>
 
-<h2 align="center">Welcome to TSDB</h2>
+<h3 align="center">Welcome to TSDB</h3>
 
 *<p align='center'>a Python toolbox to ease loading public time-series datasets</p>*
 
 <p align='center'>
     <a href='https://github.com/WenjieDu/TSDB'>
         <img alt='Python version' src='https://img.shields.io/badge/python-v3-E97040?logo=python&logoColor=white'>
     </a>
@@ -20,15 +20,15 @@
     <a href="https://github.com/WenjieDu/TSDB/graphs/contributors">
         <img alt="GitHub contributors" src="https://img.shields.io/github/contributors/wenjiedu/tsdb?color=D8E699&label=Contributors&logo=GitHub">
     </a>
     <a href="https://star-history.com/#wenjiedu/tsdb">
         <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/wenjiedu/tsdb?logo=None&color=6BB392&label=%E2%98%85%20Stars">
     </a>
     <a href="https://github.com/WenjieDu/TSDB/network/members">
-        <img alt="GitHub Repo forks" src="https://img.shields.io/github/forks/wenjiedu/pygrinder?logo=forgejo&logoColor=black&label=Forks">
+        <img alt="GitHub Repo forks" src="https://img.shields.io/github/forks/wenjiedu/tsdb?logo=forgejo&logoColor=black&label=Forks">
     </a>
     <a href="https://codeclimate.com/github/WenjieDu/TSDB">
         <img alt="Code Climate maintainability" src="https://img.shields.io/codeclimate/maintainability-percentage/WenjieDu/TSDB?color=3C7699&label=Maintainability&logo=codeclimate">
     </a>
     <a href='https://coveralls.io/github/WenjieDu/TSDB'>
         <img alt='Coveralls report' src='https://img.shields.io/coverallsCoverage/github/WenjieDu/TSDB?branch=main&logo=coveralls&color=75C1C4&label=Coverage'>
     </a>
@@ -42,15 +42,15 @@
         <img alt="Conda downloads" src="https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/conda_tsdb_downloads.json">
     </a>
     <a href='https://pepy.tech/project/tsdb'>
         <img alt='PyPI downloads' src='https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/pypi_tsdb_downloads.json'>
     </a>
 </p>
 
-> 📣 TSDB now supports a total of 1️⃣6️⃣9️⃣ time-series datasets ‼️
+> 📣 TSDB now supports a total of 1️⃣7️⃣0️⃣ time-series datasets ‼️
 
 <a href='https://github.com/WenjieDu/PyPOTS'><img src='https://pypots.com/figs/pypots_logos/PyPOTS/logo_FFBG.svg' width='160' align='left' /></a>
 TSDB is a part of
 <a href="https://github.com/WenjieDu/PyPOTS">
 PyPOTS <img align="center" src="https://img.shields.io/github/stars/WenjieDu/PyPOTS?style=social">
 </a>
 (a Python toolbox for data mining on Partially-Observed Time Series), and was separated from PyPOTS for decoupling datasets from learning algorithms.
@@ -67,25 +67,25 @@
 
 
 ## ❖ Usage Examples
 TSDB now is available on <a alt='Anaconda' href='https://anaconda.org/conda-forge/tsdb'><img align='center' src='https://img.shields.io/badge/Anaconda--lightgreen?style=social&logo=anaconda'></a>❗️
 
 Install it with `conda install tsdb `, you may need to specify the channel with option `-c conda-forge`
 
-or install from PyPI:
+or install via PyPI:
 > pip install tsdb
 
 or install from source code:
 > pip install `https://github.com/WenjieDu/TSDB/archive/main.zip`
 
 ```python
 import tsdb
 
 # list all available datasets in TSDB
-tsdb.list_available_datasets()
+tsdb.list()
 # select the dataset you need and load it, TSDB will download, extract, and process it automatically
 data = tsdb.load('physionet_2012')
 # if you need the raw data, use download_and_extract()
 tsdb.download_and_extract('physionet_2012', './save_it_here')
 # datasets you once loaded are cached, and you can check them with list_cached_data()
 tsdb.list_cache()
 # you can delete only one specific dataset and preserve others
@@ -104,28 +104,35 @@
 ## ❖ List of Available Datasets
 
 | Name                                                                                              | Main Tasks                              |
 |---------------------------------------------------------------------------------------------------|-----------------------------------------|
 | [PhysioNet Challenge 2012](dataset_profiles/physionet_2012)                                       | Forecasting, Imputation, Classification |
 | [PhysioNet Challenge 2019](dataset_profiles/physionet_2019)                                       | Forecasting, Imputation, Classification |
 | [Beijing Multi-Site Air-Quality](dataset_profiles/beijing_multisite_air_quality)                  | Forecasting, Imputation                 |
+| [Italy Air Quality](dataset_profiles/italy_air_quality)                                           | Forecasting, Imputation                 |
 | [Electricity Load Diagrams](dataset_profiles/electricity_load_diagrams)                           | Forecasting, Imputation                 |
 | [Electricity Transformer Temperature (ETT)](dataset_profiles/electricity_transformer_temperature) | Forecasting, Imputation                 |
 | [Vessel AIS](dataset_profiles/vessel_ais)                                                         | Forecasting, Imputation, Classification |
 | [UCR & UEA Datasets](dataset_profiles/ucr_uea_datasets) (all 163 datasets)                        | Classification                          |
 
 
 ## ❖ Citing TSDB/PyPOTS
 The paper introducing PyPOTS project is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
 and we are pursuing to publish it in prestigious academic venues, e.g. JMLR (track for
 [Machine Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use TSDB in your work,
 please cite PyPOTS project as below and 🌟star this repository to make others notice this library. 🤗 Thank you!
 
+<p align="center">
+<a href="https://github.com/WenjieDu/PyPOTS">
+    <img src="https://pypots.com/figs/pypots_logos/Ecosystem/PyPOTS_Ecosystem_Pipeline.png" width="95%"/>
+</a>
+</p>
+
 ``` bibtex
-@article{du2023PyPOTS,
+@article{du2023pypots,
 title={{PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series}},
 author={Wenjie Du},
 year={2023},
 eprint={2305.18811},
 archivePrefix={arXiv},
 primaryClass={cs.LG},
 url={https://arxiv.org/abs/2305.18811},
@@ -133,28 +140,13 @@
 }
 ```
 
 > Wenjie Du. (2023).
 > PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series.
 > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811
 
-or
-
-``` bibtex
-@inproceedings{du2023PyPOTS,
-title={{PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series}},
-booktitle={9th SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)},
-author={Wenjie Du},
-year={2023},
-url={https://arxiv.org/abs/2305.18811},
-}
-```
-
-> Wenjie Du. (2023).
-> PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series.
-> In *9th SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)*. https://arxiv.org/abs/2305.18811
 
 
 <details>
 <summary>🏠 Visits</summary>
 <img align='left' src='https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FWenjieDu%2FTime_Series_Database&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+April+2022&edge_flat=false'>
 </details>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
 _[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_T_S_D_B_/_l_o_g_o___F_F_B_G_._s_v_g_]
-                          ********** WWeellccoommee ttoo TTSSDDBB **********
+                           ******** WWeellccoommee ttoo TTSSDDBB ********
 *
          a Python toolbox to ease loading public time-series datasets
 *
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_t_h_e_ _l_a_t_e_s_t_ _r_e_l_e_a_s_e_ _v_e_r_s_i_o_n_]_[_B_S_D_-_3_ _l_i_c_e_n_s_e_]_[_C_o_m_m_u_n_i_t_y_]_[_G_i_t_H_u_b
        _c_o_n_t_r_i_b_u_t_o_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _f_o_r_k_s_]_[_C_o_d_e_ _C_l_i_m_a_t_e
 _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_C_o_v_e_r_a_l_l_s_ _r_e_p_o_r_t_]_[_G_i_t_H_u_b_ _T_e_s_t_i_n_g_]_[_a_r_X_i_v_ _D_O_I_]_[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]
                                _[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]
-> ð£ TSDB now supports a total of 1ï¸â£6ï¸â£9ï¸â£ time-series datasets
+> ð£ TSDB now supports a total of 1ï¸â£7ï¸â£0ï¸â£ time-series datasets
 â¼ï¸ _[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]TSDB is a
 part of _P_y_P_O_T_S_ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_W_e_n_j_i_e_D_u_/
 _P_y_P_O_T_S_?_s_t_y_l_e_=_s_o_c_i_a_l_](a Python toolbox for data mining on Partially-Observed
 Time Series), and was separated from PyPOTS for decoupling datasets from
 learning algorithms. TSDB is created to help researchers and engineers get rid
 of data collecting and downloading, and focus back on data processing details.
 TSDB provides all-in-one-stop convenience for downloading and loading open-
@@ -29,54 +29,49 @@
 notice TSDB if you think it is a useful toolkit. **Please** properly [cite TSDB
 and PyPOTS](https://github.com/WenjieDu/TSDB#-citing-tsdbpypots) in your
 publications if it helps with your research. This really means a lot to our
 open-source research. Thank you! ## â Usage Examples TSDB now is available on
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_n_a_c_o_n_d_a_-_-
 _l_i_g_h_t_g_r_e_e_n_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_o_g_o_=_a_n_a_c_o_n_d_a_]âï¸ Install it with `conda install
 tsdb `, you may need to specify the channel with option `-c conda-forge` or
-install from PyPI: > pip install tsdb or install from source code: > pip
-install `https://github.com/WenjieDu/TSDB/archive/main.zip` ```python import
-tsdb # list all available datasets in TSDB tsdb.list_available_datasets() #
-select the dataset you need and load it, TSDB will download, extract, and
-process it automatically data = tsdb.load('physionet_2012') # if you need the
-raw data, use download_and_extract() tsdb.download_and_extract
-('physionet_2012', './save_it_here') # datasets you once loaded are cached, and
-you can check them with list_cached_data() tsdb.list_cache() # you can delete
-only one specific dataset and preserve others tsdb.delete_cache
-(dataset_name='physionet_2012') # or you can delete all cache with
-delete_cached_data() to free disk space tsdb.delete_cache() # to avoid taking
-up too much space if downloading many datasets, # TSDB cache directory can be
-migrated to an external disk tsdb.migrate_cache("/mnt/external_disk/
-TSDB_cache") ``` That's all. Simple and efficient. Enjoy it! ð ## â List
-of Available Datasets | Name | Main Tasks | |----------------------------------
------------------------------------------------------------------|-------------
-----------------------------| | [PhysioNet Challenge 2012](dataset_profiles/
-physionet_2012) | Forecasting, Imputation, Classification | | [PhysioNet
-Challenge 2019](dataset_profiles/physionet_2019) | Forecasting, Imputation,
-Classification | | [Beijing Multi-Site Air-Quality](dataset_profiles/
-beijing_multisite_air_quality) | Forecasting, Imputation | | [Electricity Load
-Diagrams](dataset_profiles/electricity_load_diagrams) | Forecasting, Imputation
-| | [Electricity Transformer Temperature (ETT)](dataset_profiles/
+install via PyPI: > pip install tsdb or install from source code: > pip install
+`https://github.com/WenjieDu/TSDB/archive/main.zip` ```python import tsdb #
+list all available datasets in TSDB tsdb.list() # select the dataset you need
+and load it, TSDB will download, extract, and process it automatically data =
+tsdb.load('physionet_2012') # if you need the raw data, use
+download_and_extract() tsdb.download_and_extract('physionet_2012', './
+save_it_here') # datasets you once loaded are cached, and you can check them
+with list_cached_data() tsdb.list_cache() # you can delete only one specific
+dataset and preserve others tsdb.delete_cache(dataset_name='physionet_2012') #
+or you can delete all cache with delete_cached_data() to free disk space
+tsdb.delete_cache() # to avoid taking up too much space if downloading many
+datasets, # TSDB cache directory can be migrated to an external disk
+tsdb.migrate_cache("/mnt/external_disk/TSDB_cache") ``` That's all. Simple and
+efficient. Enjoy it! ð ## â List of Available Datasets | Name | Main Tasks
+| |----------------------------------------------------------------------------
+-----------------------|-----------------------------------------| | [PhysioNet
+Challenge 2012](dataset_profiles/physionet_2012) | Forecasting, Imputation,
+Classification | | [PhysioNet Challenge 2019](dataset_profiles/physionet_2019)
+| Forecasting, Imputation, Classification | | [Beijing Multi-Site Air-Quality]
+(dataset_profiles/beijing_multisite_air_quality) | Forecasting, Imputation | |
+[Italy Air Quality](dataset_profiles/italy_air_quality) | Forecasting,
+Imputation | | [Electricity Load Diagrams](dataset_profiles/
+electricity_load_diagrams) | Forecasting, Imputation | | [Electricity
+Transformer Temperature (ETT)](dataset_profiles/
 electricity_transformer_temperature) | Forecasting, Imputation | | [Vessel AIS]
 (dataset_profiles/vessel_ais) | Forecasting, Imputation, Classification | |
 [UCR & UEA Datasets](dataset_profiles/ucr_uea_datasets) (all 163 datasets) |
 Classification | ## â Citing TSDB/PyPOTS The paper introducing PyPOTS project
 is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811), and we
 are pursuing to publish it in prestigious academic venues, e.g. JMLR (track for
 [Machine Learning Open Source Software](https://www.jmlr.org/mloss/)). If you
 use TSDB in your work, please cite PyPOTS project as below and ðstar this
-repository to make others notice this library. ð¤ Thank you! ``` bibtex
-@article{du2023PyPOTS, title={{PyPOTS: a Python toolbox for data mining on
-Partially-Observed Time Series}}, author={Wenjie Du}, year={2023}, eprint=
-{2305.18811}, archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://
+repository to make others notice this library. ð¤ Thank you!
+_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_E_c_o_s_y_s_t_e_m_/_P_y_P_O_T_S___E_c_o_s_y_s_t_e_m___P_i_p_e_l_i_n_e_._p_n_g_]
+``` bibtex @article{du2023pypots, title={{PyPOTS: a Python toolbox for data
+mining on Partially-Observed Time Series}}, author={Wenjie Du}, year={2023},
+eprint={2305.18811}, archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://
 arxiv.org/abs/2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` > Wenjie Du.
 (2023). > PyPOTS: a Python toolbox for data mining on Partially-Observed Time
-Series. > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 or ``` bibtex
-@inproceedings{du2023PyPOTS, title={{PyPOTS: a Python toolbox for data mining
-on Partially-Observed Time Series}}, booktitle={9th SIGKDD workshop on Mining
-and Learning from Time Series (MiLeTS'23)}, author={Wenjie Du}, year={2023},
-url={https://arxiv.org/abs/2305.18811}, } ``` > Wenjie Du. (2023). > PyPOTS: a
-Python toolbox for data mining on Partially-Observed Time Series. > In *9th
-SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)*. https://
-arxiv.org/abs/2305.18811 ð  Visits[https://hits.seeyoufarm.com/api/count/
-incr/
+Series. > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 ð  Visits
+[https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FWenjieDu%2FTime_Series_Database&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+April+2022&edge_flat=false]
```

### Comparing `tsdb-0.3.1/setup.py` & `tsdb-0.4/setup.py`

 * *Files identical despite different names*

### Comparing `tsdb-0.3.1/tsdb/__init__.py` & `tsdb-0.4/tsdb/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # X.YaN # Alpha release
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
-__version__ = "0.3.1"
+__version__ = "0.4"
 
 from .data_processing import (
     CACHED_DATASET_DIR,
     list,
     load,
     download_and_extract,
     list_cache,
```

### Comparing `tsdb-0.3.1/tsdb/data_processing.py` & `tsdb-0.4/tsdb/data_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     load_physionet2012,
     load_physionet2019,
     load_electricity,
     load_ett,
     load_beijing_air_quality,
     load_ucr_uea_dataset,
     load_ais,
+    load_italy_air_quality,
 )
 from .utils.downloading import download_and_extract
 from .utils.file import purge_path, pickle_load, pickle_dump, determine_data_home
 from .utils.logging import logger
 
 CACHED_DATASET_DIR = determine_data_home()
 
@@ -96,14 +97,16 @@
                 result = load_physionet2019(dataset_saving_path)
             elif dataset_name == "electricity_load_diagrams":
                 result = load_electricity(dataset_saving_path)
             elif dataset_name == "electricity_transformer_temperature":
                 result = load_ett(dataset_saving_path)
             elif dataset_name == "beijing_multisite_air_quality":
                 result = load_beijing_air_quality(dataset_saving_path)
+            elif dataset_name == "italy_air_quality":
+                result = load_italy_air_quality(dataset_saving_path)
             elif dataset_name == "vessel_ais":
                 result = load_ais(dataset_saving_path)
             elif "ucr_uea_" in dataset_name:
                 actual_dataset_name = dataset_name.replace(
                     "ucr_uea_", ""
                 )  # delete 'ucr_uea_' in the name
                 result = load_ucr_uea_dataset(dataset_saving_path, actual_dataset_name)
```

### Comparing `tsdb-0.3.1/tsdb/database.py` & `tsdb-0.4/tsdb/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     #
     # https://github.com/WenjieDu/TSDB/tree/main/dataset_profiles/electricity_load_diagrams
     "electricity_load_diagrams": "https://archive.ics.uci.edu/ml/machine-learning-databases/00321/LD2011_2014.txt.zip",
     #
     # https://github.com/WenjieDu/TSDB/tree/main/dataset_profiles/beijing_multisite_air_quality
     "beijing_multisite_air_quality": "https://archive.ics.uci.edu/ml/machine-learning-databases/00501/"
     "PRSA2017_Data_20130301-20170228.zip",
+    # https://github.com/WenjieDu/TSDB/tree/main/dataset_profiles/italy_air_quality
+    "italy_air_quality": "https://archive.ics.uci.edu/static/public/360/air+quality.zip",
     #
     # https://github.com/WenjieDu/TSDB/tree/main/dataset_profiles/vessel_ais
     "vessel_ais": "https://zenodo.org/record/8064564/files/parquets.zip",
     #
     # https://github.com/WenjieDu/TSDB/tree/main/dataset_profiles/electricity_transformer_temperature
     "electricity_transformer_temperature": [
         "https://raw.githubusercontent.com/zhouhaoyi/ETDataset/main/ETT-small/ETTm1.csv",
```

### Comparing `tsdb-0.3.1/tsdb/loading_funcs/__init__.py` & `tsdb-0.4/tsdb/loading_funcs/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: BSD-3-Clause
 
 from .beijing_multisite_air_quality import load_beijing_air_quality
 from .electricity_load_diagrams import load_electricity
+from .electricity_transformer_temperature import load_ett
+from .italy_air_quality import load_italy_air_quality
 from .physionet_2012 import load_physionet2012
 from .physionet_2019 import load_physionet2019
 from .ucr_uea_datasets import load_ucr_uea_dataset
 from .vessel_ais import load_ais
-from .electricity_transformer_temperature import load_ett
 
 __all__ = [
     "load_beijing_air_quality",
     "load_electricity",
     "load_physionet2012",
     "load_physionet2019",
     "load_ucr_uea_dataset",
     "load_ais",
     "load_ett",
+    "load_italy_air_quality",
 ]
```

### Comparing `tsdb-0.3.1/tsdb/loading_funcs/beijing_multisite_air_quality.py` & `tsdb-0.4/tsdb/loading_funcs/beijing_multisite_air_quality.py`

 * *Files identical despite different names*

### Comparing `tsdb-0.3.1/tsdb/loading_funcs/electricity_load_diagrams.py` & `tsdb-0.4/tsdb/loading_funcs/electricity_load_diagrams.py`

 * *Files identical despite different names*

### Comparing `tsdb-0.3.1/tsdb/loading_funcs/electricity_transformer_temperature.py` & `tsdb-0.4/tsdb/loading_funcs/electricity_transformer_temperature.py`

 * *Files identical despite different names*

### Comparing `tsdb-0.3.1/tsdb/loading_funcs/physionet_2012.py` & `tsdb-0.4/tsdb/loading_funcs/physionet_2012.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,20 +52,19 @@
         with open(outcome_file_path, "r") as f:
             outcome = pd.read_csv(f)[["In-hospital_death", "RecordID"]]
         outcome["RecordID"] = outcome["RecordID"].astype(
             int
         )  # ensure RecordID's type is int
         outcome = outcome.set_index("RecordID")
         outcome_collector.append(outcome)
-    y = pd.concat(outcome_collector)
-
-    df_collector = []
 
     # iterate over all samples
+    set_collector = []
     for m_ in time_series_measurements_dir:
+        df_collector = []
         raw_data_dir = os.path.join(local_path, m_)
         for filename in os.listdir(raw_data_dir):
             recordID = int(filename.split(".txt")[0])
             with open(os.path.join(raw_data_dir, filename), "r") as f:
                 df_temp = pd.read_csv(f)
             df_temp["Time"] = df_temp["Time"].apply(lambda x: int(x.split(":")[0]))
             df_temp = df_temp.pivot_table("Value", "Time", "Parameter")
@@ -76,15 +75,20 @@
                 )
                 continue
 
             df_temp["RecordID"] = recordID
             df_temp["Age"] = df_temp.loc[0, "Age"]
             df_temp["Height"] = df_temp.loc[0, "Height"]
             df_collector.append(df_temp)
+        df = pd.concat(df_collector, sort=True)
+        set_collector.append(df)
 
-    df = pd.concat(df_collector, sort=True)
-    X = df.reset_index(drop=True)
-    unique_ids = df["RecordID"].unique()
-    y = y.loc[unique_ids]
-
-    data = {"X": X, "y": y, "static_features": ["Age", "Gender", "ICUType", "Height"]}
+    data = {
+        "set-a": set_collector[0],
+        "set-b": set_collector[1],
+        "set-c": set_collector[2],
+        "outcomes-a": outcome_collector[0],
+        "outcomes-b": outcome_collector[1],
+        "outcomes-c": outcome_collector[2],
+        "static_features": ["Age", "Gender", "ICUType", "Height"],
+    }
     return data
```

### Comparing `tsdb-0.3.1/tsdb/loading_funcs/physionet_2019.py` & `tsdb-0.4/tsdb/loading_funcs/physionet_2019.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,27 +12,29 @@
 import os
 
 import pandas as pd
 
 
 def load_physionet2019(local_path):
     time_series_measurements_dir = ["training", "training_setB"]
-    label_feature = "SepsisLabel"  # feature SepsisLabel contains labels indicating whether patients get sepsis
-    time_feature = "ICULOS"  # ICU length-of-stay (hours since ICU admit)
+    # label_feature = "SepsisLabel"  # feature SepsisLabel contains labels indicating whether patients get sepsis
+    # time_feature = "ICULOS"  # ICU length-of-stay (hours since ICU admit)
 
-    df_collector = []
+    set_collector = []
     for m_ in time_series_measurements_dir:
+        df_collector = []
         raw_data_dir = os.path.join(local_path, m_)
         for filename in os.listdir(raw_data_dir):
             recordID = filename.split(".psv")[0]
             with open(os.path.join(raw_data_dir, filename), "r") as f:
                 df_temp = pd.read_csv(f, sep="|", header=0)
             df_temp["RecordID"] = recordID
             df_collector.append(df_temp)
+        df = pd.concat(df_collector, sort=True)
+        set_collector.append(df)
 
-    df = pd.concat(df_collector, sort=True)
-    df = df.reset_index(drop=True)
-    y = df[["RecordID", time_feature, label_feature]]
-    X = df.drop(label_feature, axis=1)
-
-    data = {"X": X, "y": y, "static_features": ["Age", "Gender", "HospAdmTime"]}
+    data = {
+        "training_setA": set_collector[0],
+        "training_setB": set_collector[1],
+        "static_features": ["Age", "Gender", "Unit1", "Unit2", "HospAdmTime"],
+    }
     return data
```

### Comparing `tsdb-0.3.1/tsdb/loading_funcs/ucr_uea_datasets.py` & `tsdb-0.4/tsdb/loading_funcs/ucr_uea_datasets.py`

 * *Files identical despite different names*

### Comparing `tsdb-0.3.1/tsdb/loading_funcs/vessel_ais.py` & `tsdb-0.4/tsdb/loading_funcs/vessel_ais.py`

 * *Files identical despite different names*

### Comparing `tsdb-0.3.1/tsdb/utils/config.py` & `tsdb-0.4/tsdb/utils/config.py`

 * *Files identical despite different names*

### Comparing `tsdb-0.3.1/tsdb/utils/downloading.py` & `tsdb-0.4/tsdb/utils/downloading.py`

 * *Files identical despite different names*

### Comparing `tsdb-0.3.1/tsdb/utils/file.py` & `tsdb-0.4/tsdb/utils/file.py`

 * *Files identical despite different names*

### Comparing `tsdb-0.3.1/tsdb/utils/logging.py` & `tsdb-0.4/tsdb/utils/logging.py`

 * *Files identical despite different names*

### Comparing `tsdb-0.3.1/tsdb.egg-info/PKG-INFO` & `tsdb-0.4/tsdb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsdb
-Version: 0.3.1
+Version: 0.4
 Summary: TSDB (Time Series Data Beans): a Python toolbox helping load open-source time-series datasets
 Home-page: https://github.com/WenjieDu/TSDB
 Author: Wenjie Du
 Author-email: wenjay.du@gmail.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://tsdb.readthedocs.io/
 Project-URL: Source, https://github.com/WenjieDu/TSDB/
@@ -21,15 +21,15 @@
 Classifier: Topic :: Database
 Description-Content-Type: text/markdown
 Provides-Extra: basic
 License-File: LICENSE
 
 <a href='https://github.com/WenjieDu/TSDB'><img src="https://pypots.com/figs/pypots_logos/TSDB/logo_FFBG.svg" align='right' width='200'/></a>
 
-<h2 align="center">Welcome to TSDB</h2>
+<h3 align="center">Welcome to TSDB</h3>
 
 *<p align='center'>a Python toolbox to ease loading public time-series datasets</p>*
 
 <p align='center'>
     <a href='https://github.com/WenjieDu/TSDB'>
         <img alt='Python version' src='https://img.shields.io/badge/python-v3-E97040?logo=python&logoColor=white'>
     </a>
@@ -45,15 +45,15 @@
     <a href="https://github.com/WenjieDu/TSDB/graphs/contributors">
         <img alt="GitHub contributors" src="https://img.shields.io/github/contributors/wenjiedu/tsdb?color=D8E699&label=Contributors&logo=GitHub">
     </a>
     <a href="https://star-history.com/#wenjiedu/tsdb">
         <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/wenjiedu/tsdb?logo=None&color=6BB392&label=%E2%98%85%20Stars">
     </a>
     <a href="https://github.com/WenjieDu/TSDB/network/members">
-        <img alt="GitHub Repo forks" src="https://img.shields.io/github/forks/wenjiedu/pygrinder?logo=forgejo&logoColor=black&label=Forks">
+        <img alt="GitHub Repo forks" src="https://img.shields.io/github/forks/wenjiedu/tsdb?logo=forgejo&logoColor=black&label=Forks">
     </a>
     <a href="https://codeclimate.com/github/WenjieDu/TSDB">
         <img alt="Code Climate maintainability" src="https://img.shields.io/codeclimate/maintainability-percentage/WenjieDu/TSDB?color=3C7699&label=Maintainability&logo=codeclimate">
     </a>
     <a href='https://coveralls.io/github/WenjieDu/TSDB'>
         <img alt='Coveralls report' src='https://img.shields.io/coverallsCoverage/github/WenjieDu/TSDB?branch=main&logo=coveralls&color=75C1C4&label=Coverage'>
     </a>
@@ -67,15 +67,15 @@
         <img alt="Conda downloads" src="https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/conda_tsdb_downloads.json">
     </a>
     <a href='https://pepy.tech/project/tsdb'>
         <img alt='PyPI downloads' src='https://img.shields.io/endpoint?url=https://pypots.com/figs/downloads_badges/pypi_tsdb_downloads.json'>
     </a>
 </p>
 
-> 📣 TSDB now supports a total of 1️⃣6️⃣9️⃣ time-series datasets ‼️
+> 📣 TSDB now supports a total of 1️⃣7️⃣0️⃣ time-series datasets ‼️
 
 <a href='https://github.com/WenjieDu/PyPOTS'><img src='https://pypots.com/figs/pypots_logos/PyPOTS/logo_FFBG.svg' width='160' align='left' /></a>
 TSDB is a part of
 <a href="https://github.com/WenjieDu/PyPOTS">
 PyPOTS <img align="center" src="https://img.shields.io/github/stars/WenjieDu/PyPOTS?style=social">
 </a>
 (a Python toolbox for data mining on Partially-Observed Time Series), and was separated from PyPOTS for decoupling datasets from learning algorithms.
@@ -92,25 +92,25 @@
 
 
 ## ❖ Usage Examples
 TSDB now is available on <a alt='Anaconda' href='https://anaconda.org/conda-forge/tsdb'><img align='center' src='https://img.shields.io/badge/Anaconda--lightgreen?style=social&logo=anaconda'></a>❗️
 
 Install it with `conda install tsdb `, you may need to specify the channel with option `-c conda-forge`
 
-or install from PyPI:
+or install via PyPI:
 > pip install tsdb
 
 or install from source code:
 > pip install `https://github.com/WenjieDu/TSDB/archive/main.zip`
 
 ```python
 import tsdb
 
 # list all available datasets in TSDB
-tsdb.list_available_datasets()
+tsdb.list()
 # select the dataset you need and load it, TSDB will download, extract, and process it automatically
 data = tsdb.load('physionet_2012')
 # if you need the raw data, use download_and_extract()
 tsdb.download_and_extract('physionet_2012', './save_it_here')
 # datasets you once loaded are cached, and you can check them with list_cached_data()
 tsdb.list_cache()
 # you can delete only one specific dataset and preserve others
@@ -129,28 +129,35 @@
 ## ❖ List of Available Datasets
 
 | Name                                                                                              | Main Tasks                              |
 |---------------------------------------------------------------------------------------------------|-----------------------------------------|
 | [PhysioNet Challenge 2012](dataset_profiles/physionet_2012)                                       | Forecasting, Imputation, Classification |
 | [PhysioNet Challenge 2019](dataset_profiles/physionet_2019)                                       | Forecasting, Imputation, Classification |
 | [Beijing Multi-Site Air-Quality](dataset_profiles/beijing_multisite_air_quality)                  | Forecasting, Imputation                 |
+| [Italy Air Quality](dataset_profiles/italy_air_quality)                                           | Forecasting, Imputation                 |
 | [Electricity Load Diagrams](dataset_profiles/electricity_load_diagrams)                           | Forecasting, Imputation                 |
 | [Electricity Transformer Temperature (ETT)](dataset_profiles/electricity_transformer_temperature) | Forecasting, Imputation                 |
 | [Vessel AIS](dataset_profiles/vessel_ais)                                                         | Forecasting, Imputation, Classification |
 | [UCR & UEA Datasets](dataset_profiles/ucr_uea_datasets) (all 163 datasets)                        | Classification                          |
 
 
 ## ❖ Citing TSDB/PyPOTS
 The paper introducing PyPOTS project is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811),
 and we are pursuing to publish it in prestigious academic venues, e.g. JMLR (track for
 [Machine Learning Open Source Software](https://www.jmlr.org/mloss/)). If you use TSDB in your work,
 please cite PyPOTS project as below and 🌟star this repository to make others notice this library. 🤗 Thank you!
 
+<p align="center">
+<a href="https://github.com/WenjieDu/PyPOTS">
+    <img src="https://pypots.com/figs/pypots_logos/Ecosystem/PyPOTS_Ecosystem_Pipeline.png" width="95%"/>
+</a>
+</p>
+
 ``` bibtex
-@article{du2023PyPOTS,
+@article{du2023pypots,
 title={{PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series}},
 author={Wenjie Du},
 year={2023},
 eprint={2305.18811},
 archivePrefix={arXiv},
 primaryClass={cs.LG},
 url={https://arxiv.org/abs/2305.18811},
@@ -158,28 +165,13 @@
 }
 ```
 
 > Wenjie Du. (2023).
 > PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series.
 > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811
 
-or
-
-``` bibtex
-@inproceedings{du2023PyPOTS,
-title={{PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series}},
-booktitle={9th SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)},
-author={Wenjie Du},
-year={2023},
-url={https://arxiv.org/abs/2305.18811},
-}
-```
-
-> Wenjie Du. (2023).
-> PyPOTS: a Python toolbox for data mining on Partially-Observed Time Series.
-> In *9th SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)*. https://arxiv.org/abs/2305.18811
 
 
 <details>
 <summary>🏠 Visits</summary>
 <img align='left' src='https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FWenjieDu%2FTime_Series_Database&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+April+2022&edge_flat=false'>
 </details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsdb Version: 0.3.1 Summary: TSDB (Time Series Data
+Metadata-Version: 2.1 Name: tsdb Version: 0.4 Summary: TSDB (Time Series Data
 Beans): a Python toolbox helping load open-source time-series datasets Home-
 page: https://github.com/WenjieDu/TSDB Author: Wenjie Du Author-email:
 wenjay.du@gmail.com License: BSD-3-Clause Project-URL: Documentation, https://
 tsdb.readthedocs.io/ Project-URL: Source, https://github.com/WenjieDu/TSDB/
 Project-URL: Tracker, https://github.com/WenjieDu/TSDB/issues/ Project-URL:
 Download, https://github.com/WenjieDu/TSDB/archive/main.zip Keywords: data
 mining,time series,time-series analysis,time-series database,time-series
@@ -13,23 +13,23 @@
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: BSD License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 :: 3 Classifier: Topic :: Database Description-Content-Type: text/markdown
 Provides-Extra: basic License-File: LICENSE_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/
 _p_y_p_o_t_s___l_o_g_o_s_/_T_S_D_B_/_l_o_g_o___F_F_B_G_._s_v_g_]
-                          ********** WWeellccoommee ttoo TTSSDDBB **********
+                           ******** WWeellccoommee ttoo TTSSDDBB ********
 *
          a Python toolbox to ease loading public time-series datasets
 *
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_t_h_e_ _l_a_t_e_s_t_ _r_e_l_e_a_s_e_ _v_e_r_s_i_o_n_]_[_B_S_D_-_3_ _l_i_c_e_n_s_e_]_[_C_o_m_m_u_n_i_t_y_]_[_G_i_t_H_u_b
        _c_o_n_t_r_i_b_u_t_o_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _s_t_a_r_s_]_[_G_i_t_H_u_b_ _R_e_p_o_ _f_o_r_k_s_]_[_C_o_d_e_ _C_l_i_m_a_t_e
 _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_C_o_v_e_r_a_l_l_s_ _r_e_p_o_r_t_]_[_G_i_t_H_u_b_ _T_e_s_t_i_n_g_]_[_a_r_X_i_v_ _D_O_I_]_[_C_o_n_d_a_ _d_o_w_n_l_o_a_d_s_]
                                _[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]
-> ð£ TSDB now supports a total of 1ï¸â£6ï¸â£9ï¸â£ time-series datasets
+> ð£ TSDB now supports a total of 1ï¸â£7ï¸â£0ï¸â£ time-series datasets
 â¼ï¸ _[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_P_y_P_O_T_S_/_l_o_g_o___F_F_B_G_._s_v_g_]TSDB is a
 part of _P_y_P_O_T_S_ _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_W_e_n_j_i_e_D_u_/
 _P_y_P_O_T_S_?_s_t_y_l_e_=_s_o_c_i_a_l_](a Python toolbox for data mining on Partially-Observed
 Time Series), and was separated from PyPOTS for decoupling datasets from
 learning algorithms. TSDB is created to help researchers and engineers get rid
 of data collecting and downloading, and focus back on data processing details.
 TSDB provides all-in-one-stop convenience for downloading and loading open-
@@ -47,54 +47,49 @@
 notice TSDB if you think it is a useful toolkit. **Please** properly [cite TSDB
 and PyPOTS](https://github.com/WenjieDu/TSDB#-citing-tsdbpypots) in your
 publications if it helps with your research. This really means a lot to our
 open-source research. Thank you! ## â Usage Examples TSDB now is available on
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_A_n_a_c_o_n_d_a_-_-
 _l_i_g_h_t_g_r_e_e_n_?_s_t_y_l_e_=_s_o_c_i_a_l_&_l_o_g_o_=_a_n_a_c_o_n_d_a_]âï¸ Install it with `conda install
 tsdb `, you may need to specify the channel with option `-c conda-forge` or
-install from PyPI: > pip install tsdb or install from source code: > pip
-install `https://github.com/WenjieDu/TSDB/archive/main.zip` ```python import
-tsdb # list all available datasets in TSDB tsdb.list_available_datasets() #
-select the dataset you need and load it, TSDB will download, extract, and
-process it automatically data = tsdb.load('physionet_2012') # if you need the
-raw data, use download_and_extract() tsdb.download_and_extract
-('physionet_2012', './save_it_here') # datasets you once loaded are cached, and
-you can check them with list_cached_data() tsdb.list_cache() # you can delete
-only one specific dataset and preserve others tsdb.delete_cache
-(dataset_name='physionet_2012') # or you can delete all cache with
-delete_cached_data() to free disk space tsdb.delete_cache() # to avoid taking
-up too much space if downloading many datasets, # TSDB cache directory can be
-migrated to an external disk tsdb.migrate_cache("/mnt/external_disk/
-TSDB_cache") ``` That's all. Simple and efficient. Enjoy it! ð ## â List
-of Available Datasets | Name | Main Tasks | |----------------------------------
------------------------------------------------------------------|-------------
-----------------------------| | [PhysioNet Challenge 2012](dataset_profiles/
-physionet_2012) | Forecasting, Imputation, Classification | | [PhysioNet
-Challenge 2019](dataset_profiles/physionet_2019) | Forecasting, Imputation,
-Classification | | [Beijing Multi-Site Air-Quality](dataset_profiles/
-beijing_multisite_air_quality) | Forecasting, Imputation | | [Electricity Load
-Diagrams](dataset_profiles/electricity_load_diagrams) | Forecasting, Imputation
-| | [Electricity Transformer Temperature (ETT)](dataset_profiles/
+install via PyPI: > pip install tsdb or install from source code: > pip install
+`https://github.com/WenjieDu/TSDB/archive/main.zip` ```python import tsdb #
+list all available datasets in TSDB tsdb.list() # select the dataset you need
+and load it, TSDB will download, extract, and process it automatically data =
+tsdb.load('physionet_2012') # if you need the raw data, use
+download_and_extract() tsdb.download_and_extract('physionet_2012', './
+save_it_here') # datasets you once loaded are cached, and you can check them
+with list_cached_data() tsdb.list_cache() # you can delete only one specific
+dataset and preserve others tsdb.delete_cache(dataset_name='physionet_2012') #
+or you can delete all cache with delete_cached_data() to free disk space
+tsdb.delete_cache() # to avoid taking up too much space if downloading many
+datasets, # TSDB cache directory can be migrated to an external disk
+tsdb.migrate_cache("/mnt/external_disk/TSDB_cache") ``` That's all. Simple and
+efficient. Enjoy it! ð ## â List of Available Datasets | Name | Main Tasks
+| |----------------------------------------------------------------------------
+-----------------------|-----------------------------------------| | [PhysioNet
+Challenge 2012](dataset_profiles/physionet_2012) | Forecasting, Imputation,
+Classification | | [PhysioNet Challenge 2019](dataset_profiles/physionet_2019)
+| Forecasting, Imputation, Classification | | [Beijing Multi-Site Air-Quality]
+(dataset_profiles/beijing_multisite_air_quality) | Forecasting, Imputation | |
+[Italy Air Quality](dataset_profiles/italy_air_quality) | Forecasting,
+Imputation | | [Electricity Load Diagrams](dataset_profiles/
+electricity_load_diagrams) | Forecasting, Imputation | | [Electricity
+Transformer Temperature (ETT)](dataset_profiles/
 electricity_transformer_temperature) | Forecasting, Imputation | | [Vessel AIS]
 (dataset_profiles/vessel_ais) | Forecasting, Imputation, Classification | |
 [UCR & UEA Datasets](dataset_profiles/ucr_uea_datasets) (all 163 datasets) |
 Classification | ## â Citing TSDB/PyPOTS The paper introducing PyPOTS project
 is available on arXiv at [this URL](https://arxiv.org/abs/2305.18811), and we
 are pursuing to publish it in prestigious academic venues, e.g. JMLR (track for
 [Machine Learning Open Source Software](https://www.jmlr.org/mloss/)). If you
 use TSDB in your work, please cite PyPOTS project as below and ðstar this
-repository to make others notice this library. ð¤ Thank you! ``` bibtex
-@article{du2023PyPOTS, title={{PyPOTS: a Python toolbox for data mining on
-Partially-Observed Time Series}}, author={Wenjie Du}, year={2023}, eprint=
-{2305.18811}, archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://
+repository to make others notice this library. ð¤ Thank you!
+_[_h_t_t_p_s_:_/_/_p_y_p_o_t_s_._c_o_m_/_f_i_g_s_/_p_y_p_o_t_s___l_o_g_o_s_/_E_c_o_s_y_s_t_e_m_/_P_y_P_O_T_S___E_c_o_s_y_s_t_e_m___P_i_p_e_l_i_n_e_._p_n_g_]
+``` bibtex @article{du2023pypots, title={{PyPOTS: a Python toolbox for data
+mining on Partially-Observed Time Series}}, author={Wenjie Du}, year={2023},
+eprint={2305.18811}, archivePrefix={arXiv}, primaryClass={cs.LG}, url={https://
 arxiv.org/abs/2305.18811}, doi={10.48550/arXiv.2305.18811}, } ``` > Wenjie Du.
 (2023). > PyPOTS: a Python toolbox for data mining on Partially-Observed Time
-Series. > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 or ``` bibtex
-@inproceedings{du2023PyPOTS, title={{PyPOTS: a Python toolbox for data mining
-on Partially-Observed Time Series}}, booktitle={9th SIGKDD workshop on Mining
-and Learning from Time Series (MiLeTS'23)}, author={Wenjie Du}, year={2023},
-url={https://arxiv.org/abs/2305.18811}, } ``` > Wenjie Du. (2023). > PyPOTS: a
-Python toolbox for data mining on Partially-Observed Time Series. > In *9th
-SIGKDD workshop on Mining and Learning from Time Series (MiLeTS'23)*. https://
-arxiv.org/abs/2305.18811 ð  Visits[https://hits.seeyoufarm.com/api/count/
-incr/
+Series. > arXiv, abs/2305.18811.https://arxiv.org/abs/2305.18811 ð  Visits
+[https://hits.seeyoufarm.com/api/count/incr/
 badge.svg?url=https%3A%2F%2Fgithub.com%2FWenjieDu%2FTime_Series_Database&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Visits+since+April+2022&edge_flat=false]
```

### Comparing `tsdb-0.3.1/tsdb.egg-info/SOURCES.txt` & `tsdb-0.4/tsdb.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 tsdb.egg-info/dependency_links.txt
 tsdb.egg-info/requires.txt
 tsdb.egg-info/top_level.txt
 tsdb/loading_funcs/__init__.py
 tsdb/loading_funcs/beijing_multisite_air_quality.py
 tsdb/loading_funcs/electricity_load_diagrams.py
 tsdb/loading_funcs/electricity_transformer_temperature.py
+tsdb/loading_funcs/italy_air_quality.py
 tsdb/loading_funcs/physionet_2012.py
 tsdb/loading_funcs/physionet_2019.py
 tsdb/loading_funcs/ucr_uea_datasets.py
 tsdb/loading_funcs/vessel_ais.py
 tsdb/utils/__init__.py
 tsdb/utils/config.py
 tsdb/utils/downloading.py
```

