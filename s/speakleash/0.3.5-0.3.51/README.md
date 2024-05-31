# Comparing `tmp/speakleash-0.3.5.tar.gz` & `tmp/speakleash-0.3.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speakleash-0.3.5.tar", last modified: Sun May  5 22:16:40 2024, max compression
+gzip compressed data, was "speakleash-0.3.51.tar", last modified: Fri May 31 15:55:08 2024, max compression
```

## Comparing `speakleash-0.3.5.tar` & `speakleash-0.3.51.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 22:16:40.274949 speakleash-0.3.5/
--rw-rw-rw-   0        0        0     1082 2024-05-05 21:15:03.000000 speakleash-0.3.5/LICENSE
--rw-rw-rw-   0        0        0     3461 2024-05-05 22:16:40.272849 speakleash-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     2983 2024-05-05 21:15:03.000000 speakleash-0.3.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 22:16:40.274949 speakleash-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      669 2024-05-05 21:15:03.000000 speakleash-0.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:16:40.191643 speakleash-0.3.5/speakleash/
--rw-rw-rw-   0        0        0      573 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:16:40.223173 speakleash-0.3.5/speakleash/category_manager/
--rw-rw-rw-   0        0        0      183 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/category_manager/__init__.py
--rw-rw-rw-   0        0        0     6769 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/category_manager/category_manager.py
--rw-rw-rw-   0        0        0      298 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/config.json
--rw-rw-rw-   0        0        0      930 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/config_loader.py
--rw-rw-rw-   0        0        0     1869 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/contrib.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:16:40.237879 speakleash-0.3.5/speakleash/core/
--rw-rw-rw-   0        0        0      151 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/core/__init__.py
--rw-rw-rw-   0        0        0     3924 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/core/core.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:16:40.255653 speakleash-0.3.5/speakleash/dataset/
--rw-rw-rw-   0        0        0      167 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/dataset/__init__.py
--rw-rw-rw-   0        0        0    12921 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/dataset/dataset.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:16:40.270841 speakleash-0.3.5/speakleash/downloader/
--rw-rw-rw-   0        0        0      210 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/downloader/__init__.py
--rw-rw-rw-   0        0        0     4560 2024-05-05 21:15:03.000000 speakleash-0.3.5/speakleash/downloader/structure_downloader.py
-drwxrwxrwx   0        0        0        0 2024-05-05 22:16:40.271848 speakleash-0.3.5/speakleash.egg-info/
--rw-rw-rw-   0        0        0     3461 2024-05-05 22:16:40.000000 speakleash-0.3.5/speakleash.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      572 2024-05-05 22:16:40.000000 speakleash-0.3.5/speakleash.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 22:16:40.000000 speakleash-0.3.5/speakleash.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-05 22:16:40.000000 speakleash-0.3.5/speakleash.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-05 22:16:40.000000 speakleash-0.3.5/speakleash.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 15:55:07.947685 speakleash-0.3.51/
+-rw-rw-rw-   0        0        0     1082 2024-05-30 14:21:15.000000 speakleash-0.3.51/LICENSE
+-rw-rw-rw-   0        0        0     3467 2024-05-31 15:55:07.947685 speakleash-0.3.51/PKG-INFO
+-rw-rw-rw-   0        0        0     3017 2024-05-31 15:33:55.000000 speakleash-0.3.51/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-31 15:55:07.948707 speakleash-0.3.51/setup.cfg
+-rw-rw-rw-   0        0        0      670 2024-05-31 15:50:40.000000 speakleash-0.3.51/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 15:55:07.561134 speakleash-0.3.51/speakleash/
+-rw-rw-rw-   0        0        0      573 2024-05-30 14:21:15.000000 speakleash-0.3.51/speakleash/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 15:55:07.774146 speakleash-0.3.51/speakleash/category_manager/
+-rw-rw-rw-   0        0        0      183 2024-05-30 14:21:15.000000 speakleash-0.3.51/speakleash/category_manager/__init__.py
+-rw-rw-rw-   0        0        0     6769 2024-05-30 14:21:15.000000 speakleash-0.3.51/speakleash/category_manager/category_manager.py
+-rw-rw-rw-   0        0        0      298 2024-05-30 14:21:15.000000 speakleash-0.3.51/speakleash/config.json
+-rw-rw-rw-   0        0        0      930 2024-05-30 14:21:15.000000 speakleash-0.3.51/speakleash/config_loader.py
+-rw-rw-rw-   0        0        0     1869 2024-05-30 14:21:15.000000 speakleash-0.3.51/speakleash/contrib.py
+drwxrwxrwx   0        0        0        0 2024-05-31 15:55:07.826779 speakleash-0.3.51/speakleash/core/
+-rw-rw-rw-   0        0        0      151 2024-05-30 14:21:15.000000 speakleash-0.3.51/speakleash/core/__init__.py
+-rw-rw-rw-   0        0        0     3924 2024-05-30 14:21:15.000000 speakleash-0.3.51/speakleash/core/core.py
+drwxrwxrwx   0        0        0        0 2024-05-31 15:55:07.863570 speakleash-0.3.51/speakleash/dataset/
+-rw-rw-rw-   0        0        0      167 2024-05-30 14:21:15.000000 speakleash-0.3.51/speakleash/dataset/__init__.py
+-rw-rw-rw-   0        0        0    12921 2024-05-30 14:21:15.000000 speakleash-0.3.51/speakleash/dataset/dataset.py
+drwxrwxrwx   0        0        0        0 2024-05-31 15:55:07.914230 speakleash-0.3.51/speakleash/downloader/
+-rw-rw-rw-   0        0        0      210 2024-05-30 14:21:15.000000 speakleash-0.3.51/speakleash/downloader/__init__.py
+-rw-rw-rw-   0        0        0     4560 2024-05-30 14:21:15.000000 speakleash-0.3.51/speakleash/downloader/structure_downloader.py
+drwxrwxrwx   0        0        0        0 2024-05-31 15:55:07.740872 speakleash-0.3.51/speakleash.egg-info/
+-rw-rw-rw-   0        0        0     3467 2024-05-31 15:55:07.000000 speakleash-0.3.51/speakleash.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2024-05-31 15:55:07.000000 speakleash-0.3.51/speakleash.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 15:55:07.000000 speakleash-0.3.51/speakleash.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-05-31 15:55:07.000000 speakleash-0.3.51/speakleash.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-31 15:55:07.000000 speakleash-0.3.51/speakleash.egg-info/top_level.txt
```

### Comparing `speakleash-0.3.5/LICENSE` & `speakleash-0.3.51/LICENSE`

 * *Files identical despite different names*

### Comparing `speakleash-0.3.5/PKG-INFO` & `speakleash-0.3.51/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: speakleash
-Version: 0.3.5
+Version: 0.3.51
 Summary: SpeakLeash agnostic dataset for Polish
 Home-page: https://github.com/speakleash/speakleash
 Author: SpeakLeash Team
 Author-email: team@speakleash.org
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: tqdm
-Requires-Dist: lm_dataformat
 
 <h1 align="center">
 <img src="https://raw.githubusercontent.com/speakleash/speakleash/main/branding/logo/speakleash_logo.png" width="300">
 </h1><br>
 
 <p align="center">
     <a href="https://pypi.org/project/speakleash"><img src="https://badge.fury.io/py/speakleash.svg"></a>
@@ -22,37 +21,40 @@
     <a href="https://pypi.org/project/speakleash"><img src="https://img.shields.io/badge/python-_>=_3.6-blue"></a>
     <a href="https://speakleash.org/dashboard/"><img src="https://img.shields.io/badge/dynamic/json?url=https://cutt.ly/ywcfnFY7&query=datasetsGB&suffix=%20GB&label=datasets&color=brightgreen"></a>
     <a href="https://speakleash.org/spolecznosc-i-kontakt/"><img src="https://img.shields.io/discord/1043112910278381619?logo=discord&label=discord&color=%23603FEF"></a>
 </p>
 
 ### UPDATE 05.05.2024: 
 Due to the changes related with the hosting, it is recommended to update the version of the package to the newest one, using command:
-```python
+```bash
 pip install --upgrade speakleash
 ```
 
-[SpeakLeash](href="https://pypi.org/project/speakleash) is a lightweight library providing datasets for the Polish language
-and tools to make them useful.
+[SpeakLeash](https://pypi.org/project/speakleash) is a lightweight library providing datasets for the Polish language
+and tools to make them useful:
 
 - **Website:** https://speakleash.org/
 - **Datasets:** https://speakleash.org/dashboard/
 - **Source code:** https://github.com/speakleash/speakleash
 - **Data in action:** https://github.com/speakleash/speakleash-examples
 - **Bug reports:** https://github.com/speakleash/speakleash/issues
 
-## Installation
+Installation
+----------------------
 
 Speakleash package can be installed from PyPi and has to be installed in a virtual environment:
-```python
+
+```bash
 pip install speakleash
 ```
 
-## Basic Usage
+Basic Usage
+----------------------
 
-If you just want to see the details of the datasets
+If you just want to see the details of the datasets:
 
 ```python
 from speakleash import Speakleash
 import os
 
 base_dir = os.path.join(os.path.dirname(__file__))
 replicate_to = os.path.join(base_dir, "datasets")
@@ -60,36 +62,39 @@
 sl = Speakleash(replicate_to)
 
 for d in sl.datasets:
     size_mb = round(d.characters/1024/1024)
     print("Dataset: {0}, size: {1} MB, characters: {2}, documents: {3}".format(d.name, size_mb, d.characters, d.documents))
 ```
 
-You can use individual properties (e.g.:***characters***, ***documents***), but you can display the entire manifest
+You can use individual properties (e.g.:***characters***, ***documents***), but you can display the entire manifest:
+
 ```python
 sl = Speakleash(replicate_to)
 print(sl.get("plwiki").manifest)
 ```
 
-If you chose one of them (***.get(name of dataset)***) then you will get a lot of text data ;-)
+If you chose one of them (***.get(name of dataset)***) then you will get a lot of text data:
+
 ```python
 from speakleash import Speakleash
 import os
 
 base_dir = os.path.join(os.path.dirname(__file__))
 replicate_to = os.path.join(base_dir, "datasets")
 
 sl = Speakleash(replicate_to)
 
 wiki = sl.get("plwiki").data
 for doc in wiki:
     print(doc[:40])
 ```
 
-If you also need meta data then use the ***ext_data*** property
+If you also need meta data then use the ***ext_data*** property:
+
 ```python
 ds = sl.get("plwiki").ext_data
 for doc in ds:
     print(doc)
     txt, meta = doc
     print(meta.get("title"))
     print(txt)
@@ -101,7 +106,9 @@
 * length
 * sentences
 * words
 * verbs
 * nouns
 * symbols
 * punctuations
+
+
```

#### html2text {}

```diff
@@ -1,41 +1,42 @@
-Metadata-Version: 2.1 Name: speakleash Version: 0.3.5 Summary: SpeakLeash
+Metadata-Version: 2.1 Name: speakleash Version: 0.3.51 Summary: SpeakLeash
 agnostic dataset for Polish Home-page: https://github.com/speakleash/speakleash
-Author: SpeakLeash Team Author-email: team@speakleash.org Requires-Python:
->=3.6 Description-Content-Type: text/markdown License-File: LICENSE Requires-
-Dist: requests Requires-Dist: tqdm Requires-Dist: lm_dataformat
+Author: SpeakLeash Team Author-email: team@speakleash.org License: UNKNOWN
+Platform: UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE
 ************ [[hhttttppss::////rraaww..ggiitthhuubbuusseerrccoonntteenntt..ccoomm//ssppeeaakklleeaasshh//ssppeeaakklleeaasshh//mmaaiinn//bbrraannddiinngg//
                        llooggoo//ssppeeaakklleeaasshh__llooggoo..ppnngg]] ************
 
     _[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_s_p_e_a_k_l_e_a_s_h_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
  _o_r_g_a_n_i_s_a_t_i_o_n_-_S_p_e_a_k_l_e_a_s_h_-_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-___>_=___3_._6_-
      _b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_d_y_n_a_m_i_c_/_j_s_o_n_?_u_r_l_=_h_t_t_p_s_:_/_/_c_u_t_t_._l_y_/
 _y_w_c_f_n_F_Y_7_&_q_u_e_r_y_=_d_a_t_a_s_e_t_s_G_B_&_s_u_f_f_i_x_=_%_2_0_G_B_&_l_a_b_e_l_=_d_a_t_a_s_e_t_s_&_c_o_l_o_r_=_b_r_i_g_h_t_g_r_e_e_n_]_[_h_t_t_p_s_:
                            _/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_i_s_c_o_r_d_/
         _1_0_4_3_1_1_2_9_1_0_2_7_8_3_8_1_6_1_9_?_l_o_g_o_=_d_i_s_c_o_r_d_&_l_a_b_e_l_=_d_i_s_c_o_r_d_&_c_o_l_o_r_=_%_2_3_6_0_3_F_E_F_]
 ### UPDATE 05.05.2024: Due to the changes related with the hosting, it is
 recommended to update the version of the package to the newest one, using
-command: ```python pip install --upgrade speakleash ``` [SpeakLeash]
-(href="https://pypi.org/project/speakleash) is a lightweight library providing
-datasets for the Polish language and tools to make them useful. - **Website:**
-https://speakleash.org/ - **Datasets:** https://speakleash.org/dashboard/ -
-**Source code:** https://github.com/speakleash/speakleash - **Data in action:**
-https://github.com/speakleash/speakleash-examples - **Bug reports:** https://
-github.com/speakleash/speakleash/issues ## Installation Speakleash package can
-be installed from PyPi and has to be installed in a virtual environment:
-```python pip install speakleash ``` ## Basic Usage If you just want to see the
-details of the datasets ```python from speakleash import Speakleash import os
-base_dir = os.path.join(os.path.dirname(__file__)) replicate_to = os.path.join
-(base_dir, "datasets") sl = Speakleash(replicate_to) for d in sl.datasets:
-size_mb = round(d.characters/1024/1024) print("Dataset: {0}, size: {1} MB,
-characters: {2}, documents: {3}".format(d.name, size_mb, d.characters,
-d.documents)) ``` You can use individual properties (e.g.:***characters***,
-***documents***), but you can display the entire manifest ```python sl =
-Speakleash(replicate_to) print(sl.get("plwiki").manifest) ``` If you chose one
-of them (***.get(name of dataset)***) then you will get a lot of text data ;-
-) ```python from speakleash import Speakleash import os base_dir = os.path.join
-(os.path.dirname(__file__)) replicate_to = os.path.join(base_dir, "datasets")
-sl = Speakleash(replicate_to) wiki = sl.get("plwiki").data for doc in wiki:
-print(doc[:40]) ``` If you also need meta data then use the ***ext_data***
-property ```python ds = sl.get("plwiki").ext_data for doc in ds: print(doc)
-txt, meta = doc print(meta.get("title")) print(txt) ``` Popular meta data: *
-title * length * sentences * words * verbs * nouns * symbols * punctuations
+command: ```bash pip install --upgrade speakleash ``` [SpeakLeash](https://
+pypi.org/project/speakleash) is a lightweight library providing datasets for
+the Polish language and tools to make them useful: - **Website:** https://
+speakleash.org/ - **Datasets:** https://speakleash.org/dashboard/ - **Source
+code:** https://github.com/speakleash/speakleash - **Data in action:** https://
+github.com/speakleash/speakleash-examples - **Bug reports:** https://
+github.com/speakleash/speakleash/issues Installation ---------------------
+- Speakleash package can be installed from PyPi and has to be installed in a
+virtual environment: ```bash pip install speakleash ``` Basic Usage -----------
+----------- If you just want to see the details of the datasets: ```python from
+speakleash import Speakleash import os base_dir = os.path.join(os.path.dirname
+(__file__)) replicate_to = os.path.join(base_dir, "datasets") sl = Speakleash
+(replicate_to) for d in sl.datasets: size_mb = round(d.characters/1024/1024)
+print("Dataset: {0}, size: {1} MB, characters: {2}, documents: {3}".format
+(d.name, size_mb, d.characters, d.documents)) ``` You can use individual
+properties (e.g.:***characters***, ***documents***), but you can display the
+entire manifest: ```python sl = Speakleash(replicate_to) print(sl.get
+("plwiki").manifest) ``` If you chose one of them (***.get(name of dataset)***)
+then you will get a lot of text data: ```python from speakleash import
+Speakleash import os base_dir = os.path.join(os.path.dirname(__file__))
+replicate_to = os.path.join(base_dir, "datasets") sl = Speakleash(replicate_to)
+wiki = sl.get("plwiki").data for doc in wiki: print(doc[:40]) ``` If you also
+need meta data then use the ***ext_data*** property: ```python ds = sl.get
+("plwiki").ext_data for doc in ds: print(doc) txt, meta = doc print(meta.get
+("title")) print(txt) ``` Popular meta data: * title * length * sentences *
+words * verbs * nouns * symbols * punctuations
```

### Comparing `speakleash-0.3.5/README.md` & `speakleash-0.3.51/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,37 +8,40 @@
     <a href="https://pypi.org/project/speakleash"><img src="https://img.shields.io/badge/python-_>=_3.6-blue"></a>
     <a href="https://speakleash.org/dashboard/"><img src="https://img.shields.io/badge/dynamic/json?url=https://cutt.ly/ywcfnFY7&query=datasetsGB&suffix=%20GB&label=datasets&color=brightgreen"></a>
     <a href="https://speakleash.org/spolecznosc-i-kontakt/"><img src="https://img.shields.io/discord/1043112910278381619?logo=discord&label=discord&color=%23603FEF"></a>
 </p>
 
 ### UPDATE 05.05.2024: 
 Due to the changes related with the hosting, it is recommended to update the version of the package to the newest one, using command:
-```python
+```bash
 pip install --upgrade speakleash
 ```
 
-[SpeakLeash](href="https://pypi.org/project/speakleash) is a lightweight library providing datasets for the Polish language
-and tools to make them useful.
+[SpeakLeash](https://pypi.org/project/speakleash) is a lightweight library providing datasets for the Polish language
+and tools to make them useful:
 
 - **Website:** https://speakleash.org/
 - **Datasets:** https://speakleash.org/dashboard/
 - **Source code:** https://github.com/speakleash/speakleash
 - **Data in action:** https://github.com/speakleash/speakleash-examples
 - **Bug reports:** https://github.com/speakleash/speakleash/issues
 
-## Installation
+Installation
+----------------------
 
 Speakleash package can be installed from PyPi and has to be installed in a virtual environment:
-```python
+
+```bash
 pip install speakleash
 ```
 
-## Basic Usage
+Basic Usage
+----------------------
 
-If you just want to see the details of the datasets
+If you just want to see the details of the datasets:
 
 ```python
 from speakleash import Speakleash
 import os
 
 base_dir = os.path.join(os.path.dirname(__file__))
 replicate_to = os.path.join(base_dir, "datasets")
@@ -46,36 +49,39 @@
 sl = Speakleash(replicate_to)
 
 for d in sl.datasets:
     size_mb = round(d.characters/1024/1024)
     print("Dataset: {0}, size: {1} MB, characters: {2}, documents: {3}".format(d.name, size_mb, d.characters, d.documents))
 ```
 
-You can use individual properties (e.g.:***characters***, ***documents***), but you can display the entire manifest
+You can use individual properties (e.g.:***characters***, ***documents***), but you can display the entire manifest:
+
 ```python
 sl = Speakleash(replicate_to)
 print(sl.get("plwiki").manifest)
 ```
 
-If you chose one of them (***.get(name of dataset)***) then you will get a lot of text data ;-)
+If you chose one of them (***.get(name of dataset)***) then you will get a lot of text data:
+
 ```python
 from speakleash import Speakleash
 import os
 
 base_dir = os.path.join(os.path.dirname(__file__))
 replicate_to = os.path.join(base_dir, "datasets")
 
 sl = Speakleash(replicate_to)
 
 wiki = sl.get("plwiki").data
 for doc in wiki:
     print(doc[:40])
 ```
 
-If you also need meta data then use the ***ext_data*** property
+If you also need meta data then use the ***ext_data*** property:
+
 ```python
 ds = sl.get("plwiki").ext_data
 for doc in ds:
     print(doc)
     txt, meta = doc
     print(meta.get("title"))
     print(txt)
```

#### html2text {}

```diff
@@ -5,32 +5,33 @@
  _o_r_g_a_n_i_s_a_t_i_o_n_-_S_p_e_a_k_l_e_a_s_h_-_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-___>_=___3_._6_-
      _b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_d_y_n_a_m_i_c_/_j_s_o_n_?_u_r_l_=_h_t_t_p_s_:_/_/_c_u_t_t_._l_y_/
 _y_w_c_f_n_F_Y_7_&_q_u_e_r_y_=_d_a_t_a_s_e_t_s_G_B_&_s_u_f_f_i_x_=_%_2_0_G_B_&_l_a_b_e_l_=_d_a_t_a_s_e_t_s_&_c_o_l_o_r_=_b_r_i_g_h_t_g_r_e_e_n_]_[_h_t_t_p_s_:
                            _/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_i_s_c_o_r_d_/
         _1_0_4_3_1_1_2_9_1_0_2_7_8_3_8_1_6_1_9_?_l_o_g_o_=_d_i_s_c_o_r_d_&_l_a_b_e_l_=_d_i_s_c_o_r_d_&_c_o_l_o_r_=_%_2_3_6_0_3_F_E_F_]
 ### UPDATE 05.05.2024: Due to the changes related with the hosting, it is
 recommended to update the version of the package to the newest one, using
-command: ```python pip install --upgrade speakleash ``` [SpeakLeash]
-(href="https://pypi.org/project/speakleash) is a lightweight library providing
-datasets for the Polish language and tools to make them useful. - **Website:**
-https://speakleash.org/ - **Datasets:** https://speakleash.org/dashboard/ -
-**Source code:** https://github.com/speakleash/speakleash - **Data in action:**
-https://github.com/speakleash/speakleash-examples - **Bug reports:** https://
-github.com/speakleash/speakleash/issues ## Installation Speakleash package can
-be installed from PyPi and has to be installed in a virtual environment:
-```python pip install speakleash ``` ## Basic Usage If you just want to see the
-details of the datasets ```python from speakleash import Speakleash import os
-base_dir = os.path.join(os.path.dirname(__file__)) replicate_to = os.path.join
-(base_dir, "datasets") sl = Speakleash(replicate_to) for d in sl.datasets:
-size_mb = round(d.characters/1024/1024) print("Dataset: {0}, size: {1} MB,
-characters: {2}, documents: {3}".format(d.name, size_mb, d.characters,
-d.documents)) ``` You can use individual properties (e.g.:***characters***,
-***documents***), but you can display the entire manifest ```python sl =
-Speakleash(replicate_to) print(sl.get("plwiki").manifest) ``` If you chose one
-of them (***.get(name of dataset)***) then you will get a lot of text data ;-
-) ```python from speakleash import Speakleash import os base_dir = os.path.join
-(os.path.dirname(__file__)) replicate_to = os.path.join(base_dir, "datasets")
-sl = Speakleash(replicate_to) wiki = sl.get("plwiki").data for doc in wiki:
-print(doc[:40]) ``` If you also need meta data then use the ***ext_data***
-property ```python ds = sl.get("plwiki").ext_data for doc in ds: print(doc)
-txt, meta = doc print(meta.get("title")) print(txt) ``` Popular meta data: *
-title * length * sentences * words * verbs * nouns * symbols * punctuations
+command: ```bash pip install --upgrade speakleash ``` [SpeakLeash](https://
+pypi.org/project/speakleash) is a lightweight library providing datasets for
+the Polish language and tools to make them useful: - **Website:** https://
+speakleash.org/ - **Datasets:** https://speakleash.org/dashboard/ - **Source
+code:** https://github.com/speakleash/speakleash - **Data in action:** https://
+github.com/speakleash/speakleash-examples - **Bug reports:** https://
+github.com/speakleash/speakleash/issues Installation ---------------------
+- Speakleash package can be installed from PyPi and has to be installed in a
+virtual environment: ```bash pip install speakleash ``` Basic Usage -----------
+----------- If you just want to see the details of the datasets: ```python from
+speakleash import Speakleash import os base_dir = os.path.join(os.path.dirname
+(__file__)) replicate_to = os.path.join(base_dir, "datasets") sl = Speakleash
+(replicate_to) for d in sl.datasets: size_mb = round(d.characters/1024/1024)
+print("Dataset: {0}, size: {1} MB, characters: {2}, documents: {3}".format
+(d.name, size_mb, d.characters, d.documents)) ``` You can use individual
+properties (e.g.:***characters***, ***documents***), but you can display the
+entire manifest: ```python sl = Speakleash(replicate_to) print(sl.get
+("plwiki").manifest) ``` If you chose one of them (***.get(name of dataset)***)
+then you will get a lot of text data: ```python from speakleash import
+Speakleash import os base_dir = os.path.join(os.path.dirname(__file__))
+replicate_to = os.path.join(base_dir, "datasets") sl = Speakleash(replicate_to)
+wiki = sl.get("plwiki").data for doc in wiki: print(doc[:40]) ``` If you also
+need meta data then use the ***ext_data*** property: ```python ds = sl.get
+("plwiki").ext_data for doc in ds: print(doc) txt, meta = doc print(meta.get
+("title")) print(txt) ``` Popular meta data: * title * length * sentences *
+words * verbs * nouns * symbols * punctuations
```

### Comparing `speakleash-0.3.5/speakleash/__init__.py` & `speakleash-0.3.51/speakleash/__init__.py`

 * *Files identical despite different names*

### Comparing `speakleash-0.3.5/speakleash/category_manager/category_manager.py` & `speakleash-0.3.51/speakleash/category_manager/category_manager.py`

 * *Files identical despite different names*

### Comparing `speakleash-0.3.5/speakleash/config_loader.py` & `speakleash-0.3.51/speakleash/config_loader.py`

 * *Files identical despite different names*

### Comparing `speakleash-0.3.5/speakleash/contrib.py` & `speakleash-0.3.51/speakleash/contrib.py`

 * *Files identical despite different names*

### Comparing `speakleash-0.3.5/speakleash/core/core.py` & `speakleash-0.3.51/speakleash/core/core.py`

 * *Files identical despite different names*

### Comparing `speakleash-0.3.5/speakleash/dataset/dataset.py` & `speakleash-0.3.51/speakleash/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `speakleash-0.3.5/speakleash/downloader/structure_downloader.py` & `speakleash-0.3.51/speakleash/downloader/structure_downloader.py`

 * *Files identical despite different names*

### Comparing `speakleash-0.3.5/speakleash.egg-info/PKG-INFO` & `speakleash-0.3.51/speakleash.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: speakleash
-Version: 0.3.5
+Version: 0.3.51
 Summary: SpeakLeash agnostic dataset for Polish
 Home-page: https://github.com/speakleash/speakleash
 Author: SpeakLeash Team
 Author-email: team@speakleash.org
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: tqdm
-Requires-Dist: lm_dataformat
 
 <h1 align="center">
 <img src="https://raw.githubusercontent.com/speakleash/speakleash/main/branding/logo/speakleash_logo.png" width="300">
 </h1><br>
 
 <p align="center">
     <a href="https://pypi.org/project/speakleash"><img src="https://badge.fury.io/py/speakleash.svg"></a>
@@ -22,37 +21,40 @@
     <a href="https://pypi.org/project/speakleash"><img src="https://img.shields.io/badge/python-_>=_3.6-blue"></a>
     <a href="https://speakleash.org/dashboard/"><img src="https://img.shields.io/badge/dynamic/json?url=https://cutt.ly/ywcfnFY7&query=datasetsGB&suffix=%20GB&label=datasets&color=brightgreen"></a>
     <a href="https://speakleash.org/spolecznosc-i-kontakt/"><img src="https://img.shields.io/discord/1043112910278381619?logo=discord&label=discord&color=%23603FEF"></a>
 </p>
 
 ### UPDATE 05.05.2024: 
 Due to the changes related with the hosting, it is recommended to update the version of the package to the newest one, using command:
-```python
+```bash
 pip install --upgrade speakleash
 ```
 
-[SpeakLeash](href="https://pypi.org/project/speakleash) is a lightweight library providing datasets for the Polish language
-and tools to make them useful.
+[SpeakLeash](https://pypi.org/project/speakleash) is a lightweight library providing datasets for the Polish language
+and tools to make them useful:
 
 - **Website:** https://speakleash.org/
 - **Datasets:** https://speakleash.org/dashboard/
 - **Source code:** https://github.com/speakleash/speakleash
 - **Data in action:** https://github.com/speakleash/speakleash-examples
 - **Bug reports:** https://github.com/speakleash/speakleash/issues
 
-## Installation
+Installation
+----------------------
 
 Speakleash package can be installed from PyPi and has to be installed in a virtual environment:
-```python
+
+```bash
 pip install speakleash
 ```
 
-## Basic Usage
+Basic Usage
+----------------------
 
-If you just want to see the details of the datasets
+If you just want to see the details of the datasets:
 
 ```python
 from speakleash import Speakleash
 import os
 
 base_dir = os.path.join(os.path.dirname(__file__))
 replicate_to = os.path.join(base_dir, "datasets")
@@ -60,36 +62,39 @@
 sl = Speakleash(replicate_to)
 
 for d in sl.datasets:
     size_mb = round(d.characters/1024/1024)
     print("Dataset: {0}, size: {1} MB, characters: {2}, documents: {3}".format(d.name, size_mb, d.characters, d.documents))
 ```
 
-You can use individual properties (e.g.:***characters***, ***documents***), but you can display the entire manifest
+You can use individual properties (e.g.:***characters***, ***documents***), but you can display the entire manifest:
+
 ```python
 sl = Speakleash(replicate_to)
 print(sl.get("plwiki").manifest)
 ```
 
-If you chose one of them (***.get(name of dataset)***) then you will get a lot of text data ;-)
+If you chose one of them (***.get(name of dataset)***) then you will get a lot of text data:
+
 ```python
 from speakleash import Speakleash
 import os
 
 base_dir = os.path.join(os.path.dirname(__file__))
 replicate_to = os.path.join(base_dir, "datasets")
 
 sl = Speakleash(replicate_to)
 
 wiki = sl.get("plwiki").data
 for doc in wiki:
     print(doc[:40])
 ```
 
-If you also need meta data then use the ***ext_data*** property
+If you also need meta data then use the ***ext_data*** property:
+
 ```python
 ds = sl.get("plwiki").ext_data
 for doc in ds:
     print(doc)
     txt, meta = doc
     print(meta.get("title"))
     print(txt)
@@ -101,7 +106,9 @@
 * length
 * sentences
 * words
 * verbs
 * nouns
 * symbols
 * punctuations
+
+
```

#### html2text {}

```diff
@@ -1,41 +1,42 @@
-Metadata-Version: 2.1 Name: speakleash Version: 0.3.5 Summary: SpeakLeash
+Metadata-Version: 2.1 Name: speakleash Version: 0.3.51 Summary: SpeakLeash
 agnostic dataset for Polish Home-page: https://github.com/speakleash/speakleash
-Author: SpeakLeash Team Author-email: team@speakleash.org Requires-Python:
->=3.6 Description-Content-Type: text/markdown License-File: LICENSE Requires-
-Dist: requests Requires-Dist: tqdm Requires-Dist: lm_dataformat
+Author: SpeakLeash Team Author-email: team@speakleash.org License: UNKNOWN
+Platform: UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE
 ************ [[hhttttppss::////rraaww..ggiitthhuubbuusseerrccoonntteenntt..ccoomm//ssppeeaakklleeaasshh//ssppeeaakklleeaasshh//mmaaiinn//bbrraannddiinngg//
                        llooggoo//ssppeeaakklleeaasshh__llooggoo..ppnngg]] ************
 
     _[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_s_p_e_a_k_l_e_a_s_h_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
  _o_r_g_a_n_i_s_a_t_i_o_n_-_S_p_e_a_k_l_e_a_s_h_-_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-___>_=___3_._6_-
      _b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_d_y_n_a_m_i_c_/_j_s_o_n_?_u_r_l_=_h_t_t_p_s_:_/_/_c_u_t_t_._l_y_/
 _y_w_c_f_n_F_Y_7_&_q_u_e_r_y_=_d_a_t_a_s_e_t_s_G_B_&_s_u_f_f_i_x_=_%_2_0_G_B_&_l_a_b_e_l_=_d_a_t_a_s_e_t_s_&_c_o_l_o_r_=_b_r_i_g_h_t_g_r_e_e_n_]_[_h_t_t_p_s_:
                            _/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_d_i_s_c_o_r_d_/
         _1_0_4_3_1_1_2_9_1_0_2_7_8_3_8_1_6_1_9_?_l_o_g_o_=_d_i_s_c_o_r_d_&_l_a_b_e_l_=_d_i_s_c_o_r_d_&_c_o_l_o_r_=_%_2_3_6_0_3_F_E_F_]
 ### UPDATE 05.05.2024: Due to the changes related with the hosting, it is
 recommended to update the version of the package to the newest one, using
-command: ```python pip install --upgrade speakleash ``` [SpeakLeash]
-(href="https://pypi.org/project/speakleash) is a lightweight library providing
-datasets for the Polish language and tools to make them useful. - **Website:**
-https://speakleash.org/ - **Datasets:** https://speakleash.org/dashboard/ -
-**Source code:** https://github.com/speakleash/speakleash - **Data in action:**
-https://github.com/speakleash/speakleash-examples - **Bug reports:** https://
-github.com/speakleash/speakleash/issues ## Installation Speakleash package can
-be installed from PyPi and has to be installed in a virtual environment:
-```python pip install speakleash ``` ## Basic Usage If you just want to see the
-details of the datasets ```python from speakleash import Speakleash import os
-base_dir = os.path.join(os.path.dirname(__file__)) replicate_to = os.path.join
-(base_dir, "datasets") sl = Speakleash(replicate_to) for d in sl.datasets:
-size_mb = round(d.characters/1024/1024) print("Dataset: {0}, size: {1} MB,
-characters: {2}, documents: {3}".format(d.name, size_mb, d.characters,
-d.documents)) ``` You can use individual properties (e.g.:***characters***,
-***documents***), but you can display the entire manifest ```python sl =
-Speakleash(replicate_to) print(sl.get("plwiki").manifest) ``` If you chose one
-of them (***.get(name of dataset)***) then you will get a lot of text data ;-
-) ```python from speakleash import Speakleash import os base_dir = os.path.join
-(os.path.dirname(__file__)) replicate_to = os.path.join(base_dir, "datasets")
-sl = Speakleash(replicate_to) wiki = sl.get("plwiki").data for doc in wiki:
-print(doc[:40]) ``` If you also need meta data then use the ***ext_data***
-property ```python ds = sl.get("plwiki").ext_data for doc in ds: print(doc)
-txt, meta = doc print(meta.get("title")) print(txt) ``` Popular meta data: *
-title * length * sentences * words * verbs * nouns * symbols * punctuations
+command: ```bash pip install --upgrade speakleash ``` [SpeakLeash](https://
+pypi.org/project/speakleash) is a lightweight library providing datasets for
+the Polish language and tools to make them useful: - **Website:** https://
+speakleash.org/ - **Datasets:** https://speakleash.org/dashboard/ - **Source
+code:** https://github.com/speakleash/speakleash - **Data in action:** https://
+github.com/speakleash/speakleash-examples - **Bug reports:** https://
+github.com/speakleash/speakleash/issues Installation ---------------------
+- Speakleash package can be installed from PyPi and has to be installed in a
+virtual environment: ```bash pip install speakleash ``` Basic Usage -----------
+----------- If you just want to see the details of the datasets: ```python from
+speakleash import Speakleash import os base_dir = os.path.join(os.path.dirname
+(__file__)) replicate_to = os.path.join(base_dir, "datasets") sl = Speakleash
+(replicate_to) for d in sl.datasets: size_mb = round(d.characters/1024/1024)
+print("Dataset: {0}, size: {1} MB, characters: {2}, documents: {3}".format
+(d.name, size_mb, d.characters, d.documents)) ``` You can use individual
+properties (e.g.:***characters***, ***documents***), but you can display the
+entire manifest: ```python sl = Speakleash(replicate_to) print(sl.get
+("plwiki").manifest) ``` If you chose one of them (***.get(name of dataset)***)
+then you will get a lot of text data: ```python from speakleash import
+Speakleash import os base_dir = os.path.join(os.path.dirname(__file__))
+replicate_to = os.path.join(base_dir, "datasets") sl = Speakleash(replicate_to)
+wiki = sl.get("plwiki").data for doc in wiki: print(doc[:40]) ``` If you also
+need meta data then use the ***ext_data*** property: ```python ds = sl.get
+("plwiki").ext_data for doc in ds: print(doc) txt, meta = doc print(meta.get
+("title")) print(txt) ``` Popular meta data: * title * length * sentences *
+words * verbs * nouns * symbols * punctuations
```

### Comparing `speakleash-0.3.5/speakleash.egg-info/SOURCES.txt` & `speakleash-0.3.51/speakleash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

