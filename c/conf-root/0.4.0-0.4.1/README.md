# Comparing `tmp/conf_root-0.4.0.tar.gz` & `tmp/conf_root-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf_root-0.4.0.tar", last modified: Tue May 28 16:42:15 2024, max compression
+gzip compressed data, was "conf_root-0.4.1.tar", last modified: Fri May 31 03:40:41 2024, max compression
```

## Comparing `conf_root-0.4.0.tar` & `conf_root-0.4.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:42:15.422658 conf_root-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-28 16:42:10.000000 conf_root-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-05-28 16:42:15.422658 conf_root-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-28 16:42:10.000000 conf_root-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:42:15.418658 conf_root-0.4.0/conf_root/
--rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-05-28 16:42:10.000000 conf_root-0.4.0/conf_root/ConfRoot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-28 16:42:10.000000 conf_root-0.4.0/conf_root/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-28 16:42:10.000000 conf_root-0.4.0/conf_root/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:42:15.422658 conf_root-0.4.0/conf_root/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-28 16:42:10.000000 conf_root-0.4.0/conf_root/agents/BasicAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-28 16:42:10.000000 conf_root-0.4.0/conf_root/agents/JsonAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-28 16:42:10.000000 conf_root-0.4.0/conf_root/agents/YamlAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-28 16:42:10.000000 conf_root-0.4.0/conf_root/agents/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:42:15.422658 conf_root-0.4.0/conf_root.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-05-28 16:42:15.000000 conf_root-0.4.0/conf_root.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-28 16:42:15.000000 conf_root-0.4.0/conf_root.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 16:42:15.000000 conf_root-0.4.0/conf_root.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 16:42:15.000000 conf_root-0.4.0/conf_root.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 16:42:15.000000 conf_root-0.4.0/conf_root.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-28 16:42:10.000000 conf_root-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 16:42:15.422658 conf_root-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-28 16:42:10.000000 conf_root-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 16:42:15.422658 conf_root-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-28 16:42:10.000000 conf_root-0.4.0/tests/test_ConfigurationField.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-28 16:42:10.000000 conf_root-0.4.0/tests/test_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-28 16:42:10.000000 conf_root-0.4.0/tests/test_multi_file_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-28 16:42:10.000000 conf_root-0.4.0/tests/test_nested_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-28 16:42:10.000000 conf_root-0.4.0/tests/test_single_file_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-28 16:42:10.000000 conf_root-0.4.0/tests/test_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:40:41.268086 conf_root-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-31 03:40:36.000000 conf_root-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-31 03:40:41.268086 conf_root-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-31 03:40:36.000000 conf_root-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:40:41.264086 conf_root-0.4.1/conf_root/
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-31 03:40:36.000000 conf_root-0.4.1/conf_root/ConfRoot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-31 03:40:36.000000 conf_root-0.4.1/conf_root/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-31 03:40:36.000000 conf_root-0.4.1/conf_root/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:40:41.268086 conf_root-0.4.1/conf_root/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-31 03:40:36.000000 conf_root-0.4.1/conf_root/agents/BasicAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-31 03:40:36.000000 conf_root-0.4.1/conf_root/agents/JsonAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-31 03:40:36.000000 conf_root-0.4.1/conf_root/agents/YamlAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-31 03:40:36.000000 conf_root-0.4.1/conf_root/agents/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:40:41.268086 conf_root-0.4.1/conf_root.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-31 03:40:41.000000 conf_root-0.4.1/conf_root.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-31 03:40:41.000000 conf_root-0.4.1/conf_root.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 03:40:41.000000 conf_root-0.4.1/conf_root.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-31 03:40:41.000000 conf_root-0.4.1/conf_root.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 03:40:41.000000 conf_root-0.4.1/conf_root.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-31 03:40:36.000000 conf_root-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 03:40:41.268086 conf_root-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-31 03:40:36.000000 conf_root-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:40:41.268086 conf_root-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-31 03:40:36.000000 conf_root-0.4.1/tests/test_ConfigurationField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-31 03:40:36.000000 conf_root-0.4.1/tests/test_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-31 03:40:36.000000 conf_root-0.4.1/tests/test_multi_file_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-31 03:40:36.000000 conf_root-0.4.1/tests/test_nested_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-31 03:40:36.000000 conf_root-0.4.1/tests/test_single_file_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-31 03:40:36.000000 conf_root-0.4.1/tests/test_wrap.py
```

### Comparing `conf_root-0.4.0/LICENSE` & `conf_root-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `conf_root-0.4.0/PKG-INFO` & `conf_root-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: conf_root
-Version: 0.4.0
-Summary: Default template for PDM package
+Version: 0.4.1
+Summary: 基于dataclass的科研配置文件取用工具
 Home-page: https://github.com/ciaranchen/conf_root
 Author: ciaranchen
 Author-email: ciaranchen <ciaranchen@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ruamel-yaml>=0.18.6
 
 # Conf Root
 
 ![PyPI - Version](https://img.shields.io/pypi/v/conf_root)
 
-基于dataclass的符合逻辑的配置文件取用方式。主要想法是在大量进行实验时，参数经常变动而且难以记录。最好有一种方式能在人类能读懂的配置文件中写出所有的参数，这样每次运行的记录都相对完整且易于整理。库的主要功能如下：
+基于dataclass的科研配置文件取用工具。主要想法是在大量进行实验时，参数经常变动而且难以记录。最好有一种方式能在人类能读懂的配置文件中写出所有的参数，这样每次运行的记录都相对完整且易于整理。库的主要功能如下：
 
 1. 为您定义的类生成一个配置文件；并优先使用配置文件中的值作为类中变量的值。
 2. 将某些科研项目中的argparse转换为dataclass，进而生成配置文件；从而可以在配置文件中修改输入。
 
 > Note: 仅用于配置文件，因此不提倡在配置文件类中使用动态的变量。
 
 ## 装饰类的定义生成配置文件
@@ -76,15 +76,16 @@
 - comment: 注释。仅在Yaml的输出格式中有效。为导出文件中当前字段的行添加行内注释。
 - serialize: 自定义序列化函数。接受序列化字段的值，返回序列化的文本。
 - deserialize: 自定义反序列化函数。接受序列化后的文本，返回该字段应有的值。
 - validators: 函数的列表。在反序列化时，对获得的值依次校验；如不符合要求抛出 ValidateException.
 
 ## 解析 Argparse
 
-在科研项目中会出现一大堆parser.argument，仅需添加两行代码就可以将其命令行参数配置转换为配置文件，并在配置文件中剪辑参数。不必重复输入一长串的命令行参数，也不再需要专门的`run.sh`或者`run.bat`。
+在科研项目中会出现一大堆parser.argument，仅需添加两行代码就可以将其命令行参数配置转换为配置文件，并在配置文件中剪辑参数。不必重复输入一长串的命令行参数，也不再需要专门的`run.sh`
+或者`run.bat`。
 
 ```python
 import argparse
 from conf_root import ConfRoot
 
 # 科研项目经常出现一大堆parser.argument
 parser = argparse.ArgumentParser()
@@ -107,19 +108,15 @@
 #### `ConfRoot.from_argparse(parser: argparse.ArgumentParser, cls_name: str = 'argparse')`
 
 解析Argparse并转换为dataclass，并且用ConfRoot.wrap封装它
 
 - paser。需解析的argparse.ArgumentParser。
 - cls_name。这个参数既是产生的dataclass类的类名，也是使用ConfRoot.wrap封装时的name参数。默认值为argparse。
 
-from_argparse 目前仅支持常见的Argparse动作。这不意味着有不支持的命令行参数会导致报错，这些参数将会被忽略跳过。具体限制如下：
-
-1. Argparse 的 action 必须为 'store(即默认值)', 'store_const', 'store_true', 'store_false' 之一。
-2. Argparse 的 nargs 不支持。
-3. Argparse 中 choices 和 required 的限制将会被忽略。
+from_argparse 目前仅支持常见的官方Argparse动作，但是对于自定义的Action来说可能支持有限。这不意味着有不支持的命令行参数会导致报错，这些参数将会被忽略跳过。
 
 ## More Example
 
 支持嵌套。
 嵌套时可以只指定agent=None来避免产生存储的文件。
 
 ```python
```

### Comparing `conf_root-0.4.0/README.md` & `conf_root-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Conf Root
 
 ![PyPI - Version](https://img.shields.io/pypi/v/conf_root)
 
-基于dataclass的符合逻辑的配置文件取用方式。主要想法是在大量进行实验时，参数经常变动而且难以记录。最好有一种方式能在人类能读懂的配置文件中写出所有的参数，这样每次运行的记录都相对完整且易于整理。库的主要功能如下：
+基于dataclass的科研配置文件取用工具。主要想法是在大量进行实验时，参数经常变动而且难以记录。最好有一种方式能在人类能读懂的配置文件中写出所有的参数，这样每次运行的记录都相对完整且易于整理。库的主要功能如下：
 
 1. 为您定义的类生成一个配置文件；并优先使用配置文件中的值作为类中变量的值。
 2. 将某些科研项目中的argparse转换为dataclass，进而生成配置文件；从而可以在配置文件中修改输入。
 
 > Note: 仅用于配置文件，因此不提倡在配置文件类中使用动态的变量。
 
 ## 装饰类的定义生成配置文件
@@ -63,15 +63,16 @@
 - comment: 注释。仅在Yaml的输出格式中有效。为导出文件中当前字段的行添加行内注释。
 - serialize: 自定义序列化函数。接受序列化字段的值，返回序列化的文本。
 - deserialize: 自定义反序列化函数。接受序列化后的文本，返回该字段应有的值。
 - validators: 函数的列表。在反序列化时，对获得的值依次校验；如不符合要求抛出 ValidateException.
 
 ## 解析 Argparse
 
-在科研项目中会出现一大堆parser.argument，仅需添加两行代码就可以将其命令行参数配置转换为配置文件，并在配置文件中剪辑参数。不必重复输入一长串的命令行参数，也不再需要专门的`run.sh`或者`run.bat`。
+在科研项目中会出现一大堆parser.argument，仅需添加两行代码就可以将其命令行参数配置转换为配置文件，并在配置文件中剪辑参数。不必重复输入一长串的命令行参数，也不再需要专门的`run.sh`
+或者`run.bat`。
 
 ```python
 import argparse
 from conf_root import ConfRoot
 
 # 科研项目经常出现一大堆parser.argument
 parser = argparse.ArgumentParser()
@@ -94,19 +95,15 @@
 #### `ConfRoot.from_argparse(parser: argparse.ArgumentParser, cls_name: str = 'argparse')`
 
 解析Argparse并转换为dataclass，并且用ConfRoot.wrap封装它
 
 - paser。需解析的argparse.ArgumentParser。
 - cls_name。这个参数既是产生的dataclass类的类名，也是使用ConfRoot.wrap封装时的name参数。默认值为argparse。
 
-from_argparse 目前仅支持常见的Argparse动作。这不意味着有不支持的命令行参数会导致报错，这些参数将会被忽略跳过。具体限制如下：
-
-1. Argparse 的 action 必须为 'store(即默认值)', 'store_const', 'store_true', 'store_false' 之一。
-2. Argparse 的 nargs 不支持。
-3. Argparse 中 choices 和 required 的限制将会被忽略。
+from_argparse 目前仅支持常见的官方Argparse动作，但是对于自定义的Action来说可能支持有限。这不意味着有不支持的命令行参数会导致报错，这些参数将会被忽略跳过。
 
 ## More Example
 
 支持嵌套。
 嵌套时可以只指定agent=None来避免产生存储的文件。
 
 ```python
```

### Comparing `conf_root-0.4.0/conf_root/ConfRoot.py` & `conf_root-0.4.1/conf_root/ConfRoot.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,13 +122,13 @@
                 # 暂不考虑不支持的action
                 continue
             # TODO: handle other Action.
 
             _type = get_type(action)
             field = (name, _type, default_field(action))
             fields.append(field)
-            print(field)
+            # print(field)
 
         fields = sorted(fields, key=lambda x: x[2].default == MISSING, reverse=True)
 
         cls = make_dataclass(cls_name.replace(f'.{self.agent.default_extension}', ''), fields)
         return self.config(cls)
```

### Comparing `conf_root-0.4.0/conf_root/Configuration.py` & `conf_root-0.4.1/conf_root/Configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,11 +26,11 @@
     @property
     def all_dataclass(self):
         def _recursive_dataclass(cls):
             res = []
             if is_dataclass(cls):
                 for field in dataclasses_fields(cls):
                     res.extend(_recursive_dataclass(field.type))
-                    res.append(cls)
+                res.append(cls)
             return res
 
         return _recursive_dataclass(self.cls)
```

### Comparing `conf_root-0.4.0/conf_root/agents/BasicAgent.py` & `conf_root-0.4.1/conf_root/agents/BasicAgent.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.4.0/conf_root/agents/JsonAgent.py` & `conf_root-0.4.1/conf_root/agents/JsonAgent.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.4.0/conf_root/agents/YamlAgent.py` & `conf_root-0.4.1/conf_root/agents/YamlAgent.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,23 +89,23 @@
         data = self._load(configuration)
         return configuration.name in data
 
     def _load(self, configuration):
         if not os.path.exists(self.location):
             return {}
         with open(self.location, 'r') as f:
-            return self.get_yaml(configuration).load(f)
+            data = self.get_yaml(configuration).load(f)
+        return data if data is not None else {}
 
     def load(self, configuration: Configuration, instance):
         BasicAgent.load(self, configuration, instance)
         res = self._load(configuration)
         data = res[configuration.name]
-        # 覆盖原instance中的变量:
-        for k, v in data.items():
-            setattr(instance, k, v)
+        # 覆盖原instance中的变量
+        data2obj(instance, data)
         return instance
 
     def save(self, configuration: Configuration, instance) -> None:
         BasicAgent.save(self, configuration, instance)
         total_data = self._load(configuration)
         total_data[configuration.name] = instance
```

### Comparing `conf_root-0.4.0/conf_root/agents/utils.py` & `conf_root-0.4.1/conf_root/agents/utils.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.4.0/conf_root.egg-info/PKG-INFO` & `conf_root-0.4.1/conf_root.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: conf_root
-Version: 0.4.0
-Summary: Default template for PDM package
+Version: 0.4.1
+Summary: 基于dataclass的科研配置文件取用工具
 Home-page: https://github.com/ciaranchen/conf_root
 Author: ciaranchen
 Author-email: ciaranchen <ciaranchen@qq.com>
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ruamel-yaml>=0.18.6
 
 # Conf Root
 
 ![PyPI - Version](https://img.shields.io/pypi/v/conf_root)
 
-基于dataclass的符合逻辑的配置文件取用方式。主要想法是在大量进行实验时，参数经常变动而且难以记录。最好有一种方式能在人类能读懂的配置文件中写出所有的参数，这样每次运行的记录都相对完整且易于整理。库的主要功能如下：
+基于dataclass的科研配置文件取用工具。主要想法是在大量进行实验时，参数经常变动而且难以记录。最好有一种方式能在人类能读懂的配置文件中写出所有的参数，这样每次运行的记录都相对完整且易于整理。库的主要功能如下：
 
 1. 为您定义的类生成一个配置文件；并优先使用配置文件中的值作为类中变量的值。
 2. 将某些科研项目中的argparse转换为dataclass，进而生成配置文件；从而可以在配置文件中修改输入。
 
 > Note: 仅用于配置文件，因此不提倡在配置文件类中使用动态的变量。
 
 ## 装饰类的定义生成配置文件
@@ -76,15 +76,16 @@
 - comment: 注释。仅在Yaml的输出格式中有效。为导出文件中当前字段的行添加行内注释。
 - serialize: 自定义序列化函数。接受序列化字段的值，返回序列化的文本。
 - deserialize: 自定义反序列化函数。接受序列化后的文本，返回该字段应有的值。
 - validators: 函数的列表。在反序列化时，对获得的值依次校验；如不符合要求抛出 ValidateException.
 
 ## 解析 Argparse
 
-在科研项目中会出现一大堆parser.argument，仅需添加两行代码就可以将其命令行参数配置转换为配置文件，并在配置文件中剪辑参数。不必重复输入一长串的命令行参数，也不再需要专门的`run.sh`或者`run.bat`。
+在科研项目中会出现一大堆parser.argument，仅需添加两行代码就可以将其命令行参数配置转换为配置文件，并在配置文件中剪辑参数。不必重复输入一长串的命令行参数，也不再需要专门的`run.sh`
+或者`run.bat`。
 
 ```python
 import argparse
 from conf_root import ConfRoot
 
 # 科研项目经常出现一大堆parser.argument
 parser = argparse.ArgumentParser()
@@ -107,19 +108,15 @@
 #### `ConfRoot.from_argparse(parser: argparse.ArgumentParser, cls_name: str = 'argparse')`
 
 解析Argparse并转换为dataclass，并且用ConfRoot.wrap封装它
 
 - paser。需解析的argparse.ArgumentParser。
 - cls_name。这个参数既是产生的dataclass类的类名，也是使用ConfRoot.wrap封装时的name参数。默认值为argparse。
 
-from_argparse 目前仅支持常见的Argparse动作。这不意味着有不支持的命令行参数会导致报错，这些参数将会被忽略跳过。具体限制如下：
-
-1. Argparse 的 action 必须为 'store(即默认值)', 'store_const', 'store_true', 'store_false' 之一。
-2. Argparse 的 nargs 不支持。
-3. Argparse 中 choices 和 required 的限制将会被忽略。
+from_argparse 目前仅支持常见的官方Argparse动作，但是对于自定义的Action来说可能支持有限。这不意味着有不支持的命令行参数会导致报错，这些参数将会被忽略跳过。
 
 ## More Example
 
 支持嵌套。
 嵌套时可以只指定agent=None来避免产生存储的文件。
 
 ```python
```

### Comparing `conf_root-0.4.0/conf_root.egg-info/SOURCES.txt` & `conf_root-0.4.1/conf_root.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conf_root-0.4.0/setup.py` & `conf_root-0.4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="conf_root",  # 包名
-    version="0.4.0",  # 版本号
+    version="0.4.1",  # 版本号
     install_requires=[
         "ruamel.yaml"
     ],
     author="ciaranchen",
     author_email="ciaranchen@qq.com",
-    description="基于dataclass的符合逻辑的配置取用方式。",
+    description="基于dataclass的配置文件取用工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ciaranchen/conf_root",
     packages=["conf_root", "conf_root.agents"],  # 包含的Python模块或子包
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `conf_root-0.4.0/tests/test_ConfigurationField.py` & `conf_root-0.4.1/tests/test_ConfigurationField.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.4.0/tests/test_argparse.py` & `conf_root-0.4.1/tests/test_argparse.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.4.0/tests/test_multi_file_agent.py` & `conf_root-0.4.1/tests/test_multi_file_agent.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.4.0/tests/test_nested_dataclass.py` & `conf_root-0.4.1/tests/test_nested_dataclass.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.4.0/tests/test_single_file_agent.py` & `conf_root-0.4.1/tests/test_single_file_agent.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.4.0/tests/test_wrap.py` & `conf_root-0.4.1/tests/test_wrap.py`

 * *Files identical despite different names*

