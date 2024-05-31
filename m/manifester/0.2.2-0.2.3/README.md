# Comparing `tmp/manifester-0.2.2.tar.gz` & `tmp/manifester-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manifester-0.2.2.tar", last modified: Thu Apr  4 18:37:18 2024, max compression
+gzip compressed data, was "manifester-0.2.3.tar", last modified: Fri May 31 18:40:17 2024, max compression
```

## Comparing `manifester-0.2.2.tar` & `manifester-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:37:18.527105 manifester-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-04 18:37:03.000000 manifester-0.2.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:37:18.523105 manifester-0.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-04 18:37:03.000000 manifester-0.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:37:18.523105 manifester-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-04 18:37:03.000000 manifester-0.2.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-04 18:37:03.000000 manifester-0.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-04 18:37:03.000000 manifester-0.2.2/.github/workflows/update_manifester_image.yml
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-04 18:37:03.000000 manifester-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-04 18:37:03.000000 manifester-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-04 18:37:03.000000 manifester-0.2.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 18:37:03.000000 manifester-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19631 2024-04-04 18:37:18.527105 manifester-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-04 18:37:03.000000 manifester-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:37:18.523105 manifester-0.2.2/logs/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-04 18:37:03.000000 manifester-0.2.2/logs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:37:18.527105 manifester-0.2.2/manifester/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-04 18:37:03.000000 manifester-0.2.2/manifester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-04 18:37:03.000000 manifester-0.2.2/manifester/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     9407 2024-04-04 18:37:03.000000 manifester-0.2.2/manifester/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-04 18:37:03.000000 manifester-0.2.2/manifester/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    18728 2024-04-04 18:37:03.000000 manifester-0.2.2/manifester/manifester.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-04 18:37:03.000000 manifester-0.2.2/manifester/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:37:18.527105 manifester-0.2.2/manifester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19631 2024-04-04 18:37:18.000000 manifester-0.2.2/manifester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-04 18:37:18.000000 manifester-0.2.2/manifester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:37:18.000000 manifester-0.2.2/manifester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-04 18:37:18.000000 manifester-0.2.2/manifester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 18:37:18.000000 manifester-0.2.2/manifester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:37:03.000000 manifester-0.2.2/manifester_inventory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-04 18:37:03.000000 manifester-0.2.2/manifester_settings.yaml.example
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-04-04 18:37:03.000000 manifester-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:37:18.527105 manifester-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:37:18.527105 manifester-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-04-04 18:37:03.000000 manifester-0.2.2/tests/test_manifester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:40:17.448491 manifester-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-31 18:40:02.000000 manifester-0.2.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:40:17.444491 manifester-0.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-31 18:40:02.000000 manifester-0.2.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:40:17.444491 manifester-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-31 18:40:02.000000 manifester-0.2.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-31 18:40:02.000000 manifester-0.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-31 18:40:02.000000 manifester-0.2.3/.github/workflows/update_manifester_image.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-31 18:40:02.000000 manifester-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-31 18:40:02.000000 manifester-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-31 18:40:02.000000 manifester-0.2.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-31 18:40:02.000000 manifester-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-31 18:40:02.000000 manifester-0.2.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    19638 2024-05-31 18:40:17.448491 manifester-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-31 18:40:02.000000 manifester-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:40:17.444491 manifester-0.2.3/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-31 18:40:02.000000 manifester-0.2.3/logs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:40:17.444491 manifester-0.2.3/manifester/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 18:40:02.000000 manifester-0.2.3/manifester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-31 18:40:02.000000 manifester-0.2.3/manifester/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14923 2024-05-31 18:40:02.000000 manifester-0.2.3/manifester/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-31 18:40:02.000000 manifester-0.2.3/manifester/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18735 2024-05-31 18:40:02.000000 manifester-0.2.3/manifester/manifester.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-31 18:40:02.000000 manifester-0.2.3/manifester/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:40:17.448491 manifester-0.2.3/manifester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19638 2024-05-31 18:40:17.000000 manifester-0.2.3/manifester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-31 18:40:17.000000 manifester-0.2.3/manifester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:40:17.000000 manifester-0.2.3/manifester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-31 18:40:17.000000 manifester-0.2.3/manifester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 18:40:17.000000 manifester-0.2.3/manifester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:40:02.000000 manifester-0.2.3/manifester_inventory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-31 18:40:02.000000 manifester-0.2.3/manifester_settings.yaml.example
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-31 18:40:02.000000 manifester-0.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:40:17.448491 manifester-0.2.3/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      388 2024-05-31 18:40:02.000000 manifester-0.2.3/scripts/vault_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:40:17.448491 manifester-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:40:17.448491 manifester-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-31 18:40:02.000000 manifester-0.2.3/tests/test_manifester.py
```

### Comparing `manifester-0.2.2/.github/workflows/codeql-analysis.yml` & `manifester-0.2.3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `manifester-0.2.2/.github/workflows/python-publish.yml` & `manifester-0.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `manifester-0.2.2/.github/workflows/update_manifester_image.yml` & `manifester-0.2.3/.github/workflows/update_manifester_image.yml`

 * *Files identical despite different names*

### Comparing `manifester-0.2.2/.gitignore` & `manifester-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `manifester-0.2.2/LICENSE` & `manifester-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `manifester-0.2.2/PKG-INFO` & `manifester-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manifester
-Version: 0.2.2
+Version: 0.2.3
 Summary: Red Hat subscriptions made manifest.
 Author-email: Danny Synk <dsynk@redhat.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -215,15 +215,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
-Requires-Dist: dynaconf
+Requires-Dist: dynaconf[vault]
 Requires-Dist: logzero
 Requires-Dist: pytest
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: setuptools
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
```

### Comparing `manifester-0.2.2/README.md` & `manifester-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `manifester-0.2.2/manifester/commands.py` & `manifester-0.2.3/manifester/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,16 +56,21 @@
     inv = helpers.load_inventory_file(Path(settings.inventory_path))
     for num, allocation in enumerate(inv):
         if str(num) in allocations or allocation.get("name") in allocations or all_:
             Manifester(minimal_init=True).delete_subscription_allocation(
                 uuid=allocation.get("uuid")
             )
             if remove_manifest_file:
+                manifester_directory = (
+                    Path(os.environ["MANIFESTER_DIRECTORY"]).resolve()
+                    if "MANIFESTER_DIRECTORY" in os.environ
+                    else Path()
+                )
                 Path(
-                    f"{os.environ['MANIFESTER_DIRECTORY']}/manifests/{allocation.get('name')}_manifest.zip"
+                    f"{manifester_directory}/manifests/{allocation.get('name')}_manifest.zip"
                 ).unlink()
 
 
 @cli.command()
 @click.option("--details", is_flag=True, help="Display full inventory details")
 @click.option("--sync", is_flag=True, help="Fetch inventory data from RHSM before displaying")
 def inventory(details, sync):
```

### Comparing `manifester-0.2.2/manifester/logger.py` & `manifester-0.2.3/manifester/logger.py`

 * *Files identical despite different names*

### Comparing `manifester-0.2.2/manifester/manifester.py` & `manifester-0.2.3/manifester/manifester.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,27 @@
     process_sat_version,
     simple_retry,
     update_inventory,
 )
 from manifester.logger import setup_logzero
 from manifester.settings import settings
 
-setup_logzero(level=settings.get("log_level", "info"))
-
 
 class Manifester:
     """Main Manifester class responsible for generating a manifest from the provided settings."""
 
     def __init__(
         self,
         manifest_category=None,
         allocation_name=None,
         minimal_init=False,
         proxies=None,
         **kwargs,
     ):
+        setup_logzero(level=settings.get("log_level", "info"))
         if minimal_init:
             self.offline_token = settings.get("offline_token")
             self.token_request_url = settings.get("url").get("token_request")
             self.allocations_url = settings.get("url").get("allocations")
             self._access_token = None
             self._allocations = None
             self.token_request_data = {
```

### Comparing `manifester-0.2.2/manifester/settings.py` & `manifester-0.2.3/manifester/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 if "MANIFESTER_DIRECTORY" in os.environ:
     envar_location = Path(os.environ["MANIFESTER_DIRECTORY"])
     if envar_location.is_dir():
         MANIFESTER_DIRECTORY = envar_location
 
 settings_path = MANIFESTER_DIRECTORY.joinpath("manifester_settings.yaml")
 validators = [
-    # Validator("offline_token", must_exist=True),
+    Validator("offline_token", must_exist=True),
     Validator("simple_content_access", default="enabled"),
     Validator("username_prefix", len_min=3),
 ]
 settings = Dynaconf(
     settings_file=str(settings_path.absolute()),
     ENVVAR_PREFIX_FOR_DYNACONF="MANIFESTER",
+    load_dotenv=True,
     validators=validators,
 )
-
-settings.validators.validate()
+# settings.validators.validate()
```

### Comparing `manifester-0.2.2/manifester.egg-info/PKG-INFO` & `manifester-0.2.3/manifester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manifester
-Version: 0.2.2
+Version: 0.2.3
 Summary: Red Hat subscriptions made manifest.
 Author-email: Danny Synk <dsynk@redhat.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -215,15 +215,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
-Requires-Dist: dynaconf
+Requires-Dist: dynaconf[vault]
 Requires-Dist: logzero
 Requires-Dist: pytest
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: setuptools
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
```

### Comparing `manifester-0.2.2/manifester.egg-info/SOURCES.txt` & `manifester-0.2.3/manifester.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .flake8
 .gitignore
 .pre-commit-config.yaml
 Dockerfile
 LICENSE
+Makefile
 README.md
 manifester_inventory.yaml
 manifester_settings.yaml.example
 pyproject.toml
 .github/dependabot.yml
 .github/workflows/codeql-analysis.yml
 .github/workflows/python-publish.yml
@@ -19,8 +20,9 @@
 manifester/manifester.py
 manifester/settings.py
 manifester.egg-info/PKG-INFO
 manifester.egg-info/SOURCES.txt
 manifester.egg-info/dependency_links.txt
 manifester.egg-info/requires.txt
 manifester.egg-info/top_level.txt
+scripts/vault_login.py
 tests/test_manifester.py
```

### Comparing `manifester-0.2.2/manifester_settings.yaml.example` & `manifester-0.2.3/manifester_settings.yaml.example`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 #rhsm-manifester settings
+inventory_path: "manifester_inventory.yaml"
 log_level: "info"
 offline_token: ""
 proxies: {"https": ""}
+url:
+  token_request: "https://sso.redhat.com/auth/realms/redhat-external/protocol/openid-connect/token"
+  allocations: "https://api.access.redhat.com/management/v1/allocations"
 username_prefix: "example_username"  # replace value with a unique username
-inventory_path: "manifester_inventory.yaml"
 manifest_category:
   golden_ticket:
     # An offline token can be generated at https://access.redhat.com/management/api
     offline_token: ""
-    # Value of sat_version setting should be in the form 'sat-6.10'
-    sat_version: "sat-6.10"
+    # Value of sat_version setting should be in the form 'sat-6.14'
+    sat_version: "sat-6.14"
     # golden_ticket manifests should not use a quantity higher than 1 for any subscription
     # unless doing so is required for a test.
     subscription_data:
     # name should be an exact match of the subscription name as listed on the Customer Portal
       - name: "Software Collections and Developer Toolset"
         quantity: 1
       - name: "Red Hat Ansible Automation Platform, Standard (100 Managed Nodes)"
@@ -21,15 +24,15 @@
     simple_content_access: "enabled"
     url:
       token_request: "https://sso.redhat.com/auth/realms/redhat-external/protocol/openid-connect/token"
       allocations: "https://api.access.redhat.com/management/v1/allocations"
     proxies: {"https": ""}
   robottelo_automation:
     offline_token: ""
-    sat_version: "sat-6.10"
+    sat_version: "sat-6.14"
     subscription_data:
       - name: "Software Collections and Developer Toolset"
         quantity: 3
       - name: "Red Hat Ansible Automation Platform, Standard (100 Managed Nodes)"
         quantity: 2
     simple_content_access: "disabled"
     url:
```

### Comparing `manifester-0.2.2/pyproject.toml` & `manifester-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "click",
-    "dynaconf",
+    "dynaconf[vault]",
     "logzero",
     "pytest",
     "pyyaml",
     "requests",
     "setuptools",
 ]
 dynamic = ["version"]
@@ -152,14 +152,15 @@
     "PGH001", # No builtin eval() allowed
     "D203", # 1 blank line required before class docstring
     "D213", # Multi-line docstring summary should start at the second line
     "D406", # Section name should end with a newline
     "D407", # Section name underlining
     "E731", # do not assign a lambda expression, use a def
     "PLR0913", # Too many arguments to function call ({c_args} > {max_args})
+    "PLW1510", # subprocess.run without an explict `check` argument
     "RUF012", # Mutable class attributes should be annotated with typing.ClassVar
     "D107", # Missing docstring in __init__
 ]
 
 [tool.ruff.per-file-ignores]
 "manifester/__init__.py" = ["D104", "F401",]
 "manifester/manifester.py" = ["D401",]
```

### Comparing `manifester-0.2.2/tests/test_manifester.py` & `manifester-0.2.3/tests/test_manifester.py`

 * *Files identical despite different names*

