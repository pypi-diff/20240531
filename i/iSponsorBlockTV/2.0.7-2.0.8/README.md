# Comparing `tmp/isponsorblocktv-2.0.7.tar.gz` & `tmp/isponsorblocktv-2.0.8.tar.gz`

## Comparing `isponsorblocktv-2.0.7.tar` & `isponsorblocktv-2.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.deepsource.toml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.dockerignore
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/Dockerfile
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/config.json.template
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/docker-compose.yml
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/requirements.txt
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.github/workflows/build_docker_images.yml
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.github/workflows/release_pypi.yml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.github/workflows/update_docker_readme.yml
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/main.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/main_tui.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/__init__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/__main__.py
--rw-r--r--   0        0        0     8313 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/api_helpers.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/conditional_ttl_cache.py
--rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/config_setup.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/constants.py
--rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/dial_client.py
--rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/helpers.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/macos_install.py
--rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/main.py
--rw-r--r--   0        0        0     5735 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/setup-wizard-style.tcss
--rw-r--r--   0        0        0    35441 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/setup_wizard.py
--rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/src/iSponsorBlockTV/ytlounge.py
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/LICENSE.md
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/README.md
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/pyproject.toml
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/.deepsource.toml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/.dockerignore
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/Dockerfile
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/config.json.template
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/docker-compose.yml
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/requirements.txt
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/.github/workflows/build_docker_images.yml
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/.github/workflows/release_pypi.yml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/.github/workflows/update_docker_readme.yml
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/src/main.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/src/main_tui.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/src/iSponsorBlockTV/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/src/iSponsorBlockTV/__main__.py
+-rw-r--r--   0        0        0     8313 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/src/iSponsorBlockTV/api_helpers.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/src/iSponsorBlockTV/conditional_ttl_cache.py
+-rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/src/iSponsorBlockTV/config_setup.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/src/iSponsorBlockTV/constants.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/src/iSponsorBlockTV/dial_client.py
+-rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/src/iSponsorBlockTV/helpers.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/src/iSponsorBlockTV/macos_install.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/src/iSponsorBlockTV/main.py
+-rw-r--r--   0        0        0     5735 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/src/iSponsorBlockTV/setup-wizard-style.tcss
+-rw-r--r--   0        0        0    35441 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/src/iSponsorBlockTV/setup_wizard.py
+-rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/src/iSponsorBlockTV/ytlounge.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/LICENSE.md
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/README.md
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 isponsorblocktv-2.0.8/PKG-INFO
```

### Comparing `isponsorblocktv-2.0.7/.pre-commit-config.yaml` & `isponsorblocktv-2.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/Dockerfile` & `isponsorblocktv-2.0.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/.github/ISSUE_TEMPLATE/bug_report.md` & `isponsorblocktv-2.0.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/.github/ISSUE_TEMPLATE/feature_request.md` & `isponsorblocktv-2.0.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/.github/workflows/build_docker_images.yml` & `isponsorblocktv-2.0.8/.github/workflows/build_docker_images.yml`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/.github/workflows/release_pypi.yml` & `isponsorblocktv-2.0.8/.github/workflows/release_pypi.yml`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/.github/workflows/update_docker_readme.yml` & `isponsorblocktv-2.0.8/.github/workflows/update_docker_readme.yml`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/src/iSponsorBlockTV/api_helpers.py` & `isponsorblocktv-2.0.8/src/iSponsorBlockTV/api_helpers.py`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/src/iSponsorBlockTV/conditional_ttl_cache.py` & `isponsorblocktv-2.0.8/src/iSponsorBlockTV/conditional_ttl_cache.py`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/src/iSponsorBlockTV/config_setup.py` & `isponsorblocktv-2.0.8/src/iSponsorBlockTV/config_setup.py`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/src/iSponsorBlockTV/constants.py` & `isponsorblocktv-2.0.8/src/iSponsorBlockTV/constants.py`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/src/iSponsorBlockTV/dial_client.py` & `isponsorblocktv-2.0.8/src/iSponsorBlockTV/dial_client.py`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/src/iSponsorBlockTV/helpers.py` & `isponsorblocktv-2.0.8/src/iSponsorBlockTV/helpers.py`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/src/iSponsorBlockTV/macos_install.py` & `isponsorblocktv-2.0.8/src/iSponsorBlockTV/macos_install.py`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/src/iSponsorBlockTV/main.py` & `isponsorblocktv-2.0.8/src/iSponsorBlockTV/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,21 +48,21 @@
         except:
             # traceback.print_exc()
             return False
 
     # Main subscription loop
     async def loop(self):
         lounge_controller = self.lounge_controller
-        while not lounge_controller.linked():
-            try:
-                self.logger.debug("Refreshing auth")
-                await lounge_controller.refresh_auth()
-            except:
-                await asyncio.sleep(10)
         while not self.cancelled:
+            while not lounge_controller.linked():
+                try:
+                    self.logger.debug("Refreshing auth")
+                    await lounge_controller.refresh_auth()
+                except:
+                    await asyncio.sleep(10)
             while not (await self.is_available()) and not self.cancelled:
                 await asyncio.sleep(10)
             try:
                 await lounge_controller.connect()
             except:
                 pass
             while not lounge_controller.connected() and not self.cancelled:
```

### Comparing `isponsorblocktv-2.0.7/src/iSponsorBlockTV/setup-wizard-style.tcss` & `isponsorblocktv-2.0.8/src/iSponsorBlockTV/setup-wizard-style.tcss`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/src/iSponsorBlockTV/setup_wizard.py` & `isponsorblocktv-2.0.8/src/iSponsorBlockTV/setup_wizard.py`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/src/iSponsorBlockTV/ytlounge.py` & `isponsorblocktv-2.0.8/src/iSponsorBlockTV/ytlounge.py`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/.gitignore` & `isponsorblocktv-2.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/LICENSE.md` & `isponsorblocktv-2.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/README.md` & `isponsorblocktv-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `isponsorblocktv-2.0.7/pyproject.toml` & `isponsorblocktv-2.0.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "iSponsorBlockTV"
-version = "2.0.7"
+version = "2.0.8"
 authors = [
     {"name" = "dmunozv04"}
 ]
 description = "SponsorBlock client for all YouTube TV clients"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `isponsorblocktv-2.0.7/PKG-INFO` & `isponsorblocktv-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: iSponsorBlockTV
-Version: 2.0.7
+Version: 2.0.8
 Summary: SponsorBlock client for all YouTube TV clients
 Project-URL: Homepage, https://github.com/dmunozv04/iSponsorBlockTV
 Project-URL: Bug Tracker, https://github.com/dmunozv04/iSponsorBlockTV/issues
 Author: dmunozv04
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

