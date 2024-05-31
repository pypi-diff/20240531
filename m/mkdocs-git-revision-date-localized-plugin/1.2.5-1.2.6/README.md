# Comparing `tmp/mkdocs_git_revision_date_localized_plugin-1.2.5.tar.gz` & `tmp/mkdocs_git_revision_date_localized_plugin-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_git_revision_date_localized_plugin-1.2.5.tar", last modified: Tue Apr 30 21:22:05 2024, max compression
+gzip compressed data, was "mkdocs_git_revision_date_localized_plugin-1.2.6.tar", last modified: Fri May 31 19:07:23 2024, max compression
```

## Comparing `mkdocs_git_revision_date_localized_plugin-1.2.5.tar` & `mkdocs_git_revision_date_localized_plugin-1.2.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:22:05.158894 mkdocs_git_revision_date_localized_plugin-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-30 21:22:05.158894 mkdocs_git_revision_date_localized_plugin-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:22:05.154894 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/ci.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:22:05.154894 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/css/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/css/timeago.css
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/exclude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:22:05.158894 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/js/
--rw-r--r--   0 runner    (1001) docker     (127)    29575 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/js/timeago.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/js/timeago_mkdocs_material.js
--rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:22:05.158894 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-30 21:22:05.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-30 21:22:05.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 21:22:05.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-30 21:22:05.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-30 21:22:05.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-30 21:22:05.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 21:22:05.158894 mkdocs_git_revision_date_localized_plugin-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 21:22:05.158894 mkdocs_git_revision_date_localized_plugin-1.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    23576 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/tests/test_builds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/tests/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-30 21:21:33.000000 mkdocs_git_revision_date_localized_plugin-1.2.5/tests/test_exclude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:07:23.449905 mkdocs_git_revision_date_localized_plugin-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-31 19:06:52.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-31 19:06:52.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-31 19:07:23.449905 mkdocs_git_revision_date_localized_plugin-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-31 19:06:52.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:07:23.445905 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 19:06:52.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-31 19:06:52.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/ci.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:07:23.445905 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-31 19:06:52.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/css/timeago.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-31 19:06:52.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-31 19:06:52.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/exclude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:07:23.449905 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    29575 2024-05-31 19:06:52.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/js/timeago.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-31 19:06:52.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/js/timeago_mkdocs_material.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-05-31 19:06:52.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-31 19:06:52.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:07:23.449905 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-31 19:07:23.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-31 19:07:23.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:07:23.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-31 19:07:23.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 19:07:23.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-31 19:07:23.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 19:06:52.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 19:07:23.449905 mkdocs_git_revision_date_localized_plugin-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-31 19:06:52.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:07:23.449905 mkdocs_git_revision_date_localized_plugin-1.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    23576 2024-05-31 19:06:52.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/tests/test_builds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-05-31 19:06:52.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/tests/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-31 19:06:52.000000 mkdocs_git_revision_date_localized_plugin-1.2.6/tests/test_exclude.py
```

### Comparing `mkdocs_git_revision_date_localized_plugin-1.2.5/LICENSE` & `mkdocs_git_revision_date_localized_plugin-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_git_revision_date_localized_plugin-1.2.5/PKG-INFO` & `mkdocs_git_revision_date_localized_plugin-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-git-revision-date-localized-plugin
-Version: 1.2.5
+Version: 1.2.6
 Summary: Mkdocs plugin that enables displaying the localized date of the last git modification of a markdown file.
 Home-page: https://github.com/timvink/mkdocs-git-revision-date-localized-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs git date timeago babel plugin
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: mkdocs-git-revision-date-localized-plugin Version:
-1.2.5 Summary: Mkdocs plugin that enables displaying the localized date of the
+1.2.6 Summary: Mkdocs plugin that enables displaying the localized date of the
 last git modification of a markdown file. Home-page: https://github.com/
 timvink/mkdocs-git-revision-date-localized-plugin Author: Tim Vink Author-
 email: vinktim@gmail.com License: MIT Keywords: mkdocs git date timeago babel
 plugin Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mkdocs_git_revision_date_localized_plugin-1.2.5/README.md` & `mkdocs_git_revision_date_localized_plugin-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/ci.py` & `mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/ci.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
                 Make sure to set GIT_DEPTH to 0 in your .gitlab-ci.yml file
                 (see https://docs.gitlab.com/ee/user/project/pipelines/settings.html#git-shallow-clone).
                 """
         )
 
     # Github Actions
     elif os.getenv("GITHUB_ACTIONS") is not None and n_commits == 1:
+        # See also https://docs.github.com/en/actions/learn-github-actions/variables#default-environment-variables
         # Default is fetch-depth of 1 for github actions
         logging.warning(
             """
                 [git-revision-date-localized-plugin] Running on GitHub Actions might lead to wrong
                 Git revision dates due to a shallow git fetch depth.
 
                 Try setting fetch-depth to 0 in your GitHub Action
@@ -57,15 +58,15 @@
 
                 Remove any Shallow Fetch settings
                 (see https://docs.microsoft.com/en-us/azure/devops/pipelines/repos/pipeline-options-for-git?view=azure-devops#shallow-fetch).
                 """
         )
 
     # Bitbucket pipelines
-    elif os.getenv("CI") is not None and n_commits < 50:
+    elif os.getenv("BITBUCKET_BUILD_NUMBER") is not None and n_commits < 50:
         # Default is fetch-depth of 50 for bitbucket pipelines
         logging.warning(
             """
                 [git-revision-date-localized-plugin] Running on bitbucket pipelines might lead to wrong
                 Git revision dates due to a shallow git fetch depth.
 
                 Try setting "clone: depth" to "full" in your pipeline
```

### Comparing `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/dates.py` & `mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/dates.py`

 * *Files identical despite different names*

### Comparing `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/exclude.py` & `mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/exclude.py`

 * *Files identical despite different names*

### Comparing `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/js/timeago.min.js` & `mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/js/timeago.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/js/timeago_mkdocs_material.js` & `mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/js/timeago_mkdocs_material.js`

 * *Files identical despite different names*

### Comparing `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/plugin.py` & `mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
 from mkdocs_git_revision_date_localized_plugin.util import Util
 from mkdocs_git_revision_date_localized_plugin.exclude import exclude
 
 from typing import Any, Dict
 from collections import OrderedDict
 
+from packaging.version import Version
+
 HERE = os.path.dirname(os.path.abspath(__file__))
 
 class GitRevisionDateLocalizedPlugin(BasePlugin):
     """
     Mkdocs plugin to add revision date from Git.
 
     See https://www.mkdocs.org/user-guide/plugins
@@ -72,15 +74,15 @@
 
         # Get locale from plugin configuration
         plugin_locale = self.config.get("locale", None)
 
         # theme locale
         if "theme" in config and "locale" in config.get("theme"):
             custom_theme = config.get("theme")
-            theme_locale = custom_theme.locale if mkdocs_version >= "1.6.0" else custom_theme._vars.get("locale")
+            theme_locale = custom_theme.locale if Version(mkdocs_version) >= Version("1.6.0") else custom_theme._vars.get("locale")
             logging.debug(
                 "Locale '%s' extracted from the custom theme: '%s'"
                 % (theme_locale, custom_theme.name)
             )
         elif "theme" in config and "language" in config.get("theme"):
             custom_theme = config.get("theme")
             theme_locale = custom_theme._vars.get("language")
```

### Comparing `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin/util.py` & `mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin/util.py`

 * *Files identical despite different names*

### Comparing `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/PKG-INFO` & `mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-git-revision-date-localized-plugin
-Version: 1.2.5
+Version: 1.2.6
 Summary: Mkdocs plugin that enables displaying the localized date of the last git modification of a markdown file.
 Home-page: https://github.com/timvink/mkdocs-git-revision-date-localized-plugin
 Author: Tim Vink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs git date timeago babel plugin
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: mkdocs-git-revision-date-localized-plugin Version:
-1.2.5 Summary: Mkdocs plugin that enables displaying the localized date of the
+1.2.6 Summary: Mkdocs plugin that enables displaying the localized date of the
 last git modification of a markdown file. Home-page: https://github.com/
 timvink/mkdocs-git-revision-date-localized-plugin Author: Tim Vink Author-
 email: vinktim@gmail.com License: MIT Keywords: mkdocs git date timeago babel
 plugin Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mkdocs_git_revision_date_localized_plugin-1.2.5/mkdocs_git_revision_date_localized_plugin.egg-info/SOURCES.txt` & `mkdocs_git_revision_date_localized_plugin-1.2.6/mkdocs_git_revision_date_localized_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_git_revision_date_localized_plugin-1.2.5/setup.py` & `mkdocs_git_revision_date_localized_plugin-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 DEPENDENCIES = file.readlines()
 file.close()
 
 del file
 
 setup(
     name="mkdocs-git-revision-date-localized-plugin",
-    version="1.2.5",
+    version="1.2.6",
     description="Mkdocs plugin that enables displaying the localized date of the last git modification of a markdown file.",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     keywords="mkdocs git date timeago babel plugin",
     url="https://github.com/timvink/mkdocs-git-revision-date-localized-plugin",
     author="Tim Vink",
     author_email="vinktim@gmail.com",
```

### Comparing `mkdocs_git_revision_date_localized_plugin-1.2.5/tests/test_builds.py` & `mkdocs_git_revision_date_localized_plugin-1.2.6/tests/test_builds.py`

 * *Files identical despite different names*

### Comparing `mkdocs_git_revision_date_localized_plugin-1.2.5/tests/test_dates.py` & `mkdocs_git_revision_date_localized_plugin-1.2.6/tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `mkdocs_git_revision_date_localized_plugin-1.2.5/tests/test_exclude.py` & `mkdocs_git_revision_date_localized_plugin-1.2.6/tests/test_exclude.py`

 * *Files identical despite different names*

