# Comparing `tmp/solar_registry-0.3.5.tar.gz` & `tmp/solar_registry-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solar_registry-0.3.5.tar", last modified: Wed May 29 12:28:11 2024, max compression
+gzip compressed data, was "solar_registry-0.3.6.tar", last modified: Thu May 30 11:43:44 2024, max compression
```

## Comparing `solar_registry-0.3.5.tar` & `solar_registry-0.3.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    11357 2024-05-29 12:27:41.074115 solar_registry-0.3.5/LICENSE
--rw-r--r--   0        0        0      682 2024-05-29 12:27:41.074115 solar_registry-0.3.5/README.md
--rw-r--r--   0        0        0     1240 2024-05-29 12:28:11.658172 solar_registry-0.3.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-29 12:27:41.074115 solar_registry-0.3.5/src/solar_registry/__init__.py
--rw-r--r--   0        0        0     2282 2024-05-29 12:27:41.074115 solar_registry-0.3.5/src/solar_registry/cli.py
--rw-r--r--   0        0        0        0 2024-05-29 12:27:41.074115 solar_registry-0.3.5/src/solar_registry/commands/__init__.py
--rw-r--r--   0        0        0     5891 2024-05-29 12:27:41.074115 solar_registry-0.3.5/src/solar_registry/commands/meta_merger.py
--rw-r--r--   0        0        0        0 2024-05-29 12:27:41.074115 solar_registry-0.3.5/src/solar_registry/model/__init__.py
--rw-r--r--   0        0        0      298 2024-05-29 12:27:41.074115 solar_registry-0.3.5/src/solar_registry/model/asset.py
--rw-r--r--   0        0        0     1016 2024-05-29 12:27:41.074115 solar_registry-0.3.5/src/solar_registry/model/legacy.py
--rw-r--r--   0        0        0     4713 2024-05-29 12:27:41.074115 solar_registry-0.3.5/src/solar_registry/model/test_tool.py
--rw-r--r--   0        0        0        0 2024-05-29 12:27:41.074115 solar_registry-0.3.5/src/solar_registry/py.typed
--rw-r--r--   0        0        0        0 2024-05-29 12:27:41.074115 solar_registry-0.3.5/src/solar_registry/service/__init__.py
--rw-r--r--   0        0        0     5496 2024-05-29 12:27:41.074115 solar_registry-0.3.5/src/solar_registry/service/cos_sync.py
--rw-r--r--   0        0        0     3003 2024-05-29 12:27:41.074115 solar_registry-0.3.5/src/solar_registry/service/generator.py
--rw-r--r--   0        0        0     2699 2024-05-29 12:27:41.074115 solar_registry-0.3.5/src/solar_registry/service/pr_generator.py
--rw-r--r--   0        0        0      956 2024-05-29 12:27:41.074115 solar_registry-0.3.5/src/solar_registry/service/testtool.py
--rw-r--r--   0        0        0     2069 2024-05-29 12:27:41.074115 solar_registry-0.3.5/src/solar_registry/service/validator.py
--rw-r--r--   0        0        0        0 2024-05-29 12:27:41.074115 solar_registry-0.3.5/src/solar_registry/util/__init__.py
--rw-r--r--   0        0        0      600 2024-05-29 12:27:41.074115 solar_registry-0.3.5/src/solar_registry/util/file.py
--rw-r--r--   0        0        0        0 2024-05-29 12:27:41.074115 solar_registry-0.3.5/tests/__init__.py
--rw-r--r--   0        0        0      383 2024-05-29 12:27:41.074115 solar_registry-0.3.5/tests/test_cos_sync.py
--rw-r--r--   0        0        0     1512 2024-05-29 12:27:41.074115 solar_registry-0.3.5/tests/test_merger.py
--rw-r--r--   0        0        0      503 2024-05-29 12:27:41.074115 solar_registry-0.3.5/tests/test_pr_generator.py
--rw-r--r--   0        0        0     3880 2024-05-29 12:27:41.074115 solar_registry-0.3.5/tests/test_testtool.py
--rw-r--r--   0        0        0      299 2024-05-29 12:27:41.078115 solar_registry-0.3.5/tests/test_validator.py
--rw-r--r--   0        0        0      730 2024-05-29 12:27:41.078115 solar_registry-0.3.5/tests/testdata/error_meta_files/error_yaml_with_loose.yaml
--rw-r--r--   0        0        0     1249 2024-05-29 12:27:41.078115 solar_registry-0.3.5/tests/testdata/error_meta_files/error_yaml_with_strict.yaml
--rw-r--r--   0        0        0      774 2024-05-29 12:27:41.078115 solar_registry-0.3.5/tests/testdata/error_meta_files/error_yaml_with_strict_no_arch.yaml
--rw-r--r--   0        0        0      763 2024-05-29 12:27:41.078115 solar_registry-0.3.5/tests/testdata/error_meta_files/error_yaml_with_strict_no_os.yaml
--rw-r--r--   0        0        0     1418 2024-05-29 12:27:41.078115 solar_registry-0.3.5/tests/testdata/legacy/testtool.yaml
--rw-r--r--   0        0        0     3074 2024-05-29 12:27:41.078115 solar_registry-0.3.5/tests/testdata/pytest/testtool.yaml
--rw-r--r--   0        0        0     3607 2024-05-29 12:27:41.078115 solar_registry-0.3.5/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
--rw-r--r--   0        0        0     3090 2024-05-29 12:27:41.078115 solar_registry-0.3.5/tests/testdata/stable_index_file_check/testtools/stable.index.json
--rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 solar_registry-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-30 11:43:21.242876 solar_registry-0.3.6/LICENSE
+-rw-r--r--   0        0        0      682 2024-05-30 11:43:21.242876 solar_registry-0.3.6/README.md
+-rw-r--r--   0        0        0     1240 2024-05-30 11:43:44.418988 solar_registry-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 11:43:21.242876 solar_registry-0.3.6/src/solar_registry/__init__.py
+-rw-r--r--   0        0        0     2282 2024-05-30 11:43:21.242876 solar_registry-0.3.6/src/solar_registry/cli.py
+-rw-r--r--   0        0        0        0 2024-05-30 11:43:21.242876 solar_registry-0.3.6/src/solar_registry/commands/__init__.py
+-rw-r--r--   0        0        0     5891 2024-05-30 11:43:21.242876 solar_registry-0.3.6/src/solar_registry/commands/meta_merger.py
+-rw-r--r--   0        0        0        0 2024-05-30 11:43:21.242876 solar_registry-0.3.6/src/solar_registry/model/__init__.py
+-rw-r--r--   0        0        0      298 2024-05-30 11:43:21.242876 solar_registry-0.3.6/src/solar_registry/model/asset.py
+-rw-r--r--   0        0        0     1016 2024-05-30 11:43:21.242876 solar_registry-0.3.6/src/solar_registry/model/legacy.py
+-rw-r--r--   0        0        0     4836 2024-05-30 11:43:21.242876 solar_registry-0.3.6/src/solar_registry/model/test_tool.py
+-rw-r--r--   0        0        0        0 2024-05-30 11:43:21.242876 solar_registry-0.3.6/src/solar_registry/py.typed
+-rw-r--r--   0        0        0        0 2024-05-30 11:43:21.242876 solar_registry-0.3.6/src/solar_registry/service/__init__.py
+-rw-r--r--   0        0        0     5496 2024-05-30 11:43:21.246877 solar_registry-0.3.6/src/solar_registry/service/cos_sync.py
+-rw-r--r--   0        0        0     3003 2024-05-30 11:43:21.246877 solar_registry-0.3.6/src/solar_registry/service/generator.py
+-rw-r--r--   0        0        0     2699 2024-05-30 11:43:21.246877 solar_registry-0.3.6/src/solar_registry/service/pr_generator.py
+-rw-r--r--   0        0        0      956 2024-05-30 11:43:21.246877 solar_registry-0.3.6/src/solar_registry/service/testtool.py
+-rw-r--r--   0        0        0     2069 2024-05-30 11:43:21.246877 solar_registry-0.3.6/src/solar_registry/service/validator.py
+-rw-r--r--   0        0        0        0 2024-05-30 11:43:21.246877 solar_registry-0.3.6/src/solar_registry/util/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-30 11:43:21.246877 solar_registry-0.3.6/src/solar_registry/util/file.py
+-rw-r--r--   0        0        0        0 2024-05-30 11:43:21.246877 solar_registry-0.3.6/tests/__init__.py
+-rw-r--r--   0        0        0      383 2024-05-30 11:43:21.246877 solar_registry-0.3.6/tests/test_cos_sync.py
+-rw-r--r--   0        0        0     1512 2024-05-30 11:43:21.246877 solar_registry-0.3.6/tests/test_merger.py
+-rw-r--r--   0        0        0      503 2024-05-30 11:43:21.246877 solar_registry-0.3.6/tests/test_pr_generator.py
+-rw-r--r--   0        0        0     3880 2024-05-30 11:43:21.246877 solar_registry-0.3.6/tests/test_testtool.py
+-rw-r--r--   0        0        0      299 2024-05-30 11:43:21.246877 solar_registry-0.3.6/tests/test_validator.py
+-rw-r--r--   0        0        0      730 2024-05-30 11:43:21.246877 solar_registry-0.3.6/tests/testdata/error_meta_files/error_yaml_with_loose.yaml
+-rw-r--r--   0        0        0     1249 2024-05-30 11:43:21.246877 solar_registry-0.3.6/tests/testdata/error_meta_files/error_yaml_with_strict.yaml
+-rw-r--r--   0        0        0      774 2024-05-30 11:43:21.246877 solar_registry-0.3.6/tests/testdata/error_meta_files/error_yaml_with_strict_no_arch.yaml
+-rw-r--r--   0        0        0      763 2024-05-30 11:43:21.246877 solar_registry-0.3.6/tests/testdata/error_meta_files/error_yaml_with_strict_no_os.yaml
+-rw-r--r--   0        0        0     1418 2024-05-30 11:43:21.246877 solar_registry-0.3.6/tests/testdata/legacy/testtool.yaml
+-rw-r--r--   0        0        0     3200 2024-05-30 11:43:21.246877 solar_registry-0.3.6/tests/testdata/pytest/testtool.yaml
+-rw-r--r--   0        0        0     3607 2024-05-30 11:43:21.246877 solar_registry-0.3.6/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
+-rw-r--r--   0        0        0     3090 2024-05-30 11:43:21.246877 solar_registry-0.3.6/tests/testdata/stable_index_file_check/testtools/stable.index.json
+-rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 solar_registry-0.3.6/PKG-INFO
```

### Comparing `solar_registry-0.3.5/LICENSE` & `solar_registry-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/README.md` & `solar_registry-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/pyproject.toml` & `solar_registry-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "solar-registry"
-version = "0.3.5"
+version = "0.3.6"
 description = "Generate and merge meta data for testsolar test tools"
 authors = [
     { name = "asiazhang", email = "asiazhang2002@gmail.com" },
 ]
 dependencies = [
     "requests>=2.31.0",
     "pydantic>=2.7.1",
```

### Comparing `solar_registry-0.3.5/src/solar_registry/cli.py` & `solar_registry-0.3.6/src/solar_registry/cli.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/src/solar_registry/commands/meta_merger.py` & `solar_registry-0.3.6/src/solar_registry/commands/meta_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/src/solar_registry/model/legacy.py` & `solar_registry-0.3.6/src/solar_registry/model/legacy.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/src/solar_registry/model/test_tool.py` & `solar_registry-0.3.6/src/solar_registry/model/test_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,28 +23,31 @@
     Number = "number"
     Choices = "choices"
 
 
 class ParamDef(BaseModel):
     name: str
     value: str
+    desc: str = ""
 
     default: str
     choices: list[ParamChoice] | None = None
 
     # 兼容历史工具
     lang: str | None = None
     input_widget: ParamWidget | None = Field(None, alias="inputWidget")
-    desc: str = ""
 
     @model_validator(mode="after")
     def check_valid(self, info: ValidationInfo) -> Self:
         context = info.context
-        if context and context.get("strict") and not self.desc:
-            raise ValueError("ParamDef desc must be set")
+        if context and context.get("strict"):
+            if not self.desc:
+                raise ValueError("ParamDef desc must be set")
+            if not self.input_widget:
+                raise ValueError("ParamDef inputWidget must be set")
 
         return self
 
 
 class Entry(BaseModel):
     load: str
     run: str
```

### Comparing `solar_registry-0.3.5/src/solar_registry/service/cos_sync.py` & `solar_registry-0.3.6/src/solar_registry/service/cos_sync.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/src/solar_registry/service/generator.py` & `solar_registry-0.3.6/src/solar_registry/service/generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/src/solar_registry/service/pr_generator.py` & `solar_registry-0.3.6/src/solar_registry/service/pr_generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/src/solar_registry/service/testtool.py` & `solar_registry-0.3.6/src/solar_registry/service/testtool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/src/solar_registry/service/validator.py` & `solar_registry-0.3.6/src/solar_registry/service/validator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/src/solar_registry/util/file.py` & `solar_registry-0.3.6/src/solar_registry/util/file.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/tests/test_merger.py` & `solar_registry-0.3.6/tests/test_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/tests/test_testtool.py` & `solar_registry-0.3.6/tests/test_testtool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/tests/testdata/error_meta_files/error_yaml_with_loose.yaml` & `solar_registry-0.3.6/tests/testdata/error_meta_files/error_yaml_with_loose.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/tests/testdata/error_meta_files/error_yaml_with_strict.yaml` & `solar_registry-0.3.6/tests/testdata/error_meta_files/error_yaml_with_strict.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/tests/testdata/error_meta_files/error_yaml_with_strict_no_arch.yaml` & `solar_registry-0.3.6/tests/testdata/error_meta_files/error_yaml_with_strict_no_arch.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/tests/testdata/error_meta_files/error_yaml_with_strict_no_os.yaml` & `solar_registry-0.3.6/tests/testdata/error_meta_files/error_yaml_with_strict_no_os.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/tests/testdata/legacy/testtool.yaml` & `solar_registry-0.3.6/tests/testdata/legacy/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/tests/testdata/pytest/testtool.yaml` & `solar_registry-0.3.6/tests/testdata/pytest/testtool.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
           优点：
             - 解析准确
             - 支持数据驱动用例解析
           
           缺点：
             - 用户测试用例有运行时依赖，在加载阶段可能无法成功
             - 依赖测试运行的pip包，解析速度较慢
+    inputWidget: choices
   - name: runMode
     value: 运行用例的模式
     desc: 加载用例的模式
     default: singleprocess # choice: singleprocess/multiprocess
     choices:
       - value: singleprocess
         desc: |
@@ -61,22 +62,27 @@
           
           优点：
             - 整体执行效率高
           
           缺点：
             - 不保证用例执行顺序
             - 单机并发量设置太高可能导致执行机异常
+    inputWidget: choices
   - name: qtafSettings
     value: QTAF测试项目配置
     desc: QTAF测试项目配置
     default: ""
+    lang: python
+    inputWidget: code
   - name: extraFieldsConfig
     value: 用例额外属性
     desc: 用例额外属性
+    lang: json
     default: ""
+    inputWidget: code
 entry:
   load: "python3 /testtools/qta/src/load.py $1"
   run: "python3 /testtools/qta/src/run.py $1"
 supportOS:
   - windows
   - linux
   - darwin
```

### Comparing `solar_registry-0.3.5/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json` & `solar_registry-0.3.6/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/tests/testdata/stable_index_file_check/testtools/stable.index.json` & `solar_registry-0.3.6/tests/testdata/stable_index_file_check/testtools/stable.index.json`

 * *Files identical despite different names*

### Comparing `solar_registry-0.3.5/PKG-INFO` & `solar_registry-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solar-registry
-Version: 0.3.5
+Version: 0.3.6
 Summary: Generate and merge meta data for testsolar test tools
 Author-Email: asiazhang <asiazhang2002@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

