# Comparing `tmp/askchat-1.1.5.tar.gz` & `tmp/askchat-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "askchat-1.1.5.tar", last modified: Tue May 14 16:02:49 2024, max compression
+gzip compressed data, was "askchat-1.1.6.tar", last modified: Fri May 31 15:45:29 2024, max compression
```

## Comparing `askchat-1.1.5.tar` & `askchat-1.1.6.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:49.534645 askchat-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-14 16:02:41.000000 askchat-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-14 16:02:41.000000 askchat-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-14 16:02:49.534645 askchat-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-14 16:02:41.000000 askchat-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:49.530645 askchat-1.1.5/askchat/
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-14 16:02:41.000000 askchat-1.1.5/askchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-14 16:02:41.000000 askchat-1.1.5/askchat/ask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-14 16:02:41.000000 askchat-1.1.5/askchat/askenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8941 2024-05-14 16:02:41.000000 askchat-1.1.5/askchat/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:49.530645 askchat-1.1.5/askchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-14 16:02:49.000000 askchat-1.1.5/askchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-14 16:02:49.000000 askchat-1.1.5/askchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:02:49.000000 askchat-1.1.5/askchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-14 16:02:49.000000 askchat-1.1.5/askchat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:02:49.000000 askchat-1.1.5/askchat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 16:02:49.000000 askchat-1.1.5/askchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 16:02:49.000000 askchat-1.1.5/askchat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:49.530645 askchat-1.1.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:49.530645 askchat-1.1.5/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   492951 2024-05-14 16:02:41.000000 askchat-1.1.5/docs/assets/askchat.png
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-14 16:02:49.534645 askchat-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-14 16:02:41.000000 askchat-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:02:49.534645 askchat-1.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 16:02:41.000000 askchat-1.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-14 16:02:41.000000 askchat-1.1.5/tests/test_askchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-14 16:02:41.000000 askchat-1.1.5/tests/test_askenv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:45:29.709206 askchat-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-31 15:45:21.000000 askchat-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-31 15:45:21.000000 askchat-1.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-31 15:45:29.709206 askchat-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-31 15:45:21.000000 askchat-1.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:45:29.705206 askchat-1.1.6/askchat/
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-31 15:45:21.000000 askchat-1.1.6/askchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-31 15:45:21.000000 askchat-1.1.6/askchat/ask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-31 15:45:21.000000 askchat-1.1.6/askchat/askenv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-05-31 15:45:21.000000 askchat-1.1.6/askchat/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:45:29.705206 askchat-1.1.6/askchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-31 15:45:29.000000 askchat-1.1.6/askchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-31 15:45:29.000000 askchat-1.1.6/askchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:45:29.000000 askchat-1.1.6/askchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-31 15:45:29.000000 askchat-1.1.6/askchat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:45:29.000000 askchat-1.1.6/askchat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 15:45:29.000000 askchat-1.1.6/askchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 15:45:29.000000 askchat-1.1.6/askchat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:45:29.705206 askchat-1.1.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:45:29.709206 askchat-1.1.6/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   492951 2024-05-31 15:45:21.000000 askchat-1.1.6/docs/assets/askchat.png
+-rw-r--r--   0 runner    (1001) docker     (127)   716419 2024-05-31 15:45:21.000000 askchat-1.1.6/docs/assets/jupyter.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-31 15:45:29.709206 askchat-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-31 15:45:21.000000 askchat-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:45:29.709206 askchat-1.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-31 15:45:21.000000 askchat-1.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-31 15:45:21.000000 askchat-1.1.6/tests/test_askchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-31 15:45:21.000000 askchat-1.1.6/tests/test_askenv.py
```

### Comparing `askchat-1.1.5/LICENSE` & `askchat-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `askchat-1.1.5/PKG-INFO` & `askchat-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: askchat
-Version: 1.1.5
+Version: 1.1.6
 Summary: Interact with ChatGPT in terminal via chattool
 Home-page: https://github.com/cubenlp/askchat
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: UNKNOWN
 Keywords: askchat
```

### Comparing `askchat-1.1.5/README.md` & `askchat-1.1.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -17,17 +17,25 @@
 
 <div align="center">
 <img src="docs/assets/askchat.png" alt="Ask Chat" width="256">
 
 [English](README-en.md) | [简体中文](README.md)
 </div>
 
-在终端与 ChatGPT 交互，随时随地调用 ChatGPT。
+通过命令行运行的 ChatGPT 交互工具，随时随地调用 ChatGPT。
 
-![hello](docs/assets/svgs/hello.svg)
+<div align="center">
+    <div style="margin-top: 10px; color: #555;">终端调用</div>
+    <img src="docs/assets/svgs/hello.svg" alt="hello" width="480">
+</div>
+
+<div align="center">
+    <div style="margin-top: 10px; color: #555;">Jupyter Lab</div>
+    <img src="docs/assets/jupyter.gif" alt="jupyter" width="480">
+</div>
 
 ## 安装及配置
 
 ```bash
 pip install askchat --upgrade
 ```
 
@@ -54,25 +62,33 @@
 
 ## AskChat
 
 `askchat` 支持 API 调试，对话管理等功能。
 
 ### 使用示例
 
-1. API 调试，测试默认参数和返回结果。
-    ![debug](docs/assets/svgs/debug.svg)
+<div align="center">
+    <div style="margin-top: 10px; color: #555;">1. API 调试</div>
+    <img src="docs/assets/svgs/debug.svg" alt="debug" width="480">
+</div>
 
-2. 获取可用模型列表。
-    ![validmodels](docs/assets/svgs/validmodels.svg)
+<div align="center">
+    <div style="margin-top: 10px; color: #555;">2. 获取可用模型列表</div>
+    <img src="docs/assets/svgs/validmodels.svg" alt="validmodels" width="480">
+</div>
 
-3. 多轮对话，保存对话，加载对话等。
-    ![chatlog](docs/assets/svgs/chatlog.svg)
+<div align="center">
+    <div style="margin-top: 10px; color: #555;">3. 多轮对话，保存对话，加载对话等</div>
+    <img src="docs/assets/svgs/chatlog.svg" alt="chatlog" width="480">
+</div>
 
-4. 指定参数，使用不同的模型和 API。
-    ![para-models](docs/assets/svgs/para-models.svg)
+<div align="center">
+    <div style="margin-top: 10px; color: #555;">4. 指定参数，使用不同的模型和 API</div>
+    <img src="docs/assets/svgs/para-models.svg" alt="para-models" width="480">
+</div>
 
 ### 对话管理
 
 用户保存、加载、删除和列出对话历史记录，以及继续之前的对话。
 
 | 参数                | 示例             | 解释                                       |
 |---------------------|------------------|--------------------------------------------|
@@ -118,20 +134,23 @@
 
 ## AskEnv
 
 `askenv` 用于管理不同的环境配置，包括创建、激活、删除等操作，便于在不同的渠道间切换。
 
 ### 示例
 
-1. 创建，查看，激活和删除渠道
-    ![askenv](docs/assets/svgs/askenv.svg)
-
-2. 编辑渠道
-   ![askenv-config](docs/assets/svgs/editenv.svg)
+<div align="center">
+    <div style="margin-top: 10px; color: #555;">1. 创建渠道</div>
+    <img src="docs/assets/svgs/askenv.svg" alt="askenv" width="480">
+</div>
 
+<div align="center">
+    <div style="margin-top: 10px; color: #555;">2. 编辑渠道</div>
+    <img src="docs/assets/svgs/editenv.svg" alt="editenv" width="480">
+</div>
 
 ### 基本用法
 
 1. 创建一个新的环境配置，使用 `new` 命令。
 
     ```bash
     askenv new <name> [-a API_KEY] [-b BASE_URL] [--api-base API_BASE] [-m MODEL]
@@ -176,10 +195,12 @@
 
 7. 更新指定或默认环境配置的一项或多项设置。
 
     ```bash
     askenv config [name] [-a API_KEY] [-b BASE_URL] [--api-base API_BASE] [-m MODEL]
     ```
 
-## 问题和反馈
+## 问
+
+题和反馈
 
 使用过程中有任何问题或建议，欢迎提交 [Issue](https://github.com/cubenlp/askchat/issues)。
```

#### html2text {}

```diff
@@ -1,26 +1,34 @@
 # AskChat
              _[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_T_e_s_t_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]
          [Ask Chat][English](README-en.md) | [ç®ä½ä¸­æ](README.md)
-å¨ç»ç«¯ä¸ ChatGPT äº¤äºï¼éæ¶éå°è°ç¨ ChatGPTã ![hello](docs/
-assets/svgs/hello.svg) ## å®è£åéç½® ```bash pip install askchat --upgrade
-``` éç½®ç¯å¢åéï¼ ```bash export OPENAI_API_KEY="your-api-key" export
+éè¿å½ä»¤è¡è¿è¡ç ChatGPT äº¤äºå·¥å·ï¼éæ¶éå°è°ç¨ ChatGPTã
+                                 ç»ç«¯è°ç¨
+                                    [hello]
+                                  Jupyter Lab
+                                   [jupyter]
+## å®è£åéç½® ```bash pip install askchat --upgrade ```
+éç½®ç¯å¢åéï¼ ```bash export OPENAI_API_KEY="your-api-key" export
 OPENAI_API_BASE="https://api.openai.com/v1" export OPENAI_API_BASE_URL="https:/
 /api.openai.com" export OPENAI_API_MODEL="gpt-3.5-turbo" ```
 æ³¨ï¼`OPENAI_API_BASE` åéä¼åäº `OPENAI_API_BASE_URL`
 åéï¼äºèéä¸å³å¯ã ## ä½¿ç¨æ¹æ³
 ä½¿ç¨ç¯å¢åéï¼è¿è¡ç®åçé®ç­ï¼ ```bash ask hello world ```
 é¤æ­¤ä¹å¤ï¼å¯ä½¿ç¨ `askchat` è¿è¡æ´çµæ´»çå¯¹è¯ï¼ä½¿ç¨ `askenv`
 ç®¡çç¯å¢éç½®ã ## AskChat `askchat` æ¯æ API
-è°è¯ï¼å¯¹è¯ç®¡çç­åè½ã ### ä½¿ç¨ç¤ºä¾ 1. API
-è°è¯ï¼æµè¯é»è®¤åæ°åè¿åç»æã ![debug](docs/assets/svgs/
-debug.svg) 2. è·åå¯ç¨æ¨¡ååè¡¨ã ![validmodels](docs/assets/svgs/
-validmodels.svg) 3. å¤è½®å¯¹è¯ï¼ä¿å­å¯¹è¯ï¼å è½½å¯¹è¯ç­ã ![chatlog]
-(docs/assets/svgs/chatlog.svg) 4. æå®åæ°ï¼ä½¿ç¨ä¸åçæ¨¡åå
-APIã ![para-models](docs/assets/svgs/para-models.svg) ### å¯¹è¯ç®¡ç
+è°è¯ï¼å¯¹è¯ç®¡çç­åè½ã ### ä½¿ç¨ç¤ºä¾
+                                 1. API è°è¯
+                                    [debug]
+                          2. è·åå¯ç¨æ¨¡ååè¡¨
+                                 [validmodels]
+               3. å¤è½®å¯¹è¯ï¼ä¿å­å¯¹è¯ï¼å è½½å¯¹è¯ç­
+                                   [chatlog]
+                4. æå®åæ°ï¼ä½¿ç¨ä¸åçæ¨¡åå API
+                                 [para-models]
+### å¯¹è¯ç®¡ç
 ç¨æ·ä¿å­ãå è½½ãå é¤åååºå¯¹è¯åå²è®°å½ï¼ä»¥åç»§ç»­ä¹åçå¯¹è¯ã
 | åæ° | ç¤ºä¾ | è§£é | |---------------------|------------------|--------
 ------------------------------------| | `-c` | `askchat -c ` |
 ç»§ç»­ä¸ä¸æ¬¡çå¯¹è¯ | | `--regenerate` | `askchat -r` |
 éæ°çæä¸ä¸æ¬¡å¯¹è¯çæååå¤ | | `--load` | `askchat -l ` |
 å è½½åå²å¯¹è¯ | | `--print` | `askchat -p []` |
 æå°ä¸æ¬¡ææå®çå¯¹è¯åå² | | `--save` | `askchat -s ` |
@@ -48,24 +56,27 @@
 -debug` | æå°è°è¯æ¥å¿ | | `--valid-models` | `askchat --valid-models` |
 æå°åå« "gpt" åç§°çæ¨¡ååè¡¨ | | `--all-valid-models` | `askchat --
 all-valid-models` | æå°ææçæ¨¡å | | `--version` | `askchat -v` |
 `askchat` ççæ¬ä¿¡æ¯ | æ³¨ï¼`--all-valid-models`
 ä¼æå°ææå¯ç¨æ¨¡åï¼åæ¬ Embedding, dalle-3, tts ç­ï¼ä½¿ç¨ `--
 valid-models` å¯ä»¥è¿æ»¤æè¿äºã ## AskEnv `askenv`
 ç¨äºç®¡çä¸åçç¯å¢éç½®ï¼åæ¬åå»ºãæ¿æ´»ãå é¤ç­æä½ï¼ä¾¿äºå¨ä¸åçæ¸ éé´åæ¢ã
-### ç¤ºä¾ 1. åå»ºï¼æ¥çï¼æ¿æ´»åå é¤æ¸ é ![askenv](docs/assets/
-svgs/askenv.svg) 2. ç¼è¾æ¸ é ![askenv-config](docs/assets/svgs/editenv.svg)
+### ç¤ºä¾
+                                1. åå»ºæ¸ é
+                                   [askenv]
+                                2. ç¼è¾æ¸ é
+                                   [editenv]
 ### åºæ¬ç¨æ³ 1. åå»ºä¸ä¸ªæ°çç¯å¢éç½®ï¼ä½¿ç¨ `new` å½ä»¤ã
 ```bash askenv new [-a API_KEY] [-b BASE_URL] [--api-base API_BASE] [-m MODEL]
 ``` æèç¨ `askchat --generate-config` ä»ç¯å¢åéçæé»è®¤éç½®ï¼
 ```bash askchat --generate-config ``` 2.
 æ¿æ´»æä¸ªç¯å¢ï¼å°å¶è®¾ç½®ä¸ºå½åä½¿ç¨çéç½®ã ```bash askenv use
 ``` 3. å é¤æå®çç¯å¢éç½®æä»¶ã ```bash askenv delete askenv delete
 --default ``` 4. ååºå½åææå¯ç¨ç¯å¢ã ```bash askenv list ``` 5.
 æ¾ç¤ºæå®ç¯å¢çéç½®ä¿¡æ¯ï¼å¦ææ²¡ææå®ç¯å¢åç§°ï¼åæ¾ç¤ºé»è®¤ç¯å¢çéç½®ã
 ```bash askenv show [name] ``` 6.
 å°å½åæ¿æ´»çç¯å¢éç½®ä¿å­ä¸ºæå®åç§°çéç½®æä»¶ã ```bash
 askenv save ``` 7. æ´æ°æå®æé»è®¤ç¯å¢éç½®çä¸é¡¹æå¤é¡¹è®¾ç½®ã
 ```bash askenv config [name] [-a API_KEY] [-b BASE_URL] [--api-base API_BASE]
-[-m MODEL] ``` ## é®é¢ååé¦
+[-m MODEL] ``` ## é® é¢ååé¦
 ä½¿ç¨è¿ç¨ä¸­æä»»ä½é®é¢æå»ºè®®ï¼æ¬¢è¿æäº¤ [Issue](https://
 github.com/cubenlp/askchat/issues)ã
```

### Comparing `askchat-1.1.5/askchat/__init__.py` & `askchat-1.1.6/askchat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for askchat."""
 
 __author__ = """Rex Wang"""
 __email__ = '1073853456@qq.com'
-__version__ = '1.1.5'
+__version__ = '1.1.6'
 
 import asyncio
 from pathlib import Path
 import click
 from dotenv import set_key
 import os
```

### Comparing `askchat-1.1.5/askchat/askenv.py` & `askchat-1.1.6/askchat/askenv.py`

 * *Files identical despite different names*

### Comparing `askchat-1.1.5/askchat/cli.py` & `askchat-1.1.6/askchat/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,27 +136,27 @@
 @click.option('-a', '--api-key', default=None, help='OpenAI API key')
 @click.option('-u', '--use-env', type=EnvNameCompletionType(), help='Use environment variables from the `~/.askchat/envs`', callback=use_env_callback, expose_value=True)
 # Chat with history
 @click.option('-c', is_flag=True, help='Continue the last conversation')
 @click.option('-r', '--regenerate', is_flag=True, help='Regenerate the last conversation')
 @click.option('-l', '--load', default=None, type=ChatFileCompletionType(), callback=load_chat_callback, expose_value=False, help='Load a conversation from a file')
 # Handling chat history
-@click.option('-p', '--print', is_flag=True, help='Print the last conversation or a specific conversation')
+@click.option('-p', is_flag=True, help='Print the last conversation or a specific conversation')
 @click.option('-s', '--save', callback=save_chat_callback, expose_value=False, help='Save the conversation to a file')
 @click.option('-d', '--delete', type=ChatFileCompletionType(), callback=delete_chat_callback, expose_value=False, help='Delete the conversation from a file')
 @click.option('--list', is_flag=True, callback=list_chats_callback, expose_value=False, help='List all the conversation files')
 # Other options
 @click.option('--generate-config', is_flag=True, callback=generate_config_callback, expose_value=False, help='Generate a configuration file by environment table')
 @click.option('--debug', is_flag=True, callback=debug_log_callback, expose_value=False, help='Print debug log')
 @click.option('--valid-models', is_flag=True, callback=valid_models_callback, expose_value=False, help='Print valid models that contain "gpt" in their names')
 @click.option('--all-valid-models', is_flag=True, callback=all_valid_models_callback, expose_value=False, help='Print all valid models')
 @click.option('-v', '--version', is_flag=True, callback=version_callback, expose_value=False, help='Print the version')
 @click.option('-o', '--option', multiple=True, type=(str, str), help='Additional options for show_resp in the form of key=value')
 def main( message, model, base_url, api_base, api_key, use_env
-        , c, regenerate, print, option):
+        , c, regenerate, p, option):
     """Interact with ChatGPT in terminal via chattool"""
     setup()
     message_text = ' '.join(message).strip()
     if use_env and not message_text: return
     # set values for the environment variables
     if api_key:
         os.environ['OPENAI_API_KEY'] = api_key
@@ -164,15 +164,15 @@
         os.environ['OPENAI_API_BASE_URL'] = base_url
     if api_base:
         os.environ['OPENAI_API_BASE'] = api_base
     if model:
         os.environ['OPENAI_API_MODEL'] = model
     chattool.load_envs() # update the environment variables in chattool
     # print chat messages
-    if print:
+    if p:
         fname = message_text if message_text else '_last_chat'
         fname = f"{CONFIG_PATH}/{fname}.json"
         try:
             Chat().load(fname).print_log()
         except FileNotFoundError:
             click.echo(f"The specified conversation {fname} does not exist.")
         return
@@ -212,12 +212,19 @@
             if key in ints:
                 option[key] = int(value)
             elif key in floats:
                 option[key] = float(value)
     else:
         option = {}
     # Add chat responses
-    chat.assistant(asyncio.run(show_resp(chat, **dict(option))))
+    if option.get('stream') in ['false', 0]:
+        option['stream'] = False
+        chat.getresponse(**option)
+        for text in chat.last_message:
+            print(text, end='', flush=True)
+    else:
+        chat.assistant(asyncio.run(show_resp(chat, **dict(option))))
+        
     chat.save(LAST_CHAT_FILE, mode='w')
 
 if __name__ == '__main__':
     cli()
```

### Comparing `askchat-1.1.5/askchat.egg-info/PKG-INFO` & `askchat-1.1.6/askchat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: askchat
-Version: 1.1.5
+Version: 1.1.6
 Summary: Interact with ChatGPT in terminal via chattool
 Home-page: https://github.com/cubenlp/askchat
 Author: Rex Wang
 Author-email: 1073853456@qq.com
 License: MIT license
 Description: UNKNOWN
 Keywords: askchat
```

### Comparing `askchat-1.1.5/docs/assets/askchat.png` & `askchat-1.1.6/docs/assets/askchat.png`

 * *Files identical despite different names*

### Comparing `askchat-1.1.5/setup.py` & `askchat-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-VERSION = '1.1.5'
+VERSION = '1.1.6'
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 requirements = ['chattool>=3.1.4', "python-dotenv>=0.17.0", 'Click>=8.0']
 
 test_requirements = ['pytest>=3']
```

### Comparing `askchat-1.1.5/tests/test_askchat.py` & `askchat-1.1.6/tests/test_askchat.py`

 * *Files identical despite different names*

### Comparing `askchat-1.1.5/tests/test_askenv.py` & `askchat-1.1.6/tests/test_askenv.py`

 * *Files identical despite different names*

