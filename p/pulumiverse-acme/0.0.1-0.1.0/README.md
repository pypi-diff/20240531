# Comparing `tmp/pulumiverse_acme-0.0.1.tar.gz` & `tmp/pulumiverse_acme-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_acme-0.0.1.tar", last modified: Mon Sep 25 18:50:16 2023, max compression
+gzip compressed data, was "pulumiverse_acme-0.1.0.tar", last modified: Fri May 31 06:21:57 2024, max compression
```

## Comparing `pulumiverse_acme-0.0.1.tar` & `pulumiverse_acme-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 18:50:16.760395 pulumiverse_acme-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2023-09-25 18:50:16.760395 pulumiverse_acme-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      997 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 18:50:16.756395 pulumiverse_acme-0.0.1/pulumiverse_acme/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/pulumiverse_acme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7430 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/pulumiverse_acme/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8126 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/pulumiverse_acme/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    96677 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/pulumiverse_acme/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 18:50:16.760395 pulumiverse_acme-0.0.1/pulumiverse_acme/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/pulumiverse_acme/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/pulumiverse_acme/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/pulumiverse_acme/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/pulumiverse_acme/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/pulumiverse_acme/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/pulumiverse_acme/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10122 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/pulumiverse_acme/registration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-25 18:50:16.760395 pulumiverse_acme-0.0.1/pulumiverse_acme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/pulumiverse_acme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      596 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/pulumiverse_acme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/pulumiverse_acme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/pulumiverse_acme.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/pulumiverse_acme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/pulumiverse_acme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-25 18:50:16.760395 pulumiverse_acme-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2023-09-25 18:50:16.000000 pulumiverse_acme-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:21:57.839041 pulumiverse_acme-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-31 06:21:57.839041 pulumiverse_acme-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:21:57.835041 pulumiverse_acme-0.1.0/pulumiverse_acme/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/pulumiverse_acme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/pulumiverse_acme/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/pulumiverse_acme/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96677 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/pulumiverse_acme/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:21:57.839041 pulumiverse_acme-0.1.0/pulumiverse_acme/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/pulumiverse_acme/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/pulumiverse_acme/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/pulumiverse_acme/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/pulumiverse_acme/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/pulumiverse_acme/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/pulumiverse_acme/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10122 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/pulumiverse_acme/registration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:21:57.839041 pulumiverse_acme-0.1.0/pulumiverse_acme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/pulumiverse_acme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/pulumiverse_acme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/pulumiverse_acme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/pulumiverse_acme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/pulumiverse_acme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/pulumiverse_acme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 06:21:57.839041 pulumiverse_acme-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-31 06:21:57.000000 pulumiverse_acme-0.1.0/setup.py
```

### Comparing `pulumiverse_acme-0.0.1/PKG-INFO` & `pulumiverse_acme-0.1.0/pulumiverse_acme.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: pulumiverse_acme
-Version: 0.0.1
+Name: pulumiverse-acme
+Version: 0.1.0
 Summary: A Pulumi package for creating and managing ACME cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-acme
 Keywords: pulumi acme category/cloud
-Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # ACME Resource Provider
 
 The ACME Resource Provider lets you manage ACME resources. 
 [Let's Encrypt](https://letsencrypt.org/) is the biggest ACME CA in use.
 
@@ -56,9 +55,7 @@
 ```bash
 dotnet add package Pulumiverse.Acme
 ```
 
 ## Reference
 
 For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/acme/api-docs/).
-
-
```

### Comparing `pulumiverse_acme-0.0.1/README.md` & `pulumiverse_acme-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_acme-0.0.1/pulumiverse_acme/__init__.py` & `pulumiverse_acme-0.1.0/pulumiverse_acme/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_acme-0.0.1/pulumiverse_acme/_inputs.py` & `pulumiverse_acme-0.1.0/pulumiverse_acme/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,25 +110,19 @@
         pulumi.set(self, "proxy_header", value)
 
 
 @pulumi.input_type
 class CertificateHttpMemcachedChallengeArgs:
     def __init__(__self__, *,
                  hosts: pulumi.Input[Sequence[pulumi.Input[str]]]):
-        """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] hosts: The hosts to publish the record to.
-        """
         pulumi.set(__self__, "hosts", hosts)
 
     @property
     @pulumi.getter
     def hosts(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        """
-        The hosts to publish the record to.
-        """
         return pulumi.get(self, "hosts")
 
     @hosts.setter
     def hosts(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "hosts", value)
```

### Comparing `pulumiverse_acme-0.0.1/pulumiverse_acme/_utilities.py` & `pulumiverse_acme-0.1.0/pulumiverse_acme/_utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 
+import asyncio
+import importlib.metadata
 import importlib.util
 import inspect
 import json
 import os
-import pkg_resources
 import sys
 import typing
 
 import pulumi
 import pulumi.runtime
+from pulumi.runtime.sync_await import _sync_await
 
 from semver import VersionInfo as SemverVersion
 from parver import Version as PEP440Version
 
 
 def get_env(*args):
     for v in args:
@@ -66,15 +68,15 @@
     # pkg_resources uses setuptools to inspect the set of installed packages. We use it here to ask
     # for the currently installed version of the root package (i.e. us) and get its version.
 
     # Unfortunately, PEP440 and semver differ slightly in incompatible ways. The Pulumi engine expects
     # to receive a valid semver string when receiving requests from the language host, so it's our
     # responsibility as the library to convert our own PEP440 version into a valid semver string.
 
-    pep440_version_string = pkg_resources.require(root_package)[0].version
+    pep440_version_string = importlib.metadata.version(root_package)
     pep440_version = PEP440Version.parse(pep440_version_string)
     (major, minor, patch) = pep440_version.release
     prerelease = None
     if pep440_version.pre_tag == 'a':
         prerelease = f"alpha.{pep440_version.pre}"
     elif pep440_version.pre_tag == 'b':
         prerelease = f"beta.{pep440_version.pre}"
@@ -242,9 +244,48 @@
             'kwargs': bound_args.kwargs
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
 
+
+def call_plain(
+    tok: str,
+    props: pulumi.Inputs,
+    res: typing.Optional[pulumi.Resource] = None,
+    typ: typing.Optional[type] = None,
+) -> typing.Any:
+    """
+    Wraps pulumi.runtime.plain to force the output and return it plainly.
+    """
+
+    output = pulumi.runtime.call(tok, props, res, typ)
+
+    # Ingoring deps silently. They are typically non-empty, r.f() calls include r as a dependency.
+    result, known, secret, _ = _sync_await(asyncio.ensure_future(_await_output(output)))
+
+    problem = None
+    if not known:
+        problem = ' an unknown value'
+    elif secret:
+        problem = ' a secret value'
+
+    if problem:
+        raise AssertionError(
+            f"Plain resource method '{tok}' incorrectly returned {problem}. "
+            + "This is an error in the provider, please report this to the provider developer."
+        )
+
+    return result
+
+
+async def _await_output(o: pulumi.Output[typing.Any]) -> typing.Tuple[object, bool, bool, set]:
+    return (
+        await o._future,
+        await o._is_known,
+        await o._is_secret,
+        await o._resources,
+    )
+
 def get_plugin_download_url():
 	return "github://api.github.com/pulumiverse/pulumi-acme"
```

### Comparing `pulumiverse_acme-0.0.1/pulumiverse_acme/certificate.py` & `pulumiverse_acme-0.1.0/pulumiverse_acme/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_acme-0.0.1/pulumiverse_acme/config/vars.py` & `pulumiverse_acme-0.1.0/pulumiverse_acme/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_acme-0.0.1/pulumiverse_acme/outputs.py` & `pulumiverse_acme-0.1.0/pulumiverse_acme/outputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,25 +111,19 @@
         return pulumi.get(self, "proxy_header")
 
 
 @pulumi.output_type
 class CertificateHttpMemcachedChallenge(dict):
     def __init__(__self__, *,
                  hosts: Sequence[str]):
-        """
-        :param Sequence[str] hosts: The hosts to publish the record to.
-        """
         pulumi.set(__self__, "hosts", hosts)
 
     @property
     @pulumi.getter
     def hosts(self) -> Sequence[str]:
-        """
-        The hosts to publish the record to.
-        """
         return pulumi.get(self, "hosts")
 
 
 @pulumi.output_type
 class CertificateHttpS3Challenge(dict):
     @staticmethod
     def __key_warning(key: str):
```

### Comparing `pulumiverse_acme-0.0.1/pulumiverse_acme/provider.py` & `pulumiverse_acme-0.1.0/pulumiverse_acme/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_acme-0.0.1/pulumiverse_acme/registration.py` & `pulumiverse_acme-0.1.0/pulumiverse_acme/registration.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_acme-0.0.1/pulumiverse_acme.egg-info/PKG-INFO` & `pulumiverse_acme-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: pulumiverse-acme
-Version: 0.0.1
+Name: pulumiverse_acme
+Version: 0.1.0
 Summary: A Pulumi package for creating and managing ACME cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-acme
 Keywords: pulumi acme category/cloud
-Platform: UNKNOWN
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # ACME Resource Provider
 
 The ACME Resource Provider lets you manage ACME resources. 
 [Let's Encrypt](https://letsencrypt.org/) is the biggest ACME CA in use.
 
@@ -56,9 +55,7 @@
 ```bash
 dotnet add package Pulumiverse.Acme
 ```
 
 ## Reference
 
 For detailed reference documentation, please visit [the Pulumi registry](https://www.pulumi.com/registry/packages/acme/api-docs/).
-
-
```

### Comparing `pulumiverse_acme-0.0.1/pulumiverse_acme.egg-info/SOURCES.txt` & `pulumiverse_acme-0.1.0/pulumiverse_acme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_acme-0.0.1/setup.py` & `pulumiverse_acme-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.1"
+VERSION = "0.1.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "acme Pulumi Package - Development Version"
 
 
 setup(name='pulumiverse_acme',
-      python_requires='>=3.7',
+      python_requires='>=3.8',
       version=VERSION,
       description="A Pulumi package for creating and managing ACME cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       keywords='pulumi acme category/cloud',
       url='https://www.pulumi.com',
       project_urls={
```

