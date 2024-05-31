# Comparing `tmp/cdklabs.cdk-cicd-wrapper-0.1.0.tar.gz` & `tmp/cdklabs.cdk-cicd-wrapper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.cdk-cicd-wrapper-0.1.0.tar", last modified: Thu May 30 13:18:29 2024, max compression
+gzip compressed data, was "cdklabs.cdk-cicd-wrapper-0.1.1.tar", last modified: Fri May 31 15:37:36 2024, max compression
```

## Comparing `cdklabs.cdk-cicd-wrapper-0.1.0.tar` & `cdklabs.cdk-cicd-wrapper-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:18:29.422103 cdklabs.cdk-cicd-wrapper-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-30 13:18:23.000000 cdklabs.cdk-cicd-wrapper-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-30 13:18:23.000000 cdklabs.cdk-cicd-wrapper-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-30 13:18:29.422103 cdklabs.cdk-cicd-wrapper-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-30 13:18:23.000000 cdklabs.cdk-cicd-wrapper-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-30 13:18:23.000000 cdklabs.cdk-cicd-wrapper-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:18:29.422103 cdklabs.cdk-cicd-wrapper-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-30 13:18:23.000000 cdklabs.cdk-cicd-wrapper-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:18:29.418103 cdklabs.cdk-cicd-wrapper-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:18:29.418103 cdklabs.cdk-cicd-wrapper-0.1.0/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:18:29.418103 cdklabs.cdk-cicd-wrapper-0.1.0/src/cdklabs/cdk_cicd_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)   426555 2024-05-30 13:18:23.000000 cdklabs.cdk-cicd-wrapper-0.1.0/src/cdklabs/cdk_cicd_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:18:29.422103 cdklabs.cdk-cicd-wrapper-0.1.0/src/cdklabs/cdk_cicd_wrapper/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-30 13:18:23.000000 cdklabs.cdk-cicd-wrapper-0.1.0/src/cdklabs/cdk_cicd_wrapper/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   453762 2024-05-30 13:18:23.000000 cdklabs.cdk-cicd-wrapper-0.1.0/src/cdklabs/cdk_cicd_wrapper/_jsii/cdk-cicd-wrapper@0.1.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:18:23.000000 cdklabs.cdk-cicd-wrapper-0.1.0/src/cdklabs/cdk_cicd_wrapper/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:18:29.418103 cdklabs.cdk-cicd-wrapper-0.1.0/src/cdklabs.cdk_cicd_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-30 13:18:29.000000 cdklabs.cdk-cicd-wrapper-0.1.0/src/cdklabs.cdk_cicd_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-30 13:18:29.000000 cdklabs.cdk-cicd-wrapper-0.1.0/src/cdklabs.cdk_cicd_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:18:29.000000 cdklabs.cdk-cicd-wrapper-0.1.0/src/cdklabs.cdk_cicd_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-30 13:18:29.000000 cdklabs.cdk-cicd-wrapper-0.1.0/src/cdklabs.cdk_cicd_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-30 13:18:29.000000 cdklabs.cdk-cicd-wrapper-0.1.0/src/cdklabs.cdk_cicd_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:37:36.155284 cdklabs.cdk-cicd-wrapper-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-31 15:37:29.000000 cdklabs.cdk-cicd-wrapper-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-31 15:37:29.000000 cdklabs.cdk-cicd-wrapper-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-31 15:37:36.155284 cdklabs.cdk-cicd-wrapper-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-31 15:37:29.000000 cdklabs.cdk-cicd-wrapper-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-31 15:37:29.000000 cdklabs.cdk-cicd-wrapper-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:37:36.155284 cdklabs.cdk-cicd-wrapper-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-31 15:37:29.000000 cdklabs.cdk-cicd-wrapper-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:37:36.151284 cdklabs.cdk-cicd-wrapper-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:37:36.151284 cdklabs.cdk-cicd-wrapper-0.1.1/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:37:36.155284 cdklabs.cdk-cicd-wrapper-0.1.1/src/cdklabs/cdk_cicd_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)   429592 2024-05-31 15:37:29.000000 cdklabs.cdk-cicd-wrapper-0.1.1/src/cdklabs/cdk_cicd_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:37:36.155284 cdklabs.cdk-cicd-wrapper-0.1.1/src/cdklabs/cdk_cicd_wrapper/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-31 15:37:29.000000 cdklabs.cdk-cicd-wrapper-0.1.1/src/cdklabs/cdk_cicd_wrapper/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   455534 2024-05-31 15:37:29.000000 cdklabs.cdk-cicd-wrapper-0.1.1/src/cdklabs/cdk_cicd_wrapper/_jsii/cdk-cicd-wrapper@0.1.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:37:29.000000 cdklabs.cdk-cicd-wrapper-0.1.1/src/cdklabs/cdk_cicd_wrapper/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:37:36.155284 cdklabs.cdk-cicd-wrapper-0.1.1/src/cdklabs.cdk_cicd_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-31 15:37:36.000000 cdklabs.cdk-cicd-wrapper-0.1.1/src/cdklabs.cdk_cicd_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-31 15:37:36.000000 cdklabs.cdk-cicd-wrapper-0.1.1/src/cdklabs.cdk_cicd_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:37:36.000000 cdklabs.cdk-cicd-wrapper-0.1.1/src/cdklabs.cdk_cicd_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-31 15:37:36.000000 cdklabs.cdk-cicd-wrapper-0.1.1/src/cdklabs.cdk_cicd_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 15:37:36.000000 cdklabs.cdk-cicd-wrapper-0.1.1/src/cdklabs.cdk_cicd_wrapper.egg-info/top_level.txt
```

### Comparing `cdklabs.cdk-cicd-wrapper-0.1.0/LICENSE` & `cdklabs.cdk-cicd-wrapper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-cicd-wrapper-0.1.0/PKG-INFO` & `cdklabs.cdk-cicd-wrapper-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-cicd-wrapper
-Version: 0.1.0
+Version: 0.1.1
 Summary: This repository contains the infrastructure as code to wrap your AWS CDK project with CI/CD around it.
 Home-page: https://github.com/cdklabs/cdk-cicd-wrapper.git
 Author: CDK CI/CD Wrapper Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cicd-wrapper.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.cdk-cicd-wrapper-0.1.0/README.md` & `cdklabs.cdk-cicd-wrapper-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-cicd-wrapper-0.1.0/setup.py` & `cdklabs.cdk-cicd-wrapper-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.cdk-cicd-wrapper",
-    "version": "0.1.0",
+    "version": "0.1.1",
     "description": "This repository contains the infrastructure as code to wrap your AWS CDK project with CI/CD around it.",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-cicd-wrapper.git",
     "long_description_content_type": "text/markdown",
     "author": "CDK CI/CD Wrapper Team",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdklabs.cdk_cicd_wrapper",
         "cdklabs.cdk_cicd_wrapper._jsii"
     ],
     "package_data": {
         "cdklabs.cdk_cicd_wrapper._jsii": [
-            "cdk-cicd-wrapper@0.1.0.jsii.tgz"
+            "cdk-cicd-wrapper@0.1.1.jsii.tgz"
         ],
         "cdklabs.cdk_cicd_wrapper": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdklabs.cdk-cicd-wrapper-0.1.0/src/cdklabs/cdk_cicd_wrapper/__init__.py` & `cdklabs.cdk-cicd-wrapper-0.1.1/src/cdklabs/cdk_cicd_wrapper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3144,14 +3144,53 @@
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__58d1b1a41267fdc1330544a8fa0937f6e4a0846a56edb48b7b143e3522060932)
             check_type(argname="argument context", value=context, expected_type=type_hints["context"])
         return typing.cast(typing.Any, jsii.invoke(self, "provide", [context]))
 
 
+class ParameterResolver(
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@cdklabs/cdk-cicd-wrapper.ParameterResolver",
+):
+    '''This class provides functionality to resolve parameter values from AWS Systems Manager Parameter Store or from provided string values.'''
+
+    def __init__(self) -> None:
+        jsii.create(self.__class__, self, [])
+
+    @jsii.member(jsii_name="resolveValue")
+    @builtins.classmethod
+    def resolve_value(
+        cls,
+        scope: _constructs_77d1e7e8.Construct,
+        param: builtins.str,
+    ) -> builtins.str:
+        '''Resolves the value of a parameter, either from an SSM parameter or using the provided string value.
+
+        :param scope: The scope in which the parameter is resolved.
+        :param param: The parameter value to resolve. If it starts with 'ssm:', it will be treated as an SSM parameter name.
+
+        :return: The resolved parameter value.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__88247bee6ba65673ff953f8e7aa6ed1b590a24428384be6dc7c4f7be5a895cc0)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument param", value=param, expected_type=type_hints["param"])
+        return typing.cast(builtins.str, jsii.sinvoke(cls, "resolveValue", [scope, param]))
+
+    @jsii.python.classproperty
+    @jsii.member(jsii_name="PREFIX")
+    def PREFIX(cls) -> builtins.str:
+        '''The prefix used to identify parameter resolution from AWS Systems Manager Parameter Store.
+
+        :default: 'resolve'
+        '''
+        return typing.cast(builtins.str, jsii.sget(cls, "PREFIX"))
+
+
 @jsii.implements(IResourceProvider)
 class PhaseCommandProvider(
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdklabs/cdk-cicd-wrapper.PhaseCommandProvider",
 ):
     '''Provides the phase commands.'''
 
@@ -5879,22 +5918,33 @@
         return typing.cast(typing.List[_aws_cdk_pipelines_ceddda9d.Step], jsii.invoke(self, "preHooks", []))
 
     @jsii.member(jsii_name="provide")
     def provide(self, context: ResourceContext) -> None:
         '''Provides the deployment hook configuration for this stack provider.
 
         :param context: The resource context containing the scope, stage, environment, and blueprint properties.
-
-        :return: The deployment hook configuration with pre and post hooks.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__93749efec26f6060dadfeee523230f2893d7b4f15df00660a895c33f6aaa036f)
             check_type(argname="argument context", value=context, expected_type=type_hints["context"])
         return typing.cast(None, jsii.invoke(self, "provide", [context]))
 
+    @jsii.member(jsii_name="resolve")
+    def resolve(self, ssm_parameter_name: builtins.str) -> builtins.str:
+        '''Resolves the value of an SSM parameter.
+
+        :param ssm_parameter_name: The name of the SSM parameter to resolve.
+
+        :return: The resolved value of the SSM parameter.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__d697cdcbe532f07d04b89722be4ec6911b4b2516ffc502aba9f3652ee94e8634)
+            check_type(argname="argument ssm_parameter_name", value=ssm_parameter_name, expected_type=type_hints["ssm_parameter_name"])
+        return typing.cast(builtins.str, jsii.invoke(self, "resolve", [ssm_parameter_name]))
+
     @jsii.member(jsii_name="stacks")
     @abc.abstractmethod
     def stacks(self, context: ResourceContext) -> None:
         '''Abstract method that must be implemented by subclasses to define the stacks to be deployed.
 
         :param context: The resource context containing the scope, stage, environment, and blueprint properties.
         '''
@@ -5924,14 +5974,23 @@
         '''Getter for the resource context.
 
         :return: The resource context containing the scope, stage, environment, and blueprint properties.
         '''
         return typing.cast(ResourceContext, jsii.get(self, "context"))
 
     @builtins.property
+    @jsii.member(jsii_name="encryptionKey")
+    def _encryption_key(self) -> _aws_cdk_aws_kms_ceddda9d.Key:
+        '''Getter for the encryption key.
+
+        :return: The encryption key used in the deployment.
+        '''
+        return typing.cast(_aws_cdk_aws_kms_ceddda9d.Key, jsii.get(self, "encryptionKey"))
+
+    @builtins.property
     @jsii.member(jsii_name="env")
     def _env(self) -> _aws_cdk_ceddda9d.Environment:
         '''Getter for the deployment environment.
 
         :return: The deployment environment.
         '''
         return typing.cast(_aws_cdk_ceddda9d.Environment, jsii.get(self, "env"))
@@ -7494,14 +7553,15 @@
     "IVpcConfigNewVpc",
     "IVpcConstruct",
     "InlineShellPhaseCommand",
     "NPMPhaseCommand",
     "NPMRegistryConfig",
     "PRCheckConfig",
     "ParameterProvider",
+    "ParameterResolver",
     "PhaseCommandProvider",
     "PipelineBlueprint",
     "PipelineBlueprintBuilder",
     "PipelinePhases",
     "PipelineProps",
     "PostDeployBuildStep",
     "PostDeployExecutorStack",
@@ -7990,14 +8050,21 @@
 
 def _typecheckingstub__58d1b1a41267fdc1330544a8fa0937f6e4a0846a56edb48b7b143e3522060932(
     context: ResourceContext,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__88247bee6ba65673ff953f8e7aa6ed1b590a24428384be6dc7c4f7be5a895cc0(
+    scope: _constructs_77d1e7e8.Construct,
+    param: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__2d23320659531364ab50aa4e68cbf0b2eaee552337a74166d327cf86e8c02a08(
     context: ResourceContext,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__d9722fb3546c6a952b2b55adebbbf115305a6f7b346cf36e7ee20622e392d7b7(
@@ -8445,14 +8512,20 @@
 
 def _typecheckingstub__93749efec26f6060dadfeee523230f2893d7b4f15df00660a895c33f6aaa036f(
     context: ResourceContext,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__d697cdcbe532f07d04b89722be4ec6911b4b2516ffc502aba9f3652ee94e8634(
+    ssm_parameter_name: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__3d05ec817f774252beefe21c47c48d57bef1a1630540a04f30467dbd7ae53d72(
     context: ResourceContext,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__d9f45aee57f132f39a3dbfeafc22b558e4ef6959ec5789e3fa2ec6c8692946af(
```

### Comparing `cdklabs.cdk-cicd-wrapper-0.1.0/src/cdklabs/cdk_cicd_wrapper/_jsii/__init__.py` & `cdklabs.cdk-cicd-wrapper-0.1.1/src/cdklabs/cdk_cicd_wrapper/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import cdk_nag._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@cdklabs/cdk-cicd-wrapper",
-    "0.1.0",
+    "0.1.1",
     __name__[0:-6],
-    "cdk-cicd-wrapper@0.1.0.jsii.tgz",
+    "cdk-cicd-wrapper@0.1.1.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdklabs.cdk-cicd-wrapper-0.1.0/src/cdklabs.cdk_cicd_wrapper.egg-info/PKG-INFO` & `cdklabs.cdk-cicd-wrapper-0.1.1/src/cdklabs.cdk_cicd_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-cicd-wrapper
-Version: 0.1.0
+Version: 0.1.1
 Summary: This repository contains the infrastructure as code to wrap your AWS CDK project with CI/CD around it.
 Home-page: https://github.com/cdklabs/cdk-cicd-wrapper.git
 Author: CDK CI/CD Wrapper Team
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-cicd-wrapper.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

