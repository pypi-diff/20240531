# Comparing `tmp/va_am-0.1.6.tar.gz` & `tmp/va_am-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "va_am-0.1.6.tar", last modified: Wed May 29 16:01:29 2024, max compression
+gzip compressed data, was "va_am-0.1.7.tar", last modified: Fri May 31 07:32:52 2024, max compression
```

## Comparing `va_am-0.1.6.tar` & `va_am-0.1.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-29 16:01:29.129001 va_am-0.1.6/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    35149 2023-09-29 09:45:51.000000 va_am-0.1.6/LICENSE
--rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-05-29 16:01:29.129001 va_am-0.1.6/PKG-INFO
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     5078 2024-02-12 18:26:04.000000 va_am-0.1.6/README.md
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      756 2024-05-29 16:00:07.000000 va_am-0.1.6/pyproject.toml
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       38 2024-05-29 16:01:29.129001 va_am-0.1.6/setup.cfg
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       68 2023-09-28 11:32:10.000000 va_am-0.1.6/setup.py
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-29 16:01:29.125001 va_am-0.1.6/src/
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-29 16:01:29.125001 va_am-0.1.6/src/va_am/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      222 2024-02-20 12:03:10.000000 va_am-0.1.6/src/va_am/__init__.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       66 2023-09-28 11:12:58.000000 va_am-0.1.6/src/va_am/__main__.py
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-29 16:01:29.129001 va_am-0.1.6/src/va_am/utils/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    60986 2024-05-20 13:28:39.000000 va_am-0.1.6/src/va_am/utils/AutoEncoders.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2023-06-29 15:33:10.000000 va_am-0.1.6/src/va_am/utils/__init__.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     3123 2023-09-25 14:36:24.000000 va_am-0.1.6/src/va_am/utils/functions.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)   104327 2024-05-29 16:00:07.000000 va_am-0.1.6/src/va_am/va_am.py
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-29 16:01:29.129001 va_am-0.1.6/src/va_am.egg-info/
--rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-05-29 16:01:29.000000 va_am-0.1.6/src/va_am.egg-info/PKG-INFO
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      517 2024-05-29 16:01:29.000000 va_am-0.1.6/src/va_am.egg-info/SOURCES.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2024-05-29 16:01:29.000000 va_am-0.1.6/src/va_am.egg-info/dependency_links.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       46 2024-05-29 16:01:29.000000 va_am-0.1.6/src/va_am.egg-info/entry_points.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       71 2024-05-29 16:01:29.000000 va_am-0.1.6/src/va_am.egg-info/requires.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        6 2024-05-29 16:01:29.000000 va_am-0.1.6/src/va_am.egg-info/top_level.txt
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-29 16:01:29.129001 va_am-0.1.6/test/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.6/test/test_AutoEncoders.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1232 2024-05-20 13:28:39.000000 va_am-0.1.6/test/test_aux_va_am.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.6/test/test_io_va_am.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.6/test/test_main_va_am.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-20 13:28:39.000000 va_am-0.1.6/test/test_utils_functions.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-31 07:32:52.388596 va_am-0.1.7/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    35149 2023-09-29 09:45:51.000000 va_am-0.1.7/LICENSE
+-rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-05-31 07:32:52.384596 va_am-0.1.7/PKG-INFO
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     5078 2024-02-12 18:26:04.000000 va_am-0.1.7/README.md
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      756 2024-05-31 07:32:36.000000 va_am-0.1.7/pyproject.toml
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       38 2024-05-31 07:32:52.388596 va_am-0.1.7/setup.cfg
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       68 2023-09-28 11:32:10.000000 va_am-0.1.7/setup.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-31 07:32:52.380596 va_am-0.1.7/src/
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-31 07:32:52.384596 va_am-0.1.7/src/va_am/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      222 2024-02-20 12:03:10.000000 va_am-0.1.7/src/va_am/__init__.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       66 2023-09-28 11:12:58.000000 va_am-0.1.7/src/va_am/__main__.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-31 07:32:52.384596 va_am-0.1.7/src/va_am/utils/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    60986 2024-05-20 13:28:39.000000 va_am-0.1.7/src/va_am/utils/AutoEncoders.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2023-06-29 15:33:10.000000 va_am-0.1.7/src/va_am/utils/__init__.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     3123 2023-09-25 14:36:24.000000 va_am-0.1.7/src/va_am/utils/functions.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)   104292 2024-05-31 07:26:52.000000 va_am-0.1.7/src/va_am/va_am.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-31 07:32:52.384596 va_am-0.1.7/src/va_am.egg-info/
+-rw-r--r--   0 cosmin    (1000) cosmin    (1000)    46344 2024-05-31 07:32:52.000000 va_am-0.1.7/src/va_am.egg-info/PKG-INFO
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      517 2024-05-31 07:32:52.000000 va_am-0.1.7/src/va_am.egg-info/SOURCES.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2024-05-31 07:32:52.000000 va_am-0.1.7/src/va_am.egg-info/dependency_links.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       46 2024-05-31 07:32:52.000000 va_am-0.1.7/src/va_am.egg-info/entry_points.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       71 2024-05-31 07:32:52.000000 va_am-0.1.7/src/va_am.egg-info/requires.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        6 2024-05-31 07:32:52.000000 va_am-0.1.7/src/va_am.egg-info/top_level.txt
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2024-05-31 07:32:52.384596 va_am-0.1.7/test/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-29 17:31:40.000000 va_am-0.1.7/test/test_AutoEncoders.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1232 2024-05-29 17:31:40.000000 va_am-0.1.7/test/test_aux_va_am.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-29 17:31:40.000000 va_am-0.1.7/test/test_io_va_am.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-29 17:31:40.000000 va_am-0.1.7/test/test_main_va_am.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        0 2024-05-29 17:31:40.000000 va_am-0.1.7/test/test_utils_functions.py
```

### Comparing `va_am-0.1.6/LICENSE` & `va_am-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `va_am-0.1.6/PKG-INFO` & `va_am-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: va_am
-Version: 0.1.6
+Version: 0.1.7
 Summary: VA-AM method implementation
 Author-email: cosminmarina <cosmin.marina@uah.es>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `va_am-0.1.6/README.md` & `va_am-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `va_am-0.1.6/pyproject.toml` & `va_am-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "va_am"
-version = "0.1.6"
+version = "0.1.7"
 authors = [{name="cosminmarina", email="cosmin.marina@uah.es" }]
 description = "VA-AM method implementation"
 readme = "README.md"
 dependencies = ["requests","sympy","keras","tensorflow","xarray","netcdf4","matplotlib","pandas","numpy"]
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `va_am-0.1.6/src/va_am/utils/AutoEncoders.py` & `va_am-0.1.7/src/va_am/utils/AutoEncoders.py`

 * *Files identical despite different names*

### Comparing `va_am-0.1.6/src/va_am/utils/functions.py` & `va_am-0.1.7/src/va_am/utils/functions.py`

 * *Files identical despite different names*

### Comparing `va_am-0.1.6/src/va_am/va_am.py` & `va_am-0.1.7/src/va_am/va_am.py`

 * *Files 0% similar despite different names*

```diff
@@ -866,48 +866,48 @@
     reconstruction_Pre_AE = []
     reconstruction_Post_Analog = []
     reconstruction_Post_AE = []
     for i in range(params["iter"]):
         if params["period"] in ['both', 'pre']:
             dict_stats[f'WithoutAE-Pre{i}'] = [np.nansum(np.abs(data_of_interest_prs - analog_pre[0][i]))/img_size,
                                     np.nanmean(np.abs(data_of_interest_temp[params["temp_var_name"]].data - analog_pre[1][i])[:,int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]]),
-                                    np.nanmean(analog_pre[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]])-273.15,
+                                    np.nanmean(analog_pre[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]]),
                                     str(analog_pre[2][i].data)[:10]]
             reconstruction_Pre_Analog.append(analog_pre[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]])
         else:
             dict_stats[f'WithoutAE-Pre{i}'] = [np.nan, np.nan, np.nan]
         
         if params["period"] in ['both', 'post']:
             dict_stats[f'WithoutAE-Post{i}'] = [np.nansum(np.abs(data_of_interest_prs - analog_ind[0][i]))/img_size,
                                     np.nanmean(np.abs(data_of_interest_temp[params["temp_var_name"]].data - analog_ind[1][i])[:,int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]]),
-                                    np.nanmean(analog_ind[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]])-273.15,
+                                    np.nanmean(analog_ind[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]]),
                                     str(analog_ind[2][i].data)[:10]]
             reconstruction_Post_Analog.append(analog_ind[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]])
         else:
             dict_stats[f'WithoutAE-Post{i}'] = [np.nan, np.nan, np.nan]
         
         if params["period"] in ['both', 'pre']:
             dict_stats[f'WithAE-Pre-Pre{i}'] = [np.nansum(np.abs(data_of_interest_prs_encoded_pre - latent_analog_pre[0][i]))/img_size,
                                         np.nanmean(np.abs(data_of_interest_temp[params["temp_var_name"]].data - latent_analog_pre[1][i])[:,int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]]),
-                                        np.nanmean(latent_analog_pre[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]])-273.15,
+                                        np.nanmean(latent_analog_pre[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]]),
                                         str(latent_analog_pre[2][i].data)[:10]]
             reconstruction_Pre_AE.append(latent_analog_pre[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]])
         else:
             dict_stats[f'WithAE-Pre-Pre{i}'] = [np.nan, np.nan, np.nan]
 
         if params["period"] in ['both', 'post']:
             dict_stats[f'WithAE-Post-Post{i}'] = [np.nansum(np.abs(data_of_interest_prs_encoded_ind - latent_analog_ind[0][i]))/img_size,
                                     np.nanmean(np.abs(data_of_interest_temp[params["temp_var_name"]].data - latent_analog_ind[1][i])[:,int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]]),
-                                    np.nanmean(latent_analog_ind[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]])-273.15,
+                                    np.nanmean(latent_analog_ind[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]]),
                                     str(latent_analog_ind[2][i].data)[:10]]
             reconstruction_Post_AE.append(latent_analog_ind[1][i][int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]])
         else:
             dict_stats[f'WithAE-Post-Post{i}'] = [np.nan, np.nan, np.nan]
 
-        dict_stats[f'Original{i}']=[0,0,np.nanmean(((data_of_interest_temp[params["temp_var_name"]].data)[:,int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]]))-273.15]
+        dict_stats[f'Original{i}']=[0,0,np.nanmean(((data_of_interest_temp[params["temp_var_name"]].data)[:,int_reg[0]:int_reg[1],int_reg[2]:int_reg[3]]))]
         
         if params["verbose"]:
             print(f'Iteration {i} finished')
 
     df_stats = pd.DataFrame.from_dict(dict_stats,orient='index',columns=['prs-diff','temp-diff','temp','time'])
     Path("./comparison-csv").mkdir(parents=True, exist_ok=True)
     df_stats.to_csv(f'./comparison-csv/{params["season"]}{params["name"]}x{params["iter"]}-{params["data_of_interest_init"]}-epoch{params["n_epochs"]}-latent{params["latent_dim"]}-k{params["k"]}-arch{params["arch"]}-{"VAE" if params["use_VAE"] else "noVAE"}-analog-comparision-stats{current.year}-{current.month}-{current.day}-{current.hour}-{current.minute}-{current.second}.csv'.replace(" ","").replace("'", "").replace(",",""))
```

### Comparing `va_am-0.1.6/src/va_am.egg-info/PKG-INFO` & `va_am-0.1.7/src/va_am.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: va_am
-Version: 0.1.6
+Version: 0.1.7
 Summary: VA-AM method implementation
 Author-email: cosminmarina <cosmin.marina@uah.es>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `va_am-0.1.6/src/va_am.egg-info/SOURCES.txt` & `va_am-0.1.7/src/va_am.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `va_am-0.1.6/test/test_aux_va_am.py` & `va_am-0.1.7/test/test_aux_va_am.py`

 * *Files identical despite different names*

