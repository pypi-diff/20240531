# Comparing `tmp/hab_gui-0.8.0.tar.gz` & `tmp/hab_gui-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hab_gui-0.8.0.tar", last modified: Thu Nov  2 22:22:57 2023, max compression
+gzip compressed data, was "hab_gui-0.9.0.tar", last modified: Tue Nov 14 03:09:47 2023, max compression
```

## Comparing `hab_gui-0.8.0.tar` & `hab_gui-0.9.0.tar`

### file list

```diff
@@ -1,56 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 22:22:57.975493 hab_gui-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2023-11-02 22:22:41.000000 hab_gui-0.8.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 22:22:57.967493 hab_gui-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 22:22:57.971493 hab_gui-0.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2023-11-02 22:22:41.000000 hab_gui-0.8.0/.github/ISSUE_TEMPLATE/BUG_REPORT.md
--rw-r--r--   0 runner    (1001) docker     (127)      559 2023-11-02 22:22:41.000000 hab_gui-0.8.0/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-11-02 22:22:41.000000 hab_gui-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 22:22:57.971493 hab_gui-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-11-02 22:22:41.000000 hab_gui-0.8.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2023-11-02 22:22:41.000000 hab_gui-0.8.0/.github/workflows/static-analysis-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2023-11-02 22:22:41.000000 hab_gui-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-11-02 22:22:41.000000 hab_gui-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-11-02 22:22:41.000000 hab_gui-0.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2023-11-02 22:22:41.000000 hab_gui-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-11-02 22:22:41.000000 hab_gui-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10082 2023-11-02 22:22:57.975493 hab_gui-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2023-11-02 22:22:41.000000 hab_gui-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 22:22:57.971493 hab_gui-0.8.0/hab_gui/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-02 22:22:41.000000 hab_gui-0.8.0/hab_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2023-11-02 22:22:41.000000 hab_gui-0.8.0/hab_gui/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 22:22:57.971493 hab_gui-0.8.0/hab_gui/entry_points/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2023-11-02 22:22:41.000000 hab_gui-0.8.0/hab_gui/entry_points/base_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2023-11-02 22:22:41.000000 hab_gui-0.8.0/hab_gui/entry_points/logging_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-11-02 22:22:41.000000 hab_gui-0.8.0/hab_gui/entry_points/message_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2023-11-02 22:22:41.000000 hab_gui-0.8.0/hab_gui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-02 22:22:57.000000 hab_gui-0.8.0/hab_gui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 22:22:57.971493 hab_gui-0.8.0/hab_gui/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-02 22:22:41.000000 hab_gui-0.8.0/hab_gui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-11-02 22:22:41.000000 hab_gui-0.8.0/hab_gui/widgets/alias_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2023-11-02 22:22:41.000000 hab_gui-0.8.0/hab_gui/widgets/alias_button_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2023-11-02 22:22:41.000000 hab_gui-0.8.0/hab_gui/widgets/alias_icon_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2023-11-02 22:22:41.000000 hab_gui-0.8.0/hab_gui/widgets/pinned_uris_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-11-02 22:22:41.000000 hab_gui-0.8.0/hab_gui/widgets/splash_screen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2023-11-02 22:22:41.000000 hab_gui-0.8.0/hab_gui/widgets/uri_combobox.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2023-11-02 22:22:41.000000 hab_gui-0.8.0/hab_gui/widgets/uri_line_edit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 22:22:57.971493 hab_gui-0.8.0/hab_gui/windows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-02 22:22:41.000000 hab_gui-0.8.0/hab_gui/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2023-11-02 22:22:41.000000 hab_gui-0.8.0/hab_gui/windows/alias_launch_window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 22:22:57.971493 hab_gui-0.8.0/hab_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10082 2023-11-02 22:22:57.000000 hab_gui-0.8.0/hab_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2023-11-02 22:22:57.000000 hab_gui-0.8.0/hab_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-02 22:22:57.000000 hab_gui-0.8.0/hab_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-02 22:22:57.000000 hab_gui-0.8.0/hab_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-02 22:22:57.000000 hab_gui-0.8.0/hab_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-02 22:22:57.000000 hab_gui-0.8.0/hab_gui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-11-02 22:22:41.000000 hab_gui-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2023-11-02 22:22:41.000000 hab_gui-0.8.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-02 22:22:41.000000 hab_gui-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-02 22:22:57.975493 hab_gui-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 22:22:57.975493 hab_gui-0.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 22:22:57.975493 hab_gui-0.8.0/tests/site/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2023-11-02 22:22:41.000000 hab_gui-0.8.0/tests/site/hab-gui-alt.json
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-11-02 22:22:41.000000 hab_gui-0.8.0/tests/site/hab-gui-init.json
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-11-02 22:22:41.000000 hab_gui-0.8.0/tests/site/hab-gui.json
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-02 22:22:41.000000 hab_gui-0.8.0/tests/test_echo_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2023-11-02 22:22:41.000000 hab_gui-0.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 03:09:47.653671 hab_gui-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2023-11-14 03:09:32.000000 hab_gui-0.9.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 03:09:47.645671 hab_gui-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 03:09:47.645671 hab_gui-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2023-11-14 03:09:32.000000 hab_gui-0.9.0/.github/ISSUE_TEMPLATE/BUG_REPORT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2023-11-14 03:09:32.000000 hab_gui-0.9.0/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-11-14 03:09:32.000000 hab_gui-0.9.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 03:09:47.645671 hab_gui-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-11-14 03:09:32.000000 hab_gui-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2023-11-14 03:09:32.000000 hab_gui-0.9.0/.github/workflows/static-analysis-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2023-11-14 03:09:32.000000 hab_gui-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2023-11-14 03:09:32.000000 hab_gui-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-11-14 03:09:32.000000 hab_gui-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2023-11-14 03:09:32.000000 hab_gui-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-11-14 03:09:32.000000 hab_gui-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2023-11-14 03:09:47.653671 hab_gui-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2023-11-14 03:09:32.000000 hab_gui-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 03:09:47.645671 hab_gui-0.9.0/hab_gui/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 03:09:47.649671 hab_gui-0.9.0/hab_gui/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/entry_points/base_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/entry_points/logging_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/entry_points/message_box.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 03:09:47.649671 hab_gui-0.9.0/hab_gui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/resources/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/resources/habihat-white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/resources/habihat.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/resources/menu.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/resources/pin-off-outline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/resources/pin-outline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/resources/refresh.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-14 03:09:47.000000 hab_gui-0.9.0/hab_gui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 03:09:47.649671 hab_gui-0.9.0/hab_gui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/widgets/alias_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/widgets/alias_button_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/widgets/alias_icon_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/widgets/menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/widgets/pinned_uris_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/widgets/refresh_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/widgets/splash_screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/widgets/uri_combobox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/widgets/uri_line_edit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 03:09:47.649671 hab_gui-0.9.0/hab_gui/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2023-11-14 03:09:32.000000 hab_gui-0.9.0/hab_gui/windows/alias_launch_window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 03:09:47.649671 hab_gui-0.9.0/hab_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2023-11-14 03:09:47.000000 hab_gui-0.9.0/hab_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2023-11-14 03:09:47.000000 hab_gui-0.9.0/hab_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 03:09:47.000000 hab_gui-0.9.0/hab_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-14 03:09:47.000000 hab_gui-0.9.0/hab_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-14 03:09:47.000000 hab_gui-0.9.0/hab_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-14 03:09:47.000000 hab_gui-0.9.0/hab_gui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-11-14 03:09:32.000000 hab_gui-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2023-11-14 03:09:32.000000 hab_gui-0.9.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-14 03:09:32.000000 hab_gui-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 03:09:47.653671 hab_gui-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 03:09:47.649671 hab_gui-0.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 03:09:47.653671 hab_gui-0.9.0/tests/site/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2023-11-14 03:09:32.000000 hab_gui-0.9.0/tests/site/hab-gui-alt.json
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2023-11-14 03:09:32.000000 hab_gui-0.9.0/tests/site/hab-gui-init.json
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2023-11-14 03:09:32.000000 hab_gui-0.9.0/tests/site/hab-gui.json
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2023-11-14 03:09:32.000000 hab_gui-0.9.0/tests/test_echo_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2023-11-14 03:09:32.000000 hab_gui-0.9.0/tox.ini
```

### Comparing `hab_gui-0.8.0/.github/ISSUE_TEMPLATE/BUG_REPORT.md` & `hab_gui-0.9.0/.github/ISSUE_TEMPLATE/BUG_REPORT.md`

 * *Files identical despite different names*

### Comparing `hab_gui-0.8.0/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md` & `hab_gui-0.9.0/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md`

 * *Files identical despite different names*

### Comparing `hab_gui-0.8.0/.github/PULL_REQUEST_TEMPLATE.md` & `hab_gui-0.9.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `hab_gui-0.8.0/.github/workflows/release.yml` & `hab_gui-0.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hab_gui-0.8.0/.github/workflows/static-analysis-and-test.yml` & `hab_gui-0.9.0/.github/workflows/static-analysis-and-test.yml`

 * *Files identical despite different names*

### Comparing `hab_gui-0.8.0/.gitignore` & `hab_gui-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hab_gui-0.8.0/.pre-commit-config.yaml` & `hab_gui-0.9.0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,14 @@
     hooks:
     -   id: flake8
         additional_dependencies:
             - flake8-bugbear==22.12.6
             - Flake8-pyproject
             - pep8-naming==0.13.3
 
--   repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v2.2.0
-    hooks:
-    -   id: setup-cfg-fmt
-        args: [--min-py3-version=3.6]
-
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-json
       - id: check-toml
       - id: check-xml
       - id: check-yaml
```

### Comparing `hab_gui-0.8.0/CODE_OF_CONDUCT.md` & `hab_gui-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hab_gui-0.8.0/CONTRIBUTING.md` & `hab_gui-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hab_gui-0.8.0/LICENSE` & `hab_gui-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hab_gui-0.8.0/PKG-INFO` & `hab_gui-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hab_gui
-Version: 0.8.0
+Version: 0.9.0
 Summary: GUI for user interaction to Hab.
 Author-email: Blur Studio <opensource@blur.com>
 License: LGPL-3.0
 Project-URL: Homepage, https://github.com/blurstudio/hab-gui
 Project-URL: Source, https://github.com/blurstudio/hab-gui
 Project-URL: Tracker, https://github.com/blurstudio/hab-gui/issues
 Platform: any
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: hab>=0.22.0
+Requires-Dist: hab>=0.27.0
 Requires-Dist: Qt.py
 Provides-Extra: dev
 Requires-Dist: black==22.12.0; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: covdefaults; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8==5.0.4; extra == "dev"
@@ -212,7 +212,20 @@
     "prepend": {
         "splash_screen": [
             "Path(s)/To/Images"
         ]
     }
 }
 ```
+
+## Auto Refresh
+
+Users are likely to keep the hab launcher open for long periods of time and this
+may lead to them using out of date configuration settings. Hab Launcher has a
+refresh button to let users manually force a refresh. Note that this does not
+refresh the site configuration, configs and distros.
+
+By default it will automatically refresh every 30 minutes(`00:30:00`). You can
+configure this interval by setting `hab_gui_refresh_inverval` in your site
+configuration. This accepts a string in `%H:%M:%S` format using
+[time.strptime](https://docs.python.org/3/library/time.html#time.strptime). An
+empty string will disable this auto-refresh feature.
```

### Comparing `hab_gui-0.8.0/README.md` & `hab_gui-0.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -170,7 +170,20 @@
     "prepend": {
         "splash_screen": [
             "Path(s)/To/Images"
         ]
     }
 }
 ```
+
+## Auto Refresh
+
+Users are likely to keep the hab launcher open for long periods of time and this
+may lead to them using out of date configuration settings. Hab Launcher has a
+refresh button to let users manually force a refresh. Note that this does not
+refresh the site configuration, configs and distros.
+
+By default it will automatically refresh every 30 minutes(`00:30:00`). You can
+configure this interval by setting `hab_gui_refresh_inverval` in your site
+configuration. This accepts a string in `%H:%M:%S` format using
+[time.strptime](https://docs.python.org/3/library/time.html#time.strptime). An
+empty string will disable this auto-refresh feature.
```

### Comparing `hab_gui-0.8.0/hab_gui/cli.py` & `hab_gui-0.9.0/hab_gui/cli.py`

 * *Files identical despite different names*

### Comparing `hab_gui-0.8.0/hab_gui/entry_points/logging_exception.py` & `hab_gui-0.9.0/hab_gui/entry_points/logging_exception.py`

 * *Files identical despite different names*

### Comparing `hab_gui-0.8.0/hab_gui/entry_points/message_box.py` & `hab_gui-0.9.0/hab_gui/entry_points/message_box.py`

 * *Files identical despite different names*

### Comparing `hab_gui-0.8.0/hab_gui/widgets/alias_button.py` & `hab_gui-0.9.0/hab_gui/widgets/alias_button.py`

 * *Files identical despite different names*

### Comparing `hab_gui-0.8.0/hab_gui/widgets/alias_button_grid.py` & `hab_gui-0.9.0/hab_gui/widgets/alias_button_grid.py`

 * *Files identical despite different names*

### Comparing `hab_gui-0.8.0/hab_gui/widgets/alias_icon_button.py` & `hab_gui-0.9.0/hab_gui/widgets/alias_icon_button.py`

 * *Files identical despite different names*

### Comparing `hab_gui-0.8.0/hab_gui/widgets/pinned_uris_button.py` & `hab_gui-0.9.0/hab_gui/widgets/pinned_uris_button.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 
 from Qt import QtWidgets
 
+from .. import utils
+
 logger = logging.getLogger(__name__)
 
 
 class PinnedUriButton(QtWidgets.QToolButton):
     """A widget that gives users quick access to URI's used regularly. When the
     user clicks on this tool button, it opens a menu allowing the user to choose
     from previously saved URI's or add/remove a URI to saved user_prefs.
@@ -14,26 +16,27 @@
         resolver (hab.Resolver): The resolver used for settings.
         uri_widget (QWidget): The URIComboBox like widget used to get/set the
             current URI from.
         verbosity (int): Pass along a verbosity value for filtering of URIs
         parent (Qt.QtWidgets.QWidget, optional): Define a parent for this widget.
     """
 
-    _push_pin = "\U0001F4CC"
-    _text_pin_selected = f"{_push_pin} Pin selected URI"
-    _text_remove_uri = "\u274C Remove pin"
+    _text_main = "\U0001F4CC"
+    _text_pin_selected = "Pin selected URI"
+    _text_remove_uri = "Remove pin"
 
     def __init__(self, resolver, uri_widget, verbosity=0, parent=None):
         super().__init__(parent)
         self.resolver = resolver
         self.uri_widget = uri_widget
         self.verbosity = verbosity
 
         self.setToolTip("Select and manage quick access to commonly used URI's.")
-        self.setText(self._push_pin)
+        self.setText(self._text_main)
+        self.setIcon(utils.Paths.icon("pin-outline.svg"))
         self.setPopupMode(self.InstantPopup)
         self.refresh()
 
     def add_uri(self, uri):
         """Add this uri to `self.uris()` and save that change to user_prefs."""
         uris = self.uris()
         uris.add(uri)
@@ -61,16 +64,18 @@
     def refresh(self):
         """Rebuilds the menu shown when a user clicks on the button."""
         menu = QtWidgets.QMenu(self)
         menu.triggered.connect(self.menu_triggered)
 
         # Add management actions and menus
         act = menu.addAction(self._text_pin_selected)
+        act.setIcon(utils.Paths.icon("pin-outline.svg"))
         act.setData("pin")
         remove_menu = menu.addMenu(self._text_remove_uri)
+        remove_menu.setIcon(utils.Paths.icon("pin-off-outline.svg"))
         menu.addSeparator()
 
         # Add existing pinned URI's to both menus
         for uri in sorted(self.uris(), key=str.casefold):
             # Selects this URI in self.uri_widget
             act = menu.addAction(uri)
             act.setData("choose")
```

### Comparing `hab_gui-0.8.0/hab_gui/widgets/splash_screen.py` & `hab_gui-0.9.0/hab_gui/widgets/splash_screen.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from PyQt5 import QtGui, QtWidgets
+from Qt import QtGui, QtWidgets
 
 
 class SplashScreen(QtWidgets.QSplashScreen):
     """A widget that provides a QSplashScreen that can be used for long
     load times.  This subclass can use both static and animated images.
 
     Args:
```

### Comparing `hab_gui-0.8.0/hab_gui/widgets/uri_combobox.py` & `hab_gui-0.9.0/hab_gui/widgets/uri_combobox.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,20 +25,22 @@
 
         self.currentTextChanged.connect(self._emit_uri_changed)
 
     def _emit_uri_changed(self):
         self.uri_changed.emit(self.uri())
 
     def refresh(self):
+        current = self.uri()
         self.clear()
         if self.uri is None:
             return
         with hab.utils.verbosity_filter(self.resolver, self.verbosity):
             items = self.resolver.dump_forest(self.resolver.configs, indent="")
             self.addItems(items)
+        self.set_uri(current)
 
     def uri(self):
         return self.currentText()
 
     def set_uri(self, uri):
         # If the uri is already an item in the combo box, select it
         index = self.findText(uri)
```

### Comparing `hab_gui-0.8.0/hab_gui/widgets/uri_line_edit.py` & `hab_gui-0.9.0/hab_gui/widgets/uri_line_edit.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,12 +19,16 @@
 
         self.setPlaceholderText("Enter a URI...")
         self.textChanged.connect(self._emit_uri_changed)
 
     def _emit_uri_changed(self):
         self.uri_changed.emit(self.uri())
 
+    def refresh(self):
+        # Nothing to refresh on this widget
+        pass
+
     def uri(self):
         return self.text()
 
     def set_uri(self, uri):
         self.setText(uri)
```

### Comparing `hab_gui-0.8.0/hab_gui/windows/alias_launch_window.py` & `hab_gui-0.9.0/hab_gui/windows/alias_launch_window.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,15 @@
+import logging
+
 import hab
-from Qt import QtWidgets
+from Qt import QtCore, QtWidgets
+
+from .. import utils
+
+logger = logging.getLogger(__name__)
 
 
 class AliasLaunchWindow(QtWidgets.QMainWindow):
     """Create a window that can launch applications relevant to a project URI
 
     Contains a custom QComboBox (URIComboBox) and a QGridlayout (AliasButtonGrid)
     The ComboBox is populated with a list of available URIs. The GridLayout is
@@ -26,28 +32,57 @@
         resolver,
         uri=None,
         verbosity=0,
         button_wrap_length=3,
         button_layout=0,
         parent=None,
     ):
-        super(AliasLaunchWindow, self).__init__(parent)
+        super().__init__(parent)
         self.resolver = resolver
         self.verbosity = verbosity
         self.button_wrap_length = button_wrap_length
         self.button_layout = button_layout
 
         self.process_entry_points()
         self.init_gui(uri)
 
         # Window properties
         self.setWindowTitle("Hab Launch Aliases")
         self.setFixedWidth(400)
         self.center_window_position()
 
+        # Create a auto-refresh timer by default that forces a refresh of hab.
+        # This can be disabled by setting the site config setting to an empty string.
+        self.refresh_timer = QtCore.QTimer(self)
+        refresh_time = self.resolver.site.get("hab_gui_refresh_inverval", ["00:30:00"])
+        refresh_time = refresh_time[0]
+        if refresh_time:
+            self.refresh_timer.timeout.connect(self.refresh_cache)
+            refresh_time = utils.interval(refresh_time)
+            logger.debug(f"Setting auto-refresh interval to {refresh_time} seconds")
+            self.refresh_timer.start(refresh_time * 1000)
+
+    def apply_layout(self):
+        """Configures the layout of all widgets in this interface."""
+        column_uri_widget = 1 if self.prefs_enabled else 0
+        self.setCentralWidget(self.main_widget)
+        self.layout.addWidget(self.uri_widget, 0, column_uri_widget)
+        self.layout.addWidget(self.menu_button, 0, column_uri_widget + 1)
+        self.layout.addWidget(self.alias_buttons, 1, 0, 1, -1)
+        self.main_widget.setLayout(self.layout)
+
+        # Ensure the tab order is intuitive. This doesn't come for free because
+        # we need to pass uri_widget as an argument to pinned_uris which requires
+        # creating it first and that breaks the default tab ordering.
+        if self.prefs_enabled:
+            self.setTabOrder(self.pinned_uris, self.uri_widget)
+            self.setTabOrder(self.uri_widget, self.menu_button)
+            self.setTabOrder(self.menu_button, self.alias_buttons)
+            self.setTabOrder(self.alias_buttons, self.pinned_uris)
+
     def closeEvent(self, event):  # noqa: N802
         """Saves the currently selected URI on close if prefs are enabled."""
         self.resolver.user_prefs().uri = self.uri_widget.uri()
         super().closeEvent(event)
 
     def load_entry_point(self, name, default, allow_none=False):
         """Work function that loads the requested entry_point."""
@@ -69,80 +104,88 @@
             "hab_gui_alias_widget", "hab_gui.widgets.alias_icon_button:AliasIconButton"
         )
         # Used to display alias launch widgets
         self._cls_aliases_widget = self.load_entry_point(
             "hab_gui_aliases_widget",
             "hab_gui.widgets.alias_button_grid:AliasButtonGrid",
         )
+        # Allows the user to refresh hab configuration in case it has changed.
+        self._cls_menu_button = self.load_entry_point(
+            "hab_gui_menu_button",
+            "hab_gui.widgets.menu_button:MenuButton",
+        )
         # Allows the user to pin commonly used URI's
         self._cls_uri_pin_widget = self.load_entry_point(
             "hab_gui_uri_pin_widget",
             "hab_gui.widgets.pinned_uris_button:PinnedUriButton",
             allow_none=True,
         )
         # Interface the user uses to view and change the current URI.
         self._cls_uri_widget = self.load_entry_point(
             "hab_gui_uri_widget", "hab_gui.widgets.uri_combobox:URIComboBox"
         )
 
     def init_gui(self, uri=None):
-        self.window = QtWidgets.QWidget()
+        self.setWindowIcon(utils.Paths.icon("habihat.svg"))
+
+        self.main_widget = QtWidgets.QWidget()
         self.layout = QtWidgets.QGridLayout()
 
         self.uri_widget = self._cls_uri_widget(
             self.resolver, verbosity=self.verbosity, parent=self
         )
 
         # If prefs are enabled, insert the Pinned URI widget
-        column_uri_widget = 0
-        prefs_enabled = self.resolver.user_prefs().enabled
+        self.prefs_enabled = self.resolver.user_prefs().enabled
         if self._cls_uri_pin_widget is None:
             # The pinning widget can be disabled by setting the entry point to null
-            prefs_enabled = False
+            self.prefs_enabled = False
+
+        # Create a refresh button
+        self.menu_button = self._cls_menu_button(
+            self.resolver, verbosity=self.verbosity, hab_widget=self
+        )
 
-        if prefs_enabled:
+        if self.prefs_enabled:
             self.pinned_uris = self._cls_uri_pin_widget(
                 self.resolver, self.uri_widget, verbosity=self.verbosity, parent=self
             )
             self.layout.addWidget(self.pinned_uris, 0, 0)
-            column_uri_widget = 1
             self.pinned_uris.uri_widget = self.uri_widget
 
         self.alias_buttons = self._cls_aliases_widget(
             self.resolver,
             self.button_wrap_length,
             self.button_layout,
             self.verbosity,
             button_cls=self._cls_alias_widget,
             parent=self,
         )
 
-        self.setCentralWidget(self.window)
-        self.layout.addWidget(self.uri_widget, 0, column_uri_widget)
+        self.apply_layout()
+
+        # Connect signals
         self.uri_widget.uri_changed.connect(self.uri_changed)
-        self.layout.addWidget(self.alias_buttons, 1, 0, 1, -1)
-        self.window.setLayout(self.layout)
 
         # Check for stored URI and apply it as the current text
         if uri is None:
             uri = str(self.resolver.user_prefs().uri_check())
         if uri:
             self.uri_widget.set_uri(uri)
             self.uri_changed(uri)
 
         # Ensure the URI widget has focus by default
         self.uri_widget.setFocus()
 
-        # Ensure the tab order is intuitive. This doesn't come for free because
-        # we need to pass uri_widget as an argument to pinned_uris which requires
-        # creating it first and that breaks the default tab ordering.
-        if prefs_enabled:
-            self.setTabOrder(self.pinned_uris, self.uri_widget)
-            self.setTabOrder(self.uri_widget, self.alias_buttons)
-            self.setTabOrder(self.alias_buttons, self.pinned_uris)
+    @utils.cursor_override()
+    def refresh_cache(self):
+        logger.debug("Refresh cache")
+        self.uri_widget.refresh()
+        self.resolver.clear_caches()
+        self.alias_buttons.refresh()
 
     def uri_changed(self, uri):
         self.alias_buttons.uri = uri
         self.alias_buttons.refresh()
 
     def center_window_position(self):
         # Place window onto screen center
```

### Comparing `hab_gui-0.8.0/hab_gui.egg-info/PKG-INFO` & `hab_gui-0.9.0/hab_gui.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hab-gui
-Version: 0.8.0
+Version: 0.9.0
 Summary: GUI for user interaction to Hab.
 Author-email: Blur Studio <opensource@blur.com>
 License: LGPL-3.0
 Project-URL: Homepage, https://github.com/blurstudio/hab-gui
 Project-URL: Source, https://github.com/blurstudio/hab-gui
 Project-URL: Tracker, https://github.com/blurstudio/hab-gui/issues
 Platform: any
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: hab>=0.22.0
+Requires-Dist: hab>=0.27.0
 Requires-Dist: Qt.py
 Provides-Extra: dev
 Requires-Dist: black==22.12.0; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: covdefaults; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8==5.0.4; extra == "dev"
@@ -212,7 +212,20 @@
     "prepend": {
         "splash_screen": [
             "Path(s)/To/Images"
         ]
     }
 }
 ```
+
+## Auto Refresh
+
+Users are likely to keep the hab launcher open for long periods of time and this
+may lead to them using out of date configuration settings. Hab Launcher has a
+refresh button to let users manually force a refresh. Note that this does not
+refresh the site configuration, configs and distros.
+
+By default it will automatically refresh every 30 minutes(`00:30:00`). You can
+configure this interval by setting `hab_gui_refresh_inverval` in your site
+configuration. This accepts a string in `%H:%M:%S` format using
+[time.strptime](https://docs.python.org/3/library/time.html#time.strptime). An
+empty string will disable this auto-refresh feature.
```

### Comparing `hab_gui-0.8.0/hab_gui.egg-info/SOURCES.txt` & `hab_gui-0.9.0/hab_gui.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,19 +23,28 @@
 hab_gui.egg-info/dependency_links.txt
 hab_gui.egg-info/entry_points.txt
 hab_gui.egg-info/requires.txt
 hab_gui.egg-info/top_level.txt
 hab_gui/entry_points/base_init.py
 hab_gui/entry_points/logging_exception.py
 hab_gui/entry_points/message_box.py
+hab_gui/resources/README.md
+hab_gui/resources/habihat-white.svg
+hab_gui/resources/habihat.svg
+hab_gui/resources/menu.svg
+hab_gui/resources/pin-off-outline.svg
+hab_gui/resources/pin-outline.svg
+hab_gui/resources/refresh.svg
 hab_gui/widgets/__init__.py
 hab_gui/widgets/alias_button.py
 hab_gui/widgets/alias_button_grid.py
 hab_gui/widgets/alias_icon_button.py
+hab_gui/widgets/menu_button.py
 hab_gui/widgets/pinned_uris_button.py
+hab_gui/widgets/refresh_button.py
 hab_gui/widgets/splash_screen.py
 hab_gui/widgets/uri_combobox.py
 hab_gui/widgets/uri_line_edit.py
 hab_gui/windows/__init__.py
 hab_gui/windows/alias_launch_window.py
 tests/test_echo_message.py
 tests/site/hab-gui-alt.json
```

### Comparing `hab_gui-0.8.0/pyproject.toml` & `hab_gui-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 requires-python = ">=3.6"
 dependencies = [
-    "hab>=0.22.0",
+    "hab>=0.27.0",
     "Qt.py",
     ]
 
 # TODO We need to address how to handle PyQT and PySide installs for development
 
 dynamic = ["version"]
```

### Comparing `hab_gui-0.8.0/tests/site/hab-gui-alt.json` & `hab_gui-0.9.0/tests/site/hab-gui-alt.json`

 * *Files identical despite different names*

### Comparing `hab_gui-0.8.0/tox.ini` & `hab_gui-0.9.0/tox.ini`

 * *Files identical despite different names*

