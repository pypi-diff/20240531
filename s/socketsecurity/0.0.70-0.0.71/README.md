# Comparing `tmp/socketsecurity-0.0.70.tar.gz` & `tmp/socketsecurity-0.0.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketsecurity-0.0.70.tar", last modified: Tue May 28 23:54:10 2024, max compression
+gzip compressed data, was "socketsecurity-0.0.71.tar", last modified: Fri May 31 15:02:34 2024, max compression
```

## Comparing `socketsecurity-0.0.70.tar` & `socketsecurity-0.0.71.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-28 23:54:10.327792 socketsecurity-0.0.70/
--rw-r--r--   0 douglascoburn   (501) staff       (20)     1066 2024-05-17 19:27:22.000000 socketsecurity-0.0.70/LICENSE
--rw-r--r--   0 douglascoburn   (501) staff       (20)     4907 2024-05-28 23:54:10.327619 socketsecurity-0.0.70/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)     4136 2024-05-17 19:24:12.000000 socketsecurity-0.0.70/README.md
--rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-28 23:53:34.000000 socketsecurity-0.0.70/pyproject.toml
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-28 23:54:10.327828 socketsecurity-0.0.70/setup.cfg
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-28 23:54:10.312998 socketsecurity-0.0.70/socketsecurity/
--rw-r--r--   0 douglascoburn   (501) staff       (20)       98 2024-05-16 10:04:37.000000 socketsecurity-0.0.70/socketsecurity/__init__.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-28 23:54:10.322226 socketsecurity-0.0.70/socketsecurity/core/
--rw-r--r--   0 douglascoburn   (501) staff       (20)    26372 2024-05-28 23:53:23.000000 socketsecurity-0.0.70/socketsecurity/core/__init__.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.70/socketsecurity/core/classes.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)      785 2024-05-16 11:28:29.000000 socketsecurity-0.0.70/socketsecurity/core/exceptions.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11584 2024-05-28 23:47:19.000000 socketsecurity-0.0.70/socketsecurity/core/github.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11283 2024-05-28 23:52:15.000000 socketsecurity-0.0.70/socketsecurity/core/gitlab.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    68147 2024-05-16 10:03:15.000000 socketsecurity-0.0.70/socketsecurity/core/issues.py
--rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.70/socketsecurity/core/licenses.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.70/socketsecurity/core/messages.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     6337 2024-05-28 23:51:33.000000 socketsecurity-0.0.70/socketsecurity/socketcli.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-28 23:54:10.327406 socketsecurity-0.0.70/socketsecurity.egg-info/
--rw-r--r--   0 douglascoburn   (501) staff       (20)     4907 2024-05-28 23:54:10.000000 socketsecurity-0.0.70/socketsecurity.egg-info/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)      568 2024-05-28 23:54:10.000000 socketsecurity-0.0.70/socketsecurity.egg-info/SOURCES.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-28 23:54:10.000000 socketsecurity-0.0.70/socketsecurity.egg-info/dependency_links.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-28 23:54:10.000000 socketsecurity-0.0.70/socketsecurity.egg-info/entry_points.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-28 23:54:10.000000 socketsecurity-0.0.70/socketsecurity.egg-info/requires.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-28 23:54:10.000000 socketsecurity-0.0.70/socketsecurity.egg-info/top_level.txt
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-31 15:02:34.271751 socketsecurity-0.0.71/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     1066 2024-05-17 19:27:22.000000 socketsecurity-0.0.71/LICENSE
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     4907 2024-05-31 15:02:34.271534 socketsecurity-0.0.71/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     4136 2024-05-17 19:24:12.000000 socketsecurity-0.0.71/README.md
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-31 15:01:39.000000 socketsecurity-0.0.71/pyproject.toml
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-31 15:02:34.271800 socketsecurity-0.0.71/setup.cfg
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-31 15:02:34.252798 socketsecurity-0.0.71/socketsecurity/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       98 2024-05-16 10:04:37.000000 socketsecurity-0.0.71/socketsecurity/__init__.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-31 15:02:34.267202 socketsecurity-0.0.71/socketsecurity/core/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    28220 2024-05-31 15:01:33.000000 socketsecurity-0.0.71/socketsecurity/core/__init__.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.71/socketsecurity/core/classes.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      785 2024-05-16 11:28:29.000000 socketsecurity-0.0.71/socketsecurity/core/exceptions.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11584 2024-05-28 23:47:19.000000 socketsecurity-0.0.71/socketsecurity/core/github.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11283 2024-05-28 23:52:15.000000 socketsecurity-0.0.71/socketsecurity/core/gitlab.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    68147 2024-05-16 10:03:15.000000 socketsecurity-0.0.71/socketsecurity/core/issues.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.71/socketsecurity/core/licenses.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.71/socketsecurity/core/messages.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     6812 2024-05-31 14:55:32.000000 socketsecurity-0.0.71/socketsecurity/socketcli.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-31 15:02:34.271206 socketsecurity-0.0.71/socketsecurity.egg-info/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     4907 2024-05-31 15:02:34.000000 socketsecurity-0.0.71/socketsecurity.egg-info/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      568 2024-05-31 15:02:34.000000 socketsecurity-0.0.71/socketsecurity.egg-info/SOURCES.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-31 15:02:34.000000 socketsecurity-0.0.71/socketsecurity.egg-info/dependency_links.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-31 15:02:34.000000 socketsecurity-0.0.71/socketsecurity.egg-info/entry_points.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-31 15:02:34.000000 socketsecurity-0.0.71/socketsecurity.egg-info/requires.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-31 15:02:34.000000 socketsecurity-0.0.71/socketsecurity.egg-info/top_level.txt
```

### Comparing `socketsecurity-0.0.70/LICENSE` & `socketsecurity-0.0.71/LICENSE`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.70/PKG-INFO` & `socketsecurity-0.0.71/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.70
+Version: 0.0.71
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `socketsecurity-0.0.70/README.md` & `socketsecurity-0.0.71/README.md`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.70/pyproject.toml` & `socketsecurity-0.0.71/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketsecurity"
-version = "0.0.70"
+version = "0.0.71"
 requires-python = ">= 3.9"
 dependencies = [
     'requests',
     'mdutils',
     'prettytable',
     'argparse'
 ]
```

### Comparing `socketsecurity-0.0.70/socketsecurity/core/__init__.py` & `socketsecurity-0.0.71/socketsecurity/core/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 )
 import platform
 from glob import glob
 import time
 
 
 __author__ = 'socket.dev'
-__version__ = '0.0.70'
+__version__ = '0.0.71'
 __all__ = [
     "Core",
     "log",
     "__version__"
 ]
 
 
@@ -242,14 +242,63 @@
             if default not in org_rules:
                 action = default_rules[default]["action"]
                 org_rules[default] = {
                     "action": action
                 }
         return org_rules
 
+    # @staticmethod
+    # def get_supported_file_types() -> dict:
+    #     path = "report/supported"
+
+    @staticmethod
+    def get_manifest_files(package: Package, packages: dict) -> str:
+        if package.direct:
+            manifests = []
+            for manifest_item in package.manifestFiles:
+                manifest = manifest_item["file"]
+                manifests.append(manifest)
+            manifest_files = ";".join(manifests)
+        else:
+            manifests = []
+            for top_id in package.topLevelAncestors:
+                top_package: Package
+                top_package = packages[top_id]
+                for manifest_item in top_package.manifestFiles:
+                    manifest = manifest_item["file"]
+                    new_string = f"{package.name}@{package.version}({manifest})"
+                    manifests.append(new_string)
+            manifest_files = ";".join(manifests)
+        return manifest_files
+
+    @staticmethod
+    def create_sbom_output(diff: Diff) -> list:
+        sbom = []
+        for package_id in diff.packages:
+            package: Package
+            package = diff.packages[package_id]
+            manifest_files = Core.get_manifest_files(package, diff.packages)
+            item = {
+                "id": package.id,
+                "license": package.license,
+                "license_text": package.license_text,
+                "manifestFiles": manifest_files,
+                "score": package.score,
+                "size": package.size,
+                "ecosystem": package.type,
+                "alerts": package.alerts,
+                "direct": package.direct,
+                "name": package.name,
+                "version": package.version,
+                "author": package.author,
+                "url": package.url
+            }
+            sbom.append(item)
+        return sbom
+
     @staticmethod
     def find_files(path: str) -> list:
         """
         Globs the path for supported manifest files.
         Note: Might move the source to a JSON file
         :param path: Str - path to where the manifest files are located
         :return:
@@ -310,16 +359,16 @@
                 },
                 "requirements_*.txt": {
                     "pattern": "requirements_*.txt"
                 },
                 "requirements.frozen": {
                     "pattern": "requirements.frozen"
                 },
-                "setup.py.old": {
-                    "pattern": "setup.py.old"
+                "setup.py": {
+                    "pattern": "setup.py"
                 }
             },
             "golang": {
                 "go.mod": {
                     "pattern": "go.mod"
                 },
                 "go.sum": {
```

### Comparing `socketsecurity-0.0.70/socketsecurity/core/classes.py` & `socketsecurity-0.0.71/socketsecurity/core/classes.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.70/socketsecurity/core/exceptions.py` & `socketsecurity-0.0.71/socketsecurity/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.70/socketsecurity/core/github.py` & `socketsecurity-0.0.71/socketsecurity/core/github.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.70/socketsecurity/core/gitlab.py` & `socketsecurity-0.0.71/socketsecurity/core/gitlab.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.70/socketsecurity/core/issues.py` & `socketsecurity-0.0.71/socketsecurity/core/issues.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.70/socketsecurity/core/licenses.py` & `socketsecurity-0.0.71/socketsecurity/core/licenses.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.70/socketsecurity/core/messages.py` & `socketsecurity-0.0.71/socketsecurity/core/messages.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.70/socketsecurity/socketcli.py` & `socketsecurity-0.0.71/socketsecurity/socketcli.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,28 @@
     default='api',
     help='Integration mode choices are api, github, gitlab, and bitbucket',
     choices=["api", "github", "gitlab"],
     required=False
 )
 
 parser.add_argument(
+    '--sbom-file',
+    default=None,
+    help='If soecified save the SBOM details to the specified file',
+    required=False
+)
+
+parser.add_argument(
+    '--commit-sha',
+    default="",
+    help='Optional git commit sha',
+    required=False
+)
+
+parser.add_argument(
     '--generate-license',
     default=False,
     help='Run in license mode to generate license output',
     required=False
 )
 
 parser.add_argument(
@@ -111,14 +125,16 @@
     branch = arguments.branch
     commit_message = arguments.commit_message
     committer = arguments.committer
     default_branch = arguments.default_branch
     pr_number = arguments.pr_number
     target_path = arguments.target_path
     scm_type = arguments.scm
+    commit_sha = arguments.commit_sha
+    sbom_file = arguments.sbom_file
     license_mode = arguments.generate_license
     license_file = f"{repo}"
     if branch is not None:
         license_file += f"_{branch}"
     license_file += ".json"
     api_token = os.getenv("SOCKET_SECURITY_API_KEY") or arguments.api_token
     if api_token is None:
@@ -133,24 +149,25 @@
         from socketsecurity.core.github import Github
         scm = Github()
     elif scm_type == 'gitlab':
         from socketsecurity.core.gitlab import Gitlab
         scm = Gitlab()
     if scm is not None:
         default_branch = scm.is_default_branch
+
     base_api_url = os.getenv("BASE_API_URL") or None
     core = Core(token=api_token, request_timeout=6000, base_api_url=base_api_url)
     set_as_pending_head = False
     if default_branch:
         set_as_pending_head = True
     params = FullScanParams(
         repo=repo,
         branch=branch,
         commit_message=commit_message,
-        commit_hash="",
+        commit_hash=commit_sha,
         pull_request=pr_number,
         committers=committer,
         make_default_branch=default_branch,
         set_as_pending_head=set_as_pending_head
     )
     diff = None
     if scm is not None and scm.check_event_type() == "comment":
@@ -198,11 +215,13 @@
                 "direct": package.direct,
                 "url": package.url,
                 "license": package.license,
                 "license_text": package.license_text
             }
             all_packages[package_id] = output
         core.save_file(license_file, json.dumps(all_packages))
+    if diff is not None and sbom_file is not None:
+        core.save_file(sbom_file, json.dumps(core.create_sbom_output(diff)))
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `socketsecurity-0.0.70/socketsecurity.egg-info/PKG-INFO` & `socketsecurity-0.0.71/socketsecurity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.70
+Version: 0.0.71
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `socketsecurity-0.0.70/socketsecurity.egg-info/SOURCES.txt` & `socketsecurity-0.0.71/socketsecurity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

