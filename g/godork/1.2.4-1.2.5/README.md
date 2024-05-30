# Comparing `tmp/godork-1.2.4.tar.gz` & `tmp/godork-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godork-1.2.4.tar", last modified: Tue May 21 09:16:38 2024, max compression
+gzip compressed data, was "godork-1.2.5.tar", last modified: Thu May 30 22:15:40 2024, max compression
```

## Comparing `godork-1.2.4.tar` & `godork-1.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-21 09:16:38.954470 godork-1.2.4/
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     1069 2024-05-21 09:10:59.000000 godork-1.2.4/LICENSE
--rw-r--r--   0 thd3r     (1000) thd3r     (1000)     3257 2024-05-21 09:16:38.954470 godork-1.2.4/PKG-INFO
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     2849 2024-05-21 09:10:59.000000 godork-1.2.4/README.md
-drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-21 09:16:38.954470 godork-1.2.4/godork.egg-info/
--rw-r--r--   0 thd3r     (1000) thd3r     (1000)     3257 2024-05-21 09:16:38.000000 godork-1.2.4/godork.egg-info/PKG-INFO
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)      238 2024-05-21 09:16:38.000000 godork-1.2.4/godork.egg-info/SOURCES.txt
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)        1 2024-05-21 09:16:38.000000 godork-1.2.4/godork.egg-info/dependency_links.txt
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       43 2024-05-21 09:16:38.000000 godork-1.2.4/godork.egg-info/entry_points.txt
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       29 2024-05-21 09:16:38.000000 godork-1.2.4/godork.egg-info/requires.txt
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)        4 2024-05-21 09:16:38.000000 godork-1.2.4/godork.egg-info/top_level.txt
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       38 2024-05-21 09:16:38.954470 godork-1.2.4/setup.cfg
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)      717 2024-05-21 09:10:59.000000 godork-1.2.4/setup.py
-drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-21 09:16:38.954470 godork-1.2.4/src/
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       27 2024-05-21 09:10:59.000000 godork-1.2.4/src/__init__.py
--rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     6713 2024-05-21 09:12:47.000000 godork-1.2.4/src/godork.py
+drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-30 22:15:40.273188 godork-1.2.5/
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     1069 2024-05-30 21:52:15.000000 godork-1.2.5/LICENSE
+-rw-r--r--   0 thd3r     (1000) thd3r     (1000)     2499 2024-05-30 22:15:40.273188 godork-1.2.5/PKG-INFO
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     2091 2024-05-30 22:11:23.000000 godork-1.2.5/README.md
+drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-30 22:15:40.273188 godork-1.2.5/godork.egg-info/
+-rw-r--r--   0 thd3r     (1000) thd3r     (1000)     2499 2024-05-30 22:15:40.000000 godork-1.2.5/godork.egg-info/PKG-INFO
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)      238 2024-05-30 22:15:40.000000 godork-1.2.5/godork.egg-info/SOURCES.txt
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)        1 2024-05-30 22:15:40.000000 godork-1.2.5/godork.egg-info/dependency_links.txt
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       43 2024-05-30 22:15:40.000000 godork-1.2.5/godork.egg-info/entry_points.txt
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       29 2024-05-30 22:15:40.000000 godork-1.2.5/godork.egg-info/requires.txt
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)        4 2024-05-30 22:15:40.000000 godork-1.2.5/godork.egg-info/top_level.txt
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       38 2024-05-30 22:15:40.273188 godork-1.2.5/setup.cfg
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)      717 2024-05-30 21:52:15.000000 godork-1.2.5/setup.py
+drwxrwxr-x   0 thd3r     (1000) thd3r     (1000)        0 2024-05-30 22:15:40.273188 godork-1.2.5/src/
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)       27 2024-05-30 21:52:15.000000 godork-1.2.5/src/__init__.py
+-rw-rw-r--   0 thd3r     (1000) thd3r     (1000)     6714 2024-05-30 21:52:15.000000 godork-1.2.5/src/godork.py
```

### Comparing `godork-1.2.4/LICENSE` & `godork-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `godork-1.2.4/README.md` & `godork-1.2.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,72 @@
+Metadata-Version: 2.1
+Name: godork
+Version: 1.2.5
+Summary: Scrape Google search quickly
+Home-page: https://github.com/thd3r/godork
+Author: Thunder (@thd3r)
+Author-email: thd3r@proton.me
+License: MIT
+Keywords: godork,google dorks,google dork,google dorking
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp
+Requires-Dist: asyncio
+Requires-Dist: requests
+Requires-Dist: bs4
+
 <h1 align="center">
   Godork - Scrape Google search quickly
 </h1>
 
 <div align="center">
-  <img src="https://raw.githubusercontent.com/thd3r/godork/master/assets/images/godork-logo.png" alt="godork" width="300px">
-</div>
-
-<div align="center">
   <a href="https://python.org"><img src="https://img.shields.io/badge/Built%20with-Python-Blue"></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/license-MIT-_red.svg"></a>
   <a href="https://github.com/thd3r/godork/releases"><img src="https://img.shields.io/github/release/thd3r/godork.svg"></a>
   <a href="https://pypi.python.org/pypi/godork/"><img src="https://img.shields.io/pypi/v/godork.svg"></a>
   <a href="https://github.com/thd3r/godork/issues?q=is%3Aissue+is%3Aclosed"><img src="https://img.shields.io/github/issues-closed-raw/thd3r/godork?color=dark-green&label=issues%20fixed"></a>
-  <a href="https://github.com/thd3r/godork/tree/master?tab=readme-ov-file#contributing"><img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat"></a>
 </div>
 
 # About
 
-**Godork** can scrape results from google searches quickly by using the [asyncio](https://docs.python.org/3/library/asyncio.html) library which uses cooperative multitasking in combination with [aiohttp](https://docs.aiohttp.org) and with this tool you can extract links including their titles. This tool is also able to bypass prohibitions made by providers
+**Godork** is a tool that can quickly scrape Google search results using the [asyncio](https://docs.python.org/3/library/asyncio.html) library that uses cooperative multitasking combined with [aiohttp](https://docs.aiohttp.org) and with this tool you can extract links including their titles. This tool is also able to bypass the bans made by the provider
 
 # Installation
 
 **Godork** requires **python 3.8** or higher to install successfully
 
 ### Using Github repo
 
 ```sh
-git clone https://github.com/thd3r/godork.git && python3 setup.py install
+git clone https://github.com/thd3r/godork.git
+cd codork
+python3 setup.py install
 ```
 
 ### Using pip
 
 ```sh
 pip install godork
 ```
 
 # Usage
 
-```sh
-python3 godork.py -help
-```
-
 ### This will display help for the tool. Here are all the switches it supports.
 
+```sh
+python godork.py -help
+```
 
 ```console
-                __         __  
-  ___ ____  ___/ /__  ____/ /__
- / _ `/ _ \/ _  / _ \/ __/  '_/
- \_, /\___/\_,_/\___/_/ /_/\_\ 
-/___/                                                                                                            
-        v1.2.3 - @thd3r
-
-usage: godork [ -query [default arguments] ] [ arguments ] 
-
 Options:
   -help         show this help message and exit
   -version      show program's version number and exit
   -query QUERY  search query
   -sleep        use this option to prevent banning
   -proxy PROXY  http proxy to use with godork (eg http://127.0.0.1:8080) 
 ```
 
-# Documentation
-
-Documentation is available at https://thd3r.github.io
-
-# Contributing
-
-Contributions are welcome! If you want to contribute to **Godork** don't forget to Fork the repository
-
 # Support
 
-### Support me on 
+### Buy me a coffe
 
-<a href="https://coindrop.to/thd3r" target="_blank">
-  <img src="https://coindrop.to/embed-button.png" style="border-radius: 10px; height: 57px !important;width: 200px !important;" alt="Coindrop.to me"></img>
-</a>
+<script type="text/javascript" src="https://cdnjs.buymeacoffee.com/1.0.0/button.prod.min.js" data-name="bmc-button" data-slug="thd3r" data-color="#FFDD00" data-emoji=""  data-font="Cookie" data-text="Buy me a coffee" data-outline-color="#000000" data-font-color="#000000" data-coffee-color="#ffffff"></script>
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
+Metadata-Version: 2.1 Name: godork Version: 1.2.5 Summary: Scrape Google search
+quickly Home-page: https://github.com/thd3r/godork Author: Thunder (@thd3r)
+Author-email: thd3r@proton.me License: MIT Keywords: godork,google dorks,google
+dork,google dorking Description-Content-Type: text/markdown License-File:
+LICENSE Requires-Dist: aiohttp Requires-Dist: asyncio Requires-Dist: requests
+Requires-Dist: bs4
               ************ GGooddoorrkk -- SSccrraappee GGooooggllee sseeaarrcchh qquuiicckkllyy ************
-                                   [godork]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_B_u_i_l_t_%_2_0_w_i_t_h_-_P_y_t_h_o_n_-_B_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
    _b_a_d_g_e_/_l_i_c_e_n_s_e_-_M_I_T_-___r_e_d_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/_t_h_d_3_r_/
  _g_o_d_o_r_k_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_g_o_d_o_r_k_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
  _g_i_t_h_u_b_/_i_s_s_u_e_s_-_c_l_o_s_e_d_-_r_a_w_/_t_h_d_3_r_/_g_o_d_o_r_k_?_c_o_l_o_r_=_d_a_r_k_-_g_r_e_e_n_&_l_a_b_e_l_=_i_s_s_u_e_s_%_2_0_f_i_x_e_d_]
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_n_t_r_i_b_u_t_i_o_n_s_-_w_e_l_c_o_m_e_-_b_r_i_g_h_t_g_r_e_e_n_._s_v_g_?_s_t_y_l_e_=_f_l_a_t_]
-# About **Godork** can scrape results from google searches quickly by using the
-[asyncio](https://docs.python.org/3/library/asyncio.html) library which uses
-cooperative multitasking in combination with [aiohttp](https://
+# About **Godork** is a tool that can quickly scrape Google search results
+using the [asyncio](https://docs.python.org/3/library/asyncio.html) library
+that uses cooperative multitasking combined with [aiohttp](https://
 docs.aiohttp.org) and with this tool you can extract links including their
-titles. This tool is also able to bypass prohibitions made by providers #
+titles. This tool is also able to bypass the bans made by the provider #
 Installation **Godork** requires **python 3.8** or higher to install
 successfully ### Using Github repo ```sh git clone https://github.com/thd3r/
-godork.git && python3 setup.py install ``` ### Using pip ```sh pip install
-godork ``` # Usage ```sh python3 godork.py -help ``` ### This will display help
-for the tool. Here are all the switches it supports. ```console __ __ ___ ____
-___/ /__ ____/ /__ / _ `/ _ \/ _ / _ \/ __/ '_/ \_, /\___/\_,_/\___/_/ /_/\_\ /
-___/ v1.2.3 - @thd3r usage: godork [ -query [default arguments] ] [ arguments ]
+godork.git cd codork python3 setup.py install ``` ### Using pip ```sh pip
+install godork ``` # Usage ### This will display help for the tool. Here are
+all the switches it supports. ```sh python godork.py -help ``` ```console
 Options: -help show this help message and exit -version show program's version
 number and exit -query QUERY search query -sleep use this option to prevent
 banning -proxy PROXY http proxy to use with godork (eg http://127.0.0.1:8080)
-``` # Documentation Documentation is available at https://thd3r.github.io #
-Contributing Contributions are welcome! If you want to contribute to **Godork**
-don't forget to Fork the repository # Support ### Support me on_[_C_o_i_n_d_r_o_p_._t_o_ _m_e_]
+``` # Support ### Buy me a coffe
```

### Comparing `godork-1.2.4/setup.py` & `godork-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `godork-1.2.4/src/godork.py` & `godork-1.2.5/src/godork.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import asyncio # v3.4.3
 import random
 import time
 import json
 import os
 
-__version__ = "1.2.4"
+__version__ = "1.2.5"
 
 class OptionsArgs(object):
     
     def __init__(self):
         self.parser = ArgumentParser(
             prog="godork",
             add_help=False,
@@ -104,15 +104,15 @@
             "anonymous",
             "python",
             "aiorequest",
         ]
         return random.choice(words).strip()
 
     def regexp(self, html):
-        return findall('"><a href="\/url\?q=(.*?)&amp;sa=U&amp;', html)
+        return findall(r'\"><a href=\"\/url\?q=(.*?)&amp', html)
 
     def params(self, q, p):
         return {
             "q": q,                 
             "start": p, # parameter defines the maximum number of results to return
         }
     
@@ -157,15 +157,15 @@
             self.should_sleep() # Sleep to prevent banning
             async with session.get(
                 url=url,
                 params=params,
                 proxy=self.proxy,
                 allow_redirects=False,
                 headers={
-                    "User-Agent": f"{self.random_words()}/1.2.0",
+                    "User-Agent": f"{self.random_words()}/{__version__}",
                     "Referer": "https://www.google.com/"
                 },
                 ) as resp:
                 html = await resp.text()
                 if self.banned(html):
                     raise RuntimeError("[\033[91mERR\033[0m] Your IP address has been blocked by a search engine provider")
                 if resp.status != 200:
```

