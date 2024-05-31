# Comparing `tmp/nonebot_plugin_qqshell-0.1.0a1.tar.gz` & `tmp/nonebot_plugin_qqshell-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_qqshell-0.1.0a1.tar", max compression
+gzip compressed data, was "nonebot_plugin_qqshell-0.1.0a2.tar", max compression
```

## Comparing `nonebot_plugin_qqshell-0.1.0a1.tar` & `nonebot_plugin_qqshell-0.1.0a2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      689 2024-05-31 07:13:06.252066 nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/__init__.py
--rw-r--r--   0        0        0      793 2024-05-31 06:37:34.682017 nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/config.py
--rw-r--r--   0        0        0     1428 2024-05-31 06:38:08.519375 nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/handler.py
--rw-r--r--   0        0        0      685 2024-05-31 06:08:33.155475 nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/services.py
--rw-r--r--   0        0        0    39455 2024-05-11 08:59:15.461050 nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/static/images/rikka1.png
--rw-r--r--   0        0        0      264 2024-05-11 07:23:59.255421 nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/template_env.py
--rw-r--r--   0        0        0      520 2024-05-30 09:13:07.638186 nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/templates/shell_panel.html
--rw-r--r--   0        0        0     2040 2024-05-31 05:56:20.152484 nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/templates/xterm.html
--rw-r--r--   0        0        0        0 2024-05-30 05:31:27.596571 nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/utils/__init__.py
--rw-r--r--   0        0        0     2271 2024-05-31 06:26:22.526574 nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/utils/shell.py
--rw-r--r--   0        0        0      651 2024-05-31 07:20:56.878477 nonebot_plugin_qqshell-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     1346 2024-05-31 07:06:11.790769 nonebot_plugin_qqshell-0.1.0a1/README.md
--rw-r--r--   0        0        0     2148 1970-01-01 00:00:00.000000 nonebot_plugin_qqshell-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0      561 2024-05-31 07:23:50.129422 nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/__init__.py
+-rw-r--r--   0        0        0      793 2024-05-31 06:37:34.682017 nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/config.py
+-rw-r--r--   0        0        0     1428 2024-05-31 06:38:08.519375 nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/handler.py
+-rw-r--r--   0        0        0      685 2024-05-31 06:08:33.155475 nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/services.py
+-rw-r--r--   0        0        0    39455 2024-05-11 08:59:15.461050 nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/static/images/rikka1.png
+-rw-r--r--   0        0        0      264 2024-05-11 07:23:59.255421 nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/template_env.py
+-rw-r--r--   0        0        0      520 2024-05-30 09:13:07.638186 nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/templates/shell_panel.html
+-rw-r--r--   0        0        0     2040 2024-05-31 05:56:20.152484 nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/templates/xterm.html
+-rw-r--r--   0        0        0        0 2024-05-30 05:31:27.596571 nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/utils/__init__.py
+-rw-r--r--   0        0        0     2271 2024-05-31 06:26:22.526574 nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/utils/shell.py
+-rw-r--r--   0        0        0      651 2024-05-31 07:27:36.294846 nonebot_plugin_qqshell-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1346 2024-05-31 07:06:11.790769 nonebot_plugin_qqshell-0.1.0a2/README.md
+-rw-r--r--   0        0        0     2148 1970-01-01 00:00:00.000000 nonebot_plugin_qqshell-0.1.0a2/PKG-INFO
```

### Comparing `nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/__init__.py` & `nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-from nonebot import require
-require("nonebot_plugin_htmlrender")
-
-from nonebot.plugin import PluginMetadata
-
-from .config import Config
-from .handler import shell_handler
-
-__plugin_meta__ = PluginMetadata(
-    name="QQShell 是一个类 WebSSH、XShell 的运行在机器人的 SSH Shell，在 QQ 中自由运行你的命令吧",
-    description=(
-        "QQShell 能执行任何你所能想到的服务器命令\n"
-        "   >shell cd /\n"
-        "   >shell pwd\n"
-        "   >shell su\n"
-    ),
-    usage=">shell <你的指令>",
-    config=Config,
-    homepage="https://github.com/yejue/nonebot-plugin-qqshell.git",
-    type="application",
-    supported_adapters={"~onebot.v11"}
-)
+from nonebot import require
+require("nonebot_plugin_htmlrender")
+
+from nonebot.plugin import PluginMetadata
+
+from .config import Config
+from .handler import shell_handler
+
+__plugin_meta__ = PluginMetadata(
+    name="QQShell",
+    description="QQShell 是一个类 WebSSH、XShell 的运行在机器人的 SSH Shell，在 QQ 中自由运行你的命令吧",
+    usage=">shell <你的指令>",
+    config=Config,
+    homepage="https://github.com/yejue/nonebot-plugin-qqshell.git",
+    type="application",
+    supported_adapters={"~onebot.v11"}
+)
```

### Comparing `nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/config.py` & `nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/handler.py` & `nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/handler.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/services.py` & `nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/services.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/static/images/rikka1.png` & `nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/static/images/rikka1.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/templates/shell_panel.html` & `nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/templates/shell_panel.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/templates/xterm.html` & `nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/templates/xterm.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_qqshell-0.1.0a1/nonebot_plugin_qqshell/utils/shell.py` & `nonebot_plugin_qqshell-0.1.0a2/nonebot_plugin_qqshell/utils/shell.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_qqshell-0.1.0a1/pyproject.toml` & `nonebot_plugin_qqshell-0.1.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-qqshell"
-version = "0.1.0a1"
+version = "0.1.0a2"
 description = "QQShell 是一个类 WebSSH、XShell 的运行在机器人的 SSH Shell，在 QQ 中自由运行你的命令吧"
 authors = ["yejue <1145331931@qq.com>"]
 readme = "README.md"
 license = "GPLv3"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nonebot_plugin_qqshell-0.1.0a1/README.md` & `nonebot_plugin_qqshell-0.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_qqshell-0.1.0a1/PKG-INFO` & `nonebot_plugin_qqshell-0.1.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-qqshell
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: QQShell 是一个类 WebSSH、XShell 的运行在机器人的 SSH Shell，在 QQ 中自由运行你的命令吧
 License: GPLv3
 Author: yejue
 Author-email: 1145331931@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

