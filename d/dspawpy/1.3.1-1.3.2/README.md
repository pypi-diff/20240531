# Comparing `tmp/dspawpy-1.3.1.tar.gz` & `tmp/dspawpy-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspawpy-1.3.1.tar", last modified: Thu May 23 06:52:09 2024, max compression
+gzip compressed data, was "dspawpy-1.3.2.tar", last modified: Fri May 31 09:58:45 2024, max compression
```

## Comparing `dspawpy-1.3.1.tar` & `dspawpy-1.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-23 06:52:09.074069 dspawpy-1.3.1/
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     1055 2024-05-16 07:21:06.000000 dspawpy-1.3.1/LICENSE.txt
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    13314 2024-05-23 06:52:09.073069 dspawpy-1.3.1/PKG-INFO
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    13132 2024-05-23 06:46:23.000000 dspawpy-1.3.1/README.md
-drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-23 06:52:09.041685 dspawpy-1.3.1/dspawpy/
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)      727 2024-05-23 06:52:06.000000 dspawpy-1.3.1/dspawpy/__init__.py
-drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-23 06:52:09.053143 dspawpy-1.3.1/dspawpy/analysis/
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.1/dspawpy/analysis/__init__.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    30293 2024-05-17 02:08:20.000000 dspawpy-1.3.1/dspawpy/analysis/aimdtools.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    17645 2024-05-17 02:08:20.000000 dspawpy-1.3.1/dspawpy/analysis/vacf.py
-drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-23 06:52:09.057463 dspawpy-1.3.1/dspawpy/cli/
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.1/dspawpy/cli/__init__.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    47125 2024-05-21 10:46:53.000000 dspawpy-1.3.1/dspawpy/cli/aux.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     8493 2024-05-17 02:08:20.000000 dspawpy-1.3.1/dspawpy/cli/cli.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    17882 2024-05-17 02:08:20.000000 dspawpy-1.3.1/dspawpy/cli/menu_prompts.py
-drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-23 06:52:09.062409 dspawpy-1.3.1/dspawpy/diffusion/
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.1/dspawpy/diffusion/__init__.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     3551 2024-05-17 02:08:20.000000 dspawpy-1.3.1/dspawpy/diffusion/neb.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    63177 2024-05-21 10:39:47.000000 dspawpy-1.3.1/dspawpy/diffusion/nebtools.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    10751 2024-05-17 02:08:20.000000 dspawpy-1.3.1/dspawpy/diffusion/pathfinder.py
-drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-23 06:52:09.069069 dspawpy-1.3.1/dspawpy/io/
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.1/dspawpy/io/__init__.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    63596 2024-05-21 10:32:07.000000 dspawpy-1.3.1/dspawpy/io/read.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    26595 2024-05-21 09:41:42.000000 dspawpy-1.3.1/dspawpy/io/structure.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    30761 2024-05-21 10:30:01.000000 dspawpy-1.3.1/dspawpy/io/utils.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    27382 2024-05-17 02:08:20.000000 dspawpy-1.3.1/dspawpy/io/write.py
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    55240 2024-05-21 10:37:48.000000 dspawpy-1.3.1/dspawpy/plot.py
-drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-23 06:52:09.071070 dspawpy-1.3.1/dspawpy.egg-info/
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    13314 2024-05-23 06:52:08.000000 dspawpy-1.3.1/dspawpy.egg-info/PKG-INFO
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)      651 2024-05-23 06:52:08.000000 dspawpy-1.3.1/dspawpy.egg-info/SOURCES.txt
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        1 2024-05-23 06:52:08.000000 dspawpy-1.3.1/dspawpy.egg-info/dependency_links.txt
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)       76 2024-05-23 06:52:08.000000 dspawpy-1.3.1/dspawpy.egg-info/entry_points.txt
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)       67 2024-05-23 06:52:08.000000 dspawpy-1.3.1/dspawpy.egg-info/requires.txt
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        8 2024-05-23 06:52:08.000000 dspawpy-1.3.1/dspawpy.egg-info/top_level.txt
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)       38 2024-05-23 06:52:09.075070 dspawpy-1.3.1/setup.cfg
--rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     1016 2024-05-23 06:52:06.000000 dspawpy-1.3.1/setup.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-31 09:58:45.822100 dspawpy-1.3.2/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     1055 2024-05-16 07:21:06.000000 dspawpy-1.3.2/LICENSE.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    13677 2024-05-31 09:58:45.821098 dspawpy-1.3.2/PKG-INFO
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    13497 2024-05-31 09:58:01.000000 dspawpy-1.3.2/README.md
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-31 09:58:45.785104 dspawpy-1.3.2/dspawpy/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)      728 2024-05-31 09:58:42.000000 dspawpy-1.3.2/dspawpy/__init__.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-31 09:58:45.796099 dspawpy-1.3.2/dspawpy/analysis/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.2/dspawpy/analysis/__init__.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    30294 2024-05-27 07:54:15.000000 dspawpy-1.3.2/dspawpy/analysis/aimdtools.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    17653 2024-05-27 07:53:54.000000 dspawpy-1.3.2/dspawpy/analysis/vacf.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-31 09:58:45.802100 dspawpy-1.3.2/dspawpy/cli/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.2/dspawpy/cli/__init__.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    49499 2024-05-27 07:57:36.000000 dspawpy-1.3.2/dspawpy/cli/aux.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     8480 2024-05-31 09:57:55.000000 dspawpy-1.3.2/dspawpy/cli/cli.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    17880 2024-05-27 07:56:32.000000 dspawpy-1.3.2/dspawpy/cli/menu_prompts.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-31 09:58:45.808100 dspawpy-1.3.2/dspawpy/diffusion/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.2/dspawpy/diffusion/__init__.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     3551 2024-05-17 02:08:20.000000 dspawpy-1.3.2/dspawpy/diffusion/neb.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    63806 2024-05-31 09:58:01.000000 dspawpy-1.3.2/dspawpy/diffusion/nebtools.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    10751 2024-05-17 02:08:20.000000 dspawpy-1.3.2/dspawpy/diffusion/pathfinder.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-31 09:58:45.818101 dspawpy-1.3.2/dspawpy/io/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-16 07:21:06.000000 dspawpy-1.3.2/dspawpy/io/__init__.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    55547 2024-05-31 09:58:01.000000 dspawpy-1.3.2/dspawpy/io/read.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    26597 2024-05-27 07:56:00.000000 dspawpy-1.3.2/dspawpy/io/structure.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    31054 2024-05-31 09:58:01.000000 dspawpy-1.3.2/dspawpy/io/utils.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    27446 2024-05-27 07:56:10.000000 dspawpy-1.3.2/dspawpy/io/write.py
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    54483 2024-05-31 09:58:01.000000 dspawpy-1.3.2/dspawpy/plot.py
+drwxr-xr-x   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        0 2024-05-31 09:58:45.819098 dspawpy-1.3.2/dspawpy.egg-info/
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)    13677 2024-05-31 09:58:45.000000 dspawpy-1.3.2/dspawpy.egg-info/PKG-INFO
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)      651 2024-05-31 09:58:45.000000 dspawpy-1.3.2/dspawpy.egg-info/SOURCES.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        1 2024-05-31 09:58:45.000000 dspawpy-1.3.2/dspawpy.egg-info/dependency_links.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)       45 2024-05-31 09:58:45.000000 dspawpy-1.3.2/dspawpy.egg-info/entry_points.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)       73 2024-05-31 09:58:45.000000 dspawpy-1.3.2/dspawpy.egg-info/requires.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)        8 2024-05-31 09:58:45.000000 dspawpy-1.3.2/dspawpy.egg-info/top_level.txt
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)       38 2024-05-31 09:58:45.823100 dspawpy-1.3.2/setup.cfg
+-rw-r--r--   0 zzl_ubuntu22  (1000) zzl_ubuntu22  (1000)     1004 2024-05-31 09:58:42.000000 dspawpy-1.3.2/setup.py
```

### Comparing `dspawpy-1.3.1/LICENSE.txt` & `dspawpy-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dspawpy-1.3.1/PKG-INFO` & `dspawpy-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 1.3.1
+Version: 1.3.2
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 Author-email: ZhengZhilin@hzwtech.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pymatgen
 Requires-Dist: statsmodels
 Requires-Dist: h5py
 Requires-Dist: prompt_toolkit
 Requires-Dist: loguru
-Requires-Dist: polars
+Requires-Dist: polars>=0.18
 Requires-Dist: ruamel.yaml
 
 ![Pyversion](https://img.shields.io/badge/dynamic/json?query=info.requires_python&label=python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fgeojson-rewind%2Fjson)
 ![PyPI](https://img.shields.io/pypi/v/dspawpy?label=pypi%20package)
 ![PyPI - Downloads](https://static.pepy.tech/badge/dspawpy/month)
 
 # Introduction （简介）
@@ -37,14 +37,22 @@
 
 ```bash
 conda install -c conda-forge dspawpy
 ```
 
 ## CHANGELOG （版本更新简述）
 
+### 1.3.2
+
+- 重要变更： 使用python3.8以下版本将无法启动程序
+- 重要变更： 正式用 polars 库替换 pandas 库
+- BUG修复： 移除setup.py中已不存在的ecli入口
+- BUG修复： wannier.json 不存在 SpinType 键导致读取失败
+- BUG修复： 瓦尼尔能带对比时，未正确读取 system.json 中的费米能级信息
+
 ### 1.3.1
 
 - BUG修复： 修复userscripts和cli中的一些问题
 - BUG修复： 修复json文件读取函数中的导包语句缺失问题
 - 功能强化： 10.2 支持读取aimd.json文件绘制物理量变化曲线图（仅无法读取压力变化）
 
 ### 1.3.0
```

### Comparing `dspawpy-1.3.1/README.md` & `dspawpy-1.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,22 @@
 
 ```bash
 conda install -c conda-forge dspawpy
 ```
 
 ## CHANGELOG （版本更新简述）
 
+### 1.3.2
+
+- 重要变更： 使用python3.8以下版本将无法启动程序
+- 重要变更： 正式用 polars 库替换 pandas 库
+- BUG修复： 移除setup.py中已不存在的ecli入口
+- BUG修复： wannier.json 不存在 SpinType 键导致读取失败
+- BUG修复： 瓦尼尔能带对比时，未正确读取 system.json 中的费米能级信息
+
 ### 1.3.1
 
 - BUG修复： 修复userscripts和cli中的一些问题
 - BUG修复： 修复json文件读取函数中的导包语句缺失问题
 - 功能强化： 10.2 支持读取aimd.json文件绘制物理量变化曲线图（仅无法读取压力变化）
 
 ### 1.3.0
```

### Comparing `dspawpy-1.3.1/dspawpy/__init__.py` & `dspawpy-1.3.2/dspawpy/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
-__version__ = "1.3.1"
+__version__ = "1.3.2"
 
-from loguru import logger
 import os
 import sys
 
-# check python version must be 3.6+
-assert sys.version_info >= (3, 6)
+from loguru import logger
+
+# check python version must be 3.8+
+assert sys.version_info >= (3, 8)
 
 logger.remove()
 level = os.getenv("dspawpy_log_level")
 if level is None:  # default to simulate no log
     level = "concise"
     logger.add(
         sys.stderr,
```

### Comparing `dspawpy-1.3.1/dspawpy/analysis/aimdtools.py` & `dspawpy-1.3.2/dspawpy/analysis/aimdtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
+from typing import TYPE_CHECKING, List, Optional, Sequence, Union
+
 from loguru import logger
-from typing import List, Union, Optional, Sequence, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from pymatgen.core.structure import Structure
 
 
 class MSD:
     # 用于实际计算均方位移的类，摘自pymatgen开源项目
```

### Comparing `dspawpy-1.3.1/dspawpy/analysis/vacf.py` & `dspawpy-1.3.2/dspawpy/analysis/vacf.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This module has not been tested yet, use at your own risk!
 """
 
 import numpy as np
 
 
 def welch(M, sym=1):
-    """Welch window. Function skeleton shamelessly stolen from
+    """Welch window. Function skeleton shamelementssly stolen from
     scipy.signal.bartlett() and others."""
     if M < 1:
         return np.array([])
     if M == 1:
         return np.ones(1, dtype=float)
     odd = M % 2
     if not sym and not odd:
@@ -191,15 +191,15 @@
 
 
 def sum(arr, axis=None, keepdims=False, **kwds):
     """This numpy.sum() with some features implemented which can be found in
     numpy v1.7 and later: `axis` can be a tuple to select arbitrary axes to sum
     over.
     We also have a `keepdims` keyword, which however works completely different
-    from numpy. Docstrings shamelessly stolen from numpy and adapted here
+    from numpy. Docstrings shamelementssly stolen from numpy and adapted here
     and there.
 
     Parameters
     ----------
     arr : nd array
     axis : None or int or tuple of ints, optional
         Axis or axes along which a sum is performed. The default (`axis` =
```

### Comparing `dspawpy-1.3.1/dspawpy/cli/aux.py` & `dspawpy-1.3.2/dspawpy/cli/aux.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-import threading
-from ruamel.yaml import YAML
 import os
+import threading
+from typing import Literal, Optional, Tuple
 
-from .menu_prompts import Dcheck, Dio, Dresponse, Dselect, Dparameter
 from loguru import logger
-from typing import Optional, List
 from prompt_toolkit import prompt
-from prompt_toolkit.completion import PathCompleter, WordCompleter, FuzzyCompleter
+from prompt_toolkit.completion import (
+    Completer,
+    FuzzyCompleter,
+    PathCompleter,
+    WordCompleter,
+)
+from ruamel.yaml import YAML
+
+from .menu_prompts import Dcheck, Dio, Dparameter, Dresponse, Dselect
 
 pc = FuzzyCompleter(PathCompleter(expanduser=True))  # path completion
 
 yaml = YAML()
 yaml.explicit_start = True
 yamllog = open(os.path.expanduser("~/.dp_record.yaml"), "a")
 
@@ -27,31 +33,32 @@
         import sys
 
         sys.stdout.close()
         sys.stdout = self._original_stdout
 
 
 @logger.catch
-def save_figure_dpi300(outfile):
+def save_figure_dpi300(outfile: str):
     """Save matplotlib figure with dpi=300"""
     import os
+
     import matplotlib.pyplot as plt
 
     absfile = os.path.abspath(outfile)
     os.makedirs(os.path.dirname(absfile), exist_ok=True)
     plt.tight_layout()
     plt.savefig(absfile, dpi=300)
     logger.critical(f"--> {absfile}")
 
 
 @logger.catch
 def get_input(
     user_prompt: str,
     valid_inputs: list,
-    completer=None,
+    completer: Optional[Completer] = None,
     allow_empty: bool = False,
     default_user_input: str = "",
 ) -> str:
     """Until user give valid input, or return default input if allow_empty is True and user input is empty."""
     if completer is None:
         completer = FuzzyCompleter(WordCompleter(valid_inputs))  # list completion
     from prompt_toolkit import prompt
@@ -67,15 +74,15 @@
                 return user_input
 
 
 @logger.catch
 def get_inputs(
     user_prompt: str,
     valid_inputs: list,
-    completer=None,
+    completer: Optional[Completer] = None,
     allow_empty: bool = False,
 ) -> list:
     """Return valid_inputs list if given empty"""
     if completer is None:
         completer = FuzzyCompleter(WordCompleter(valid_inputs))  # list completion
     from prompt_toolkit import prompt
 
@@ -93,296 +100,307 @@
             if valid:
                 return user_inputs
             else:
                 continue
 
 
 @logger.catch()
-def get_lims(user_prompt, lan) -> Optional[List[float]]:
+def get_lims(
+    user_prompt: str, language: Literal["EN", "CN"]
+) -> Optional[Tuple[float, float]]:
     """get lower and higher limits from user input"""
 
     while True:
         userInput = input(user_prompt).strip()
         if userInput == "":
             return None
         else:
             if " " not in userInput:
-                logger.warning(f"!!! {userInput}{Dresponse[lan][0]}")
+                logger.warning(f"!!! {userInput}{Dresponse[language][0]}")
                 continue
             elif len(userInput.split(" ")) != 2:
-                logger.warning(f"!!! {userInput}{Dresponse[lan][1]}")
+                logger.warning(f"!!! {userInput}{Dresponse[language][1]}")
                 continue
             else:
                 try:
                     lims = userInput.split(" ")
                     lower = float(lims[0])
                     higher = float(lims[1])
                     return lower, higher
 
                 except Exception:
-                    logger.warning(f"!!! {userInput}{Dresponse[lan][2]}")
+                    logger.warning(f"!!! {userInput}{Dresponse[language][2]}")
                     continue
 
 
 @logger.catch
-def pre_ele_band(lan):
+def pre_ele_band(language: Literal["EN", "CN"]):
     def imp():
         global get_band_data, BSPlotter
-        from dspawpy.io.read import get_band_data
         from pymatgen.electronic_structure.plotter import BSPlotter
 
+        from dspawpy.io.read import get_band_data
+
     import_thread = threading.Thread(target=imp)
     import_thread.start()
 
     D = {}
-    D["inf"] = prompt(Dio[lan]["band"], completer=pc)
-    D["ylims"] = get_lims(Dparameter[lan][10], lan)
-    D["figure"] = prompt(Dio[lan]["figure"], completer=pc) or "band.png"
+    D["inf"] = prompt(Dio[language]["band"], completer=pc)
+    D["ylims"] = get_lims(Dparameter[language][10], language)
+    D["figure"] = prompt(Dio[language]["figure"], completer=pc) or "band.png"
 
     import_thread.join()
 
     band_data = get_band_data(D["inf"])
     bsp = BSPlotter(band_data)
 
     return bsp, band_data, D
 
 
 @logger.catch
-def pre_ele_pband(lan):
+def pre_ele_pband(language: Literal["EN", "CN"]):
     def imp():
         global get_band_data, BSPlotterProjected
-        from dspawpy.io.read import get_band_data
         from pymatgen.electronic_structure.plotter import BSPlotterProjected
 
+        from dspawpy.io.read import get_band_data
+
     import_thread = threading.Thread(target=imp)
     import_thread.start()
 
     D = {}
-    D["inf"] = prompt(Dio[lan]["pband"], completer=pc)
-    D["ylims"] = get_lims(Dparameter[lan][10], lan)
-    D["figure"] = prompt(Dio[lan]["figure"], completer=pc) or "band_projected.png"
+    D["inf"] = prompt(Dio[language]["pband"], completer=pc)
+    D["ylims"] = get_lims(Dparameter[language][10], language)
+    D["figure"] = prompt(Dio[language]["figure"], completer=pc) or "band_projected.png"
 
     import_thread.join()
 
     band_data = get_band_data(D["inf"])
     bsp = BSPlotterProjected(band_data)
 
     return bsp, band_data, D
 
 
 @logger.catch
-def pre_ph_band(lan):
+def pre_ph_band(language: Literal["EN", "CN"]):
     def imp():
         global get_phonon_band_data, PhononBSPlotter
         from dspawpy.io.read import get_phonon_band_data
 
         with HidePrints():
             from pymatgen.phonon.plotter import PhononBSPlotter
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
 
     D = {}
-    D["inf"] = prompt(Dio[lan]["phband"], completer=pc)
-    D["ylims"] = get_lims(Dparameter[lan][10], lan)
-    D["figure"] = prompt(Dio[lan]["figure"], completer=pc) or "ph_band.png"
+    D["inf"] = prompt(Dio[language]["phband"], completer=pc)
+    D["ylims"] = get_lims(Dparameter[language][10], language)
+    D["figure"] = prompt(Dio[language]["figure"], completer=pc) or "ph_band.png"
 
     import_thread.join()
 
     band_data = get_phonon_band_data(D["inf"])
     bsp = PhononBSPlotter(band_data)
 
     return bsp, band_data, D
 
 
 @logger.catch
-def pre_ele_dos(lan):
+def pre_ele_dos(language: Literal["EN", "CN"]):
     def imp():
         global DosPlotter, get_dos_data
         from pymatgen.electronic_structure.plotter import DosPlotter
+
         from dspawpy.io.read import get_dos_data
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
 
     D = {}
-    D["inf"] = prompt(Dio[lan]["dos"], completer=pc)
-    D["xlims"] = get_lims(Dparameter[lan][9], lan)
-    D["ylims"] = get_lims(Dparameter[lan][10], lan)
-    D["shift"] = get_input(Dselect[lan][3], ["y", "n"])
-    D["figure"] = prompt(Dio[lan]["figure"], completer=pc) or "dos.png"
+    D["inf"] = prompt(Dio[language]["dos"], completer=pc)
+    D["xlims"] = get_lims(Dparameter[language][9], language)
+    D["ylims"] = get_lims(Dparameter[language][10], language)
+    D["shift"] = get_input(Dselect[language][3], ["y", "n"])
+    D["figure"] = prompt(Dio[language]["figure"], completer=pc) or "dos.png"
 
     import_thread.join()
 
     dos_data = get_dos_data(D["inf"])
     if D["shift"] == "y":
         dos_plotter = DosPlotter(stack=False, zero_at_efermi=True)
     else:
         dos_plotter = DosPlotter(stack=False, zero_at_efermi=True)
 
     return dos_plotter, dos_data, D
 
 
 @logger.catch
-def pre_ele_pdos(lan):
+def pre_ele_pdos(language: Literal["EN", "CN"]):
     def imp():
         global DosPlotter, get_dos_data, CompleteDos
+        from pymatgen.electronic_structure.dos import CompleteDos
         from pymatgen.electronic_structure.plotter import DosPlotter
+
         from dspawpy.io.read import get_dos_data
-        from pymatgen.electronic_structure.dos import CompleteDos
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
 
     D = {}
-    D["inf"] = prompt(Dio[lan]["pdos"], completer=pc)
-    D["xlims"] = get_lims(Dparameter[lan][9], lan)
-    D["ylims"] = get_lims(Dparameter[lan][10], lan)
-    D["shift"] = get_input(Dselect[lan][3], ["y", "n"])
-    D["figure"] = prompt(Dio[lan]["figure"], completer=pc) or "pdos.png"
+    D["inf"] = prompt(Dio[language]["pdos"], completer=pc)
+    D["xlims"] = get_lims(Dparameter[language][9], language)
+    D["ylims"] = get_lims(Dparameter[language][10], language)
+    D["shift"] = get_input(Dselect[language][3], ["y", "n"])
+    D["figure"] = prompt(Dio[language]["figure"], completer=pc) or "pdos.png"
 
     import_thread.join()
     dos_data = get_dos_data(D["inf"])
     assert isinstance(dos_data, CompleteDos)
     if D["shift"] == "y":
         dos_plotter = DosPlotter(stack=False, zero_at_efermi=True)
     else:
         dos_plotter = DosPlotter(stack=False, zero_at_efermi=True)
 
     return dos_plotter, dos_data, D
 
 
 @logger.catch
-def pre_ph_dos(lan):
+def pre_ph_dos(language: Literal["EN", "CN"]):
     def imp():
         global PhononDosPlotter, get_phonon_dos_data
         from dspawpy.io.read import get_phonon_dos_data
 
         with HidePrints():
             from pymatgen.phonon.plotter import PhononDosPlotter
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
 
     D = {}
-    D["inf"] = prompt(Dio[lan]["phdos"], completer=pc)
-    D["xlims"] = get_lims(Dparameter[lan][9], lan)
-    D["ylims"] = get_lims(Dparameter[lan][10], lan)
-    D["figure"] = prompt(Dio[lan]["figure"], completer=pc) or "ph_dos.png"
+    D["inf"] = prompt(Dio[language]["phdos"], completer=pc)
+    D["xlims"] = get_lims(Dparameter[language][9], language)
+    D["ylims"] = get_lims(Dparameter[language][10], language)
+    D["figure"] = prompt(Dio[language]["figure"], completer=pc) or "ph_dos.png"
     import_thread.join()
 
     dos_data = get_phonon_dos_data(D["inf"])
     dos_plotter = PhononDosPlotter(stack=False, sigma=None)
 
     return dos_plotter, dos_data, D
 
 
 @logger.catch
-def online_check(dv, lan):
+def online_check(local_dspawpy_version: str, language: Literal["EN", "CN"]):
     """fetch latses version of dspawpy from pypi"""
     latest_version = None
     # requests is dependency of pymatgen
-    from requests import get, exceptions
     from os.path import expanduser
 
+    from requests import exceptions, get
+
     try:
-        logger.info(Dcheck[lan][0])
+        logger.info(Dcheck[language][0])
         response = get("https://pypi.org/pypi/dspawpy/json", timeout=3)
         latest_version = response.json()["info"]["version"]
         error_message = None
     except ModuleNotFoundError:
-        error_message = Dcheck[lan][1]
+        error_message = Dcheck[language][1]
     except exceptions.Timeout:
-        error_message = Dcheck[lan][2]
+        error_message = Dcheck[language][2]
     except exceptions.RequestException as e:
-        error_message = f"{Dcheck[lan][3]} {e}"
+        error_message = f"{Dcheck[language][3]} {e}"
     except Exception as e:
-        error_message = f"{Dcheck[lan][4]} {e}"
+        error_message = f"{Dcheck[language][4]} {e}"
     finally:
         if latest_version:
-            if latest_version != dv:
-                logger.info(f"{latest_version} > {dv}; {Dcheck[lan][1]}")
+            if latest_version != local_dspawpy_version:
+                logger.info(
+                    f"{latest_version} > {local_dspawpy_version}; {Dcheck[language][1]}"
+                )
             else:
-                logger.info(f"{latest_version} = {dv}; {Dcheck[lan][6]}")
+                logger.info(
+                    f"{latest_version} = {local_dspawpy_version}; {Dcheck[language][6]}"
+                )
 
             with open(expanduser("~/.dspawpy_latest_version"), "w") as fin:
                 fin.write(latest_version)
         else:
-            logger.info(Dcheck[lan][7])
+            logger.info(Dcheck[language][7])
 
     return error_message
 
 
 @logger.catch
-def verify_dspawpy_version(check, lan):
+def verify_dspawpy_version(check: bool, language: Literal["EN", "CN"]):
     """may skip online check"""
     error_message = None
     import dspawpy
 
     try:
         dv = dspawpy.__version__
     except Exception:
-        dv = Dresponse[lan][11]
+        dv = Dresponse[language][11]
     finally:
         from os.path import dirname
 
         df = dirname(dspawpy.__file__)
 
     logger.info(f"{dv}: {df}")
 
     if check:
         from os.path import expanduser, isfile
 
         if isfile(expanduser("~/.dspawpy_latest_version")):
             with open(expanduser("~/.dspawpy_latest_version"), "r") as fin:
                 latest_version = fin.read().strip()
             if dv != latest_version:
-                error_message = online_check(dv, lan)
+                error_message = online_check(dv, language)
         else:
-            error_message = online_check(dv, lan)
+            error_message = online_check(dv, language)
 
         if error_message is not None:
             logger.info(error_message)
 
 
 @logger.catch
-def s2(lan):
+def s2(language: Literal["EN", "CN"]):
     """structure结构转化"""
 
     def imp():
         global convert
         from dspawpy.io.structure import convert
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
 
     D = {}
     D["menu"] = 2
-    D["in"] = prompt(Dio[lan]["ins"], completer=pc)
-    D["out"] = prompt(Dio[lan]["outs"], completer=pc)
+    D["in"] = prompt(Dio[language]["ins"], completer=pc)
+    D["out"] = prompt(Dio[language]["outs"], completer=pc)
     import_thread.join()
 
     convert(infile=D["in"], outfile=D["out"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s3_1(lan):
+def s3_1(language: Literal["EN", "CN"]):
     """volumetricData可视化"""
 
     def imp():
         global write_VESTA
         from dspawpy.io.write import write_VESTA
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
 
     D = {}
     D["menu"] = 31
-    D["inf"] = prompt(Dio[lan]["inf"], completer=pc)
+    D["inf"] = prompt(Dio[language]["inf"], completer=pc)
     _list = ["rho", "potential", "elf", "pcharge", "rhoBound"]
     D["task"] = get_input(
         f"{_list}: ",
         _list,
         completer=WordCompleter(_list),
     )
 
@@ -391,131 +409,132 @@
         if D["inf"].endswith(".h5"):
             from dspawpy.io.read import load_h5
 
             data = load_h5(D["inf"])
             keys = [k.split("/")[-1] for k in data.keys() if k.startswith("/Potential")]
 
             if len(keys) == 0:
-                raise ValueError(f"{Dresponse[lan][3]}{D['infile']}")
+                raise ValueError(f"{Dresponse[language][3]}{D['infile']}")
             elif len(keys) == 1:
                 subtype = keys[0]
             else:
                 subtype = get_input(
-                    f"{Dselect[lan][0]} {keys}: ",
+                    f"{Dselect[language][0]} {keys}: ",
                     keys,
                     completer=WordCompleter(keys),
                 )
 
         elif D["inf"].endswith(".json"):
             from json import load
 
             with open(D["inf"], "r") as fin:
                 data = load(fin)
                 if "Potential" not in data.keys():
-                    raise ValueError(f"{Dresponse[lan][3]} {D['infile']}")
+                    raise ValueError(f"{Dresponse[language][3]} {D['infile']}")
                 keys = [k for k in data["Potential"].keys()]
 
             if len(keys) == 1:
                 subtype = keys[0]
             else:
                 subtype = get_input(
-                    f"{Dselect[lan][0]} {keys}",
+                    f"{Dselect[language][0]} {keys}",
                     keys,
                     completer=WordCompleter(keys),
                 )
         else:
-            raise ValueError(Dresponse[lan][2])
+            raise ValueError(Dresponse[language][2])
 
-    D["outfile"] = prompt(Dio[lan]["outf"], completer=pc)
+    D["outfile"] = prompt(Dio[language]["outf"], completer=pc)
     if D["outfile"].split(".")[-1].lower() == "cube":
         D["format"] = "cube"
     elif (
         D["outfile"].split(".")[-1].lower() == "vesta"
         or D["outfile"].split(".")[-1].lower() == "vasp"
     ):
         D["format"] = "vesta"
     else:
-        D["format"] = get_input(Dselect[lan][2], ["cube", "vesta", "vasp"])
+        D["format"] = get_input(Dselect[language][2], ["cube", "vesta", "vasp"])
 
     import_thread.join()
     write_VESTA(
         in_filename=D["inf"],
         data_type=D["task"],
         out_filename=D["outfile"],
         subtype=subtype,
         format=D["format"],
     )
-    logger.info(Dresponse[lan][5])
+    logger.info(Dresponse[language][5])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s3_2(lan):
+def s3_2(language: Literal["EN", "CN"]):
     """差分volumetricData可视化"""
 
     def imp():
         global write_delta_rho_vesta
         from dspawpy.io.write import write_delta_rho_vesta
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
 
     D = {}
     D["menu"] = 32
-    D["total"] = prompt(Dio[lan]["tcharge"], completer=pc)
+    D["total"] = prompt(Dio[language]["tcharge"], completer=pc)
     D["individuals"] = []
     while True:
         individual = prompt(
-            Dio[lan]["pcharge"],
+            Dio[language]["pcharge"],
             completer=pc,
         )
         if individual == "":
             break
         D["individuals"].append(individual)
 
-    D["outfile"] = prompt(Dio[lan]["outf"], completer=pc)
+    D["outfile"] = prompt(Dio[language]["outf"], completer=pc)
 
     if D["outfile"].split(".")[-1].lower() == "cube":
         D["format"] = "cube"
     elif (
         D["outfile"].split(".")[-1].lower() == "vesta"
         or D["outfile"].split(".")[-1].lower() == "vasp"
     ):
         D["format"] = "vesta"
     else:
-        D["format"] = get_input(Dselect[lan][2], ["cube", "vesta", "vasp"])
+        D["format"] = get_input(Dselect[language][2], ["cube", "vesta", "vasp"])
 
     import_thread.join()
     write_delta_rho_vesta(
         total=D["total"],
         individuals=D["individuals"],
         output=D["outfile"],
         format=D["format"],
     )
-    logger.info(Dresponse[lan][5])
+    logger.info(Dresponse[language][5])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s3_3(lan):
+def s3_3(language: Literal["EN", "CN"]):
     """volumetricData面平均"""
 
     def imp():
         global plt, average_along_axis
 
-        from dspawpy.plot import average_along_axis
         import matplotlib.pyplot as plt
 
+        from dspawpy.plot import average_along_axis
+
     import_thread = threading.Thread(target=imp)
     import_thread.start()
 
     D = {}
     D["menu"] = 33
-    D["inf"] = prompt(Dio[lan]["inf"], completer=pc)
-    D["axes"] = get_input(Dselect[lan][1], ["0", "1", "2"])
+    D["inf"] = prompt(Dio[language]["inf"], completer=pc)
+    D["axes"] = get_input(Dselect[language][1], ["0", "1", "2"])
     _list = ["rho", "potential", "elf", "pcharge", "rhoBound"]
     D["task"] = get_input(
         str(_list),
         _list,
         completer=WordCompleter(_list),
     )
 
@@ -526,43 +545,43 @@
         if D["inf"].endswith(".h5"):
             from dspawpy.io.read import load_h5
 
             data = load_h5(D["inf"])
             keys = [k.split("/")[-1] for k in data.keys() if k.startswith("/Potential")]
 
             if len(keys) == 0:
-                raise ValueError(f"{Dresponse[lan][3]}{D['infile']}")
+                raise ValueError(f"{Dresponse[language][3]}{D['infile']}")
             elif len(keys) == 1:
                 D["subtype"] = keys[0]
             else:
                 D["subtype"] = get_input(
-                    Dselect[lan][0],
+                    Dselect[language][0],
                     keys,
                     completer=WordCompleter(keys),
                 )
 
         elif D["inf"].endswith(".json"):
             from json import load
 
             with open(D["inf"], "r") as fin:
                 data = load(fin)
                 if "Potential" not in data.keys():
-                    raise ValueError(f"{Dresponse[lan][3]}{D['infile']}")
+                    raise ValueError(f"{Dresponse[language][3]}{D['infile']}")
                 keys = [k for k in data["Potential"].keys()]
 
             if len(keys) == 1:
                 D["subtype"] = keys[0]
             else:
                 D["subtype"] = get_input(
-                    Dselect[lan][0],
+                    Dselect[language][0],
                     keys,
                     completer=WordCompleter(keys),
                 )
         else:
-            raise ValueError(Dresponse[lan][4])
+            raise ValueError(Dresponse[language][4])
         k = D["subtype"]
     elif D["task"] == "elf":
         k = "TotalELF"
     elif D["task"] == "pcharge":
         k = "TotalCharge"
     elif D["task"] == "rhoBound":
         k = "Rho"
@@ -580,86 +599,88 @@
             label=f"axis{ai}",
         )
     if len(axes_indices) > 1:
         plt.legend()
 
     plt.xlabel("Grid Index")
     plt.ylabel(k)
-    D["figure"] = prompt(Dio[lan]["figure"], completer=pc)
+    D["figure"] = prompt(Dio[language]["figure"], completer=pc)
 
     save_figure_dpi300(D["figure"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s4_1(lan):
+def s4_1(language: Literal["EN", "CN"]):
     """普通能带"""
-    bsp, band_data, D = pre_ele_band(lan)
+    bsp, band_data, D = pre_ele_band(language)
     D["menu"] = 41
 
     is_metal = band_data.is_metal()
     if is_metal:
         bsp.get_plot(ylim=D["ylims"])
     else:
-        D["shift"] = get_input(Dselect[lan][3], ["y", "n"])
+        D["shift"] = get_input(Dselect[language][3], ["y", "n"])
         if D["shift"] == "y":
-            from dspawpy.io.read import get_band_data
             from pymatgen.electronic_structure.plotter import BSPlotter
 
+            from dspawpy.io.read import get_band_data
+
             band_data = get_band_data(D["inf"], zero_to_efermi=True)
             bsp = BSPlotter(band_data)
             bsp.get_plot(False, ylim=D["ylims"])
         else:
             bsp.get_plot(ylim=D["ylims"])
 
     save_figure_dpi300(D["figure"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s4_2(lan):
+def s4_2(language: Literal["EN", "CN"]):
     """将能带投影到每一种元素分别作图，数据点大小表示该元素对该轨道的贡献"""
-    bsp, band_data, D = pre_ele_pband(lan)
+    bsp, band_data, D = pre_ele_pband(language)
     D["menu"] = 42
 
     is_metal = band_data.is_metal()
     if is_metal:
         bsp.get_elt_projected_plots(ylim=D["ylims"])
     else:
-        D["shift"] = get_input(Dselect[lan][3], ["y", "n"])
+        D["shift"] = get_input(Dselect[language][3], ["y", "n"])
         if D["shift"] == "y":
-            from dspawpy.io.read import get_band_data
             from pymatgen.electronic_structure.plotter import BSPlotterProjected
 
+            from dspawpy.io.read import get_band_data
+
             band_data = get_band_data(D["inf"], zero_to_efermi=True)
             bsp = BSPlotterProjected(band_data)
             bsp.get_elt_projected_plots(ylim=D["ylims"])
         else:
             bsp.get_elt_projected_plots(ylim=D["ylims"])
 
     save_figure_dpi300(D["figure"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s4_3(lan):
+def s4_3(language: Literal["EN", "CN"]):
     """能带投影到不同元素的不同轨道"""
-    bsp, band_data, D = pre_ele_pband(lan)
+    bsp, band_data, D = pre_ele_pband(language)
     D["menu"] = 43
 
-    banddatastructure = band_data.structure
-    assert banddatastructure is not None
-    logger.info(banddatastructure)
-    es = banddatastructure.composition.elements
+    banddatatructure = band_data.structure
+    assert banddatatructure is not None
+    logger.info(banddatatructure)
+    es = banddatatructure.composition.elements
     D["dictio"] = {}
 
     from pymatgen.core import Element
 
     while True:
-        _e = get_input(Dselect[lan][4], [str(e) for e in es], allow_empty=True)
+        _e = get_input(Dselect[language][4], [str(e) for e in es], allow_empty=True)
         if _e == "":
             break
         e = Element(_e)
 
         available_orbitals = ["s"]
         orbitals = e.atomic_orbitals
         assert isinstance(orbitals, dict)
@@ -667,56 +688,57 @@
             if "p" in o:
                 available_orbitals.append("p")
             elif "d" in o:
                 available_orbitals.append("d")
             elif "f" in o:
                 available_orbitals.append("f")
         unique_orbitals = list(set(available_orbitals))
-        _o = get_input(Dselect[lan][5], unique_orbitals)
+        _o = get_input(Dselect[language][5], unique_orbitals)
         _os = _o.split(" ")
         dict_eo = {_e: _os}
         # update dictio
         D["dictio"].update(dict_eo)
 
-    logger.info(f"{Dselect[lan][6]}, {D['dictio']}")
+    logger.info(f"{Dselect[language][6]}, {D['dictio']}")
 
     is_metal = band_data.is_metal()
     if is_metal:
         bsp.get_projected_plots_dots(D["dictio"])
     else:
-        D["shift"] = get_input(Dselect[lan][3], ["y", "n"])
+        D["shift"] = get_input(Dselect[language][3], ["y", "n"])
         if D["shift"] == "y":
-            from dspawpy.io.read import get_band_data
             from pymatgen.electronic_structure.plotter import BSPlotterProjected
 
+            from dspawpy.io.read import get_band_data
+
             band_data = get_band_data(D["inf"], zero_to_efermi=True)
             bsp = BSPlotterProjected(band_data)
             bsp.get_projected_plots_dots(D["dictio"], False, ylim=D["ylims"])
         else:
             bsp.get_projected_plots_dots(D["dictio"], ylim=D["ylims"])
 
     save_figure_dpi300(D["figure"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s4_4(lan):
+def s4_4(language: Literal["EN", "CN"]):
     """将能带投影到不同原子的不同轨道"""
-    bsp, band_data, D = pre_ele_pband(lan)
+    bsp, band_data, D = pre_ele_pband(language)
     D["menu"] = 44
 
-    banddatastructure = band_data.structure
-    assert banddatastructure is not None
-    logger.info(banddatastructure)
-    sites = banddatastructure.sites
+    banddatatructure = band_data.structure
+    assert banddatatructure is not None
+    logger.info(banddatatructure)
+    sites = banddatatructure.sites
     ns = [str(i) for i in range(len(sites))]
     D["dictio"] = {}
     D["dictpa"] = {}
     while True:
-        _n = get_input(Dselect[lan][7], ns, allow_empty=True)
+        _n = get_input(Dselect[language][7], ns, allow_empty=True)
         if _n == "":
             break
         _e = sites[int(_n)].specie
         available_orbitals = ["s"]
         orbitals = _e.atomic_orbitals
         for o in orbitals:
             if "p" in o:
@@ -739,33 +761,34 @@
                 available_orbitals.append("f0")
                 available_orbitals.append("f1")
                 available_orbitals.append("f2")
                 available_orbitals.append("f3")
 
         unique_orbitals = list(set(available_orbitals))
         D["dictpa"].update({str(_e): [int(_n) + 2]})
-        _os = get_inputs(Dselect[lan][8], unique_orbitals)
+        _os = get_inputs(Dselect[language][8], unique_orbitals)
         dict_eo = {str(_e): _os}
         # update dictio
         D["dictio"].update(dict_eo)
 
     logger.info(f"dictpa: {D['dictpa']}")
     logger.info(f"dictio: {D['dictio']}")
 
     is_metal = band_data.is_metal()
     if is_metal:
         bsp.get_projected_plots_dots_patom_pmorb(
             D["dictio"], D["dictpa"], ylim=D["ylims"]
         )
     else:
-        D["shift"] = get_input(Dselect[lan][3], ["y", "n"])
+        D["shift"] = get_input(Dselect[language][3], ["y", "n"])
         if D["shift"] == "y":
-            from dspawpy.io.read import get_band_data
             from pymatgen.electronic_structure.plotter import BSPlotterProjected
 
+            from dspawpy.io.read import get_band_data
+
             band_data = get_band_data(D["inf"], zero_to_efermi=True)
 
             bsp = BSPlotterProjected(band_data)
             bsp.get_projected_plots_dots_patom_pmorb(
                 D["dictio"],
                 D["dictpa"],
                 zero_to_efermi=False,
@@ -777,123 +800,125 @@
             )
 
     save_figure_dpi300(D["figure"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s4_5(lan):
+def s4_5(language: Literal["EN", "CN"]):
     """能带反折叠处理"""
 
     def imp():
         global plot_bandunfolding, plt
-        from dspawpy.plot import plot_bandunfolding
         import matplotlib.pyplot as plt
 
+        from dspawpy.plot import plot_bandunfolding
+
     import_thread = threading.Thread(target=imp)
     import_thread.start()
-    bsp, band_data, D = pre_ele_pband(lan)
+    bsp, band_data, D = pre_ele_pband(language)
     D["menu"] = 45
     import_thread.join()
 
     plot_bandunfolding(D["inf"])
     plt.ylim(D["ylims"])
     save_figure_dpi300(D["figure"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s4_6(lan):
+def s4_6(language: Literal["EN", "CN"]):
     """band-compare能带对比图处理"""
 
     def imp():
         global get_band_data, BSPlotter
-        from dspawpy.io.read import get_band_data
         from pymatgen.electronic_structure.plotter import BSPlotter
 
+        from dspawpy.io.read import get_band_data
+
     import_thread = threading.Thread(target=imp)
     import_thread.start()
-    bsp, band_data, D = pre_ele_band(lan)
+    bsp, band_data, D = pre_ele_band(language)
     D["menu"] = 46
-    D["infile2"] = prompt(Dio[lan]["wband"], completer=pc)
+    D["infile2"] = prompt(Dio[language]["wband"], completer=pc)
     if D["infile2"].endswith(".json"):
         D["infile3"] = prompt(
-            Dio[lan]["sysjson"],
+            Dio[language]["sysjson"],
             completer=pc,
         )
         D["infile2"] = [D["infile2"], D["infile3"]]
     import_thread.join()
 
     if isinstance(D["infile2"], list):
         bd1 = get_band_data(D["infile2"][0], D["infile2"][1])
     else:  # str
         bd1 = get_band_data(D["infile2"])
-    assert bd1 is not None, Dresponse[lan][6]
+    assert bd1 is not None, Dresponse[language][6]
     bsp = BSPlotter(bs=bd1)
     bsp2 = BSPlotter(bs=band_data)
     bsp.add_bs(bsp2._bs)
     bsp.get_plot(bs_labels=["wannier interpolated", "DFT"], ylim=D["ylims"])
     save_figure_dpi300(D["figure"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s5_1(lan):
+def s5_1(language: Literal["EN", "CN"]):
     """总的态密度"""
-    dos_plotter, dos_data, D = pre_ele_dos(lan)
+    dos_plotter, dos_data, D = pre_ele_dos(language)
     D["menu"] = 51
     dos_plotter.add_dos("total dos", dos=dos_data)
     dos_plotter.get_plot(xlim=D["xlims"], ylim=D["ylims"])
     save_figure_dpi300(D["figure"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s5_2(lan):
+def s5_2(language: Literal["EN", "CN"]):
     """将态密度投影到不同的轨道上"""
-    dos_plotter, dos_data, D = pre_ele_pdos(lan)
+    dos_plotter, dos_data, D = pre_ele_pdos(language)
     D["menu"] = 52
     dos_plotter.add_dos_dict(dos_data.get_spd_dos())
     dos_plotter.get_plot(xlim=D["xlims"], ylim=D["ylims"])
     save_figure_dpi300(D["figure"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s5_3(lan):
+def s5_3(language: Literal["EN", "CN"]):
     """将态密度投影到不同的元素上"""
-    dos_plotter, dos_data, D = pre_ele_pdos(lan)
+    dos_plotter, dos_data, D = pre_ele_pdos(language)
     D["menu"] = 53
     dos_plotter.add_dos_dict(dos_data.get_element_dos())
     dos_plotter.get_plot(xlim=D["xlims"], ylim=D["ylims"])
     save_figure_dpi300(D["figure"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s5_4(lan):
+def s5_4(language: Literal["EN", "CN"]):
     """将态密度投影到不同原子的不同轨道上"""
 
     def imp():
         global Orbital
         from pymatgen.electronic_structure.core import Orbital
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
-    dos_plotter, dos_data, D = pre_ele_pdos(lan)
+    dos_plotter, dos_data, D = pre_ele_pdos(language)
     D["menu"] = 54
     logger.info(dos_data.structure)
     sites = dos_data.structure.sites
     numbers = [str(i) for i in range(len(sites))]
 
     D["ns"] = []
     D["oss"] = []
     _e = None
     while True:
-        _n = get_input(Dselect[lan][7], numbers, allow_empty=True)
+        _n = get_input(Dselect[language][7], numbers, allow_empty=True)
         if _n == "":
             break
         available_orbitals = ["s"]
         _e = sites[int(_n)].specie
         orbitals = _e.atomic_orbitals
         assert isinstance(orbitals, dict)
         for o in orbitals:
@@ -915,15 +940,15 @@
                 available_orbitals.append("f_2")
                 available_orbitals.append("f_1")
                 available_orbitals.append("f0")
                 available_orbitals.append("f1")
                 available_orbitals.append("f2")
                 available_orbitals.append("f3")
         unique_orbitals = list(set(available_orbitals))
-        _os = get_inputs(Dselect[lan][8], unique_orbitals)
+        _os = get_inputs(Dselect[language][8], unique_orbitals)
         D["ns"].append(_n)
         D["oss"].append(_os)
 
     assert _e is not None
     import_thread.join()
     for _n, _os in zip(D["ns"], D["oss"]):
         for _orb in _os:
@@ -936,50 +961,51 @@
             )
     dos_plotter.get_plot(xlim=D["xlims"], ylim=D["ylims"])
     save_figure_dpi300(D["figure"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s5_5(lan):
+def s5_5(language: Literal["EN", "CN"]):
     """将态密度投影到不同原子的分裂d轨道(t2g, eg)上"""
-    dos_plotter, dos_data, D = pre_ele_pdos(lan)
+    dos_plotter, dos_data, D = pre_ele_pdos(language)
     D["menu"] = 55
     logger.info(dos_data.structure)
     sites = dos_data.structure.sites
     numbers = [str(e) for e in range(len(sites))]
-    D["ais"] = get_input(Dselect[lan][7], numbers)
+    D["ais"] = get_input(Dselect[language][7], numbers)
 
     atom_indices = [int(ai) for ai in D["ais"].split()]
     for atom_index in atom_indices:
         dos_plotter.add_dos_dict(
             dos_data.get_site_t2g_eg_resolved_dos(dos_data.structure[atom_index])
         )
 
     dos_plotter.get_plot(xlim=D["xlims"], ylim=D["ylims"])
     save_figure_dpi300(D["figure"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s5_6(lan):
+def s5_6(language: Literal["EN", "CN"]):
     """d-带中心分析"""
 
     def imp():
         global get_dos_data, d_band, os
+        import os
+
         from dspawpy.io.read import get_dos_data
         from dspawpy.io.utils import d_band
-        import os
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 56
-    D["inf"] = prompt(Dio[lan]["pdos"], completer=pc)
-    D["outfile"] = prompt(Dio[lan]["txt"], completer=pc)
+    D["inf"] = prompt(Dio[language]["pdos"], completer=pc)
+    D["outfile"] = prompt(Dio[language]["txt"], completer=pc)
     import_thread.join()
 
     dos_data = get_dos_data(D["inf"])
     os.makedirs(os.path.dirname(os.path.abspath(D["outfile"])), exist_ok=True)
     with open(D["outfile"], "w") as f:
         for spin in dos_data.densities:
             # up, down = (1, -1)
@@ -994,137 +1020,141 @@
             c = d_band(spin, dos_data)
             f.write(str(c) + "\n")
             logger.info(c)
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s6_1(lan):
+def s6_1(language: Literal["EN", "CN"]):
     """将能带和态密度显示在一张图上"""
 
     def imp():
         global BSDOSPlotter, pltbd, get_band_data, get_dos_data
         from pymatgen.electronic_structure.plotter import BSDOSPlotter
-        from dspawpy.plot import pltbd
+
         from dspawpy.io.read import get_band_data, get_dos_data
+        from dspawpy.plot import pltbd
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
 
     D = {}
     D["menu"] = 61
-    D["bandf"] = prompt(Dio[lan]["band"], completer=pc)
-    D["dosf"] = prompt(Dio[lan]["dos"], completer=pc)
-    D["ylims"] = get_lims(Dparameter[lan][10], lan)
-    D["outfile"] = prompt(Dio[lan]["figure"], completer=pc)
+    D["bandf"] = prompt(Dio[language]["band"], completer=pc)
+    D["dosf"] = prompt(Dio[language]["dos"], completer=pc)
+    D["ylims"] = get_lims(Dparameter[language][10], language)
+    D["outfile"] = prompt(Dio[language]["figure"], completer=pc)
     import_thread.join()
 
     band_data = get_band_data(D["bandf"])
     dos_data = get_dos_data(D["dosf"])
 
     bdp = BSDOSPlotter(dos_projection=None)  # pyright: ignore [reportArgumentType]
 
     pltbd(bdp, band_data, dos_data, ylim=D["ylims"], filename=D["outfile"])  # type: ignore
 
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s6_2(lan):
+def s6_2(language: Literal["EN", "CN"]):
     """将能带和投影态密度显示在一张图上"""
 
     def imp():
         global BSDOSPlotter, pltbd, get_band_data, get_dos_data
-        from dspawpy.io.read import get_band_data, get_dos_data
         from pymatgen.electronic_structure.plotter import BSDOSPlotter
+
+        from dspawpy.io.read import get_band_data, get_dos_data
         from dspawpy.plot import pltbd
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 61
-    D["bandf"] = prompt(Dio[lan]["band"], completer=pc)
-    D["dosf"] = prompt(Dio[lan]["dos"], completer=pc)
-    D["ylims"] = get_lims(Dparameter[lan][10], lan)
-    D["outfile"] = prompt(Dio[lan]["figure"], completer=pc)
+    D["bandf"] = prompt(Dio[language]["band"], completer=pc)
+    D["dosf"] = prompt(Dio[language]["dos"], completer=pc)
+    D["ylims"] = get_lims(Dparameter[language][10], language)
+    D["outfile"] = prompt(Dio[language]["figure"], completer=pc)
     import_thread.join()
 
     band_data = get_band_data(D["bandf"])
     dos_data = get_dos_data(D["dosf"])
 
     bdp = BSDOSPlotter(dos_projection="element")
 
     pltbd(bdp, band_data, dos_data, ylim=D["ylims"], filename=D["outfile"])  # type: ignore
 
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s7(lan):
+def s7(language: Literal["EN", "CN"]):
     """optical光学性质数据处理"""
 
     def imp():
         global plot_optical, makedirs
         from os import makedirs
+
         from dspawpy.plot import plot_optical
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 7
-    D["inf"] = prompt(Dio[lan]["optical"], completer=pc)
+    D["inf"] = prompt(Dio[language]["optical"], completer=pc)
     _list = [
         "AbsorptionCoefficient",
         "ExtinctionCoefficient",
         "RefractiveIndex",
         "Reflectance",
     ]
     D["keys"] = get_inputs(
-        Dselect[lan][16],
+        Dselect[language][16],
         _list,
         completer=WordCompleter(_list),
         allow_empty=True,
     )
     _list2 = ["X", "Y", "Z", "XY", "YZ", "ZX"]
     D["label"] = get_inputs(
-        Dselect[lan][17],
+        Dselect[language][17],
         _list2,
         completer=WordCompleter(_list2),
         allow_empty=True,
     )
 
-    D["outd"] = prompt(Dio[lan]["outd"], completer=pc)
+    D["outd"] = prompt(Dio[language]["outd"], completer=pc)
     import_thread.join()
 
     if D["outd"].strip() != "":
         makedirs(D["outd"], exist_ok=True)
     plot_optical(datafile=D["inf"], keys=D["keys"], axes=D["label"], prefix=D["outd"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s8_1(lan):
+def s8_1(language: Literal["EN", "CN"]):
     """输入文件之生成中间构型"""
 
     def imp():
         global NEB, write_neb_structures, read, os
+        import os
+
         from dspawpy.diffusion.neb import NEB, write_neb_structures
         from dspawpy.io.structure import read
-        import os
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
 
     D = {}
     D["menu"] = 81
-    D["inits"] = prompt(Dio[lan]["inits"], completer=pc)
-    D["fins"] = prompt(Dio[lan]["fins"], completer=pc)
-    D["nmiddle"] = int(input(Dparameter[lan][8]))
-    D["method"] = get_input(Dselect[lan][10], ["IDPP", "Linear"])
-    D["outd"] = prompt(Dio[lan]["outd"], completer=pc)
+    D["inits"] = prompt(Dio[language]["inits"], completer=pc)
+    D["fins"] = prompt(Dio[language]["fins"], completer=pc)
+    D["nmiddle"] = int(input(Dparameter[language][8]))
+    D["method"] = get_input(Dselect[language][10], ["IDPP", "Linear"])
+    D["outd"] = prompt(Dio[language]["outd"], completer=pc)
 
     if D["outd"] == "":
         D["outd"] = "."
 
     import_thread.join()
     init_struct = read(D["inits"])[0]
     final_struct = read(D["fins"])[0]
@@ -1132,75 +1162,76 @@
     neb = NEB(init_struct, final_struct, D["nmiddle"] + 2)
     if D["method"] == "Linear":
         structures = neb.linear_interpolate()
     else:
         try:
             structures = neb.idpp_interpolate()
         except Exception:
-            logger.error(Dresponse[lan][7])
+            logger.error(Dresponse[language][7])
             structures = neb.linear_interpolate()
-            logger.warning(Dresponse[lan][8])
+            logger.warning(Dresponse[language][8])
 
     absdir = os.path.abspath(D["outd"])
     os.makedirs(os.path.dirname(absdir), exist_ok=True)
     write_neb_structures(structures, fmt="as", path=absdir)
-    logger.info(f"{Dresponse[lan][9]} {D['outd']}")
+    logger.info(f"{Dresponse[language][9]} {D['outd']}")
 
-    yn = get_input(Dselect[lan][11], ["y", "n"])
+    yn = get_input(Dselect[language][11], ["y", "n"])
     if yn.lower().startswith("y"):
         from dspawpy.diffusion.nebtools import write_json_chain, write_xyz_chain
 
         write_xyz_chain(preview=True, directory=absdir)
         write_json_chain(preview=True, directory=absdir)
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s8_2(lan):
+def s8_2(language: Literal["EN", "CN"]):
     """绘制能垒图"""
 
     def imp():
         global plot_barrier, os
-        from dspawpy.diffusion.nebtools import plot_barrier
         import os
 
+        from dspawpy.diffusion.nebtools import plot_barrier
+
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 82
-    D["ind"] = prompt(Dio[lan]["neb"], completer=pc)
-    D["figure"] = prompt(Dio[lan]["figure"], completer=pc)
-    logger.info(Dresponse[lan][10])
+    D["ind"] = prompt(Dio[language]["neb"], completer=pc)
+    D["figure"] = prompt(Dio[language]["figure"], completer=pc)
+    logger.info(Dresponse[language][10])
     import_thread.join()
 
     if os.path.isdir(D["ind"]):
         plot_barrier(directory=D["ind"], figname=D["figure"], show=False)
     elif os.path.isfile(D["ind"]):
         plot_barrier(datafile=D["ind"], figname=D["figure"], show=False)
     else:
         raise TypeError(D["inf"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s8_3(lan):
+def s8_3(language: Literal["EN", "CN"]):
     """过渡态计算概览"""
 
     def imp():
         global summary, os
-        from dspawpy.diffusion.nebtools import summary
-
         import os
 
+        from dspawpy.diffusion.nebtools import summary
+
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 82
-    D["ind"] = prompt(Dio[lan]["nebdir"], completer=pc)
-    D["outd"] = prompt(Dio[lan]["outd"], completer=pc)
+    D["ind"] = prompt(Dio[language]["nebdir"], completer=pc)
+    D["outd"] = prompt(Dio[language]["outd"], completer=pc)
     import_thread.join()
 
     assert os.path.isdir(D["ind"])
     absdir = os.path.abspath(D["outd"])
     os.makedirs(os.path.dirname(absdir), exist_ok=True)
     summary(
         directory=D["ind"],
@@ -1208,201 +1239,202 @@
         figname=f"{absdir}/neb_summary.png",
         show=False,
     )
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s8_4(lan):
+def s8_4(language: Literal["EN", "CN"]):
     """NEB链可视化"""
 
     def imp():
         global write_json_chain, write_xyz_chain
         from dspawpy.diffusion.nebtools import write_json_chain, write_xyz_chain
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 84
-    D["yn"] = get_input(Dselect[lan][11], ["y", "n"])
-    D["ind"] = prompt(Dio[lan]["nebdir"], completer=pc)
+    D["yn"] = get_input(Dselect[language][11], ["y", "n"])
+    D["ind"] = prompt(Dio[language]["nebdir"], completer=pc)
     if D["yn"] == "y":
         step = 0
     else:
-        step = int(input(Dselect[lan][12]))  # XXX
-    dst = prompt(Dio[lan]["outd"], completer=pc)
+        step = int(input(Dselect[language][12]))  # XXX
+    dst = prompt(Dio[language]["outd"], completer=pc)
     import_thread.join()
 
     write_xyz_chain(False, D["ind"], step, dst)
     write_json_chain(False, D["ind"], step, dst)
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s8_5(lan):
+def s8_5(language: Literal["EN", "CN"]):
     """计算构型间距"""
 
     def imp():
         global read, get_distance
-        from dspawpy.io.structure import read
         from dspawpy.diffusion.nebtools import get_distance
+        from dspawpy.io.structure import read
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 85
-    D["infile1"] = prompt(Dparameter[lan][12], completer=pc)
-    D["infile2"] = prompt(Dparameter[lan][13], completer=pc)
+    D["infile1"] = prompt(Dparameter[language][12], completer=pc)
+    D["infile2"] = prompt(Dparameter[language][13], completer=pc)
     import_thread.join()
     s1 = read(D["infile1"])[0]
     s2 = read(D["infile2"])[0]
     result = get_distance(
         s1.frac_coords, s2.frac_coords, s1.lattice.matrix, s2.lattice.matrix
     )
     logger.info(str(result))
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s8_6(lan):
+def s8_6(language: Literal["EN", "CN"]):
     """neb续算"""
 
     def imp():
         global restart
         from dspawpy.diffusion.nebtools import restart
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 86
-    D["ind"] = prompt(Dio[lan]["neb"], completer=pc)
-    D["outd"] = prompt(Dio[lan]["outd"], completer=pc)
+    D["ind"] = prompt(Dio[language]["neb"], completer=pc)
+    D["outd"] = prompt(Dio[language]["outd"], completer=pc)
     import_thread.join()
     restart(D["ind"], D["outd"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s9_1(lan):
+def s9_1(language: Literal["EN", "CN"]):
     """声子能带数据处理"""
-    bsp, band_data, D = pre_ph_band(lan)
+    bsp, band_data, D = pre_ph_band(language)
     D["menu"] = 91
     bsp.get_plot(ylim=D["ylims"])  # pyright: ignore [reportArgumentType]
     save_figure_dpi300(D["figure"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s9_2(lan):
+def s9_2(language: Literal["EN", "CN"]):
     """声子态密度数据处理"""
-    dos_plotter, dos_data, D = pre_ph_dos(lan)
+    dos_plotter, dos_data, D = pre_ph_dos(language)
     D["menu"] = 92
     dos_plotter.add_dos(label="Phonon", dos=dos_data)
     dos_plotter.get_plot(
         xlim=D["xlims"],  # pyright: ignore [reportArgumentType]
         ylim=D["ylims"],  # pyright: ignore [reportArgumentType]
         units="thz",
     )
 
     save_figure_dpi300(D["figure"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s9_3(lan):
+def s9_3(language: Literal["EN", "CN"]):
     """声子热力学数据处理"""
 
     def imp():
         global plot_phonon_thermal
         from dspawpy.plot import plot_phonon_thermal
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 93
-    D["inf"] = prompt(Dio[lan]["inf"], completer=pc)
-    D["figure"] = prompt(Dio[lan]["figure"], completer=pc)
+    D["inf"] = prompt(Dio[language]["inf"], completer=pc)
+    D["figure"] = prompt(Dio[language]["figure"], completer=pc)
     import_thread.join()
 
     plot_phonon_thermal(D["inf"], D["figure"], False)
 
 
 @logger.catch
-def s10_1(lan):
+def s10_1(language: Literal["EN", "CN"]):
     """轨迹文件转换格式为.xyz或.dump"""
 
     def imp():
         global convert
         from dspawpy.io.structure import convert
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 101
-    D["inf"] = prompt(Dio[lan]["inf"], completer=pc)
-    D["outf"] = prompt(Dio[lan]["outf"], completer=pc)
+    D["inf"] = prompt(Dio[language]["inf"], completer=pc)
+    D["outf"] = prompt(Dio[language]["outf"], completer=pc)
     import_thread.join()
     convert(D["inf"], outfile=D["outf"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s10_2(lan):
+def s10_2(language: Literal["EN", "CN"]):
     """动力学过程中能量、温度等变化曲线"""
 
     def imp():
         global plot_aimd
         from dspawpy.plot import plot_aimd
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 102
-    D["inf"] = prompt(Dio[lan]["inf"], completer=pc)
-    D["figure"] = prompt(Dio[lan]["figure"], completer=pc)
+    D["inf"] = prompt(Dio[language]["inf"], completer=pc)
+    D["figure"] = prompt(Dio[language]["figure"], completer=pc)
     import_thread.join()
     plot_aimd(D["inf"], show=False, figname=D["figure"])
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s10_3(lan):
+def s10_3(language: Literal["EN", "CN"]):
     """均方位移（MSD）"""
 
     def imp():
         global MSD, _get_time_step, plot_msd, read, np
+        import numpy as np
+
         from dspawpy.analysis.aimdtools import MSD, _get_time_step, plot_msd
         from dspawpy.io.structure import read
-        import numpy as np
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 103
-    D["inf"] = prompt(Dio[lan]["inf"], completer=pc)
-    D["figure"] = prompt(Dio[lan]["figure"], completer=pc)
+    D["inf"] = prompt(Dio[language]["inf"], completer=pc)
+    D["figure"] = prompt(Dio[language]["figure"], completer=pc)
     D["msdtype"] = (
-        get_input(Dselect[lan][13], ["xyz", "xy", "xz", "yz", "x", "y", "z", ""])
+        get_input(Dselect[language][13], ["xyz", "xy", "xz", "yz", "x", "y", "z", ""])
         or "xyz"
     )
     if D["msdtype"] == "":
         D["msdtype"] = "xyz"
 
-    D["timestep"] = input(Dparameter[lan][0])
-    D["xlims"] = get_lims(Dparameter[lan][9], lan)
-    D["ylims"] = get_lims(Dparameter[lan][10], lan)
+    D["timestep"] = input(Dparameter[language][0])
+    D["xlims"] = get_lims(Dparameter[language][9], language)
+    D["ylims"] = get_lims(Dparameter[language][10], language)
 
     import_thread.join()
     structures = read(D["inf"])
     initial_structure = structures[0]
     logger.info(initial_structure)
     unique_elements = list(set(str(s) for s in initial_structure.species))
     unique_atomic_numbers = [str(i) for i in range(len(initial_structure.sites))]
     select_str = get_input(
-        Dselect[lan][9], unique_elements + unique_atomic_numbers + [""]
+        Dselect[language][9], unique_elements + unique_atomic_numbers + [""]
     )
     if select_str == "":
         D["select"] = "all"
     else:
         if ":" in select_str:  # slice, '1:3', '1:3:2'
             D["select"] = select_str
         elif " " in select_str:  # list of symbols or atom indices, '1 2 3', 'H He Li'
@@ -1425,164 +1457,164 @@
 
     logger.info(D["select"])
 
     if D["timestep"] == "":
         if isinstance(D["inf"], str) or len(D["inf"]) == 1:
             ts = _get_time_step(D["inf"])
         else:
-            logger.warning(Dresponse[lan][12])
+            logger.warning(Dresponse[language][12])
             ts = 1.0
     else:
         ts = float(D["timestep"])
 
     msd_calculator = MSD(structures, D["select"], D["msdtype"])
     msd = msd_calculator.run()
 
     xs = np.arange(msd_calculator.n_frames) * ts
     plot_msd(xs, msd, D["xlims"], D["ylims"], figname=D["figure"], show=False)
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s10_4(lan):
+def s10_4(language: Literal["EN", "CN"]):
     """均方根偏差（RMSD）"""
 
     def imp():
         global get_lagtime_rmsd, plot_rmsd
         from dspawpy.analysis.aimdtools import get_lagtime_rmsd, plot_rmsd
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 104
-    D["inf"] = prompt(Dio[lan]["inf"], completer=pc)
-    D["figure"] = prompt(Dio[lan]["figure"], completer=pc)
-    D["timestep"] = input(Dparameter[lan][0])
+    D["inf"] = prompt(Dio[language]["inf"], completer=pc)
+    D["figure"] = prompt(Dio[language]["figure"], completer=pc)
+    D["timestep"] = input(Dparameter[language][0])
     if D["timestep"] == "":
         D["timestep"] = None
     else:
         D["timestep"] = float(D["timestep"])
-    D["xlims"] = get_lims(Dparameter[lan][9], lan)
-    D["ylims"] = get_lims(Dparameter[lan][10], lan)
+    D["xlims"] = get_lims(Dparameter[language][9], language)
+    D["ylims"] = get_lims(Dparameter[language][10], language)
     import_thread.join()
 
     lagtime, rmsd = get_lagtime_rmsd(D["inf"], D["timestep"])
     plot_rmsd(lagtime, rmsd, D["xlims"], D["ylims"], D["figure"], False)
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s10_5(lan):
+def s10_5(language: Literal["EN", "CN"]):
     """径向分布函数（RDF）"""
 
     def imp():
         global get_rs_rdfs, plot_rdf, read
         from dspawpy.analysis.aimdtools import get_rs_rdfs, plot_rdf
         from dspawpy.io.structure import read
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 105
-    D["inf"] = prompt(Dio[lan]["inf"], completer=pc)
-    D["figure"] = prompt(Dio[lan]["figure"], completer=pc)
-    D["rmin"] = float(input(Dparameter[lan][1]) or 0)
-    D["rmax"] = float(input(Dparameter[lan][2]) or 10)
-    D["ngrid"] = int(input(Dparameter[lan][3]) or 101)
-    D["sigma"] = float(input(Dparameter[lan][4]) or 0)
+    D["inf"] = prompt(Dio[language]["inf"], completer=pc)
+    D["figure"] = prompt(Dio[language]["figure"], completer=pc)
+    D["rmin"] = float(input(Dparameter[language][1]) or 0)
+    D["rmax"] = float(input(Dparameter[language][2]) or 10)
+    D["ngrid"] = int(input(Dparameter[language][3]) or 101)
+    D["sigma"] = float(input(Dparameter[language][4]) or 0)
     D["xlims"] = [D["rmin"], D["rmax"]]
-    D["ylims"] = get_lims(Dparameter[lan][10], lan)
+    D["ylims"] = get_lims(Dparameter[language][10], language)
 
     import_thread.join()
     strs = read(datafile=D["inf"])
     logger.info(f"{strs[0]}")
     unique_elements = list(set([str(i) for i in strs[0].species]))
-    ele1 = get_input(Dselect[lan][14], unique_elements)
-    ele2 = get_input(Dselect[lan][15], unique_elements)
+    ele1 = get_input(Dselect[language][14], unique_elements)
+    ele2 = get_input(Dselect[language][15], unique_elements)
     rs, rdfs = get_rs_rdfs(
         D["inf"], ele1, ele2, D["rmin"], D["rmax"], D["ngrid"], D["sigma"]
     )
     plot_rdf(rs, rdfs, ele1, ele2, D["xlims"], D["ylims"], D["figure"], False)
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s11(lan):
+def s11(language: Literal["EN", "CN"]):
     """Polarization铁电极化数据处理"""
 
     def imp():
         global plot_polarization_figure
         from dspawpy.plot import plot_polarization_figure
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 11
-    D["inf"] = prompt(Dio[lan]["polarization"], completer=pc)
-    D["figure"] = prompt(Dio[lan]["figure"], completer=pc)
-    D["rep"] = int(input(Dparameter[lan][5]) or 2)
+    D["inf"] = prompt(Dio[language]["polarization"], completer=pc)
+    D["figure"] = prompt(Dio[language]["figure"], completer=pc)
+    D["rep"] = int(input(Dparameter[language][5]) or 2)
     import_thread.join()
 
     plot_polarization_figure(D["inf"], D["rep"], figname=D["figure"], show=False)
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s12(lan):
+def s12(language: Literal["EN", "CN"]):
     """ZPE零点振动能数据处理"""
 
     def imp():
         global getZPE
         from dspawpy.io.utils import getZPE
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 12
-    D["inf"] = prompt(Dio[lan]["txt"], completer=pc)
+    D["inf"] = prompt(Dio[language]["txt"], completer=pc)
     import_thread.join()
 
     logger.info(getZPE(D["inf"]))
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s13_1(lan):
+def s13_1(language: Literal["EN", "CN"]):
     """吸附质"""
 
     def imp():
         global getTSads
         from dspawpy.io.utils import getTSads
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 12
-    D["inf"] = prompt(Dio[lan]["txt"], completer=pc)
-    D["T"] = float(input(Dparameter[lan][6]) or 298.15)
+    D["inf"] = prompt(Dio[language]["txt"], completer=pc)
+    D["T"] = float(input(Dparameter[language][6]) or 298.15)
     TSads = getTSads(D["inf"], D["T"])
     logger.info("Entropy contribution, T*S (eV): ", TSads)
     yaml.dump(D, yamllog)
 
 
 @logger.catch
-def s13_2(lan):
+def s13_2(language: Literal["EN", "CN"]):
     """理想气体"""
 
     def imp():
         global getTSgas
         from dspawpy.io.utils import getTSgas
 
     import_thread = threading.Thread(target=imp)
     import_thread.start()
     D = {}
     D["menu"] = 12
-    D["inf"] = prompt(Dio[lan]["txt"], completer=pc)
-    D["T"] = float(input(Dparameter[lan][6]) or 298.15)
-    D["P"] = float(input(Dparameter[lan][7]) or 101325.0)
+    D["inf"] = prompt(Dio[language]["txt"], completer=pc)
+    D["T"] = float(input(Dparameter[language][6]) or 298.15)
+    D["P"] = float(input(Dparameter[language][7]) or 101325.0)
     import_thread.join()
 
     TSgas = getTSgas(
         fretxt=D["inf"][0],
         datafile=D["inf"][1],
         temperature=D["T"],
         pressure=D["P"],
```

### Comparing `dspawpy-1.3.1/dspawpy/cli/cli.py` & `dspawpy-1.3.2/dspawpy/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
         1. select task
         2. wait for user input, while importing functions in the background to reduce waiting time
         3. pass user input to the selected task and run it
         4. get output
     mode 2. non-interactive: run in script
         select task and pass user input directly to the selected task
     """
-    from dspawpy.cli.menu_prompts import menus, logo, Dupdate
-    from dspawpy.cli.aux import verify_dspawpy_version
     from dspawpy.cli import aux
+    from dspawpy.cli.aux import verify_dspawpy_version
+    from dspawpy.cli.menu_prompts import Dupdate, logo, menus
 
     args = get_args()
     lan = args.language
 
     if not args.hide:
         logger.info(logo[lan])
 
@@ -105,19 +105,20 @@
         )
         D["menu"] = 1
         D["yn"] = yn
         if yn.lower() == "y":
             from os import system
 
             if system(cmd) == 0:
-                D["result"] = [f">>>>>> {Dupdate[lan][1]}", f"{Dupdate[lan][2]}"]
+                result = [f">>>>>> {Dupdate[lan][1]}", f"{Dupdate[lan][2]}"]
             else:
-                D["result"] = [f"!!!!!! {Dupdate[lan][3]}"]
-            logger.info("\n".join(D["result"]))
+                result = [f"!!!!!! {Dupdate[lan][3]}"]
+            logger.info("\n".join(result))
         import os
+
         from ruamel.yaml import YAML
 
         yaml = YAML()
         yaml.explicit_start = True
         with open(os.path.expanduser("~/.dp_record.yaml"), "a") as f:
             yaml.dump(D, f)
```

### Comparing `dspawpy-1.3.1/dspawpy/cli/menu_prompts.py` & `dspawpy-1.3.2/dspawpy/cli/menu_prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         5: """
 === 5 dos plotting ===
 
 1: total dos plotting 
 2: orbital projected dos plotting 
 3: element projected dos plotting 
 4: atom's orbital projected dos plotting 
-5: atom's splited d orbital (t2g, eg) projected dos plotting 
+5: atom's split d orbital (t2g, eg) projected dos plotting 
 6: d-band center analysis
   
 0: return to main menu 
 --> enter a number and press 'Enter' to select corresponding action: """,
         6: """
 === 6 bandDos aligned plotting ===
```

### Comparing `dspawpy-1.3.1/dspawpy/diffusion/neb.py` & `dspawpy-1.3.2/dspawpy/diffusion/neb.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.3.1/dspawpy/diffusion/nebtools.py` & `dspawpy-1.3.2/dspawpy/diffusion/nebtools.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 from typing import Optional
+
 from loguru import logger
 
 
 @logger.catch
 def _zip_folder(folder_path: str, output_path: str):
     import os
 
@@ -173,14 +174,15 @@
 
     >>> plot_barrier(datafile='dspawpy_proj/dspawpy_tests/inputs/2.15/neb.h5', method='pchip', figname='dspawpy_proj/dspawpy_tests/outputs/doctest/barrier_h5.png', show=False) # doctest: +ELLIPSIS
     ==> .../doctest/barrier_h5.png
     >>> plot_barrier(datafile='dspawpy_proj/dspawpy_tests/inputs/2.15/neb.json', method='pchip', figname='dspawpy_proj/dspawpy_tests/outputs/doctest/barrier_json.png', show=False) # doctest: +ELLIPSIS
     ==> .../doctest/barrier_json.png
     """
     import os
+
     import numpy as np
 
     if directory is not None:
         # read data
         subfolders, resort_mfs, rcs, ens, dEs = _getef(os.path.abspath(directory))
 
     elif datafile:
@@ -244,30 +246,22 @@
     except Exception:
         raise ValueError(f"Please check whether {kwargs} is valid for {method}！")
 
     xnew = np.linspace(rcs[0], rcs[-1], 100)
     ynew = inter_f(xnew)
 
     if raw:
-        try:
-            import polars as pl
-
-            pl.DataFrame({"x_raw": rcs, "y_raw": dEs}).write_csv(
-                "raw_xy.csv",
-            )
-            pl.DataFrame({"x_interpolated": xnew, "y_interpolated": ynew}).write_csv(
-                "raw_interpolated_xy.csv",
-            )
-        except ModuleNotFoundError:
-            import pandas as pd
+        import polars as pl
 
-            pd.DataFrame({"x_raw": rcs, "y_raw": dEs}).to_csv("raw_xy.csv")
-            pd.DataFrame({"x_interpolated": xnew, "y_interpolated": ynew}).to_csv(
-                "raw_interpolated_xy.csv",
-            )
+        pl.DataFrame({"x_raw": rcs, "y_raw": dEs}).write_csv(
+            "raw_xy.csv",
+        )
+        pl.DataFrame({"x_interpolated": xnew, "y_interpolated": ynew}).write_csv(
+            "raw_interpolated_xy.csv",
+        )
 
     # plot
     import matplotlib.pyplot as plt  # noqa: E402
 
     if kwargs:
         plt.plot(xnew, ynew, label=method + str(kwargs))
     else:
@@ -318,14 +312,18 @@
 
     Examples
     --------
     >>> from dspawpy.diffusion.nebtools import plot_neb_converge
     >>> result = plot_neb_converge(neb_dir='dspawpy_proj/dspawpy_tests/inputs/2.15', image_key='01', figname='dspawpy_proj/dspawpy_tests/outputs/doctest/neb_converge1.png',show=False) # doctest: +ELLIPSIS
     ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/neb_converge1.png
     """
+    import os
+
+    import numpy as np
+
     from dspawpy.io.utils import get_absfile
     import os
     import numpy as np
 
     absfile = get_absfile(neb_dir, "neb")
     if absfile.endswith("h5"):
         import h5py
@@ -369,26 +367,19 @@
 
     x = np.arange(len(maxforce))
 
     force = maxforce
     energy = total_energy
 
     if raw:
-        try:
-            import polars as pl
+        import polars as pl
 
-            pl.DataFrame({"x": x, "force": force, "energy": energy}).write_csv(
-                "neb_conv.csv",
-            )
-        except ModuleNotFoundError:
-            import pandas as pd
-
-            pd.DataFrame({"x": x, "force": force, "energy": energy}).to_csv(
-                "neb_conv.csv",
-            )
+        pl.DataFrame({"x": x, "force": force, "energy": energy}).write_csv(
+            "neb_conv.csv",
+        )
 
     import matplotlib.pyplot as plt  # noqa: E402
 
     fig = plt.figure()
     ax1 = fig.add_subplot(111)
     ax1.plot(x, force, label="Max Force", c="black")
     ax1.set_xlabel("Number of ionic step")
@@ -426,56 +417,45 @@
     -------
     打印各构型的能量和受力
 
     Examples
     --------
     >>> from dspawpy.diffusion.nebtools import printef
     >>> printef(directory='dspawpy_proj/dspawpy_tests/inputs/2.15')
-    FolderName  Force(eV/Å)    RC(Å)    Energy(eV)  E-E0(eV)
-            00     0.180272 0.000000 -39637.098409  0.000000
-            01     0.026337 0.542789 -39637.018595  0.079814
-            02     0.024798 1.086800 -39636.880144  0.218265
-            03     0.234429 1.588367 -39636.998366  0.100043
-            04     0.014094 2.089212 -39637.089994  0.008414
+    shape: (5, 5)
+    ┌────────────┬─────────────┬──────────┬───────────────┬──────────┐
+    │ FolderName ┆ Force(eV/Å) ┆ RC(Å)    ┆ Energy(eV)    ┆ E-E0(eV) │
+    │ ---        ┆ ---         ┆ ---      ┆ ---           ┆ ---      │
+    │ str        ┆ f32         ┆ f32      ┆ f32           ┆ f32      │
+    ╞════════════╪═════════════╪══════════╪═══════════════╪══════════╡
+    │ 00         ┆ 0.180272    ┆ 0.0      ┆ -39637.097656 ┆ 0.0      │
+    │ 01         ┆ 0.026337    ┆ 0.542789 ┆ -39637.019531 ┆ 0.079814 │
+    │ 02         ┆ 0.024798    ┆ 1.0868   ┆ -39636.878906 ┆ 0.218265 │
+    │ 03         ┆ 0.234429    ┆ 1.588367 ┆ -39637.0      ┆ 0.100043 │
+    │ 04         ┆ 0.014094    ┆ 2.089212 ┆ -39637.089844 ┆ 0.008414 │
+    └────────────┴─────────────┴──────────┴───────────────┴──────────┘
     """
-    from dspawpy.diffusion.nebtools import _getef
     import numpy as np
 
-    data = np.array(_getef(directory)).T
-
-    import pandas as pd
+    from dspawpy.diffusion.nebtools import _getef
 
-    pd.set_option("display.float_format", "{:.6f}".format)
+    arr = np.array(_getef(directory))
+    data = {
+        "FolderName": arr[0],
+        "Force(eV/Å)": arr[1],
+        "RC(Å)": arr[2],
+        "Energy(eV)": arr[3],
+        "E-E0(eV)": arr[4],
+    }
+    import polars as pl
 
-    df = pd.DataFrame(
-        data,
-        columns=["FolderName", "Force(eV/Å)", "RC(Å)", "Energy(eV)", "E-E0(eV)"],
-    )
-    df["Force(eV/Å)"] = df["Force(eV/Å)"].astype(float)
-    df["RC(Å)"] = df["RC(Å)"].astype(float)
-    df["Energy(eV)"] = df["Energy(eV)"].astype(float)
-    df["E-E0(eV)"] = df["E-E0(eV)"].astype(float)
-    print(df.to_string(index=False))
-    # try:
-    #     import polars as pl
-    #
-    #     df = pl.DataFrame(
-    #         data,
-    #         schema=["FolderName", "Force(eV/Å)", "RC(Å)", "Energy(eV)", "E-E0(eV)"],
-    #     )
-    #     col_names = [col_name for col_name in df.columns if col_name != "FolderName"]
-    #     df.with_columns(pl.col(col_names).cast(pl.Float32, strict=False))
-    #     print(df)
-    # except ModuleNotFoundError:
-    #     import pandas as pd
-    #
-    #     df = pd.DataFrame(
-    #         data,
-    #         columns=["FolderName", "Force(eV/Å)", "RC(Å)", "Energy(eV)", "E-E0(eV)"],
-    #     )
+    _df = pl.DataFrame(data)
+    col_names = [col_name for col_name in _df.columns if col_name != "FolderName"]
+    df = _df.with_columns(pl.col(col_names).cast(pl.Float32, strict=False))
+    print(df)
 
 
 @logger.catch
 def restart(directory: str = ".", output: str = "bakfile"):
     """将旧NEB任务归档压缩，并在原路径下准备续算
 
     Parameters
@@ -496,29 +476,34 @@
     ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/neb_backup
 
     续算准备工作可能需要较长时间才能完成，请耐心等待
     """
     import os
     import shutil
 
-    absout = os.path.abspath(output)
+    absolute_output = os.path.abspath(output)
     absdir = os.path.abspath(directory)
 
-    if os.path.isdir(absout):
+    if os.path.isdir(absolute_output):
         from datetime import datetime
 
-        shutil.move(absout, absout + "_" + datetime.now().strftime("%Y%m%d%H%M%S"))
-        logger.warning(f"{absout} already exists, renamed to {absout}_datetime")
+        shutil.move(
+            absolute_output,
+            absolute_output + "_" + datetime.now().strftime("%Y%m%d%H%M%S"),
+        )
+        logger.warning(
+            f"{absolute_output} already exists, renamed to {absolute_output}_datetime"
+        )
 
     subfolders = get_neb_subfolders(absdir, return_abs=True)  # 获取子文件夹路径
-    os.makedirs(absout, exist_ok=True)  # 创建bakfile文件夹
+    os.makedirs(absolute_output, exist_ok=True)  # 创建bakfile文件夹
     # 先处理子文件夹00，01...
     for subfolder_old in subfolders:
         folder_index = subfolder_old.split("/")[-1]  # 00，01...
-        subfolder_back = os.path.join(absout, folder_index)  # 子文件夹备份到此
+        subfolder_back = os.path.join(absolute_output, folder_index)  # 子文件夹备份到此
         shutil.move(subfolder_old, subfolder_back)
         os.makedirs(subfolder_old, exist_ok=True)  # 原文件夹清空了
 
         latestStructureFile = f"{subfolder_back}/latestStructure{folder_index}.as"
         structureFile = f"{subfolder_back}/structure{folder_index}.as"
 
         # 将结构文件复制到原路径下用于续算，有ls则用之，否则用s代替，都没有则报错
@@ -535,15 +520,15 @@
         s_bk = os.path.join(absdir, f"structure{folder_index}.as")
         if os.path.isfile(latestStructureFile):
             shutil.copy(latestStructureFile, ls_bk)
         if os.path.isfile(structureFile):
             shutil.copy(structureFile, s_bk)
 
         # 处理备份路径下的子文件夹
-        zf = f"{absout}/{folder_index}.zip"
+        zf = f"{absolute_output}/{folder_index}.zip"
         _zip_folder(subfolder_back, zf)  # 压缩子文件夹
         # 清空备份子文件夹
         for file in os.listdir(subfolder_back):
             os.remove(os.path.join(subfolder_back, file))
 
         # 将压缩包、结构文件移入
         shutil.move(zf, f"{subfolder_back}/{folder_index}.zip")
@@ -555,32 +540,32 @@
         elif os.path.isfile(s_bk):
             shutil.move(s_bk, f"{subfolder_back}/structure{folder_index}.as")
         else:
             raise FileNotFoundError(f"Both {ls_bk} and {s_bk} not found")
 
     # 再处理老NEB文件夹主目录下的单个文件
     # 备份neb.h5,neb.json和DS-PAW.log
-    tmp_dir = os.path.join(absout, "tmp")
+    tmp_dir = os.path.join(absolute_output, "tmp")
     os.makedirs(tmp_dir, exist_ok=True)
     if os.path.isfile(f"{absdir}/neb.h5"):
         shutil.move(f"{absdir}/neb.h5", f"{tmp_dir}/neb.h5")
 
     if os.path.isfile(f"{absdir}/neb.json"):
         shutil.move(f"{absdir}/neb.json", f"{tmp_dir}/neb.json")
 
     if len(os.listdir(tmp_dir)) > 0:  # 如果有数据文件
-        _zip_folder(tmp_dir, f"{absout}/neb_data.zip")
+        _zip_folder(tmp_dir, f"{absolute_output}/neb_data.zip")
         for f in os.listdir(tmp_dir):
             os.remove(os.path.join(tmp_dir, f))
         os.removedirs(tmp_dir)
 
     if os.path.isfile(f"{absdir}/DS-PAW.log"):
-        shutil.move(f"{absdir}/DS-PAW.log", f"{absout}/DS-PAW.log")
+        shutil.move(f"{absdir}/DS-PAW.log", f"{absolute_output}/DS-PAW.log")
 
-    print(f"==> {absout}")
+    print(f"==> {absolute_output}")
 
 
 @logger.catch
 def set_pbc(spo):
     """根据周期性边界条件将分数坐标分量移入 [-0.5, 0.5) 区间
 
     Parameters
@@ -635,20 +620,26 @@
         传递给plot_barrier的参数
 
     Examples
     --------
     >>> from dspawpy.diffusion.nebtools import summary
     >>> directory = 'dspawpy_proj/dspawpy_tests/inputs/2.15' # NEB计算路径，默认当前路径
     >>> summary(directory, show=False, figname='dspawpy_proj/dspawpy_tests/outputs/doctest/neb_barrier.png') # doctest: +ELLIPSIS
-    FolderName  Force(eV/Å)    RC(Å)    Energy(eV)  E-E0(eV)
-            00     0.180272 0.000000 -39637.098409  0.000000
-            01     0.026337 0.542789 -39637.018595  0.079814
-            02     0.024798 1.086800 -39636.880144  0.218265
-            03     0.234429 1.588367 -39636.998366  0.100043
-            04     0.014094 2.089212 -39637.089994  0.008414
+    shape: (5, 5)
+    ┌────────────┬─────────────┬──────────┬───────────────┬──────────┐
+    │ FolderName ┆ Force(eV/Å) ┆ RC(Å)    ┆ Energy(eV)    ┆ E-E0(eV) │
+    │ ---        ┆ ---         ┆ ---      ┆ ---           ┆ ---      │
+    │ str        ┆ f32         ┆ f32      ┆ f32           ┆ f32      │
+    ╞════════════╪═════════════╪══════════╪═══════════════╪══════════╡
+    │ 00         ┆ 0.180272    ┆ 0.0      ┆ -39637.097656 ┆ 0.0      │
+    │ 01         ┆ 0.026337    ┆ 0.542789 ┆ -39637.019531 ┆ 0.079814 │
+    │ 02         ┆ 0.024798    ┆ 1.0868   ┆ -39636.878906 ┆ 0.218265 │
+    │ 03         ┆ 0.234429    ┆ 1.588367 ┆ -39637.0      ┆ 0.100043 │
+    │ 04         ┆ 0.014094    ┆ 2.089212 ┆ -39637.089844 ┆ 0.008414 │
+    └────────────┴─────────────┴──────────┴───────────────┴──────────┘
     ==> .../doctest/neb_barrier.png
     ==> .../doctest/01/converge.png
     ==> .../doctest/02/converge.png
     ==> .../doctest/03/converge.png
 
     若inifin=false，用户必须将自洽的scf.h5或system.json放到初末态子文件夹中
     """
@@ -664,17 +655,17 @@
     plt.clf()  # 清空画布再画图
     plot_barrier(directory=absdir, raw=raw, **kwargs)
 
     # 3. 绘制并保存结构优化过程的能量和受力收敛过程图到各构型文件夹中
     subfolders = get_neb_subfolders(absdir)
     for subfolder in subfolders[1 : len(subfolders) - 1]:
         if outdir:
-            absout = os.path.abspath(outdir)
-            os.makedirs(os.path.join(absout, subfolder), exist_ok=True)
-            pngfile = f"{absout}/{subfolder}/converge.png"
+            absolute_output = os.path.abspath(outdir)
+            os.makedirs(os.path.join(absolute_output, subfolder), exist_ok=True)
+            pngfile = f"{absolute_output}/{subfolder}/converge.png"
         else:
             pngfile = (
                 f"dspawpy_proj/dspawpy_tests/outputs/doctest/{subfolder}/converge.png"
             )
 
         plot_neb_converge(
             neb_dir=absdir,
@@ -922,22 +913,22 @@
         maxForces,
         tangents,
         iDirects,
     ) = raw
 
     # 写入文件
     xyzfile = output[:-5] + ".xyz"
-    absout = os.path.abspath(xyzfile)
+    absolute_output = os.path.abspath(xyzfile)
     Nstep = len(subfolders)  # 选定离子步，展示构型链
-    with open(absout, "w") as f:
+    with open(absolute_output, "w") as f:
         # Nstep
         for n in range(Nstep):
-            eles = Elems[n]  # 针对每个构型
+            elements = Elems[n]  # 针对每个构型
             # 原子数不会变，就是不合并的元素总数
-            f.write("%d\n" % len(eles))
+            f.write("%d\n" % len(elements))
             # lattice
             f.write(
                 'Lattice="%f %f %f %f %f %f %f %f %f" Properties=species:S:1:pos:R:3 pbc="T T T"\n'
                 % (
                     Latvs[n, 0],
                     Latvs[n, 1],
                     Latvs[n, 2],
@@ -946,20 +937,20 @@
                     Latvs[n, 5],
                     Latvs[n, 6],
                     Latvs[n, 7],
                     Latvs[n, 8],
                 )
             )
             # position and element
-            for i in range(len(eles)):
+            for i in range(len(elements)):
                 f.write(
                     "%s %f %f %f\n"
-                    % (eles[i], Poses[n, i, 0], Poses[n, i, 1], Poses[n, i, 2])
+                    % (elements[i], Poses[n, i, 0], Poses[n, i, 1], Poses[n, i, 2])
                 )
-    print(f"==> {absout}")
+    print(f"==> {absolute_output}")
 
 
 @logger.catch
 def _from_structures(directory: str, ls: bool = False):
     """从structure00.as，structure01.as，...，中读取结构信息，
     写入neb_chain_init，以便用DeviceStudio打开观察
 
@@ -1256,17 +1247,18 @@
 
     Returns
     -------
     用于json文件的各个数组
     """
 
     import os
-    import numpy as np
     from json import load
 
+    import numpy as np
+
     absdir = os.path.abspath(directory)
     # ^ 前期设置
     neb_js = os.path.join(absdir, "01/neb01.json")
     with open(neb_js, "r") as f:
         data = load(f)
     total_steps = len(data)
 
@@ -1532,21 +1524,21 @@
         "RelaxedStructure": RSList,
         "UnrelaxedStructure": URSList,
     }
 
     # ^ 将字典写入json文件
     import os
 
-    absout = os.path.abspath(output)
-    with open(absout, "w") as f:
+    absolute_output = os.path.abspath(output)
+    with open(absolute_output, "w") as f:
         from json import dump
 
         dump(data, f, indent=4)
 
-    print(f"==> {absout}")
+    print(f"==> {absolute_output}")
 
 
 @logger.catch
 def _getef(directory: str = "."):
     """读取NEB计算时各构型的能量和受力，NEB计算可以未收敛
     但如果初末态自洽在别处完成，请手动将其移入00等文件夹中！
 
@@ -1565,14 +1557,15 @@
         反应坐标列表
     ens: list
         电子总能列表
     dEs: list
         与初始构型的能量差列表
     """
     import os
+
     import numpy as np
 
     absdir = os.path.abspath(directory)
     subfolders = get_neb_subfolders(absdir)
     Nimage = len(subfolders)
 
     ens = []
@@ -1795,29 +1788,20 @@
     except Exception:
         raise ValueError(f"Please check whether {kwargs} is valid for {method}！")
 
     xnew = np.linspace(rcs[0], rcs[-1], 100)
     ynew = inter_f(xnew)
 
     if raw:
-        try:
-            import polars as pl
-
-            pl.DataFrame({"x_raw": rcs, "y_raw": dEs}).write_csv("raw_xy.csv")
-            pl.DataFrame({"x_interpolated": xnew, "y_interpolated": ynew}).write_csv(
-                "raw_interpolated_xy.csv"
-            )
-        except ModuleNotFoundError:
-            import pandas as pd
-
-            pd.DataFrame({"x_raw": rcs, "y_raw": dEs}).to_csv("raw_xy.csv")
-            pd.DataFrame({"x_interpolated": xnew, "y_interpolated": ynew}).to_csv(
-                "raw_interpolated_xy.csv"
-            )
+        import polars as pl
 
+        pl.DataFrame({"x_raw": rcs, "y_raw": dEs}).write_csv("raw_xy.csv")
+        pl.DataFrame({"x_interpolated": xnew, "y_interpolated": ynew}).write_csv(
+            "raw_interpolated_xy.csv"
+        )
     # plot
     import matplotlib.pyplot as plt  # noqa: E402
 
     if kwargs:
         plt.plot(xnew, ynew, label=method + str(kwargs))
     else:
         plt.plot(xnew, ynew, label=method)
```

### Comparing `dspawpy-1.3.1/dspawpy/diffusion/pathfinder.py` & `dspawpy-1.3.2/dspawpy/diffusion/pathfinder.py`

 * *Files identical despite different names*

### Comparing `dspawpy-1.3.1/dspawpy/io/read.py` & `dspawpy-1.3.2/dspawpy/io/read.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
+from typing import TYPE_CHECKING, Optional, Sequence
+
 from loguru import logger
-from typing import Optional, TYPE_CHECKING, Sequence
 
 if TYPE_CHECKING:
     from pymatgen.electronic_structure.bandstructure import BandStructureSymmLine
 
 
 @logger.catch
 def get_band_data(
@@ -404,19 +405,19 @@
     D_mag_fix : dict
         磁矩、自由度相关信息
 
     Examples
     --------
 
     >>> from dspawpy.io.read import get_sinfo
-    >>> Nstep, eles, pos, latv, D_mag_fix = get_sinfo(datafile='dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5', scaled=False, si=None, ele=None, ai=None) # doctest: +ELLIPSIS
+    >>> Nstep, elements, pos, latv, D_mag_fix = get_sinfo(datafile='dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5', scaled=False, si=None, ele=None, ai=None) # doctest: +ELLIPSIS
     Reading ...dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5...
-    >>> Nstep, eles, pos, latv, D_mag_fix = get_sinfo(datafile='dspawpy_proj/dspawpy_tests/inputs/2.1/relax.json', scaled=False, si=None, ele=None, ai=None) # doctest: +ELLIPSIS
+    >>> Nstep, elements, pos, latv, D_mag_fix = get_sinfo(datafile='dspawpy_proj/dspawpy_tests/inputs/2.1/relax.json', scaled=False, si=None, ele=None, ai=None) # doctest: +ELLIPSIS
     Reading ...dspawpy_proj/dspawpy_tests/inputs/2.1/relax.json...
-    >>> Nstep, eles, pos, latv, D_mag_fix = get_sinfo(datafile='dspawpy_proj/dspawpy_tests/inputs/2.2/rho.json', scaled=False) # doctest: +ELLIPSIS
+    >>> Nstep, elements, pos, latv, D_mag_fix = get_sinfo(datafile='dspawpy_proj/dspawpy_tests/inputs/2.2/rho.json', scaled=False) # doctest: +ELLIPSIS
     Reading ...dspawpy_proj/dspawpy_tests/inputs/2.2/rho.json...
 
     这些信息可以用于进一步构建Structure对象，
     具体参考 dspawpy.io.structure.build_Structures_from_datafile 函数
     """
     assert (
         ele is None or ai is None
@@ -594,170 +595,16 @@
             else:  # Cartesian coordinates
                 for k, ind in enumerate(indices):  # 步数
                     for j, sli in enumerate(location):
                         poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], lattices[k])
 
         elif "/RelaxedStructure" in hf.keys():  # 最新NEB链
             raise NotImplementedError("neb.h5 is not supported yet")
-        #     N_images = np.array(hf.get("/RelaxedStructure")).shape[
-        #         0
-        #     ]  # Image00, Image01, ...
-        #     elements = np.empty(shape=(N_images,), dtype=np.float32)
-        #     Natom = len(elements)
-        #     lattices = np.empty(shape=(N_images, 3, 3), dtype=np.float32)
-        #     poses = np.empty(shape=(N_images, Natom, 3), dtype=np.float32)
-        #     atomFixs = np.empty(shape=(N_images, Natom, 3))
-        #     latticeFixs = np.empty(shape=(N_images, 9))
-        #     for i in range(N_images):
-        #         subfolder_name = "Image%02d" % i
-        #         _ele = np.array(hf.get(f"/RelaxedStructure/{subfolder_name}/Elements"))[
-        #             0
-        #         ]
-        #         _lat = np.array(hf.get(f"/RelaxedStructure/{subfolder_name}/Lattice"))[
-        #             0
-        #         ]
-        #         _pos = np.array(hf.get(f"/RelaxedStructure/{subfolder_name}/Position"))[
-        #             0
-        #         ]
-        #         elements[i] = _ele
-        #         lattices[i] = _lat
-        #         poses[i] = _pos
-        #
-        #         try:  # fix atom
-        #             atomFix_raw = np.array(
-        #                 hf.get(f"/RelaxedStructure/{subfolder_name}/Fix")
-        #             )
-        #             atomFix = np.array(
-        #                 ["True" if _v else "False" for _v in atomFix_raw]
-        #             ).reshape(-1, 3)
-        #         except Exception:
-        #             atomFix = np.full(shape=(Natom, 3), fill_value="False")
-        #         atomFixs[i] = atomFix
-        #
-        #         try:  # fix lattice
-        #             latticeFix = (
-        #                 np.array(
-        #                     hf.get(f"/RelaxedStructure/{subfolder_name}/FixLattice")
-        #                 )
-        #                 .astype(bool)
-        #                 .flatten()
-        #             )
-        #             assert latticeFix.shape == (9,)
-        #             latticeFix = latticeFix.reshape(
-        #                 9,
-        #             )  # (9,)
-        #         except Exception as e:
-        #             if str(e):  # ignore empty AssertionError()
-        #                 print(e)
-        #             latticeFix = np.full(shape=(9,), fill_value="False")
-        #         latticeFixs[i] = latticeFix
-        #
-        #     iNoncollinear = False
-        #     try:  # 自旋计算
-        #         if "/MagInfo/TotalMagOnAtom" in hf.keys():  # collinear
-        #             mag = np.array(hf.get("/MagInfo/TotalMagOnAtom"))  # Natom x 1
-        #             mags = np.repeat(mag[np.newaxis, :], Nstep, axis=0).tolist()
-        #             D_mag_fix = {
-        #                 "Mag": mags,
-        #                 "Fix_x": atomFixs[:, :, 0],
-        #                 "Fix_y": atomFixs[:, :, 1],
-        #                 "Fix_z": atomFixs[:, :, 2],
-        #                 "LatticeFixs": latticeFixs,
-        #             }
-        #         elif "/MagInfo/TotalMagOnAtomX" in hf.keys():  # noncollinear
-        #             magx = np.array(hf.get("/MagInfo/TotalMagOnAtomX"))  # Natom x 1
-        #             magy = np.array(hf.get("/MagInfo/TotalMagOnAtomY"))  # Natom x 1
-        #             magz = np.array(hf.get("/MagInfo/TotalMagOnAtomZ"))  # Natom x 1
-        #             iNoncollinear = True
-        #             D_mag_fix = {
-        #                 "Mag_x": np.repeat(magx[np.newaxis, :], Nstep, axis=0).tolist(),
-        #                 "Mag_y": np.repeat(magy[np.newaxis, :], Nstep, axis=0).tolist(),
-        #                 "Mag_z": np.repeat(magz[np.newaxis, :], Nstep, axis=0).tolist(),
-        #                 "Fix_x": atomFixs[:, :, 0],
-        #                 "Fix_y": atomFixs[:, :, 1],
-        #                 "Fix_z": atomFixs[:, :, 2],
-        #                 "LatticeFixs": latticeFixs,
-        #             }
-        #         else:
-        #             mag = np.zeros(shape=(Natom, 1))
-        #
-        #     except Exception as e:
-        #         if str(e):  # ignore empty AssertionError()
-        #             print(e)
-        #         mag = np.zeros(shape=(Natom, 1))
-        #
-        #     if scaled:  # Fractional coordinates
-        #         for k, ind in enumerate(indices):  # 步数
-        #             for j, sli in enumerate(location):  # atom si
-        #                 poses[k, j, :] = np.dot(poses[k, :, sli], np.eye(3, 3))
-        #     else:  # Cartesian coordinates
-        #         for k, ind in enumerate(indices):  # 步数
-        #             for j, sli in enumerate(location):
-        #                 poses[k, j, :] = np.dot(poses[k, :, sli], lats)
-        #
         elif "/UnitAtomInfo" in hf.keys():  # phonon 仅读取单胞信息
             raise NotImplementedError("phonon.h5 is not supported yet")
-            # hfDict = load_h5(absfile)
-            # s = _get_structure(hfDict, "/UnitAtomInfo")
-            # elements = np.array(get_ele_from_h5(absfile), dtype=object)
-            # Natom = len(elements)
-            # poses = [s.cart_coords]
-            # lattices = [s.lattice.matrix]
-            # Nstep = 1
-            #
-            # atomFixs = np.empty(shape=(Natom, 3))
-            # atomFix = np.full(shape=(Natom, 3), fill_value="False")
-            # atomFixs[0] = atomFix
-            # latticeFixs = np.empty(shape=(9,))
-            # latticeFix = np.full(shape=(9,), fill_value="False")
-            # latticeFixs[0] = latticeFix
-
-            # iNoncollinear = False
-            # try:  # 自旋计算
-            #     if "/MagInfo/TotalMagOnAtom" in hf.keys():  # collinear
-            #         mag = np.array(hf.get("/MagInfo/TotalMagOnAtom"))  # Natom x 1
-            #     elif "/MagInfo/TotalMagOnAtomX" in hf.keys():  # noncollinear
-            #         magx = np.array(hf.get("/MagInfo/TotalMagOnAtomX"))  # Natom x 1
-            #         magy = np.array(hf.get("/MagInfo/TotalMagOnAtomY"))  # Natom x 1
-            #         magz = np.array(hf.get("/MagInfo/TotalMagOnAtomZ"))  # Natom x 1
-            #         iNoncollinear = True
-            #     else:
-            #         mag = np.zeros(shape=(Natom, 1))
-            #
-            # except Exception as e:
-            #     if str(e):  # ignore empty AssertionError()
-            #         print(e)
-            #     mag = np.zeros(shape=(Natom, 1))
-            #
-            # if iNoncollinear is False:
-            #     mags = np.repeat(mag[np.newaxis, :], Nstep, axis=0).tolist()
-            #     D_mag_fix = {
-            #         "Mag": mags,
-            #         "Fix_x": atomFixs[:, :, 0],
-            #         "Fix_y": atomFixs[:, :, 1],
-            #         "Fix_z": atomFixs[:, :, 2],
-            #         "LatticeFixs": latticeFixs,
-            #     }
-            # else:
-            #     D_mag_fix = {
-            #         "Mag_x": np.repeat(magx[np.newaxis, :], Nstep, axis=0).tolist(),
-            #         "Mag_y": np.repeat(magy[np.newaxis, :], Nstep, axis=0).tolist(),
-            #         "Mag_z": np.repeat(magz[np.newaxis, :], Nstep, axis=0).tolist(),
-            #         "Fix_x": atomFixs[:, :, 0],
-            #         "Fix_y": atomFixs[:, :, 1],
-            #         "Fix_z": atomFixs[:, :, 2],
-            #         "LatticeFixs": latticeFixs,
-            #     }
-
-            # if scaled:  # Fractional coordinates
-            #     for j, sli in enumerate(location):  # atom si
-            #         poses[k, j, :] = np.dot(wrapped_poses[:, sli], np.eye(3, 3))
-            # else:  # Cartesian coordinates
-            #     for j, sli in enumerate(location):
-            #         poses[k, j, :] = np.dot(wrapped_poses[:, sli], lats)
 
         else:  # rho, potential, elf, pcharge
             hfDict = load_h5(absfile)
             s = _get_structure(hfDict, "/AtomInfo")
             elements = np.array(get_ele_from_h5(absfile), dtype=object)
             poses = [s.cart_coords]
             lattices = [s.lattice.matrix]
@@ -788,15 +635,15 @@
             D_mag_fix = None
 
         elif "UnitAtomInfo" in data:  # phonon task
             raise NotImplementedError("Read from phonon.json is not supported yet.")
         elif "IniFin" in data:  # neb.json
             raise NotImplementedError("Read from neb.json is not supported yet.")
         elif "WannierInfo" in data:
-            raise NotImplementedError("wannier.json has no stucture info!")
+            raise NotImplementedError("wannier.json has no structure info!")
 
         else:  # multi-steps task
             if "Structures" in data:
                 Total_step = len(data["Structures"])  # aimd.json
             else:
                 Total_step = len(data)  # relax.json, neb01.json
 
@@ -992,22 +839,22 @@
     Parameters
     ----------
     dir_h5 : str
         h5文件路径
 
     Returns
     -------
-    datas: dict
+    data: dict
         数据字典
 
     Examples
     --------
     >>> from dspawpy.io.read import load_h5
-    >>> datas = load_h5(dir_h5='dspawpy_proj/dspawpy_tests/inputs/2.2/scf.h5')
-    >>> datas.keys()
+    >>> data = load_h5(dir_h5='dspawpy_proj/dspawpy_tests/inputs/2.2/scf.h5')
+    >>> data.keys()
     dict_keys(['/AtomInfo/CoordinateType', '/AtomInfo/Elements', '/AtomInfo/Grid', '/AtomInfo/Lattice', '/AtomInfo/Position', '/Eigenvalue/CBM/BandIndex', '/Eigenvalue/CBM/Energy', '/Eigenvalue/CBM/Kpoint', '/Eigenvalue/NumberOfBand', '/Eigenvalue/Spin1/BandEnergies', '/Eigenvalue/Spin1/Kpoints/Coordinates', '/Eigenvalue/Spin1/Kpoints/Grid', '/Eigenvalue/Spin1/Kpoints/NumberOfKpoints', '/Eigenvalue/Spin1/Occupation', '/Eigenvalue/VBM/BandIndex', '/Eigenvalue/VBM/Energy', '/Eigenvalue/VBM/Kpoint', '/Electron', '/Energy/EFermi', '/Energy/TotalEnergy', '/Energy/TotalEnergy0', '/Force/ForceOnAtoms', '/Stress/Direction', '/Stress/Pressure', '/Stress/Stress', '/Stress/Total', '/Structures/FinalStep', '/Structures/Step-1/Lattice', '/Structures/Step-1/Position'])
     """
 
     @logger.catch
     def get_names(key, h5_object):
         names.append(h5_object.name)
 
@@ -1017,37 +864,39 @@
             if name_inTheList.find(name + "/") != -1:
                 return False
         return True
 
     import numpy as np
 
     @logger.catch
-    def get_datas(key, h5_object):
+    def get_data(key, h5_object):
         if is_dataset(h5_object.name):
-            data = np.asarray(h5_object)
-            if data.dtype == "|S1":  # 转成字符串 并根据";"分割
-                byte2str = [str(bi, "utf-8") for bi in data]
+            _data = np.asarray(h5_object)
+            if _data.dtype == "|S1":  # 转成字符串 并根据";"分割
+                byte2str = [str(bi, "utf-8") for bi in _data]
                 string = ""
                 for char in byte2str:
                     string += char
-                data = np.array([elem for elem in string.strip().split(";")])
+                _data = np.array([elem for elem in string.strip().split(";")])
             # "/group1/group2/.../groupN/dataset" : value
-            datas[h5_object.name] = data.tolist()
+            data[h5_object.name] = _data.tolist()
+
+    import os
 
     from h5py import File
 
     import os
 
     with File(os.path.abspath(dir_h5), "r") as fin:
         names = []
-        datas = {}
+        data = {}
         fin.visititems(get_names)
-        fin.visititems(get_datas)
+        fin.visititems(get_data)
 
-        return datas
+        return data
 
 
 @logger.catch
 def load_h5_todict(dir_h5: str) -> dict:
     """与上一个函数区别在于合并了部分同类数据，例如
 
     /Structures/Step-1/* 和 /Structures/Step-2/* 并入 /Structures/ 组内
@@ -1058,20 +907,20 @@
             D[L[0]] = L[1]
             return
         else:
             if L[0] not in D.keys():
                 D[L[0]] = {}
             create_dict(L[1:], D[L[0]])
 
-    datas = load_h5(dir_h5)
+    data = load_h5(dir_h5)
 
     groups_value_list = []
-    for key in datas.keys():
+    for key in data.keys():
         tmp_list = key[1:].strip().split("/")  # [1:] 截去root
-        tmp_list.append(datas[key])
+        tmp_list.append(data[key])
         # groups_value_list[i]结构: [group1, group2, ..., groupN, dataset, value]
         groups_value_list.append(tmp_list)
 
     groups_value_dict = {}
     for data in groups_value_list:
         create_dict(data, groups_value_dict)
 
@@ -1241,16 +1090,15 @@
     # h5 -> CompleteDos Obj
     total_dos = _get_total_dos(dos)
     structure = _get_structure(dos, "/AtomInfo")
     N = len(structure)
     pdos = [{} for i in range(N)]
     number_of_spin = 2 if dos["/DosInfo/SpinType"][0] == "collinear" else 1
 
-    from pymatgen.electronic_structure.core import Orbital
-    from pymatgen.electronic_structure.core import Spin
+    from pymatgen.electronic_structure.core import Orbital, Spin
 
     for i in range(number_of_spin):
         spin_key = "Spin" + str(i + 1)
         spin = Spin.up if i == 0 else Spin.down
         if dos["/DosInfo/Project"][0]:
             atomindexs = dos["/DosInfo/" + spin_key + "/ProjectDos/AtomIndexs"][0]
             orbitindexs = dos["/DosInfo/" + spin_key + "/ProjectDos/OrbitIndexs"][0]
@@ -1284,16 +1132,15 @@
     # json -> CompleteDos Obj
     total_dos = _get_total_dos_json(dos)
     structure = _get_structure_json(dos["AtomInfo"])
     N = len(structure)
     pdos = [{} for i in range(N)]
     number_of_spin = 2 if dos["DosInfo"]["SpinType"] == "collinear" else 1
 
-    from pymatgen.electronic_structure.core import Orbital
-    from pymatgen.electronic_structure.core import Spin
+    from pymatgen.electronic_structure.core import Orbital, Spin
 
     for i in range(number_of_spin):
         spin_key = "Spin" + str(i + 1)
         spin = Spin.up if i == 0 else Spin.down
         if dos["DosInfo"]["Project"]:
             project = dos["DosInfo"][spin_key]["ProjectDos"]
             for p in project:
@@ -1369,14 +1216,15 @@
     else:
         number_of_spin = 2
 
     symmetry_kPoints_index = band[f"/{bd}/SymmetryKPointsIndex"]
 
     efermi = band[f"/{bd}/EFermi"][0]
     eigenvals = {}
+    import numpy as np
     from pymatgen.electronic_structure.core import Spin
     import numpy as np
 
     for i in range(number_of_spin):
         spin_key = "Spin" + str(i + 1)
         spin = Spin.up if i == 0 else Spin.down
 
@@ -1449,36 +1297,37 @@
     iwan: bool = False,
     zero_to_efermi: bool = False,
 ):
     # syst is only required for wannier band structure
     if iwan:
         bd = "WannBandInfo"
         assert syst is not None, "syst is required for wannier band structure"
-        structure = _get_structure_json(syst["AtomInfo"])
         efermi = syst["Energy"]["EFermi"]
+        structure = _get_structure_json(syst["AtomInfo"])
     else:
         bd = "BandInfo"
+        if "EFermi" in band[bd]:
+            efermi = band[bd]["EFermi"]
+        else:
+            logger.warning("EFermi not found in band data, set to 0")
+            efermi = 0
         structure = _get_structure_json(band["AtomInfo"])
 
     number_of_band = band[bd]["NumberOfBand"]
     number_of_kpoints = band[bd]["NumberOfKpoints"]
-    if band[bd]["SpinType"][0] != "collinear":
+    # ! wannier.json has no SpinType key
+    # if band[bd]["SpinType"][0] != "collinear":
+    if "Spin2" not in band[bd]:
         number_of_spin = 1
     else:
         number_of_spin = 2
 
     symmetry_kPoints_index = band[bd]["SymmetryKPointsIndex"]
-
-    if "EFermi" in band[bd]:
-        efermi = band[bd]["EFermi"]
-    else:
-        logger.warning("EFermi not found in band data, set to 0")
-        efermi = 0
-
     eigenvals = {}
+    import numpy as np
     from pymatgen.electronic_structure.core import Spin
     import numpy as np
 
     for i in range(number_of_spin):
         spin_key = "Spin" + str(i + 1)
         spin = Spin.up if i == 0 else Spin.down
 
@@ -1527,14 +1376,15 @@
                         np.asarray(project_data)
                         .reshape((number_of_kpoints, number_of_band))
                         .T
                     )
                 projections[spin] = projection
 
     if zero_to_efermi:
+        logger.warning("Setting efemi to 0 because zero_to_efermi is True")
         efermi = 0  # set to 0
 
     return structure, kpoints, eigenvals, efermi, labels_dict, projections
 
 
 @logger.catch
 def _get_phonon_band_data_h5(band: dict):
@@ -1592,18 +1442,18 @@
 
     return symmmetry_qpoints, symmetry_qPoints_index, qpoints, structure, frequencies
 
 
 @logger.catch
 def pel_from_as(spath: str, scaled: bool = False):
     """backup here for compatibility"""
-    import numpy as np
-
     import os
 
+    import numpy as np
+
     absfile = os.path.abspath(spath)
     with open(absfile, "r") as f:
         lines = f.readlines()
         Natom = int(lines[1])  # 原子总数
         ele = [line.split()[0] for line in lines[7 : 7 + Natom]]  # 元素列表
 
         # 晶格矢量
@@ -1622,25 +1472,7 @@
 
         if scaled:
             pos = spos
         else:
             pos = np.dot(spos, latv)
 
     return pos, ele, latv
-
-
-@logger.catch
-def _remove_extra_kpoint(
-    band_data: dict, symmetry_kPoints_index: Sequence, number_of_band: int
-):
-    keep_data = []
-    for i in range(len(symmetry_kPoints_index) - 1):
-        if i == 0:
-            start_index = symmetry_kPoints_index[i] - 1
-            end_index = symmetry_kPoints_index[i + 1]
-        else:
-            start_index = symmetry_kPoints_index[i] + 1
-            end_index = symmetry_kPoints_index[i + 1]
-
-        tmp = band_data[start_index * number_of_band : end_index * number_of_band]
-        keep_data.extend(tmp)
-    return keep_data
```

### Comparing `dspawpy-1.3.1/dspawpy/io/structure.py` & `dspawpy-1.3.2/dspawpy/io/structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # -*- coding: utf-8 -*-
+from typing import List, Optional, Union
+
 from loguru import logger
-from typing import List, Union, Optional
+
 from dspawpy.io.utils import reader
 
 
 @logger.catch
 def build_Structures_from_datafile(
     datafile: Union[str, List[str]], si=None, ele=None, ai=None, fmt=None, task="scf"
 ):
```

### Comparing `dspawpy-1.3.1/dspawpy/io/utils.py` & `dspawpy-1.3.2/dspawpy/io/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 # ! some functions are extracted from ase
 # see https://wiki.fysik.dtu.dk/ase/index.html
 
 from typing import List
 from loguru import logger
 import numpy as np
+from loguru import logger
 
 Na = 6.02214179e23  # 阿伏伽德罗常数 单位 /mol
 h = 6.6260696e-34  # 普朗克常数 单位J*s
 kB = 1.3806503e-23  # 玻尔兹曼常数 J/K
 R = Na * kB  # 理想气体常数 J/(K*mol)
 amu = 1.66053906660e-27  # 原子质量单位 kg
 k = 1.380649e-23 / 1.602176634e-19  # eV/K
@@ -268,54 +269,54 @@
 
 atomic_numbers = {}
 for Z, symbol in enumerate(chemical_symbols):
     atomic_numbers[symbol] = Z
 
 
 @logger.catch
-def eles2masses(eles: List[str]) -> np.ndarray:
+def elements2masses(elements: List[str]) -> np.ndarray:
     """将元素列表转换为质量列表
 
     Parameters
     ----------
-    eles : List[str]
+    elements : List[str]
         元素列表
 
     Returns
     -------
     List[float]
         质量列表
 
     Examples
     --------
-    >>> from dspawpy.io.utils import eles2masses
-    >>> eles = ["H", "O"]
-    >>> masses = eles2masses(eles)
+    >>> from dspawpy.io.utils import elements2masses
+    >>> elements = ["H", "O"]
+    >>> masses = elements2masses(elements)
     >>> masses
     [1.008, 15.999]
     """
     masses = []
-    for e in eles:
+    for e in elements:
         masses.append(atomic_masses_iupac2016[atomic_numbers[e]])
     return np.array(masses).tolist()
 
 
 @logger.catch
 def get_ma(elements, positions, Natom):
     """Get the moments of inertia along the principal axes.
 
     The three principal moments of inertia are computed from the
     eigenvalues of the symmetric inertial tensor. Periodic boundary
     conditions are ignored. Units of the moments of inertia are
     amu*angstrom**2.
     """
-    masses = eles2masses(elements)
+    masses = elements2masses(elements)
     com = np.dot(masses, positions) / np.sum(masses)
     positions -= com  # translate center of mass to origin
-    masses = eles2masses(elements)
+    masses = elements2masses(elements)
 
     # Initialize elements of the inertial tensor
     I11 = I22 = I33 = I12 = I13 = I23 = 0.0
     for i in range(Natom):
         x, y, z = positions[i]
         m = masses[i]
 
@@ -481,14 +482,16 @@
 
         if self.geometry == "nonlinear":  # rotational heat capacity
             Cv_r = 3.0 / 2.0 * k
         elif self.geometry == "linear":
             Cv_r = k
         elif self.geometry == "monatomic":
             Cv_r = 0.0
+        else:
+            raise ValueError("Unknown geometry.")
         print(fmt % ("Cv_rot (0->T)", Cv_r * temperature))
         H += Cv_r * temperature
 
         dH_v = self._vibrational_energy_contribution(temperature)
         print(fmt % ("Cv_vib (0->T)", dH_v))
         H += dH_v
 
@@ -510,41 +513,43 @@
             raise RuntimeError(
                 "elements, symmetrynumber, and spin must be "
                 "specified for entropy and free energy "
                 "calculations."
             )
         S = 0.0
         # Translational entropy (term inside the log is in SI units).
-        mass = sum(eles2masses(self.elements)) * amu  # kg/molecule
+        mass = sum(elements2masses(self.elements)) * amu  # kg/molecule
         S_t = (2 * np.pi * mass * kB * temperature / h**2) ** (3.0 / 2)
         S_t *= kB * temperature / self.referencepressure
         S_t = k * (np.log(S_t) + 5.0 / 2.0)
         S += S_t
 
         # Rotational entropy (term inside the log is in SI units).
         if self.geometry == "monatomic":
             S_r = 0.0
         elif self.geometry == "nonlinear":
             inertias = (
                 get_ma(self.elements, self.positions, self.natoms)
                 * amu
                 / (10.0**10) ** 2
             )  # kg m^2
-            S_r = np.sqrt(np.pi * np.product(inertias)) / self.sigma
+            S_r = np.sqrt(np.pi * np.prod(inertias)) / self.sigma
             S_r *= (8.0 * np.pi**2 * kB * temperature / h**2) ** (3.0 / 2.0)
             S_r = k * (np.log(S_r) + 3.0 / 2.0)
         elif self.geometry == "linear":
             inertias = (
                 get_ma(self.elements, self.positions, self.natoms)
                 * amu
                 / (10.0**10) ** 2
             )  # kg m^2
             inertia = max(inertias)  # should be two identical and one zero
             S_r = 8 * np.pi**2 * inertia * kB * temperature / self.sigma / h**2
             S_r = k * (np.log(S_r) + 1.0)
+        else:
+            raise ValueError("Unknown geometry.")
         S += S_r
         # Electronic entropy.
         S_e = k * np.log(2 * self.spin + 1)
         S += S_e
         # Vibrational entropy.
         S_v = self._vibrational_entropy_contribution(temperature)
         S += S_v
@@ -641,42 +646,42 @@
             else:
                 ve.append(float(lines[i].split()[-1]) / 1000)
     if datafile is not None:
         absfile = get_absfile(datafile, task="frequency")
         if absfile.endswith(".h5"):
             from dspawpy.io.read import get_ele_from_h5
 
-            eles = get_ele_from_h5(absfile)
+            elements = get_ele_from_h5(absfile)
             import h5py
 
             data = h5py.File(absfile)
             poses = np.array(data.get("/AtomInfo/Position")).reshape(-1, 3)
 
         elif absfile.endswith(".json"):
             import json
 
             with open(absfile) as f:
                 data = json.load(f)
             atoms = data["AtomInfo"]["Atoms"]
-            eles = []
+            elements = []
             poses = []
             for i in range(len(atoms)):
-                eles.append(atoms[i]["Element"])
+                elements.append(atoms[i]["Element"])
                 poses.append(atoms[i]["Position"])
         else:
             raise TypeError("Only support h5/json file")
     else:
-        eles = elements
+        elements = elements
         poses = positions
 
     # 计算熵的能量贡献
     thermo = IdealGasThermo(
         vib_energies=ve,  # eV
         potentialenergy=potentialenergy,  # eV
-        elements=eles,
+        elements=elements,
         geometry=geometry,
         positions=poses,  # Angstrom
         symmetrynumber=symmetrynumber,
         spin=spin,
     )
     S = thermo.get_entropy(temperature, pressure)
     dE = S * temperature
@@ -720,16 +725,16 @@
     Efermi = dos_data.efermi
     epsilon = dos_d.energies - Efermi  # shift d-band center
 
     N1 = dos_d.densities[spin]
     M1 = epsilon * N1
     from scipy import integrate
 
-    SummaM1 = integrate.simps(M1, epsilon)
-    SummaN1 = integrate.simps(N1, epsilon)
+    SummaM1 = integrate.simpson(M1, x=epsilon)
+    SummaN1 = integrate.simpson(N1, x=epsilon)
 
     return SummaM1 / SummaN1
 
 
 @logger.catch
 def getZPE(fretxt: str = "frequency.txt"):
     """从fretext中读取数据，计算ZPE
@@ -842,15 +847,17 @@
 
     print("--> T*S (eV):", sum_S)
 
     return sum_S
 
 
 @logger.catch
-def get_absfile(datafile: str, task: str, only_h5: bool = False):  # -> absfile
+def get_absfile(
+    datafile: str, task: str, only_h5: bool = False, verbose: bool = True
+):  # -> absfile
     """根据给定的datafile，返回所需数据文件的绝对路径
 
     Parameters
     ----------
     datafile: str
         h5/json数据文件路径或其文件夹路径，可以是相对路径
     task: str
@@ -903,14 +910,16 @@
             if not os.path.isfile(absfile):
                 raise FileNotFoundError(f"No {absfile}")
             else:
                 assert absfile.endswith(".h5") or absfile.endswith(
                     ".json"
                 ), f"Only support h5/json file, but got {absfile}"
 
+    if verbose:
+        logger.info(f"Reading {absfile}...")
     return absfile
 
 
 # extract from ASE
 @logger.catch
 def string2symbols(s: str) -> List[str]:
     """Convert string to list of chemical symbols."""
@@ -933,46 +942,46 @@
 class Formula:
     @logger.catch
     def __init__(
         self,
         formula: str = "",
         *,
         strict: bool = False,
-        format: str = "",
+        fmt: str = "",
         _tree=None,
         _count=None,
     ):
         """Chemical formula object.
 
         Parameters
         ----------
         formula: str
             Text string representation of formula.  Examples: ``'6CO2'``,
             ``'30Cu+2CO'``, ``'Pt(CO)6'``.
         strict: bool
             Only allow real chemical symbols.
-        format: str
-            Reorder according to *format*.  Must be one of hill, metal,
+        fmt: str
+            Reorder according to *fmt*.  Must be one of hill, metal,
             abc or reduce.
 
         Examples
         --------
         >>> from dspawpy.io.utils import Formula
         >>> w = Formula('H2O')
 
         Raises
         ------
         ValueError
             on malformed formula
         """
-        if format:
+        if fmt:
             assert _tree is None and _count is None
-            if format not in {"hill", "metal", "abc", "reduce"}:
-                raise ValueError(f"Illegal format: {format}")
-            formula = Formula(formula).format(format)
+            if fmt not in {"hill", "metal", "abc", "reduce"}:
+                raise ValueError(f"Illegal fmt: {fmt}")
+            formula = format(Formula(formula), fmt)
         self._formula = formula
         self._tree = _tree or parse(formula)
         self._count = _count or count_tree(self._tree)
         if strict:
             for symbol in self._count:
                 if symbol not in atomic_numbers:
                     raise ValueError("Unknown chemical symbol: " + symbol)
@@ -1042,15 +1051,15 @@
             if number:
                 unit = (symb, int(number))
             else:
                 unit = symb
             f = f[m.end() :]
         units.append(unit)
     if len(units) == 1:
-        return unit
+        return units[0]
     return units
 
 
 @logger.catch
 def count_tree(tree):
     if isinstance(tree, str):
         return {tree: 1}
```

### Comparing `dspawpy-1.3.1/dspawpy/io/write.py` & `dspawpy-1.3.2/dspawpy/io/write.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
+from typing import List, Optional, Sequence
+
 from loguru import logger
-from typing import Optional, List, Sequence
 
 Bohr = 0.52917721067  # Angstrom
 
 
 @logger.catch
 def _write_xyz_traj(
     structures: list,
@@ -29,16 +30,16 @@
             f"{absxyz} already exists and will be overwritten!",
             category=UserWarning,
         )
     os.makedirs(os.path.dirname(absxyz), exist_ok=True)
     with open(absxyz, "w") as f:
         # Nstep
         for _, structure in enumerate(structures):
-            eles = [s.species_string for s in structure.sites]
-            f.write("%d\n" % len(eles))
+            elements = [s.species_string for s in structure.sites]
+            f.write("%d\n" % len(elements))
             # lattice
             lm = structure.lattice.matrix
             f.write(
                 'Lattice="%f %f %f %f %f %f %f %f %f" Properties=species:S:1:pos:R:3 pbc="T T T"\n'
                 % (
                     lm[0, 0],
                     lm[0, 1],
@@ -49,17 +50,18 @@
                     lm[2, 0],
                     lm[2, 1],
                     lm[2, 2],
                 )
             )
             # position and element
             poses = structure.cart_coords
-            for j in range(len(eles)):
+            for j in range(len(elements)):
                 f.write(
-                    "%s %f %f %f\n" % (eles[j], poses[j, 0], poses[j, 1], poses[j, 2])
+                    "%s %f %f %f\n"
+                    % (elements[j], poses[j, 0], poses[j, 1], poses[j, 2])
                 )
 
     print(f"==> {absxyz}")
 
 
 @logger.catch
 def _write_dump_traj(
@@ -83,20 +85,20 @@
     logger.warning(f"{absdump} already exists and will be overwritten!")
     os.makedirs(os.path.dirname(absdump), exist_ok=True)
     from dspawpy.io.read import _get_lammps_non_orthogonal_box
 
     with open(absdump, "w") as f:
         for n, structure in enumerate(structures):
             lat = structure.lattice.matrix
-            eles = [s.species_string for s in structure.sites]
+            elements = [s.species_string for s in structure.sites]
             poses = structure.cart_coords
 
             box_bounds = _get_lammps_non_orthogonal_box(lat)
             f.write("ITEM: TIMESTEP\n%d\n" % n)
-            f.write("ITEM: NUMBER OF ATOMS\n%d\n" % (len(eles)))
+            f.write("ITEM: NUMBER OF ATOMS\n%d\n" % (len(elements)))
             f.write("ITEM: BOX BOUNDS xy xz yz xx yy zz\n")
             f.write(
                 "%f %f %f\n%f %f %f\n %f %f %f\n"
                 % (
                     box_bounds[0][0],
                     box_bounds[0][1],
                     box_bounds[0][2],
@@ -105,19 +107,19 @@
                     box_bounds[1][2],
                     box_bounds[2][0],
                     box_bounds[2][1],
                     box_bounds[2][2],
                 )
             )
             f.write("ITEM: ATOMS type x y z id\n")
-            for i in range(len(eles)):
+            for i in range(len(elements)):
                 f.write(
                     "%s %f %f %f %d\n"
                     % (
-                        eles[i],
+                        elements[i],
                         poses[i, 0],
                         poses[i, 1],
                         poses[i, 2],
                         i + 1,
                     )
                 )
     print(f"==> {absdump}")
@@ -192,16 +194,16 @@
     0.055 0.055 0.000     -0.0740864
     0.110 0.110 0.000     -0.8811762
     0.165 0.165 0.000     -2.1283864
     0.220 0.220 0.000     -4.0559144
     0.275 0.275 0.000     -6.8291031
     0.330 0.330 0.000    -10.1550910
     """
-    from dspawpy.io.structure import read
     from dspawpy.io.read import load_h5
+    from dspawpy.io.structure import read
 
     if in_filename.endswith(".h5"):
         data = load_h5(in_filename)
         structure = read(in_filename)[0]
         grid = data["/AtomInfo/Grid"]  # get grid array
         if data_type == "rho" or data_type == "rhoBound":
             vd = data["/Rho/TotalCharge"]
@@ -298,18 +300,19 @@
     ...     individuals=['dspawpy_proj/dspawpy_tests/inputs/supplement/A.h5', 'dspawpy_proj/dspawpy_tests/inputs/supplement/B.h5'],
     ...     output='dspawpy_proj/dspawpy_tests/outputs/doctest/delta_rho.cube') # doctest: +ELLIPSIS
     Reading ...dspawpy_proj/dspawpy_tests/inputs/supplement/AB.h5...
     Reading ...dspawpy_proj/dspawpy_tests/inputs/supplement/A.h5...
     Reading ...dspawpy_proj/dspawpy_tests/inputs/supplement/B.h5...
     ==> ...dspawpy_proj/dspawpy_tests/outputs/doctest/delta_rho.cube
     """
-    from dspawpy.io.structure import read
-    from dspawpy.io.read import load_h5
     import os
 
+    from dspawpy.io.read import load_h5
+    from dspawpy.io.structure import read
+
     abstotal = os.path.abspath(total)
     structure = read(abstotal)[0]
 
     if abstotal.endswith(".h5"):
         dataAB = load_h5(abstotal)
         rho = dataAB["/Rho/TotalCharge"]
         grid = dataAB["/AtomInfo/Grid"]
@@ -364,15 +367,15 @@
 ):
     r"""Deprecated. Use :func:`dspawpy.io.structure.write` instead."""
     logger.warning(
         "dspawpy.io.write.to_file is deprecated"
         "Use dspawpy.io.structure.write instead.",
         DeprecationWarning,
     )
-    from .structure import write
+    from dspawpy.io.structure import write
 
     write(structure, filename, fmt, coords_are_cartesian)
 
 
 @logger.catch
 def _write_atoms(fileobj, structure, idirect: bool = False):
     fileobj.write("DS-PAW Structure\n")
```

### Comparing `dspawpy-1.3.1/dspawpy/plot.py` & `dspawpy-1.3.2/dspawpy/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,17 +47,38 @@
 
     Examples
     --------
     >>> from dspawpy.plot import average_along_axis
 
     读取 potential.h5 文件中的数据，绘图并保存原始绘图数据到csv文件
 
-    >>> average_along_axis(datafile='dspawpy_proj/dspawpy_tests/inputs/2.7/potential.h5', task='potential', axis=2, smooth=True, smooth_frac=0.8) # doctest: +ELLIPSIS
-    Reading .../dspawpy_proj/dspawpy_tests/inputs/2.7/potential.h5...
-    <module 'matplotlib.pyplot' from '.../matplotlib/pyplot.py'>
+    >>> plt = average_along_axis(datafile='dspawpy_proj/dspawpy_tests/inputs/3.3/rho.h5', task='rho', axis=2, smooth=True, smooth_frac=0.8) # doctest: +ELLIPSIS
+    >>> plt.savefig('dspawpy_proj/dspawpy_tests/outputs/doctest/rho_h5.png')
+    >>> plt = average_along_axis(datafile='dspawpy_proj/dspawpy_tests/inputs/3.3/rho.json', task='rho', axis=2, smooth=True, smooth_frac=0.8) # doctest: +ELLIPSIS
+    >>> plt.savefig('dspawpy_proj/dspawpy_tests/outputs/doctest/rho_json.png')
+
+    >>> plt = average_along_axis(datafile='dspawpy_proj/dspawpy_tests/inputs/2.7/potential.h5', task='potential', axis=2, smooth=True, smooth_frac=0.8, raw=True) # doctest: +ELLIPSIS
+    >>> plt.savefig('dspawpy_proj/dspawpy_tests/outputs/doctest/potential_h5.png')
+    >>> plt = average_along_axis(datafile='dspawpy_proj/dspawpy_tests/inputs/2.7/potential.json', task='potential', axis=2, smooth=True, smooth_frac=0.8) # doctest: +ELLIPSIS
+    >>> plt.savefig('dspawpy_proj/dspawpy_tests/outputs/doctest/potential_json.png')
+
+    >>> plt = average_along_axis(datafile='dspawpy_proj/dspawpy_tests/inputs/2.8/elf.h5', task='elf', axis=2, smooth=True, smooth_frac=0.8) # doctest: +ELLIPSIS
+    >>> plt.savefig('dspawpy_proj/dspawpy_tests/outputs/doctest/elf_h5.png')
+    >>> plt = average_along_axis(datafile='dspawpy_proj/dspawpy_tests/inputs/2.8/elf.json', task='elf', axis=2, smooth=True, smooth_frac=0.8) # doctest: +ELLIPSIS
+    >>> plt.savefig('dspawpy_proj/dspawpy_tests/outputs/doctest/elf_json.png')
+
+    >>> plt = average_along_axis(datafile='dspawpy_proj/dspawpy_tests/inputs/2.9/pcharge.h5', task='pcharge', axis=2, smooth=True, smooth_frac=0.8) # doctest: +ELLIPSIS
+    >>> plt.savefig('dspawpy_proj/dspawpy_tests/outputs/doctest/pcharge_h5.png')
+    >>> plt = average_along_axis(datafile='dspawpy_proj/dspawpy_tests/inputs/2.9/pcharge.json', task='pcharge', axis=2, smooth=True, smooth_frac=0.8) # doctest: +ELLIPSIS
+    >>> plt.savefig('dspawpy_proj/dspawpy_tests/outputs/doctest/pcharge_json.png')
+
+    >>> plt = average_along_axis(datafile='dspawpy_proj/dspawpy_tests/inputs/2.28/rhoBound.h5', task='rhoBound', axis=2, smooth=True, smooth_frac=0.8) # doctest: +ELLIPSIS
+    >>> plt.savefig('dspawpy_proj/dspawpy_tests/outputs/doctest/rhoBound_h5.png')
+    >>> plt = average_along_axis(datafile='dspawpy_proj/dspawpy_tests/inputs/2.28/rhoBound.json', task='rhoBound', axis=2, smooth=True, smooth_frac=0.8) # doctest: +ELLIPSIS
+    >>> plt.savefig('dspawpy_proj/dspawpy_tests/outputs/doctest/rhoBound_json.png')
     """
     assert task in [
         "rho",
         "potential",
         "elf",
         "pcharge",
         "rhoBound",
@@ -68,15 +89,14 @@
 
     if isinstance(datafile, list) or isinstance(datafile, np.ndarray):
         ys = datafile  # expect np.ndarray or list
     else:
         from dspawpy.io.utils import get_absfile
 
         absfile = get_absfile(datafile, task)
-        print(f"Reading {absfile}...")
 
         if absfile.endswith(".h5"):
             hfile = absfile
             from dspawpy.io.read import load_h5
 
             hdict = load_h5(hfile)
             grid = hdict["/AtomInfo/Grid"]
@@ -102,17 +122,16 @@
                 _key = f"/ELF/{subtype}"
             elif task == "pcharge":
                 if subtype is None:
                     subtype = "TotalCharge"
                 _key = f"/Pcharge/1/{subtype}"
             elif task == "rhoBound":
                 if subtype is None:
-                    _key = "/Rho"
-                else:
-                    _key = subtype
+                    subtype = "TotalCharge"
+                _key = f"/Rho/{subtype}"
             else:
                 raise ValueError("Only support rho, potential, elf, pcharge, rhoBound")
 
             if _key not in hdict:
                 raise KeyError(f"No {_key} key")
 
             tmp_pot = np.asarray(hdict[_key]).reshape([-1, 1], order="C")
@@ -148,57 +167,43 @@
                 ys = np.asarray(jdict["ELF"][subtype]).reshape(grid, order="F")
             elif task == "pcharge":
                 if subtype is None:
                     subtype = "TotalCharge"
                 ys = np.asarray(jdict["Pcharge"][0][subtype]).reshape(grid, order="F")
             else:
                 if subtype is None:
-                    subtype = "Rho"
-                ys = np.asarray(jdict[subtype]).reshape(grid, order="F")
+                    subtype = "TotalCharge"
+                ys = np.asarray(jdict["Rho"][subtype]).reshape(grid, order="F")
 
         else:
-            raise TypeError("Only suport h5/json file")
+            raise TypeError("Only support h5/json file")
 
     all_axis = [0, 1, 2]
     all_axis.remove(axis)
     y = np.mean(ys, tuple(all_axis))  # type: ignore
     x = np.arange(len(y))
 
     import matplotlib.pyplot as plt
 
     if raw:
-        try:
-            import polars as pl
+        import polars as pl
 
-            pl.DataFrame({"x": x, "y": y}).write_csv(
-                f"raw{task}_axis{axis}.csv",
-            )
-        except ModuleNotFoundError:
-            import pandas as pd
-
-            pd.DataFrame({"x": x, "y": y}).to_csv(
-                f"raw{task}_axis{axis}.csv",
-            )
+        pl.DataFrame({"x": x, "y": y}).write_csv(
+            f"raw{task}_axis{axis}.csv",
+        )
     if smooth:
         import statsmodels.api as sm
 
         s = sm.nonparametric.lowess(y, x, frac=smooth_frac)
         if raw:
-            try:
-                import polars as pl
-
-                pl.DataFrame({"x": s[:, 0], "y": s[:, 1]}).write_csv(
-                    f"raw{task}_axis{axis}_smooth.csv",
-                )
-            except ModuleNotFoundError:
-                import pandas as pd
+            import polars as pl
 
-                pd.DataFrame({"x": s[:, 0], "y": s[:, 1]}).to_csv(
-                    f"raw{task}_axis{axis}_smooth.csv",
-                )
+            pl.DataFrame({"x": s[:, 0], "y": s[:, 1]}).write_csv(
+                f"raw{task}_axis{axis}_smooth.csv",
+            )
 
         plt.plot(s[:, 0], s[:, 1], label="macroscopic average", **kwargs)
 
     plt.plot(x, y, **kwargs)
 
     return plt
 
@@ -240,23 +245,15 @@
 
     Examples
     ----------
     >>> from dspawpy.plot import plot_aimd
 
     读取 aimd.h5 文件内容，画出动能、总能、温度、体积的收敛过程图，并保存相应数据到 rawaimd_*.csv 中
 
-    >>> plot_aimd(datafile='dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5', flags_str='1245', raw=False, show=False, figname=None) # doctest: +ELLIPSIS
-    For subfigure 1
-    Reading .../dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5...
-    For subfigure 2
-    Reading .../dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5...
-    For subfigure 4
-    Reading .../dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5...
-    For subfigure 5
-    Reading .../dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5...
+    >>> plot_aimd(datafile='dspawpy_proj/dspawpy_tests/inputs/2.18/aimd.h5', flags_str='1 2 3 4 5', raw=True, show=False, figname="aimdconv.png")
     """
     # 处理用户读取，按顺序去重
     temp = set()
     flags = [x for x in flags_str if x not in temp and (temp.add(x) or True)]
     if " " in flags:  # remove space
         flags.remove(" ")
 
@@ -276,30 +273,27 @@
 
     fig, axes = plt.subplots(N_figs, 1, sharex=True, figsize=(6, 2 * N_figs))
     if N_figs == 1:  # 'AxesSubplot' object is not subscriptable
         axes = [axes]  # 避免上述类型错误
     fig.suptitle("DSPAW AIMD")
 
     for i, flag in enumerate(flags):
-        print("For subfigure " + flag)
         # 读取数据
-        xs, ys = _read_aimd_converge_data(datafile, flag)
-        if raw:
-            try:
-                import polars as pl
+        if i == 0:
+            xs, ys = _read_aimd_converge_data(datafile, flag, verbose=True)
+        else:
+            xs, ys = _read_aimd_converge_data(datafile, flag, verbose=False)
+        logger.info("For subfigure " + flag)
 
-                pl.DataFrame({"x": xs, "y": ys}).write_csv(
-                    f"rawaimd_{flag}.csv",
-                )
-            except ModuleNotFoundError:
-                import pandas as pd
+        if raw:
+            import polars as pl
 
-                pd.DataFrame({"x": xs, "y": ys}).to_csv(
-                    f"rawaimd_{flag}.csv",
-                )
+            pl.DataFrame({"x": xs, "y": ys}).write_csv(
+                f"rawaimd_{flag}.csv",
+            )
 
         axes[i].plot(xs, ys)  # 绘制坐标点
         # 子图的y轴标签
         if flag == "1":
             axes[i].set_ylabel("Kinetic Energy (eV)")
         elif flag == "2":
             axes[i].set_ylabel("Energy (eV)")
@@ -314,15 +308,15 @@
     # save and show
     if figname:
         import os
 
         absfig = os.path.abspath(figname)
         os.makedirs(os.path.dirname(absfig), exist_ok=True)
         plt.savefig(absfig, dpi=300)
-        print(f"==> {absfig}")
+        logger.info(f"==> {absfig}")
     if show:
         plt.show()
 
 
 @logger.catch
 def plot_bandunfolding(
     datafile: str = "band.h5",
@@ -355,21 +349,19 @@
 
     Examples
     --------
 
     绘图并保存绘图数据到rawbandunfolding.csv
 
     >>> from dspawpy.plot import plot_bandunfolding
-    >>> plot_bandunfolding("dspawpy_proj/dspawpy_tests/inputs/2.22/band.h5", raw=True) # doctest: +ELLIPSIS
-    Reading .../dspawpy_proj/dspawpy_tests/inputs/2.22/band.h5...
+    >>> plt = plot_bandunfolding("dspawpy_proj/dspawpy_tests/inputs/2.22/band.h5", raw=True) # doctest: +ELLIPSIS
     """
     from dspawpy.io.utils import get_absfile
 
     absfile = get_absfile(datafile, task="band")
-    print(f"Reading {absfile}...")
     import numpy as np
 
     if absfile.endswith(".h5"):
         from h5py import File
 
         f = File(absfile, "r")
         if ef is None:
@@ -395,31 +387,17 @@
     celtot = np.array(data).reshape((number_of_kpoints, number_of_band)).T
     proj_wt = np.array(weight).reshape((number_of_kpoints, number_of_band)).T
     X2, Y2, Z2, emin = getEwtData(
         number_of_kpoints, number_of_band, celtot, proj_wt, ef, de, dele
     )
 
     if raw:
-        try:
-            import polars as pl
+        import polars as pl
 
-            pl.DataFrame({"Y": Y2, "Z": Z2}).write_csv(
-                "rawbandunfolding.csv",
-                schemas=["Y", "color"],
-                index_label="X",
-            )  # type: ignore
-        except ModuleNotFoundError:
-            import pandas as pd
-
-            pd.DataFrame({"Y": Y2, "Z": Z2}).to_csv(
-                "rawbandunfolding.csv",
-                header=["Y", "color"],
-                index=True,
-                index_label="X",
-            )
+        pl.DataFrame({"Y": Y2, "Z": Z2}).write_csv("rawbandunfolding.csv")
 
     import matplotlib.pyplot as plt
 
     plt.clf()
     plt.scatter(X2, Y2, c=Z2, cmap="hot")
     plt.xlim(0, 200)
     plt.ylim(emin - 0.5, 15)
@@ -454,35 +432,33 @@
     keys: List[str]
         可选 "AbsorptionCoefficient", "ExtinctionCoefficient", "RefractiveIndex", "Reflectance" 中的任意一个，默认 "AbsorptionCoefficient"
     axes : List[str]
         序号，默认"X", "Y", "Z", "XY", "YZ", "ZX"
     raw : bool
         是否保存绘图数据到csv
 
-    Exapmles
+    Examples
     --------
 
     绘图并保存绘图数据到rawoptical.csv
 
     >>> from dspawpy.plot import plot_optical
-    >>> plot_optical("dspawpy_proj/dspawpy_tests/inputs/2.12/scf.h5", "AbsorptionCoefficient", ['X', 'Y'], prefix='dspawpy_proj/dspawpy_tests/outputs/doctest') # doctest: +ELLIPSIS
-    Reading .../dspawpy_proj/dspawpy_tests/inputs/2.12/scf.h5...
-    >>> plot_optical("dspawpy_proj/dspawpy_tests/inputs/2.12/optical.json", ["AbsorptionCoefficient"], ['X', 'Y'], prefix='dspawpy_proj/dspawpy_tests/outputs/doctest') # doctest: +ELLIPSIS
-    Reading .../dspawpy_proj/dspawpy_tests/inputs/2.12/optical.json...
+    >>> plot_optical("dspawpy_proj/dspawpy_tests/inputs/2.12/scf.h5", "AbsorptionCoefficient", ['X', 'Y'], prefix='dspawpy_proj/dspawpy_tests/outputs/doctest')
+    >>> plot_optical("dspawpy_proj/dspawpy_tests/inputs/2.12/optical.json", ["AbsorptionCoefficient"], ['X', 'Y'], prefix='dspawpy_proj/dspawpy_tests/outputs/doctest', raw=True)
     """
     import matplotlib.pyplot as plt
+    import numpy as np
     from scipy.interpolate import interp1d
+
     from dspawpy.io.utils import get_absfile
-    import numpy as np
 
     if isinstance(keys, str):
         keys = [keys]
 
     absfile = get_absfile(datafile, task="optical")
-    print(f"Reading {absfile}...")
     data = {}
     if absfile.endswith("h5"):
         from dspawpy.io.read import load_h5
 
         data_all = load_h5(absfile)
         energy = data_all["/OpticalInfo/EnergyAxe"]
         for k in keys:
@@ -515,48 +491,30 @@
         plt.legend()
         if prefix == "":
             plt.savefig(f"{k}.png")
         else:
             plt.savefig(f"{prefix}/{k}.png")
 
     if raw:
-        try:
-            import polars as pl
+        import polars as pl
 
-            for k in data:
-                dictOriginal = {"energy": energy}
-                dictInterp = {"energy": energy_spline}
-                for a in axes:
-                    dictOriginal.update(
-                        {k + a: np.asarray(data[k]).reshape(len(energy), 6)[:, dd[a]]}
-                    )
-                    dictInterp.update({k + a: data_spline_dict[k + a]})
-                pl.DataFrame(dictOriginal).write_csv(
-                    f"rawoptical{k}.csv",
-                )
-                pl.DataFrame(dictInterp).write_csv(
-                    f"rawoptical_spline{k}.csv",
-                )
-        except ModuleNotFoundError:
-            import pandas as pd
-
-            for k in data:
-                dictOriginal = {"energy": energy}
-                dictInterp = {"energy": energy_spline}
-                for a in axes:
-                    dictOriginal.update(
-                        {k + a: np.asarray(data[k]).reshape(len(energy), 6)[:, dd[a]]}
-                    )
-                    dictInterp.update({k + a: data_spline_dict[k + a]})
-                pd.DataFrame(dictOriginal).to_csv(
-                    f"rawoptical{k}.csv",
-                )
-                pd.DataFrame(dictInterp).to_csv(
-                    f"rawoptical_spline{k}.csv",
+        for k in data:
+            dictOriginal = {"energy": energy}
+            dictInterp = {"energy": energy_spline}
+            for a in axes:
+                dictOriginal.update(
+                    {k + a: np.asarray(data[k]).reshape(len(energy), 6)[:, dd[a]]}
                 )
+                dictInterp.update({k + a: data_spline_dict[k + a]})
+            pl.DataFrame(dictOriginal).write_csv(
+                f"rawoptical{k}.csv",
+            )
+            pl.DataFrame(dictInterp).write_csv(
+                f"rawoptical_spline{k}.csv",
+            )
 
 
 @logger.catch
 def plot_phonon_thermal(
     datafile: str = "phonon.h5",
     figname: str = "phonon.png",
     show: bool = True,
@@ -581,22 +539,20 @@
     ----------
     figname : str
         图片路径，默认 'phonon.png'
 
     Examples
     --------
     >>> from dspawpy.plot import plot_phonon_thermal
-    >>> plot_phonon_thermal('dspawpy_proj/dspawpy_tests/inputs/2.26/phonon.h5', figname='dspawpy_proj/dspawpy_tests/outputs/doctest/phonon_thermal.png', show=False) # doctest: +ELLIPSIS
-    Reading .../dspawpy_proj/dspawpy_tests/inputs/2.26/phonon.h5...
-    ==> .../dspawpy_proj/dspawpy_tests/outputs/doctest/phonon_thermal.png
+    >>> plot_phonon_thermal('dspawpy_proj/dspawpy_tests/inputs/2.26/phonon.h5', figname='dspawpy_proj/dspawpy_tests/outputs/doctest/phonon_thermal_h5.png', show=False)
+    >>> plot_phonon_thermal('dspawpy_proj/dspawpy_tests/inputs/2.26/phonon.json', figname='dspawpy_proj/dspawpy_tests/outputs/doctest/phonon_thermal_json.png', show=False, raw=True)
     """
     from dspawpy.io.utils import get_absfile
 
     absfile = get_absfile(datafile, task="phonon")
-    print(f"Reading {absfile}...")
 
     import numpy as np
 
     if absfile.endswith(".h5"):
         hfile = absfile
         from h5py import File
 
@@ -619,40 +575,26 @@
         entropy = np.array(data["ThermalInfo"]["Entropy"])
         heat_capacity = np.array(data["ThermalInfo"]["HeatCapacity"])
         helmholts_free_energy = np.array(data["ThermalInfo"]["HelmholtzFreeEnergy"])
     else:
         raise TypeError("Only support h5/json file")
 
     if raw:
-        try:
-            import polars as pl
-
-            pl.DataFrame(
-                {
-                    "temp": temp,
-                    "entropy": entropy,
-                    "heat_capacity": heat_capacity,
-                    "helmholts_free_energy": helmholts_free_energy,
-                }
-            ).write_csv(
-                "rawphonon.csv",
-            )
-        except ModuleNotFoundError:
-            import pandas as pd
+        import polars as pl
 
-            pd.DataFrame(
-                {
-                    "temp": temp,
-                    "entropy": entropy,
-                    "heat_capacity": heat_capacity,
-                    "helmholts_free_energy": helmholts_free_energy,
-                }
-            ).to_csv(
-                "rawphonon.csv",
-            )
+        pl.DataFrame(
+            {
+                "temp": temp,
+                "entropy": entropy,
+                "heat_capacity": heat_capacity,
+                "helmholts_free_energy": helmholts_free_energy,
+            }
+        ).write_csv(
+            "rawphonon.csv",
+        )
 
     import matplotlib.pyplot as plt
 
     plt.plot(temp, entropy, c="red", label="Entropy (J/K/mol)")
     plt.plot(temp, heat_capacity, c="green", label="Heat Capacity (J/K/mol)")
     plt.plot(
         temp, helmholts_free_energy, c="blue", label="Helmholtz Free Energy (kJ/mol)"
@@ -668,15 +610,15 @@
     # save and show
     if figname:
         import os
 
         absfig = os.path.abspath(figname)
         os.makedirs(os.path.dirname(absfig), exist_ok=True)
         plt.savefig(absfig, dpi=300)
-        print(f"==> {absfig}")
+        logger.info(f"==> {absfig}")
     if show:
         plt.show()
 
 
 @logger.catch
 def plot_polarization_figure(
     directory: str,
@@ -708,16 +650,16 @@
     -------
     axes: matplotlib.axes._subplots.AxesSubplot
         可传递给其他函数进行进一步处理
 
     Examples
     --------
     >>> from dspawpy.plot import plot_polarization_figure
-    >>> result = plot_polarization_figure(directory='dspawpy_proj/dspawpy_tests/inputs/2.20', figname='dspawpy_proj/dspawpy_tests/outputs/doctest/pol.png', show=False) # doctest: +ELLIPSIS
-    ==> .../dspawpy_proj/dspawpy_tests/outputs/doctest/pol.png
+    >>> result = plot_polarization_figure(directory='dspawpy_proj/dspawpy_tests/inputs/2.20', figname='dspawpy_proj/dspawpy_tests/outputs/doctest/pol1.png', show=False, annotation=True, annotation_style=1)
+    >>> result = plot_polarization_figure(directory='dspawpy_proj/dspawpy_tests/inputs/2.20', figname='dspawpy_proj/dspawpy_tests/outputs/doctest/pol2.png', show=False, annotation=True, annotation_style=2)
     """
     assert repetition >= 0, "The number of repetitions must be a natural number"
     subfolders, quantum, totals = _get_subfolders_quantum_totals(directory)
     number_sfs = [int(sf) for sf in subfolders]
     import matplotlib.pyplot as plt
 
     fig, axes = plt.subplots(1, 3, sharey=True)
@@ -786,32 +728,27 @@
                             ys[-1, i] - np.max(ys) / repetition / 5,
                         ),
                     )
             else:
                 raise ValueError("annotation_style must be 1 or 2")
 
         if raw:
-            try:
-                import polars as pl
-
-                pl.DataFrame(ys).write_csv(f"pol_{xyz[j]}.csv")
-            except ModuleNotFoundError:
-                import pandas as pd
+            import polars as pl
 
-                pd.DataFrame(ys).to_csv(f"pol_{xyz[j]}.csv")
+            pl.DataFrame(ys).write_csv(f"pol_{xyz[j]}.csv")
 
     plt.tight_layout()
     # save and show
     if figname:
         import os
 
         absfig = os.path.abspath(figname)
         os.makedirs(os.path.dirname(absfig), exist_ok=True)
         plt.savefig(absfig, dpi=300)
-        print(f"==> {absfig}")
+        logger.info(f"==> {absfig}")
     if show:
         plt.show()
 
     return axes
 
 
 @logger.catch
@@ -849,17 +786,16 @@
         except Exception:
             pass
     subfolders.sort()  # 从小到大排序
 
     # quantum number if constant across the whole calculation, read only once
     absh5 = f"{os.path.join(absdir, subfolders[0])}/scf.h5"
     absjs = f"{os.path.join(absdir, subfolders[0])}/polarization.json"
-    from h5py import File
-
     import numpy as np
+    from h5py import File
 
     if os.path.isfile(absjs):
         quantum = np.array(File(absh5).get("/PolarizationInfo/Quantum"))
     elif os.path.isfile(absjs):
         with open(absjs, "r") as f:
             from json import load
 
@@ -927,15 +863,17 @@
         if x > Z2_half:
             Z2[i] = Z2_half
 
     return X2, Y2, Z2, emin
 
 
 @logger.catch(exception=ValueError)
-def _read_aimd_converge_data(datafile: str, index: Optional[str] = None):
+def _read_aimd_converge_data(
+    datafile: str, index: Optional[str] = None, verbose: bool = True
+):
     """从datafile指定的路径读取index指定的数据，返回绘图用的xs和ys两个数组
 
     Parameters
     ----------
     datafile : str or list
         hdf5文件路径，如 'aimd.h5' 或 ['aimd.h5', 'aimd2.h5']
     index : str
@@ -961,21 +899,20 @@
         xs = np.linspace(1, len(xs), len(xs))
         return xs, ys
 
     # search datafile in the given directory
     elif isinstance(datafile, str):
         from dspawpy.io.utils import get_absfile
 
-        absfile = get_absfile(datafile, task="aimd")
+        absfile = get_absfile(datafile, task="aimd", verbose=verbose)
 
         if datafile.endswith("h5"):
             from h5py import File
 
             hf = File(absfile)  # 加载h5文件
-            print(f"Reading {absfile}...")
             Nstep = len(np.array(hf.get("/Structures"))) - 2  # 步数（可能存在未完成的）
             ys = np.full(Nstep, np.nan)  # 准备一个空数组
             # 开始读取
             if index == "5":
                 for i in range(1, Nstep + 1):
                     ys[i - 1] = np.linalg.det(
                         np.array(hf.get("/Structures/Step-%d/Lattice" % i))
@@ -1118,19 +1055,20 @@
 
     >>> bdp = BSDOSPlotter(bs_projection=None,dos_projection="elements")
     >>> plt = bdp.get_plot(bs=band_data, dos=dos_data)
 
     for old version pymatgen, it returns plt, otherwise may return axes, ref to userscripts for how to user them.
     """
     import numpy as np
-
     import palettable
 
     if colors is None:
-        colors: list = palettable.colorbrewer.qualitative.Set1_9.mpl_colors  # type: ignore
+        _colors = palettable.colorbrewer.qualitative.Set1_9.mpl_colors  # type: ignore
+    else:
+        _colors = colors
 
     # self -> BSDOSPlotter
     bs_projection = bdp.bs_projection
     dos_projection = bdp.dos_projection
     vb_energy_range = bdp.vb_energy_range
     cb_energy_range = bdp.cb_energy_range
     fixed_cb_energy = bdp.fixed_cb_energy
@@ -1270,43 +1208,43 @@
         if spin in band_energies:
             for band_idx, band in enumerate(band_energies[spin]):
                 current_pos = 0
                 for x_distances in x_distances_list:
                     sub_band = band[current_pos : current_pos + len(x_distances)]
                     # ! highlight the band close to the Fermi level
                     if np.max(np.abs(sub_band)) < demax:
-                        bs_ax.plot(x_distances, sub_band, color=colors[0], linewidth=3)
+                        bs_ax.plot(x_distances, sub_band, color=_colors[0], linewidth=3)
                     else:
                         if spin == Spin.up:
                             bs_ax.plot(
-                                x_distances, sub_band, color=colors[0], linewidth=1
+                                x_distances, sub_band, color=_colors[0], linewidth=1
                             )
                         elif spin == Spin.down:
                             bs_ax.plot(
-                                x_distances, sub_band, color=colors[1], linewidth=1
+                                x_distances, sub_band, color=_colors[1], linewidth=1
                             )
                     current_pos += len(x_distances)
 
     # add legend for band structure
     if spin_count == 2:
         if bs_legend and not rgb_legend:
             handles = []
 
             if bs_projection is None:
                 import matplotlib.lines as mlines
 
                 handles = [
                     mlines.Line2D(
-                        [], [], linewidth=2, color=colors[0], label="spin up"
+                        [], [], linewidth=2, color=_colors[0], label="spin up"
                     ),
                     mlines.Line2D(
                         [],
                         [],
                         linewidth=2,
-                        color=colors[1],
+                        color=_colors[1],
                         label="spin down",
                     ),
                 ]
 
             bs_ax.legend(
                 handles=handles,
                 fancybox=True,
@@ -1350,20 +1288,20 @@
                     for idx, el in enumerate(elements):
                         if spin_count == 1:
                             el_dos = dos.get_element_dos()
                             dos_densities = el_dos[Element(el)].densities[spin] * int(
                                 spin
                             )
                             label = el if spin == Spin.up else None
-                            dos_ax.plot(dos_densities, dos_energies, color=colors[idx])
+                            dos_ax.plot(dos_densities, dos_energies, color=_colors[idx])
                             dos_ax.fill_betweenx(
                                 dos_energies,
                                 0,
                                 dos_densities,
-                                color=colors[idx],
+                                color=_colors[idx],
                                 alpha=alpha,
                                 label=label,
                             )
                         elif spin_count == 2:
                             if el not in ["O", "Cu"]:  # TODO generalize
                                 continue
                             el_spd_dos = dos.get_element_spd_dos(el)
@@ -1374,21 +1312,21 @@
                                     continue
                                 if orb in el_spd_dos:
                                     dos_densities = el_spd_dos[orb].densities[
                                         spin
                                     ] * int(spin)
                                     label = f"{el}-{orb}" if spin == Spin.up else None  # type: ignore
                                     dos_ax.plot(
-                                        dos_densities, dos_energies, color=colors[idx]
+                                        dos_densities, dos_energies, color=_colors[idx]
                                     )
                                     dos_ax.fill_betweenx(
                                         dos_energies,
                                         0,
                                         dos_densities,
-                                        color=colors[idx],
+                                        color=_colors[idx],
                                         alpha=alpha,
                                         label=label,
                                     )
 
         # get index of lowest and highest energy being plotted, used to help auto-scale DOS x-axis
         emin_idx = next(x[0] for x in enumerate(dos_energies) if x[1] >= emin)
         emax_idx = len(dos_energies) - next(
@@ -1430,16 +1368,16 @@
 
     return plt
 
 
 @logger.catch
 def plot_dos(
     dosplotter,
-    xlim: Optional[List[float]] = None,
-    ylim: Optional[List[float]] = None,
+    xlim: Optional[Tuple[float, float]] = None,
+    ylim: Optional[Tuple[float, float]] = None,
     invert_axes: bool = False,
     beta_dashed: bool = False,
     raw: bool = False,
 ):
     """Get a matplotlib plot showing the DOS.
 
     Args:
@@ -1470,17 +1408,16 @@
     import matplotlib.pyplot as plt
 
     if isinstance(ax, type(plt)):
         ax = ax.gca()  # type: ignore
 
     # Note that this complicated processing of energies is to allow for
     # stacked plots in matplotlib.
-    from pymatgen.electronic_structure.core import Spin
-
     import numpy as np
+    from pymatgen.electronic_structure.core import Spin
 
     for dos in dosplotter._doses.values():
         energies = dos["energies"]
         densities = dos["densities"]
         if not ys:
             ys = {
                 Spin.up: np.zeros(energies.shape),
@@ -1576,19 +1513,12 @@
     legend_text = (
         ax.get_legend().get_texts()
     )  # all the text.Text instance in the legend
     plt.setp(legend_text, fontsize=30)
     plt.tight_layout()
 
     if raw:
-        try:
-            import polars as pl
-
-            df = pl.DataFrame(dd)
-            df.write_csv("dos_raw.csv")
-        except ModuleNotFoundError:
-            import pandas as pd
-
-            df = pd.DataFrame(dd)
-            df.to_csv("dos_raw.csv")
+        import polars as pl
 
+        df = pl.DataFrame(dd)
+        df.write_csv("dos_raw.csv")
     return ax
```

### Comparing `dspawpy-1.3.1/dspawpy.egg-info/PKG-INFO` & `dspawpy-1.3.2/dspawpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 1.3.1
+Version: 1.3.2
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 Author-email: ZhengZhilin@hzwtech.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pymatgen
 Requires-Dist: statsmodels
 Requires-Dist: h5py
 Requires-Dist: prompt_toolkit
 Requires-Dist: loguru
-Requires-Dist: polars
+Requires-Dist: polars>=0.18
 Requires-Dist: ruamel.yaml
 
 ![Pyversion](https://img.shields.io/badge/dynamic/json?query=info.requires_python&label=python&url=https%3A%2F%2Fpypi.org%2Fpypi%2Fgeojson-rewind%2Fjson)
 ![PyPI](https://img.shields.io/pypi/v/dspawpy?label=pypi%20package)
 ![PyPI - Downloads](https://static.pepy.tech/badge/dspawpy/month)
 
 # Introduction （简介）
@@ -37,14 +37,22 @@
 
 ```bash
 conda install -c conda-forge dspawpy
 ```
 
 ## CHANGELOG （版本更新简述）
 
+### 1.3.2
+
+- 重要变更： 使用python3.8以下版本将无法启动程序
+- 重要变更： 正式用 polars 库替换 pandas 库
+- BUG修复： 移除setup.py中已不存在的ecli入口
+- BUG修复： wannier.json 不存在 SpinType 键导致读取失败
+- BUG修复： 瓦尼尔能带对比时，未正确读取 system.json 中的费米能级信息
+
 ### 1.3.1
 
 - BUG修复： 修复userscripts和cli中的一些问题
 - BUG修复： 修复json文件读取函数中的导包语句缺失问题
 - 功能强化： 10.2 支持读取aimd.json文件绘制物理量变化曲线图（仅无法读取压力变化）
 
 ### 1.3.0
```

### Comparing `dspawpy-1.3.1/dspawpy.egg-info/SOURCES.txt` & `dspawpy-1.3.2/dspawpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dspawpy-1.3.1/setup.py` & `dspawpy-1.3.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,31 +10,29 @@
         encoding="utf-8",
     ) as fin:
         return fin.read()
 
 
 setup(
     name="dspawpy",
-    version="1.3.1",
+    version="1.3.2",
     packages=find_packages(),
     url="http://www.hzwtech.com/",
     license="MIT",
     author="Hzwtech",
     author_email="ZhengZhilin@hzwtech.com",
     description="Tools for dspaw",
     install_requires=[
         "pymatgen",
         "statsmodels",
         "h5py",  # parse h5
         "prompt_toolkit",  # cli completer
         "loguru",  # log
-        "polars",  # speed up pandas
+        "polars>=0.18",  # speed up pandas, write_csv starts from 0.18
         "ruamel.yaml",  # ordered yaml
     ],
     python_requires=">=3.8",
-    entry_points={
-        "console_scripts": ["cli=dspawpy.cli.cli:main", "ecli=dspawpy.cli.cli_en:main"]
-    },
+    entry_points={"console_scripts": ["cli=dspawpy.cli.cli:main"]},
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     license_files=("LICENSE.txt",),
 )
```

