# Comparing `tmp/hokusai-2.1.1.tar.gz` & `tmp/hokusai-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hokusai-2.1.1.tar", max compression
+gzip compressed data, was "hokusai-2.2.0.tar", max compression
```

## Comparing `hokusai-2.1.1.tar` & `hokusai-2.2.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     1068 2024-01-12 14:21:51.221443 hokusai-2.1.1/LICENSE.txt
--rw-r--r--   0        0        0    10621 2024-01-12 14:21:51.221443 hokusai-2.1.1/README.md
--rw-r--r--   0        0        0        6 2024-01-12 14:21:51.225443 hokusai-2.1.1/hokusai/RELEASE_VERSION
--rw-r--r--   0        0        0        6 2024-01-12 14:22:32.873800 hokusai-2.1.1/hokusai/VERSION
--rw-r--r--   0        0        0       96 2024-01-12 14:21:51.225443 hokusai-2.1.1/hokusai/__init__.py
--rw-r--r--   0        0        0      282 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/cli/__init__.py
--rw-r--r--   0        0        0     4644 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/cli/base.py
--rw-r--r--   0        0        0     4090 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/cli/dev.py
--rw-r--r--   0        0        0     3080 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/cli/pipeline.py
--rw-r--r--   0        0        0     9088 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/cli/production.py
--rw-r--r--   0        0        0     3608 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/cli/registry.py
--rw-r--r--   0        0        0    10427 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/cli/review_app.py
--rw-r--r--   0        0        0     9006 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/cli/staging.py
--rw-r--r--   0        0        0      210 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/command_line.py
--rw-r--r--   0        0        0     1117 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/__init__.py
--rw-r--r--   0        0        0      112 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/build.py
--rw-r--r--   0        0        0     3241 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/check.py
--rw-r--r--   0        0        0     1578 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/command_tree.py
--rw-r--r--   0        0        0     1979 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/configure.py
--rw-r--r--   0        0        0     1759 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/deployment.py
--rw-r--r--   0        0        0     4045 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/development.py
--rw-r--r--   0        0        0     1195 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/env.py
--rw-r--r--   0        0        0      717 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/gitcompare.py
--rw-r--r--   0        0        0      774 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/gitdiff.py
--rw-r--r--   0        0        0      797 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/gitlog.py
--rw-r--r--   0        0        0     1860 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/images.py
--rw-r--r--   0        0        0     5349 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/kubernetes.py
--rw-r--r--   0        0        0     1270 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/logs.py
--rw-r--r--   0        0        0     1908 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/namespace.py
--rw-r--r--   0        0        0      769 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/pull.py
--rw-r--r--   0        0        0     2805 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/push.py
--rw-r--r--   0        0        0      622 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/retag.py
--rw-r--r--   0        0        0      270 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/run.py
--rw-r--r--   0        0        0     3925 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/setup.py
--rw-r--r--   0        0        0     1924 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/test.py
--rw-r--r--   0        0        0      129 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/commands/version.py
--rw-r--r--   0        0        0        0 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/lib/__init__.py
--rw-r--r--   0        0        0      968 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/lib/command.py
--rw-r--r--   0        0        0     7156 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/lib/common.py
--rw-r--r--   0        0        0     4840 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/lib/config.py
--rw-r--r--   0        0        0     1011 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/lib/config_loader.py
--rw-r--r--   0        0        0       22 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/lib/constants.py
--rw-r--r--   0        0        0     1044 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/lib/docker_compose_helpers.py
--rw-r--r--   0        0        0      911 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/lib/environment.py
--rw-r--r--   0        0        0      182 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/lib/exceptions.py
--rw-r--r--   0        0        0     1941 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/lib/global_config.py
--rw-r--r--   0        0        0     1200 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/lib/representers.py
--rw-r--r--   0        0        0      873 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/lib/template_renderer.py
--rw-r--r--   0        0        0      660 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/lib/template_selector.py
--rw-r--r--   0        0        0        0 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/services/__init__.py
--rw-r--r--   0        0        0     4554 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/services/command_runner.py
--rw-r--r--   0        0        0     1861 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/services/configmap.py
--rw-r--r--   0        0        0    11054 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/services/deployment.py
--rw-r--r--   0        0        0     1273 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/services/docker.py
--rw-r--r--   0        0        0     5075 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/services/ecr.py
--rw-r--r--   0        0        0     1490 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/services/kubectl.py
--rw-r--r--   0        0        0      856 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/services/s3.py
--rw-r--r--   0        0        0     1856 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/services/yaml_spec.py
--rw-r--r--   0        0        0      136 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/templates/.dockerignore.j2
--rw-r--r--   0        0        0      313 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/templates/Dockerfile.j2
--rw-r--r--   0        0        0       80 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/templates/hokusai/build.yml.j2
--rw-r--r--   0        0        0      144 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/templates/hokusai/development.yml.j2
--rw-r--r--   0        0        0     1193 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/templates/hokusai/production.yml.j2
--rw-r--r--   0        0        0     1190 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/templates/hokusai/staging.yml.j2
--rw-r--r--   0        0        0      152 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/templates/hokusai/test.yml.j2
--rw-r--r--   0        0        0      132 2024-01-12 14:21:51.229443 hokusai-2.1.1/hokusai/version.py
--rw-r--r--   0        0        0     1040 2024-01-12 14:22:32.877800 hokusai-2.1.1/pyproject.toml
--rw-r--r--   0        0        0    11996 1970-01-01 00:00:00.000000 hokusai-2.1.1/setup.py
--rw-r--r--   0        0        0    11530 1970-01-01 00:00:00.000000 hokusai-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-31 15:00:38.008792 hokusai-2.2.0/LICENSE.txt
+-rw-r--r--   0        0        0    10655 2024-05-31 15:00:38.008792 hokusai-2.2.0/README.md
+-rw-r--r--   0        0        0        6 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/RELEASE_VERSION
+-rw-r--r--   0        0        0        6 2024-05-31 15:01:20.969121 hokusai-2.2.0/hokusai/VERSION
+-rw-r--r--   0        0        0       96 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/__init__.py
+-rw-r--r--   0        0        0      282 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/cli/__init__.py
+-rw-r--r--   0        0        0     4644 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/cli/base.py
+-rw-r--r--   0        0        0     4090 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/cli/dev.py
+-rw-r--r--   0        0        0     3080 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/cli/pipeline.py
+-rw-r--r--   0        0        0     9088 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/cli/production.py
+-rw-r--r--   0        0        0     3608 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/cli/registry.py
+-rw-r--r--   0        0        0    10562 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/cli/review_app.py
+-rw-r--r--   0        0        0     9006 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/cli/staging.py
+-rw-r--r--   0        0        0      210 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/command_line.py
+-rw-r--r--   0        0        0     1117 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/build.py
+-rw-r--r--   0        0        0     3241 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/check.py
+-rw-r--r--   0        0        0     1578 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/command_tree.py
+-rw-r--r--   0        0        0     1979 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/configure.py
+-rw-r--r--   0        0        0     1806 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/deployment.py
+-rw-r--r--   0        0        0     4045 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/development.py
+-rw-r--r--   0        0        0     1195 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/env.py
+-rw-r--r--   0        0        0      717 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/gitcompare.py
+-rw-r--r--   0        0        0      774 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/gitdiff.py
+-rw-r--r--   0        0        0      797 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/gitlog.py
+-rw-r--r--   0        0        0     1860 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/images.py
+-rw-r--r--   0        0        0     5539 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/kubernetes.py
+-rw-r--r--   0        0        0     1270 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/logs.py
+-rw-r--r--   0        0        0     1908 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/namespace.py
+-rw-r--r--   0        0        0      769 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/pull.py
+-rw-r--r--   0        0        0     2805 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/push.py
+-rw-r--r--   0        0        0      622 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/retag.py
+-rw-r--r--   0        0        0      270 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/run.py
+-rw-r--r--   0        0        0     3925 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/setup.py
+-rw-r--r--   0        0        0     1924 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/test.py
+-rw-r--r--   0        0        0      129 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/commands/version.py
+-rw-r--r--   0        0        0        0 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/lib/__init__.py
+-rw-r--r--   0        0        0      968 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/lib/command.py
+-rw-r--r--   0        0        0     7349 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/lib/common.py
+-rw-r--r--   0        0        0     4840 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/lib/config.py
+-rw-r--r--   0        0        0     1011 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/lib/config_loader.py
+-rw-r--r--   0        0        0       22 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/lib/constants.py
+-rw-r--r--   0        0        0     1044 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/lib/docker_compose_helpers.py
+-rw-r--r--   0        0        0      911 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/lib/environment.py
+-rw-r--r--   0        0        0      182 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/lib/exceptions.py
+-rw-r--r--   0        0        0     1941 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/lib/global_config.py
+-rw-r--r--   0        0        0     1200 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/lib/representers.py
+-rw-r--r--   0        0        0      873 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/lib/template_renderer.py
+-rw-r--r--   0        0        0      660 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/lib/template_selector.py
+-rw-r--r--   0        0        0        0 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/services/__init__.py
+-rw-r--r--   0        0        0     4554 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/services/command_runner.py
+-rw-r--r--   0        0        0     1861 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/services/configmap.py
+-rw-r--r--   0        0        0    11129 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/services/deployment.py
+-rw-r--r--   0        0        0     1273 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/services/docker.py
+-rw-r--r--   0        0        0     5075 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/services/ecr.py
+-rw-r--r--   0        0        0     1489 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/services/kubectl.py
+-rw-r--r--   0        0        0      856 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/services/s3.py
+-rw-r--r--   0        0        0     2109 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/services/yaml_spec.py
+-rw-r--r--   0        0        0      136 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/templates/.dockerignore.j2
+-rw-r--r--   0        0        0      313 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/templates/Dockerfile.j2
+-rw-r--r--   0        0        0       80 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/templates/hokusai/build.yml.j2
+-rw-r--r--   0        0        0      144 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/templates/hokusai/development.yml.j2
+-rw-r--r--   0        0        0     1409 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/templates/hokusai/production.yml.j2
+-rw-r--r--   0        0        0     1406 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/templates/hokusai/staging.yml.j2
+-rw-r--r--   0        0        0      152 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/templates/hokusai/test.yml.j2
+-rw-r--r--   0        0        0      132 2024-05-31 15:00:38.016792 hokusai-2.2.0/hokusai/version.py
+-rw-r--r--   0        0        0     1078 2024-05-31 15:01:20.969121 hokusai-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0    12036 1970-01-01 00:00:00.000000 hokusai-2.2.0/setup.py
+-rw-r--r--   0        0        0    11571 1970-01-01 00:00:00.000000 hokusai-2.2.0/PKG-INFO
```

### Comparing `hokusai-2.1.1/LICENSE.txt` & `hokusai-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/README.md` & `hokusai-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -131,38 +131,36 @@
 echo 'export LDFLAGS="-L/usr/local/opt/openssl@1.1/lib"' >> ~/.bash_profile
 echo 'export CPPFLAGS="-I/usr/local/opt/openssl@1.1/include"' >> ~/.bash_profile
 echo 'export PKG_CONFIG_PATH="/usr/local/opt/openssl@1.1/lib/pkgconfig"' >> ~/.bash_profile
 ```
 
 ### Python
 
-Hokusai is currently tested on Python 3.9.10 so we recommend using that Python version.
+Hokusai is currently tested on Python 3.10 so we recommend using that Python version.
 
 If you use Pyenv to install Python, you should see an output similar to this:
 
 ```
-pyenv install 3.9.10
-
-    python-build: use openssl from homebrew
-    python-build: use readline from homebrew
-
-    Downloading Python-3.9.10.tar.xz...
-    -> https://www.python.org/ftp/python/3.9.10/Python-3.9.10.tar.xz
-    Installing Python-3.9.10...
-    python-build: use tcl-tk from homebrew
-    python-build: use readline from homebrew
-    python-build: use zlib from xcode sdk
-
-    Installed Python-3.9.10 to $HOME/.pyenv/versions/3.9.10
+$ pyenv install 3.10
+python-build: use openssl@1.1 from homebrew
+python-build: use readline from homebrew
+Downloading Python-3.10.13.tar.xz...
+-> https://www.python.org/ftp/python/3.10.13/Python-3.10.13.tar.xz
+Installing Python-3.10.13...
+python-build: use tcl-tk from homebrew
+python-build: use readline from homebrew
+python-build: use ncurses from homebrew
+python-build: use zlib from xcode sdk
+Installed Python-3.10.13 to /Users/jxu/.pyenv/versions/3.10.13
 ```
 
 With the desired Python version installed, activate it globally:
 
 ```
-pyenv global 3.9.10
+pyenv global 3.10
 ```
 
 Note: If you want to create a PyInstaller distribution, Python must be installed with development libraries. Use the environment variable `PYTHON_CONFIGURE_OPTS="--enable-framework"` on Darwin and `PYTHON_CONFIGURE_OPTS="--enable-shared"` on Linux when running `pyenv install`.
 
 ### Virtualenv
 
 We recommend using a virtual environment to isolate Hokusai's dependencies from that of other projects on your local environment.
@@ -172,14 +170,15 @@
 ### Poetry
 
 Use [Poetry](https://python-poetry.org/) to install Hokusai's dependencies as well as Hokusai itself in [editable mode](https://pip-python3.readthedocs.io/en/latest/reference/pip_install.html#editable-installs). Please see [this guide](https://python-poetry.org/docs/basic-usage/) for working with Poetry.
 
 Install Poetry:
 
 ```
+pip install --upgrade pip
 pip install poetry
 ```
 
 Install dependencies and Hokusai in editable mode:
 
 ```
 poetry install
@@ -200,24 +199,24 @@
 ```
 brew install minikube
 minikube start --kubernetes-version=<version of your Kubernetes clusters, example: v1.2.3>
 ```
 
 ### Run tests
 
-To run unit and smoke tests:
+To run unit tests:
 
 ```
 make test
 ```
 
 To run integration tests:
 
 ```
-make integration
+make integration-local
 ```
 
 Only specific modules, TestClasses, or even methods:
 
 ```
 python -m unittest test.unit.test_module.TestClass.test_method
 ```
```

#### html2text {}

```diff
@@ -61,59 +61,60 @@
 use brew-installed `openssl` and `readline` libraries, and xcode-installed
 `zlib` library. And make sure these libraries are correctly linked. Like so:
 ``` brew install openssl readline zlib echo 'export PATH="/usr/local/opt/
 openssl@1.1/bin:$PATH"' >> ~/.bash_profile echo 'export LDFLAGS="-L/usr/local/
 opt/openssl@1.1/lib"' >> ~/.bash_profile echo 'export CPPFLAGS="-I/usr/local/
 opt/openssl@1.1/include"' >> ~/.bash_profile echo 'export PKG_CONFIG_PATH="/
 usr/local/opt/openssl@1.1/lib/pkgconfig"' >> ~/.bash_profile ``` ### Python
-Hokusai is currently tested on Python 3.9.10 so we recommend using that Python
+Hokusai is currently tested on Python 3.10 so we recommend using that Python
 version. If you use Pyenv to install Python, you should see an output similar
-to this: ``` pyenv install 3.9.10 python-build: use openssl from homebrew
-python-build: use readline from homebrew Downloading Python-3.9.10.tar.xz... -
-> https://www.python.org/ftp/python/3.9.10/Python-3.9.10.tar.xz Installing
-Python-3.9.10... python-build: use tcl-tk from homebrew python-build: use
-readline from homebrew python-build: use zlib from xcode sdk Installed Python-
-3.9.10 to $HOME/.pyenv/versions/3.9.10 ``` With the desired Python version
-installed, activate it globally: ``` pyenv global 3.9.10 ``` Note: If you want
-to create a PyInstaller distribution, Python must be installed with development
-libraries. Use the environment variable `PYTHON_CONFIGURE_OPTS="--enable-
-framework"` on Darwin and `PYTHON_CONFIGURE_OPTS="--enable-shared"` on Linux
-when running `pyenv install`. ### Virtualenv We recommend using a virtual
-environment to isolate Hokusai's dependencies from that of other projects on
-your local environment. The Pyenv install comes with [pyenv-virtualenv](https:/
-/github.com/pyenv/pyenv-virtualenv) which can be used to create virtual
-environments. ### Poetry Use [Poetry](https://python-poetry.org/) to install
-Hokusai's dependencies as well as Hokusai itself in [editable mode](https://
-pip-python3.readthedocs.io/en/latest/reference/pip_install.html#editable-
-installs). Please see [this guide](https://python-poetry.org/docs/basic-usage/
-) for working with Poetry. Install Poetry: ``` pip install poetry ``` Install
+to this: ``` $ pyenv install 3.10 python-build: use openssl@1.1 from homebrew
+python-build: use readline from homebrew Downloading Python-3.10.13.tar.xz... -
+> https://www.python.org/ftp/python/3.10.13/Python-3.10.13.tar.xz Installing
+Python-3.10.13... python-build: use tcl-tk from homebrew python-build: use
+readline from homebrew python-build: use ncurses from homebrew python-build:
+use zlib from xcode sdk Installed Python-3.10.13 to /Users/jxu/.pyenv/versions/
+3.10.13 ``` With the desired Python version installed, activate it globally:
+``` pyenv global 3.10 ``` Note: If you want to create a PyInstaller
+distribution, Python must be installed with development libraries. Use the
+environment variable `PYTHON_CONFIGURE_OPTS="--enable-framework"` on Darwin and
+`PYTHON_CONFIGURE_OPTS="--enable-shared"` on Linux when running `pyenv
+install`. ### Virtualenv We recommend using a virtual environment to isolate
+Hokusai's dependencies from that of other projects on your local environment.
+The Pyenv install comes with [pyenv-virtualenv](https://github.com/pyenv/pyenv-
+virtualenv) which can be used to create virtual environments. ### Poetry Use
+[Poetry](https://python-poetry.org/) to install Hokusai's dependencies as well
+as Hokusai itself in [editable mode](https://pip-python3.readthedocs.io/en/
+latest/reference/pip_install.html#editable-installs). Please see [this guide]
+(https://python-poetry.org/docs/basic-usage/) for working with Poetry. Install
+Poetry: ``` pip install --upgrade pip pip install poetry ``` Install
 dependencies and Hokusai in editable mode: ``` poetry install ``` To update
 dependencies: ``` poetry lock ``` ## Testing ### Install Minikube [Minikube]
 (https://minikube.sigs.k8s.io/docs/start/) is used for integration tests. ```
 brew install minikube minikube start --kubernetes-version= ``` ### Run tests To
-run unit and smoke tests: ``` make test ``` To run integration tests: ``` make
-integration ``` Only specific modules, TestClasses, or even methods: ``` python
--m unittest test.unit.test_module.TestClass.test_method ``` Tip: Set `DEBUG=1`
-environment variable to print boto logging ## Distributing Hokusai ### Beta
-Release Merging a branch into `main` automatically creates a beta version
-useful for testing. A [script](./scripts/update_version_file.sh) that runs in
-CI automatically generates a Beta version number and writes it into [VERSION]
-(./hokusai/VERSION) file. The version number is based on the combination of the
-latest canonical version found in [RELEASE_VERSION](./hokusai/RELEASE_VERSION)
-file and the latest Git commit in `main` branch. [VERSION](./hokusai/VERSION)
-file in version control has just a dummy number (e.g. 999.999.999). To install
-the beta: #### MacOS ``` $ brew uninstall hokusai $ brew uninstall hokusai-beta
-$ brew update $ brew tap artsy/formulas $ brew install hokusai-beta ``` ####
-Linux ``` curl -sSL https://raw.githubusercontent.com/artsy/hokusai/main/get-
-hokusai.sh | sudo bash -s beta ``` ### Official Release To create an official
-release, such as `v1.2.3`, perform the following: - Create a branch named
-`prepare-v1.2.3` and make the following changes: - Bump canonical version in
-[RELEASE_VERSION](./hokusai/RELEASE_VERSION) file. - Upate [CHANGELOG](./
-CHANGELOG.md). - Open a PR to merge into `main`. Please see [past PRs](https://
-github.com/artsy/hokusai/
+run unit tests: ``` make test ``` To run integration tests: ``` make
+integration-local ``` Only specific modules, TestClasses, or even methods: ```
+python -m unittest test.unit.test_module.TestClass.test_method ``` Tip: Set
+`DEBUG=1` environment variable to print boto logging ## Distributing Hokusai
+### Beta Release Merging a branch into `main` automatically creates a beta
+version useful for testing. A [script](./scripts/update_version_file.sh) that
+runs in CI automatically generates a Beta version number and writes it into
+[VERSION](./hokusai/VERSION) file. The version number is based on the
+combination of the latest canonical version found in [RELEASE_VERSION](./
+hokusai/RELEASE_VERSION) file and the latest Git commit in `main` branch.
+[VERSION](./hokusai/VERSION) file in version control has just a dummy number
+(e.g. 999.999.999). To install the beta: #### MacOS ``` $ brew uninstall
+hokusai $ brew uninstall hokusai-beta $ brew update $ brew tap artsy/formulas $
+brew install hokusai-beta ``` #### Linux ``` curl -sSL https://
+raw.githubusercontent.com/artsy/hokusai/main/get-hokusai.sh | sudo bash -s beta
+``` ### Official Release To create an official release, such as `v1.2.3`,
+perform the following: - Create a branch named `prepare-v1.2.3` and make the
+following changes: - Bump canonical version in [RELEASE_VERSION](./hokusai/
+RELEASE_VERSION) file. - Upate [CHANGELOG](./CHANGELOG.md). - Open a PR to
+merge into `main`. Please see [past PRs](https://github.com/artsy/hokusai/
 pulls?q=is%3Apr+Release+is%3Aclosed+%22prepare+version%22) for example. - [Open
 a PR](https://github.com/artsy/hokusai/compare/release...main?expand=1) to
 merge `main` into `release`. Please see [past PRs](https://github.com/artsy/
 hokusai/pulls?q=is%3Apr+is%3Aclosed+%22release+version%22) for example. A CI
 [script](./scripts/update_version_file.sh) will copy the version in
 [RELEASE_VERSION](./hokusai/RELEASE_VERSION) file to [VERSION](./hokusai/
 VERSION) file. ## The Name The project is named for the great Japanese artist
```

### Comparing `hokusai-2.1.1/hokusai/cli/base.py` & `hokusai-2.2.0/hokusai/cli/base.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/cli/dev.py` & `hokusai-2.2.0/hokusai/cli/dev.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/cli/pipeline.py` & `hokusai-2.2.0/hokusai/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/cli/production.py` & `hokusai-2.2.0/hokusai/cli/production.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/cli/registry.py` & `hokusai-2.2.0/hokusai/cli/registry.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/cli/review_app.py` & `hokusai-2.2.0/hokusai/cli/review_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,44 +35,47 @@
 def create(app_name, verbose):
   """Creates the Kubernetes based resources defined in ./hokusai/{APP_NAME}.yml"""
   command(
     hokusai.k8s_create,
     KUBE_CONTEXT,
     tag=app_name,
     namespace=clean_string(app_name),
-    filename=os.path.join(CWD, HOKUSAI_CONFIG_DIR, "%s.yml" % app_name)
+    filename=os.path.join(CWD, HOKUSAI_CONFIG_DIR, "%s.yml" % app_name),
+    render_template=False
   )
 
 
 @review_app.command(context_settings=CONTEXT_SETTINGS)
 @click.argument('app_name', type=click.STRING)
 @click.option('-v', '--verbose', type=click.BOOL, is_flag=True, help='Verbose output')
 def delete(app_name, verbose):
   """Deletes the Kubernetes based resources defined in ./hokusai/{APP_NAME}.yml"""
   set_verbosity(verbose)
   command(
     hokusai.k8s_delete,
     KUBE_CONTEXT,
     namespace=clean_string(app_name),
-    filename=os.path.join(CWD, HOKUSAI_CONFIG_DIR, "%s.yml" % app_name)
+    filename=os.path.join(CWD, HOKUSAI_CONFIG_DIR, "%s.yml" % app_name),
+    render_template=False
   )
 
 
 @review_app.command(context_settings=CONTEXT_SETTINGS)
 @click.argument('app_name', type=click.STRING)
 @click.option('-v', '--verbose', type=click.BOOL, is_flag=True, help='Verbose output')
 def update(app_name, verbose):
   """Updates the Kubernetes based resources defined in ./hokusai/{APP_NAME}.yml"""
   set_verbosity(verbose)
   command(
     hokusai.k8s_update,
     KUBE_CONTEXT,
     namespace=clean_string(app_name),
     filename=os.path.join(CWD, HOKUSAI_CONFIG_DIR, "%s.yml" % app_name),
-    skip_checks=True
+    skip_checks=True,
+    render_template=False
   )
 
 
 @review_app.command(context_settings=CONTEXT_SETTINGS)
 @click.argument('app_name', type=click.STRING)
 @click.option('--resources/--no-resources', default=True, help='Print Kubernetes API objects defined in ./hokusai/APP_NAME.yml (default: true)')
 @click.option('--pods/--no-pods', default=True, help='Print pods (default: true)')
@@ -86,15 +89,16 @@
     hokusai.k8s_status,
     KUBE_CONTEXT,
     resources,
     pods,
     describe,
     top,
     namespace=clean_string(app_name),
-    filename=os.path.join(CWD, HOKUSAI_CONFIG_DIR, "%s.yml" % app_name)
+    filename=os.path.join(CWD, HOKUSAI_CONFIG_DIR, "%s.yml" % app_name),
+    render_template=False
   )
 
 
 @review_app.command(context_settings=CONTEXT_SETTINGS)
 @click.argument('app_name', type=click.STRING)
 @click.argument('container_command', type=click.STRING)
 @click.option('--tty', type=click.BOOL, is_flag=True, help='Attach the terminal')
@@ -160,15 +164,16 @@
     tag,
     migration,
     constraint,
     git_remote,
     timeout,
     namespace=clean_string(app_name),
     update_config=update_config,
-    filename=os.path.join(CWD, HOKUSAI_CONFIG_DIR, "%s.yml" % app_name)
+    filename=os.path.join(CWD, HOKUSAI_CONFIG_DIR, "%s.yml" % app_name),
+    render_template=False
   )
 
 
 @review_app.command(context_settings=CONTEXT_SETTINGS)
 @click.option('-v', '--verbose', type=click.BOOL, is_flag=True, help='Verbose output')
 def list(verbose):
   """List existing review apps of the project"""
```

### Comparing `hokusai-2.1.1/hokusai/cli/staging.py` & `hokusai-2.2.0/hokusai/cli/staging.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/commands/__init__.py` & `hokusai-2.2.0/hokusai/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/commands/check.py` & `hokusai-2.2.0/hokusai/commands/check.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/commands/command_tree.py` & `hokusai-2.2.0/hokusai/commands/command_tree.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/commands/configure.py` & `hokusai-2.2.0/hokusai/commands/configure.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/commands/deployment.py` & `hokusai-2.2.0/hokusai/commands/deployment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,39 @@
 from hokusai.lib.common import print_green
 from hokusai.services.deployment import Deployment
 from hokusai.services.command_runner import CommandRunner
 from hokusai.services.ecr import ECR
 from hokusai.lib.exceptions import HokusaiError
 
-def update(context, tag, migration, constraint, git_remote, timeout,
-            namespace=None, update_config=False, filename=None):
+def update(
+  context,
+  tag,
+  migration,
+  constraint,
+  git_remote,
+  timeout,
+  namespace=None,
+  update_config=False,
+  filename=None,
+  render_template=True
+):
   if migration is not None:
     print_green("Running migration '%s' on %s..." % (migration, context), newline_after=True)
     return_code = CommandRunner(context, namespace=namespace).run(tag, migration, constraint=constraint, tty=False)
     if return_code:
       raise HokusaiError("Migration failed with return code %s" % return_code, return_code=return_code)
-  Deployment(context, namespace=namespace).update(tag, constraint, git_remote, timeout,
-                                                  update_config=update_config, filename=filename)
+  Deployment(context, namespace=namespace).update(
+    tag,
+    constraint,
+    git_remote,
+    timeout,
+    update_config=update_config,
+    filename=filename,
+    render_template=render_template
+  )
   print_green("Deployment(s) updated to %s" % tag)
 
 
 def refresh(context, deployment_name, namespace=None):
   deployment = Deployment(context, deployment_name=deployment_name, namespace=namespace)
   deployment.refresh()
```

### Comparing `hokusai-2.1.1/hokusai/commands/development.py` & `hokusai-2.2.0/hokusai/commands/development.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/commands/env.py` & `hokusai-2.2.0/hokusai/commands/env.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/commands/gitcompare.py` & `hokusai-2.2.0/hokusai/commands/gitcompare.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/commands/gitdiff.py` & `hokusai-2.2.0/hokusai/commands/gitdiff.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/commands/gitlog.py` & `hokusai-2.2.0/hokusai/commands/gitlog.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/commands/images.py` & `hokusai-2.2.0/hokusai/commands/images.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/commands/kubernetes.py` & `hokusai-2.2.0/hokusai/commands/kubernetes.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,22 @@
 from hokusai.lib.template_selector import TemplateSelector
 from hokusai.services.ecr import ECR
 from hokusai.services.kubectl import Kubectl
 from hokusai.services.configmap import ConfigMap
 from hokusai.services.yaml_spec import YamlSpec
 from hokusai.lib.exceptions import HokusaiError
 
-def k8s_create(context, tag='latest', namespace=None, filename=None, environment=()):
+def k8s_create(
+  context,
+  tag='latest',
+  namespace=None,
+  filename=None,
+  environment=(),
+  render_template=True
+):
   if filename is None:
     yaml_template = TemplateSelector().get(os.path.join(CWD, HOKUSAI_CONFIG_DIR, context))
   else:
     yaml_template = TemplateSelector().get(filename)
 
   ecr = ECR()
   if not ecr.project_repo_exists():
@@ -34,22 +41,30 @@
         raise HokusaiError("Error: environment variables must be of the form 'KEY=VALUE'")
       split = s.split('=', 1)
       configmap.update(split[0], split[1])
     configmap.create()
     print_green("Created configmap %s-environment" % config.project_name)
 
   kctl = Kubectl(context, namespace=namespace)
-  yaml_spec = YamlSpec(yaml_template).to_file()
+  yaml_spec = YamlSpec(yaml_template, render_template).to_file()
 
   shout(kctl.command("create --save-config -f %s" % yaml_spec), print_output=True)
   print_green("Created Kubernetes environment %s" % yaml_template)
 
 
-def k8s_update(context, namespace=None, filename=None, check_branch="main",
-                check_remote=None, skip_checks=False, dry_run=False):
+def k8s_update(
+  context,
+  namespace=None,
+  filename=None,
+  check_branch="main",
+  check_remote=None,
+  skip_checks=False,
+  dry_run=False,
+  render_template=True
+):
   if filename is None:
     yaml_template = TemplateSelector().get(os.path.join(CWD, HOKUSAI_CONFIG_DIR, context))
   else:
     yaml_template = TemplateSelector().get(filename)
 
   if not skip_checks:
     current_branch = None
@@ -66,50 +81,59 @@
     remotes = [check_remote] if check_remote else shout('git remote').splitlines()
     for remote in remotes:
       shout("git fetch %s" % remote)
       if returncode("git diff --quiet %s/%s" % (remote, current_branch)):
         raise HokusaiError("Local branch %s is divergent from %s/%s.  Aborting." % (current_branch, remote, current_branch))
 
   kctl = Kubectl(context, namespace=namespace)
-  yaml_spec = YamlSpec(yaml_template).to_file()
+  yaml_spec = YamlSpec(yaml_template, render_template).to_file()
 
   if dry_run:
     shout(kctl.command("apply -f %s --dry-run" % yaml_spec), print_output=True)
     print_green("Updated Kubernetes environment %s (dry run)" % yaml_template)
   else:
     shout(kctl.command("apply -f %s" % yaml_spec), print_output=True)
     print_green("Updated Kubernetes environment %s" % yaml_template)
 
 
-def k8s_delete(context, namespace=None, filename=None):
+def k8s_delete(context, namespace=None, filename=None, render_template=True):
   if filename is None:
     yaml_template = TemplateSelector().get(os.path.join(CWD, HOKUSAI_CONFIG_DIR, context))
   else:
     yaml_template = TemplateSelector().get(filename)
 
   if filename is None:
     configmap = ConfigMap(context, namespace=namespace)
     configmap.destroy()
     print_green("Deleted configmap %s-environment" % config.project_name)
 
   kctl = Kubectl(context, namespace=namespace)
-  yaml_spec = YamlSpec(yaml_template).to_file()
+  yaml_spec = YamlSpec(yaml_template, render_template).to_file()
 
   shout(kctl.command("delete -f %s" % yaml_spec), print_output=True)
   print_green("Deleted Kubernetes environment %s" % yaml_template)
 
 
-def k8s_status(context, resources, pods, describe, top, namespace=None, filename=None):
+def k8s_status(
+  context,
+  resources,
+  pods,
+  describe,
+  top,
+  namespace=None,
+  filename=None,
+  render_template=True
+):
   if filename is None:
     yaml_template = TemplateSelector().get(os.path.join(CWD, HOKUSAI_CONFIG_DIR, context))
   else:
     yaml_template = TemplateSelector().get(filename)
 
   kctl = Kubectl(context, namespace=namespace)
-  yaml_spec = YamlSpec(yaml_template).to_file()
+  yaml_spec = YamlSpec(yaml_template, render_template).to_file()
 
   if describe:
     kctl_cmd = "describe"
     output = ""
   else:
     kctl_cmd = "get"
     output = " -o wide"
```

### Comparing `hokusai-2.1.1/hokusai/commands/logs.py` & `hokusai-2.2.0/hokusai/commands/logs.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/commands/namespace.py` & `hokusai-2.2.0/hokusai/commands/namespace.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/commands/pull.py` & `hokusai-2.2.0/hokusai/commands/pull.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/commands/push.py` & `hokusai-2.2.0/hokusai/commands/push.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/commands/retag.py` & `hokusai-2.2.0/hokusai/commands/retag.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/commands/setup.py` & `hokusai-2.2.0/hokusai/commands/setup.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/commands/test.py` & `hokusai-2.2.0/hokusai/commands/test.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/lib/command.py` & `hokusai-2.2.0/hokusai/lib/command.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/lib/common.py` & `hokusai-2.2.0/hokusai/lib/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,20 @@
 
 EXIT_SIGNALS = [signal.SIGHUP, signal.SIGINT, signal.SIGQUIT, signal.SIGPIPE, signal.SIGTERM]
 
 VERBOSE = False
 
 AWS_DEFAULT_REGION = 'us-east-1'
 
+
+def ansi_escape(raw_string):
+  ''' rid string of ANSI esapes such as color '''
+  escape_regex = re.compile(r'\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])')
+  return escape_regex.sub('', raw_string)
+
 def clean_string(str):
   return str.lower().replace('_', '-')
 
 def get_platform():
   ''' get the platform (e.g. darwin, linux) of the machine '''
   return platform.system().lower()
```

### Comparing `hokusai-2.1.1/hokusai/lib/config.py` & `hokusai-2.2.0/hokusai/lib/config.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/lib/config_loader.py` & `hokusai-2.2.0/hokusai/lib/config_loader.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/lib/docker_compose_helpers.py` & `hokusai-2.2.0/hokusai/lib/docker_compose_helpers.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/lib/environment.py` & `hokusai-2.2.0/hokusai/lib/environment.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/lib/global_config.py` & `hokusai-2.2.0/hokusai/lib/global_config.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/lib/representers.py` & `hokusai-2.2.0/hokusai/lib/representers.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/lib/template_renderer.py` & `hokusai-2.2.0/hokusai/lib/template_renderer.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/lib/template_selector.py` & `hokusai-2.2.0/hokusai/lib/template_selector.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/services/command_runner.py` & `hokusai-2.2.0/hokusai/services/command_runner.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/services/configmap.py` & `hokusai-2.2.0/hokusai/services/configmap.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/services/deployment.py` & `hokusai-2.2.0/hokusai/services/deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,24 @@
     self.kctl = Kubectl(self.context, namespace=namespace)
     self.ecr = ECR()
     if deployment_name:
       self.cache = [self.kctl.get_object("deployment %s" % deployment_name)]
     else:
       self.cache = self.kctl.get_objects('deployment', selector="app=%s,layer=application" % config.project_name)
 
-  def update(self, tag, constraint, git_remote, timeout, update_config=False, filename=None):
+  def update(
+    self,
+    tag,
+    constraint,
+    git_remote,
+    timeout,
+    update_config=False,
+    filename=None,
+    render_template=True
+  ):
     if not self.ecr.project_repo_exists():
       raise HokusaiError("Project repo does not exist.  Aborting.")
 
     digest = self.ecr.image_digest_for_tag(tag)
     if digest is None:
       raise HokusaiError("Could not find an image digest for tag %s.  Aborting." % tag)
     digest_half = digest[len(digest)//2:]
@@ -65,15 +74,15 @@
         raise HokusaiError("Pre-deploy hook failed with return code %s" % return_code, return_code=return_code)
 
     if filename is None:
       yaml_template = TemplateSelector().get(os.path.join(CWD, HOKUSAI_CONFIG_DIR, self.context))
     else:
       yaml_template = TemplateSelector().get(filename)
 
-    yaml_spec = YamlSpec(yaml_template).to_list()
+    yaml_spec = YamlSpec(yaml_template, render_template).to_list()
 
     # If a review app, a canary app or the canonical app while updating config,
     # bust the deployment cache and populate deployments from the yaml file
     if filename or update_config:
       self.cache = []
       for item in yaml_spec:
         if item['kind'] == 'Deployment':
```

### Comparing `hokusai-2.1.1/hokusai/services/docker.py` & `hokusai-2.2.0/hokusai/services/docker.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/services/ecr.py` & `hokusai-2.2.0/hokusai/services/ecr.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/services/kubectl.py` & `hokusai-2.2.0/hokusai/services/kubectl.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         shout(f'{self.kubectl} config view'),
         Loader=yaml.FullLoader
       )['contexts']
     ]
 
   def get_object(self, obj):
     ''' run kubectl get <object> '''
-    cmd = self.command(f'get {obj} -o json)')
+    cmd = self.command(f'get {obj} -o json')
     try:
       return json.loads(shout(cmd))
     except ValueError:
       return None
 
   def get_objects(self, obj, selector=None):
     ''' run kubectl get <object> with selectors '''
```

### Comparing `hokusai-2.1.1/hokusai/services/s3.py` & `hokusai-2.2.0/hokusai/services/s3.py`

 * *Files identical despite different names*

### Comparing `hokusai-2.1.1/hokusai/services/yaml_spec.py` & `hokusai-2.2.0/hokusai/services/yaml_spec.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 import os
-import atexit
-from tempfile import NamedTemporaryFile
 
+import atexit
+import jinja2
 import yaml
 
+from tempfile import NamedTemporaryFile
+
 from botocore.exceptions import NoCredentialsError
 
 from hokusai.lib.config import config, HOKUSAI_TMP_DIR
 from hokusai.lib.config_loader import ConfigLoader
 from hokusai.lib.template_renderer import TemplateRenderer
 from hokusai.lib.common import print_yellow
 from hokusai.lib.exceptions import HokusaiError
 
 from hokusai.services.ecr import ECR
 
+
 class YamlSpec:
-  def __init__(self, template_file):
+  def __init__(self, template_file, render_template=True):
     self.template_file = template_file
     self.ecr = ECR()
     self.tmp_filename = None
+    self.render_template = render_template
     atexit.register(self.cleanup)
 
   def to_string(self):
-    template_config = {
-      "project_name": config.project_name
-    }
-
-    try:
-      template_config["project_repo"] = self.ecr.project_repo
-    except NoCredentialsError:
-      print_yellow("WARNING: Could not get template variable project_repo")
-
-    if config.template_config_files:
-      for template_config_file in config.template_config_files:
-        try:
-          config_loader = ConfigLoader(template_config_file)
-          template_config.update(config_loader.load())
-        except NoCredentialsError:
-          print_yellow("WARNING: Could not get template config file %s" % template_config_file)
-
-    return TemplateRenderer(self.template_file, template_config).render()
+    if self.render_template:
+      template_config = {
+        "project_name": config.project_name
+      }
+
+      try:
+        template_config["project_repo"] = self.ecr.project_repo
+      except NoCredentialsError:
+        print_yellow("WARNING: Could not get template variable project_repo")
+
+      if config.template_config_files:
+        for template_config_file in config.template_config_files:
+          try:
+            config_loader = ConfigLoader(template_config_file)
+            template_config.update(config_loader.load())
+          except NoCredentialsError:
+            print_yellow("WARNING: Could not get template config file %s" % template_config_file)
+
+      return TemplateRenderer(self.template_file, template_config).render()
+    else:
+      with open(self.template_file, 'r') as f:
+        content = f.read().strip()
+      return content
 
   def to_file(self):
     file_basename = os.path.basename(self.template_file)
     if file_basename.endswith('.j2'):
       file_basename = file_basename.rstrip('.j2')
     f = NamedTemporaryFile(delete=False, dir=HOKUSAI_TMP_DIR, mode='w')
     self.tmp_filename = f.name
```

### Comparing `hokusai-2.1.1/hokusai/templates/hokusai/production.yml.j2` & `hokusai-2.2.0/hokusai/templates/hokusai/staging.yml.j2`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 ---
-apiVersion: extensions/v1beta1
+apiVersion: apps/v1
 kind: Deployment
 metadata:
   name: {% raw %}{{ project_name }}{% endraw %}-web
   namespace: default
+  labels:
+    app: {% raw %}{{ project_name }}{% endraw %}
+    component: web
+    layer: application
 spec:
-  replicas: 2
+  replicas: 1
   strategy:
     rollingUpdate:
       maxSurge: 1
       maxUnavailable: 0
     type: RollingUpdate
+  selector:
+    matchLabels:
+      app: {% raw %}{{ project_name }}{% endraw %}
+      component: web
+      layer: application
   template:
     metadata:
       labels:
         app: {% raw %}{{ project_name }}{% endraw %}
         component: web
         layer: application
       name: {% raw %}{{ project_name }}{% endraw %}-web
     spec:
       containers:
       - name: {% raw %}{{ project_name }}{% endraw %}-web
         envFrom:
         - configMapRef:
             name: {% raw %}{{ project_name }}{% endraw %}-environment
-        image: {% raw %}{{ project_repo }}{% endraw %}:production
+        image: {% raw %}{{ project_repo }}{% endraw %}:staging
         imagePullPolicy: Always
         ports:
         - containerPort: 80
 ---
 apiVersion: v1
 kind: Service
 metadata:
```

### Comparing `hokusai-2.1.1/hokusai/templates/hokusai/staging.yml.j2` & `hokusai-2.2.0/hokusai/templates/hokusai/production.yml.j2`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 ---
-apiVersion: extensions/v1beta1
+apiVersion: apps/v1
 kind: Deployment
 metadata:
   name: {% raw %}{{ project_name }}{% endraw %}-web
   namespace: default
+  labels:
+    app: {% raw %}{{ project_name }}{% endraw %}
+    component: web
+    layer: application
 spec:
-  replicas: 1
+  replicas: 2
   strategy:
     rollingUpdate:
       maxSurge: 1
       maxUnavailable: 0
     type: RollingUpdate
+  selector:
+    matchLabels:
+      app: {% raw %}{{ project_name }}{% endraw %}
+      component: web
+      layer: application
   template:
     metadata:
       labels:
         app: {% raw %}{{ project_name }}{% endraw %}
         component: web
         layer: application
       name: {% raw %}{{ project_name }}{% endraw %}-web
     spec:
       containers:
       - name: {% raw %}{{ project_name }}{% endraw %}-web
         envFrom:
         - configMapRef:
             name: {% raw %}{{ project_name }}{% endraw %}-environment
-        image: {% raw %}{{ project_repo }}{% endraw %}:staging
+        image: {% raw %}{{ project_repo }}{% endraw %}:production
         imagePullPolicy: Always
         ports:
         - containerPort: 80
 ---
 apiVersion: v1
 kind: Service
 metadata:
```

### Comparing `hokusai-2.1.1/pyproject.toml` & `hokusai-2.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [project]
 dynamic = ["version"]
+name = "hokusai"
 
 [tool.poetry]
 name = "hokusai"
-version = "2.1.1"
+version = "2.2.0"
 description = "Artsy Docker development toolkit"
 authors = ["Isac Petruzzi <isac@artsymail.com>"]
 maintainers = ["Jian-Feng Xu <jian-feng@artsymail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "http://github.com/artsy/hokusai"
 include = ["hokusai/VERSION"]
 
 [tool.poetry.dependencies]
-boto3 = "==1.21.28"
+boto3 = "^1.34.25"
 click = "==8.1.0"
 click-repl = "==0.2.0"
 Jinja2 = "==3.1.1"
 MarkupSafe = "==2.1.1"
 packaging = "==21.3"
 prompt-toolkit = "==3.0.28"
 python = ">=3.9,<3.11"
 PyYAML = "==6.0.1"
 termcolor = "==1.1.0"
 
 [tool.poetry.dev-dependencies]
 coverage = "^6.3.2"
+gitpython = "^3.1.40"
 httpretty = "^1.1.4"
 ipdb = "^0.13.9"
 mock = "^4.0.3"
 pyinstaller = "^4.6"
 pylint = "^2.13.2"
 pytest = "^7.2.1"
 pytest-describe = "^2.0.1"
```

### Comparing `hokusai-2.1.1/setup.py` & `hokusai-2.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 package_data = \
 {'': ['*'], 'hokusai': ['templates/*', 'templates/hokusai/*']}
 
 install_requires = \
 ['Jinja2==3.1.1',
  'MarkupSafe==2.1.1',
  'PyYAML==6.0.1',
- 'boto3==1.21.28',
+ 'boto3>=1.34.25,<2.0.0',
  'click-repl==0.2.0',
  'click==8.1.0',
  'packaging==21.3',
  'prompt-toolkit==3.0.28',
  'termcolor==1.1.0']
 
 entry_points = \
 {'console_scripts': ['hokusai = hokusai.command_line:main']}
 
 setup_kwargs = {
     'name': 'hokusai',
-    'version': '2.1.1',
+    'version': '2.2.0',
     'description': 'Artsy Docker development toolkit',
-    'long_description': '## HOKUSAI [![CircleCI](https://circleci.com/gh/artsy/hokusai/tree/main.svg?style=svg)](https://circleci.com/gh/artsy/hokusai/tree/main)\n\n<a href="https://en.wikipedia.org/wiki/Hokusai"><img height="300" src="hokusai.jpg"></a>\n\nHokusai is a Docker + Kubernetes CLI for application developers.\n\nHokusai "dockerizes" applications and manages their lifecycle throughout development, testing, and release cycles.\n\nHokusai wraps calls to [Kubectl](https://kubernetes.io/), [Docker](https://www.docker.com/), [Docker-Compose](https://docs.docker.com/compose/) and [Git](https://git-scm.com/) with a CLI, and defines a CI workflow.\n\nHokusai currently only supports Kubernetes deployments on AWS, configured to pull from ECS container repositories (ECR), although other providers may be added in the future.\n\n### Why Hokusai?\n\nAt [Artsy](http://www.artsy.net), as we began working with Kubernetes, while impressed with its design, capabilities, and flexibility, we were in need of tooling we could deliver to agile development teams that addressed the day-to-day tasks of application development, delivery, introspection and maintenance, while providing a clean and uncomplicated interface.\n\nTransitioning teams to the Docker / Kubernetes ecosystem can be intimidating, and comes with a steep learning curve. We set out to create a Heroku-like CLI that would shepherd the application developer into the ecosystems of Docker and Kubernetes, and while introducing new tooling and concepts, outlining a clear practice for dependency management, local development, testing and CI, image repository structure, deployment and orchestration.\n\n## Installation\n\n### MacOS\n\nWe recommend installing via Homebrew:\n\n```\n$ brew update\n$ brew tap artsy/formulas\n$ brew install hokusai\n```\n\nIf you previously installed Hokusai via an alternate installation method, you may need to force the `link` step.\n\n```\n$ brew link --overwrite hokusai\n```\n\nIf you previously installed Hokusai via Pip, you may want to first uninstall it:\n\n```\n$ pip uninstall hokusai\n```\n\n### Linux\n\n```\ncurl -sSL https://raw.githubusercontent.com/artsy/hokusai/main/get-hokusai.sh | sudo bash\n```\n\nNote: This method installs Hokusai to `/usr/local/bin/hokusai`.\n\n### Pip\n\nHokusai can be installed via Pip, on MacOS or Linux. If you do so, please first go through [Pyenv](#Pyenv), [Python](#Python), and [Virtualenv](#Virtualenv) steps.\n\nPython 3.7+ is required.\n\n```\npip install hokusai\n```\n\nNote: If Pip fails at upgrading your system Python packages, try:\n\n```\npip install hokusai --ignore-installed\n```\n\n### Docker\n\nWe also maintain [Hokusai Docker images](https://hub.docker.com/r/artsy/hokusai) for running Hokusai in Docker.\n\n### Github\n\nRelease artifacts are available on [Github](https://github.com/artsy/hokusai/releases).\n\n### AWS S3\n\nRelease artifacts are also available in AWS S3. You can use this [convenience script](get-hokusai.sh) or Curl to fetch them.\n\n### A note on Python 2.x\n\nHokusai currently supports Python 3.7+ only. The last version that supported Python 2.x was [v0.5.18](https://github.com/artsy/hokusai/tree/v0.5.18).\n\n## Setup\n\nWe assume that your org admin has already set up a Kubernetes cluster and an AWS infrastructure, and that your local environment has Git, Docker, and Docker-Compose installed. Perform the following steps to get Hokusai working:\n\n1. Ensure your org admin has completed the steps mentioned in [Administering Hokusai](./docs/Administering_Hokusai.md).\n\n2. Configure your local environment with [AWS credentials](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html#configuring-credentials).\n\n3. Run [hokusai configure command](docs/Command_Reference.md#configuring-hokusai-for-your-organization).\n\n4. Optionally, enable Bash autocompletion:\n\n    ```\n    eval "$(_HOKUSAI_COMPLETE=source hokusai)"\n    ```\n\n## Getting Started\n\nOnce Hokusai is configured, you can start using it on a project. Please see [Getting Started](./docs/Getting_Started.md).\n\n## Command Reference\n\nA full command reference can be found in [Command Reference](./docs/Command_Reference.md).\n\n## Review Apps\n\nHokusai can be used to simplify the process of spinning up a "review app" instance of your project, based on a feature branch or pull request.\n\nFull details are in the [Review App reference](./docs/Review_Apps.md).\n\n## Hokusai Files\n\nA descripton of all the [files used by Hokusai](docs/hokusai_files.md).\n\n## Developing Hokusai\n\nTo work on Hokusai itself, please set up:\n\n### Pyenv\n\nWe recommend using [Pyenv](https://github.com/pyenv/pyenv) to install the correct version of Python. For a tutorial of Pyenv, see [this guide](https://realpython.com/intro-to-pyenv/).\n\nWhen installing on MacOS, please make sure to use brew-installed `openssl` and `readline` libraries, and xcode-installed `zlib` library. And make sure these libraries are correctly linked. Like so:\n\n```\nbrew install openssl readline zlib\n\necho \'export PATH="/usr/local/opt/openssl@1.1/bin:$PATH"\' >> ~/.bash_profile\necho \'export LDFLAGS="-L/usr/local/opt/openssl@1.1/lib"\' >> ~/.bash_profile\necho \'export CPPFLAGS="-I/usr/local/opt/openssl@1.1/include"\' >> ~/.bash_profile\necho \'export PKG_CONFIG_PATH="/usr/local/opt/openssl@1.1/lib/pkgconfig"\' >> ~/.bash_profile\n```\n\n### Python\n\nHokusai is currently tested on Python 3.9.10 so we recommend using that Python version.\n\nIf you use Pyenv to install Python, you should see an output similar to this:\n\n```\npyenv install 3.9.10\n\n    python-build: use openssl from homebrew\n    python-build: use readline from homebrew\n\n    Downloading Python-3.9.10.tar.xz...\n    -> https://www.python.org/ftp/python/3.9.10/Python-3.9.10.tar.xz\n    Installing Python-3.9.10...\n    python-build: use tcl-tk from homebrew\n    python-build: use readline from homebrew\n    python-build: use zlib from xcode sdk\n\n    Installed Python-3.9.10 to $HOME/.pyenv/versions/3.9.10\n```\n\nWith the desired Python version installed, activate it globally:\n\n```\npyenv global 3.9.10\n```\n\nNote: If you want to create a PyInstaller distribution, Python must be installed with development libraries. Use the environment variable `PYTHON_CONFIGURE_OPTS="--enable-framework"` on Darwin and `PYTHON_CONFIGURE_OPTS="--enable-shared"` on Linux when running `pyenv install`.\n\n### Virtualenv\n\nWe recommend using a virtual environment to isolate Hokusai\'s dependencies from that of other projects on your local environment.\n\nThe Pyenv install comes with [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv) which can be used to create virtual environments.\n\n### Poetry\n\nUse [Poetry](https://python-poetry.org/) to install Hokusai\'s dependencies as well as Hokusai itself in [editable mode](https://pip-python3.readthedocs.io/en/latest/reference/pip_install.html#editable-installs). Please see [this guide](https://python-poetry.org/docs/basic-usage/) for working with Poetry.\n\nInstall Poetry:\n\n```\npip install poetry\n```\n\nInstall dependencies and Hokusai in editable mode:\n\n```\npoetry install\n```\n\nTo update dependencies:\n\n```\npoetry lock\n```\n\n## Testing\n\n### Install Minikube\n\n[Minikube](https://minikube.sigs.k8s.io/docs/start/) is used for integration tests.\n\n```\nbrew install minikube\nminikube start --kubernetes-version=<version of your Kubernetes clusters, example: v1.2.3>\n```\n\n### Run tests\n\nTo run unit and smoke tests:\n\n```\nmake test\n```\n\nTo run integration tests:\n\n```\nmake integration\n```\n\nOnly specific modules, TestClasses, or even methods:\n\n```\npython -m unittest test.unit.test_module.TestClass.test_method\n```\n\nTip: Set `DEBUG=1` environment variable to print boto logging\n\n\n## Distributing Hokusai\n\n### Beta Release\n\nMerging a branch into `main` automatically creates a beta version useful for testing. A [script](./scripts/update_version_file.sh) that runs in CI automatically generates a Beta version number and writes it into [VERSION](./hokusai/VERSION) file. The version number is based on the combination of the latest canonical version found in [RELEASE_VERSION](./hokusai/RELEASE_VERSION) file and the latest Git commit in `main` branch. [VERSION](./hokusai/VERSION) file in version control has just a dummy number (e.g. 999.999.999).\n\nTo install the beta:\n\n#### MacOS\n\n```\n$ brew uninstall hokusai\n$ brew uninstall hokusai-beta\n$ brew update\n$ brew tap artsy/formulas\n$ brew install hokusai-beta\n```\n\n#### Linux\n\n```\ncurl -sSL https://raw.githubusercontent.com/artsy/hokusai/main/get-hokusai.sh | sudo bash -s beta\n```\n\n### Official Release\n\nTo create an official release, such as `v1.2.3`, perform the following:\n\n- Create a branch named `prepare-v1.2.3` and make the following changes:\n  - Bump canonical version in [RELEASE_VERSION](./hokusai/RELEASE_VERSION) file.\n  - Upate [CHANGELOG](./CHANGELOG.md).\n  - Open a PR to merge into `main`. Please see [past PRs](https://github.com/artsy/hokusai/pulls?q=is%3Apr+Release+is%3Aclosed+%22prepare+version%22) for example.\n\n- [Open a PR](https://github.com/artsy/hokusai/compare/release...main?expand=1) to merge `main` into `release`. Please see [past PRs](https://github.com/artsy/hokusai/pulls?q=is%3Apr+is%3Aclosed+%22release+version%22) for example.\n\nA CI [script](./scripts/update_version_file.sh) will copy the version in [RELEASE_VERSION](./hokusai/RELEASE_VERSION) file to [VERSION](./hokusai/VERSION) file.\n\n## The Name\n\nThe project is named for the great Japanese artist [Katsushika Hokusai](https://www.artsy.net/article/artsy-editorial-7-things-hokusai-creator-great-wave) (1760-1849).\n\n## About Artsy\n\n<a href="https://www.artsy.net/">\n  <img align="left" src="https://avatars2.githubusercontent.com/u/546231?s=200&v=4"/>\n</a>\n\nThis project is the work of engineers at [Artsy][footer_website], the world\'s\nleading and largest online art marketplace and platform for discovering art.\nOne of our core [Engineering Principles][footer_principles] is being [Open\nSource by Default][footer_open] which means we strive to share as many details\nof our work as possible.\n\nYou can learn more about this work from [our blog][footer_blog] and by following\n[@ArtsyOpenSource][footer_twitter] or explore our public data by checking out\n[our API][footer_api]. If you\'re interested in a career at Artsy, read through\nour [job postings][footer_jobs]!\n\n[footer_website]: https://www.artsy.net/\n[footer_principles]: https://github.com/artsy/README/blob/main/culture/engineering-principles.md\n[footer_open]: https://github.com/artsy/README/blob/main/culture/engineering-principles.md\n[footer_blog]: https://artsy.github.io/\n[footer_twitter]: https://twitter.com/ArtsyOpenSource\n[footer_api]: https://developers.artsy.net/\n[footer_jobs]: https://www.artsy.net/jobs\n',
+    'long_description': '## HOKUSAI [![CircleCI](https://circleci.com/gh/artsy/hokusai/tree/main.svg?style=svg)](https://circleci.com/gh/artsy/hokusai/tree/main)\n\n<a href="https://en.wikipedia.org/wiki/Hokusai"><img height="300" src="hokusai.jpg"></a>\n\nHokusai is a Docker + Kubernetes CLI for application developers.\n\nHokusai "dockerizes" applications and manages their lifecycle throughout development, testing, and release cycles.\n\nHokusai wraps calls to [Kubectl](https://kubernetes.io/), [Docker](https://www.docker.com/), [Docker-Compose](https://docs.docker.com/compose/) and [Git](https://git-scm.com/) with a CLI, and defines a CI workflow.\n\nHokusai currently only supports Kubernetes deployments on AWS, configured to pull from ECS container repositories (ECR), although other providers may be added in the future.\n\n### Why Hokusai?\n\nAt [Artsy](http://www.artsy.net), as we began working with Kubernetes, while impressed with its design, capabilities, and flexibility, we were in need of tooling we could deliver to agile development teams that addressed the day-to-day tasks of application development, delivery, introspection and maintenance, while providing a clean and uncomplicated interface.\n\nTransitioning teams to the Docker / Kubernetes ecosystem can be intimidating, and comes with a steep learning curve. We set out to create a Heroku-like CLI that would shepherd the application developer into the ecosystems of Docker and Kubernetes, and while introducing new tooling and concepts, outlining a clear practice for dependency management, local development, testing and CI, image repository structure, deployment and orchestration.\n\n## Installation\n\n### MacOS\n\nWe recommend installing via Homebrew:\n\n```\n$ brew update\n$ brew tap artsy/formulas\n$ brew install hokusai\n```\n\nIf you previously installed Hokusai via an alternate installation method, you may need to force the `link` step.\n\n```\n$ brew link --overwrite hokusai\n```\n\nIf you previously installed Hokusai via Pip, you may want to first uninstall it:\n\n```\n$ pip uninstall hokusai\n```\n\n### Linux\n\n```\ncurl -sSL https://raw.githubusercontent.com/artsy/hokusai/main/get-hokusai.sh | sudo bash\n```\n\nNote: This method installs Hokusai to `/usr/local/bin/hokusai`.\n\n### Pip\n\nHokusai can be installed via Pip, on MacOS or Linux. If you do so, please first go through [Pyenv](#Pyenv), [Python](#Python), and [Virtualenv](#Virtualenv) steps.\n\nPython 3.7+ is required.\n\n```\npip install hokusai\n```\n\nNote: If Pip fails at upgrading your system Python packages, try:\n\n```\npip install hokusai --ignore-installed\n```\n\n### Docker\n\nWe also maintain [Hokusai Docker images](https://hub.docker.com/r/artsy/hokusai) for running Hokusai in Docker.\n\n### Github\n\nRelease artifacts are available on [Github](https://github.com/artsy/hokusai/releases).\n\n### AWS S3\n\nRelease artifacts are also available in AWS S3. You can use this [convenience script](get-hokusai.sh) or Curl to fetch them.\n\n### A note on Python 2.x\n\nHokusai currently supports Python 3.7+ only. The last version that supported Python 2.x was [v0.5.18](https://github.com/artsy/hokusai/tree/v0.5.18).\n\n## Setup\n\nWe assume that your org admin has already set up a Kubernetes cluster and an AWS infrastructure, and that your local environment has Git, Docker, and Docker-Compose installed. Perform the following steps to get Hokusai working:\n\n1. Ensure your org admin has completed the steps mentioned in [Administering Hokusai](./docs/Administering_Hokusai.md).\n\n2. Configure your local environment with [AWS credentials](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html#configuring-credentials).\n\n3. Run [hokusai configure command](docs/Command_Reference.md#configuring-hokusai-for-your-organization).\n\n4. Optionally, enable Bash autocompletion:\n\n    ```\n    eval "$(_HOKUSAI_COMPLETE=source hokusai)"\n    ```\n\n## Getting Started\n\nOnce Hokusai is configured, you can start using it on a project. Please see [Getting Started](./docs/Getting_Started.md).\n\n## Command Reference\n\nA full command reference can be found in [Command Reference](./docs/Command_Reference.md).\n\n## Review Apps\n\nHokusai can be used to simplify the process of spinning up a "review app" instance of your project, based on a feature branch or pull request.\n\nFull details are in the [Review App reference](./docs/Review_Apps.md).\n\n## Hokusai Files\n\nA descripton of all the [files used by Hokusai](docs/hokusai_files.md).\n\n## Developing Hokusai\n\nTo work on Hokusai itself, please set up:\n\n### Pyenv\n\nWe recommend using [Pyenv](https://github.com/pyenv/pyenv) to install the correct version of Python. For a tutorial of Pyenv, see [this guide](https://realpython.com/intro-to-pyenv/).\n\nWhen installing on MacOS, please make sure to use brew-installed `openssl` and `readline` libraries, and xcode-installed `zlib` library. And make sure these libraries are correctly linked. Like so:\n\n```\nbrew install openssl readline zlib\n\necho \'export PATH="/usr/local/opt/openssl@1.1/bin:$PATH"\' >> ~/.bash_profile\necho \'export LDFLAGS="-L/usr/local/opt/openssl@1.1/lib"\' >> ~/.bash_profile\necho \'export CPPFLAGS="-I/usr/local/opt/openssl@1.1/include"\' >> ~/.bash_profile\necho \'export PKG_CONFIG_PATH="/usr/local/opt/openssl@1.1/lib/pkgconfig"\' >> ~/.bash_profile\n```\n\n### Python\n\nHokusai is currently tested on Python 3.10 so we recommend using that Python version.\n\nIf you use Pyenv to install Python, you should see an output similar to this:\n\n```\n$ pyenv install 3.10\npython-build: use openssl@1.1 from homebrew\npython-build: use readline from homebrew\nDownloading Python-3.10.13.tar.xz...\n-> https://www.python.org/ftp/python/3.10.13/Python-3.10.13.tar.xz\nInstalling Python-3.10.13...\npython-build: use tcl-tk from homebrew\npython-build: use readline from homebrew\npython-build: use ncurses from homebrew\npython-build: use zlib from xcode sdk\nInstalled Python-3.10.13 to /Users/jxu/.pyenv/versions/3.10.13\n```\n\nWith the desired Python version installed, activate it globally:\n\n```\npyenv global 3.10\n```\n\nNote: If you want to create a PyInstaller distribution, Python must be installed with development libraries. Use the environment variable `PYTHON_CONFIGURE_OPTS="--enable-framework"` on Darwin and `PYTHON_CONFIGURE_OPTS="--enable-shared"` on Linux when running `pyenv install`.\n\n### Virtualenv\n\nWe recommend using a virtual environment to isolate Hokusai\'s dependencies from that of other projects on your local environment.\n\nThe Pyenv install comes with [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv) which can be used to create virtual environments.\n\n### Poetry\n\nUse [Poetry](https://python-poetry.org/) to install Hokusai\'s dependencies as well as Hokusai itself in [editable mode](https://pip-python3.readthedocs.io/en/latest/reference/pip_install.html#editable-installs). Please see [this guide](https://python-poetry.org/docs/basic-usage/) for working with Poetry.\n\nInstall Poetry:\n\n```\npip install --upgrade pip\npip install poetry\n```\n\nInstall dependencies and Hokusai in editable mode:\n\n```\npoetry install\n```\n\nTo update dependencies:\n\n```\npoetry lock\n```\n\n## Testing\n\n### Install Minikube\n\n[Minikube](https://minikube.sigs.k8s.io/docs/start/) is used for integration tests.\n\n```\nbrew install minikube\nminikube start --kubernetes-version=<version of your Kubernetes clusters, example: v1.2.3>\n```\n\n### Run tests\n\nTo run unit tests:\n\n```\nmake test\n```\n\nTo run integration tests:\n\n```\nmake integration-local\n```\n\nOnly specific modules, TestClasses, or even methods:\n\n```\npython -m unittest test.unit.test_module.TestClass.test_method\n```\n\nTip: Set `DEBUG=1` environment variable to print boto logging\n\n\n## Distributing Hokusai\n\n### Beta Release\n\nMerging a branch into `main` automatically creates a beta version useful for testing. A [script](./scripts/update_version_file.sh) that runs in CI automatically generates a Beta version number and writes it into [VERSION](./hokusai/VERSION) file. The version number is based on the combination of the latest canonical version found in [RELEASE_VERSION](./hokusai/RELEASE_VERSION) file and the latest Git commit in `main` branch. [VERSION](./hokusai/VERSION) file in version control has just a dummy number (e.g. 999.999.999).\n\nTo install the beta:\n\n#### MacOS\n\n```\n$ brew uninstall hokusai\n$ brew uninstall hokusai-beta\n$ brew update\n$ brew tap artsy/formulas\n$ brew install hokusai-beta\n```\n\n#### Linux\n\n```\ncurl -sSL https://raw.githubusercontent.com/artsy/hokusai/main/get-hokusai.sh | sudo bash -s beta\n```\n\n### Official Release\n\nTo create an official release, such as `v1.2.3`, perform the following:\n\n- Create a branch named `prepare-v1.2.3` and make the following changes:\n  - Bump canonical version in [RELEASE_VERSION](./hokusai/RELEASE_VERSION) file.\n  - Upate [CHANGELOG](./CHANGELOG.md).\n  - Open a PR to merge into `main`. Please see [past PRs](https://github.com/artsy/hokusai/pulls?q=is%3Apr+Release+is%3Aclosed+%22prepare+version%22) for example.\n\n- [Open a PR](https://github.com/artsy/hokusai/compare/release...main?expand=1) to merge `main` into `release`. Please see [past PRs](https://github.com/artsy/hokusai/pulls?q=is%3Apr+is%3Aclosed+%22release+version%22) for example.\n\nA CI [script](./scripts/update_version_file.sh) will copy the version in [RELEASE_VERSION](./hokusai/RELEASE_VERSION) file to [VERSION](./hokusai/VERSION) file.\n\n## The Name\n\nThe project is named for the great Japanese artist [Katsushika Hokusai](https://www.artsy.net/article/artsy-editorial-7-things-hokusai-creator-great-wave) (1760-1849).\n\n## About Artsy\n\n<a href="https://www.artsy.net/">\n  <img align="left" src="https://avatars2.githubusercontent.com/u/546231?s=200&v=4"/>\n</a>\n\nThis project is the work of engineers at [Artsy][footer_website], the world\'s\nleading and largest online art marketplace and platform for discovering art.\nOne of our core [Engineering Principles][footer_principles] is being [Open\nSource by Default][footer_open] which means we strive to share as many details\nof our work as possible.\n\nYou can learn more about this work from [our blog][footer_blog] and by following\n[@ArtsyOpenSource][footer_twitter] or explore our public data by checking out\n[our API][footer_api]. If you\'re interested in a career at Artsy, read through\nour [job postings][footer_jobs]!\n\n[footer_website]: https://www.artsy.net/\n[footer_principles]: https://github.com/artsy/README/blob/main/culture/engineering-principles.md\n[footer_open]: https://github.com/artsy/README/blob/main/culture/engineering-principles.md\n[footer_blog]: https://artsy.github.io/\n[footer_twitter]: https://twitter.com/ArtsyOpenSource\n[footer_api]: https://developers.artsy.net/\n[footer_jobs]: https://www.artsy.net/jobs\n',
     'author': 'Isac Petruzzi',
     'author_email': 'isac@artsymail.com',
     'maintainer': 'Jian-Feng Xu',
     'maintainer_email': 'jian-feng@artsymail.com',
     'url': 'http://github.com/artsy/hokusai',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['hokusai',
 'hokusai.cli', 'hokusai.commands', 'hokusai.lib', 'hokusai.services']
 package_data = \ {'': ['*'], 'hokusai': ['templates/*', 'templates/hokusai/*']}
 install_requires = \ ['Jinja2==3.1.1', 'MarkupSafe==2.1.1', 'PyYAML==6.0.1',
-'boto3==1.21.28', 'click-repl==0.2.0', 'click==8.1.0', 'packaging==21.3',
-'prompt-toolkit==3.0.28', 'termcolor==1.1.0'] entry_points = \
-{'console_scripts': ['hokusai = hokusai.command_line:main']} setup_kwargs =
-{ 'name': 'hokusai', 'version': '2.1.1', 'description': 'Artsy Docker
+'boto3>=1.34.25,<2.0.0', 'click-repl==0.2.0', 'click==8.1.0',
+'packaging==21.3', 'prompt-toolkit==3.0.28', 'termcolor==1.1.0'] entry_points =
+\ {'console_scripts': ['hokusai = hokusai.command_line:main']} setup_kwargs =
+{ 'name': 'hokusai', 'version': '2.2.0', 'description': 'Artsy Docker
 development toolkit', 'long_description': '## HOKUSAI [![CircleCI](https://
 circleci.com/gh/artsy/hokusai/tree/main.svg?style=svg)](https://circleci.com/
 gh/artsy/hokusai/tree/main)\n\n_[_h_o_k_u_s_a_i_._j_p_g_]\n\nHokusai is a Docker +
 Kubernetes CLI for application developers.\n\nHokusai "dockerizes" applications
 and manages their lifecycle throughout development, testing, and release
 cycles.\n\nHokusai wraps calls to [Kubectl](https://kubernetes.io/), [Docker]
 (https://www.docker.com/), [Docker-Compose](https://docs.docker.com/compose/
@@ -75,43 +75,45 @@
 `zlib` library. And make sure these libraries are correctly linked. Like so:
 \n\n```\nbrew install openssl readline zlib\n\necho \'export PATH="/usr/local/
 opt/openssl@1.1/bin:$PATH"\' >> ~/.bash_profile\necho \'export LDFLAGS="-L/usr/
 local/opt/openssl@1.1/lib"\' >> ~/.bash_profile\necho \'export CPPFLAGS="-I/
 usr/local/opt/openssl@1.1/include"\' >> ~/.bash_profile\necho \'export
 PKG_CONFIG_PATH="/usr/local/opt/openssl@1.1/lib/pkgconfig"\' >>
 ~/.bash_profile\n```\n\n### Python\n\nHokusai is currently tested on Python
-3.9.10 so we recommend using that Python version.\n\nIf you use Pyenv to
-install Python, you should see an output similar to this:\n\n```\npyenv install
-3.9.10\n\n python-build: use openssl from homebrew\n python-build: use readline
-from homebrew\n\n Downloading Python-3.9.10.tar.xz...\n -> https://
-www.python.org/ftp/python/3.9.10/Python-3.9.10.tar.xz\n Installing Python-
-3.9.10...\n python-build: use tcl-tk from homebrew\n python-build: use readline
-from homebrew\n python-build: use zlib from xcode sdk\n\n Installed Python-
-3.9.10 to $HOME/.pyenv/versions/3.9.10\n```\n\nWith the desired Python version
-installed, activate it globally:\n\n```\npyenv global 3.9.10\n```\n\nNote: If
-you want to create a PyInstaller distribution, Python must be installed with
-development libraries. Use the environment variable `PYTHON_CONFIGURE_OPTS="--
-enable-framework"` on Darwin and `PYTHON_CONFIGURE_OPTS="--enable-shared"` on
-Linux when running `pyenv install`.\n\n### Virtualenv\n\nWe recommend using a
-virtual environment to isolate Hokusai\'s dependencies from that of other
-projects on your local environment.\n\nThe Pyenv install comes with [pyenv-
-virtualenv](https://github.com/pyenv/pyenv-virtualenv) which can be used to
-create virtual environments.\n\n### Poetry\n\nUse [Poetry](https://python-
-poetry.org/) to install Hokusai\'s dependencies as well as Hokusai itself in
-[editable mode](https://pip-python3.readthedocs.io/en/latest/reference/
+3.10 so we recommend using that Python version.\n\nIf you use Pyenv to install
+Python, you should see an output similar to this:\n\n```\n$ pyenv install
+3.10\npython-build: use openssl@1.1 from homebrew\npython-build: use readline
+from homebrew\nDownloading Python-3.10.13.tar.xz...\n-> https://www.python.org/
+ftp/python/3.10.13/Python-3.10.13.tar.xz\nInstalling Python-3.10.13...\npython-
+build: use tcl-tk from homebrew\npython-build: use readline from
+homebrew\npython-build: use ncurses from homebrew\npython-build: use zlib from
+xcode sdk\nInstalled Python-3.10.13 to /Users/jxu/.pyenv/versions/
+3.10.13\n```\n\nWith the desired Python version installed, activate it
+globally:\n\n```\npyenv global 3.10\n```\n\nNote: If you want to create a
+PyInstaller distribution, Python must be installed with development libraries.
+Use the environment variable `PYTHON_CONFIGURE_OPTS="--enable-framework"` on
+Darwin and `PYTHON_CONFIGURE_OPTS="--enable-shared"` on Linux when running
+`pyenv install`.\n\n### Virtualenv\n\nWe recommend using a virtual environment
+to isolate Hokusai\'s dependencies from that of other projects on your local
+environment.\n\nThe Pyenv install comes with [pyenv-virtualenv](https://
+github.com/pyenv/pyenv-virtualenv) which can be used to create virtual
+environments.\n\n### Poetry\n\nUse [Poetry](https://python-poetry.org/) to
+install Hokusai\'s dependencies as well as Hokusai itself in [editable mode]
+(https://pip-python3.readthedocs.io/en/latest/reference/
 pip_install.html#editable-installs). Please see [this guide](https://python-
 poetry.org/docs/basic-usage/) for working with Poetry.\n\nInstall Poetry:
-\n\n```\npip install poetry\n```\n\nInstall dependencies and Hokusai in
-editable mode:\n\n```\npoetry install\n```\n\nTo update dependencies:
-\n\n```\npoetry lock\n```\n\n## Testing\n\n### Install Minikube\n\n[Minikube]
-(https://minikube.sigs.k8s.io/docs/start/) is used for integration
-tests.\n\n```\nbrew install minikube\nminikube start --kubernetes-
-version=\n```\n\n### Run tests\n\nTo run unit and smoke tests:\n\n```\nmake
-test\n```\n\nTo run integration tests:\n\n```\nmake integration\n```\n\nOnly
-specific modules, TestClasses, or even methods:\n\n```\npython -m unittest
+\n\n```\npip install --upgrade pip\npip install poetry\n```\n\nInstall
+dependencies and Hokusai in editable mode:\n\n```\npoetry install\n```\n\nTo
+update dependencies:\n\n```\npoetry lock\n```\n\n## Testing\n\n### Install
+Minikube\n\n[Minikube](https://minikube.sigs.k8s.io/docs/start/) is used for
+integration tests.\n\n```\nbrew install minikube\nminikube start --kubernetes-
+version=\n```\n\n### Run tests\n\nTo run unit tests:\n\n```\nmake
+test\n```\n\nTo run integration tests:\n\n```\nmake integration-
+local\n```\n\nOnly specific modules, TestClasses, or even methods:
+\n\n```\npython -m unittest
 test.unit.test_module.TestClass.test_method\n```\n\nTip: Set `DEBUG=1`
 environment variable to print boto logging\n\n\n## Distributing Hokusai\n\n###
 Beta Release\n\nMerging a branch into `main` automatically creates a beta
 version useful for testing. A [script](./scripts/update_version_file.sh) that
 runs in CI automatically generates a Beta version number and writes it into
 [VERSION](./hokusai/VERSION) file. The version number is based on the
 combination of the latest canonical version found in [RELEASE_VERSION](./
```

### Comparing `hokusai-2.1.1/PKG-INFO` & `hokusai-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hokusai
-Version: 2.1.1
+Version: 2.2.0
 Summary: Artsy Docker development toolkit
 Home-page: http://github.com/artsy/hokusai
 License: MIT
 Author: Isac Petruzzi
 Author-email: isac@artsymail.com
 Maintainer: Jian-Feng Xu
 Maintainer-email: jian-feng@artsymail.com
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Jinja2 (==3.1.1)
 Requires-Dist: MarkupSafe (==2.1.1)
 Requires-Dist: PyYAML (==6.0.1)
-Requires-Dist: boto3 (==1.21.28)
+Requires-Dist: boto3 (>=1.34.25,<2.0.0)
 Requires-Dist: click (==8.1.0)
 Requires-Dist: click-repl (==0.2.0)
 Requires-Dist: packaging (==21.3)
 Requires-Dist: prompt-toolkit (==3.0.28)
 Requires-Dist: termcolor (==1.1.0)
 Project-URL: Repository, http://github.com/artsy/hokusai
 Description-Content-Type: text/markdown
@@ -158,38 +158,36 @@
 echo 'export LDFLAGS="-L/usr/local/opt/openssl@1.1/lib"' >> ~/.bash_profile
 echo 'export CPPFLAGS="-I/usr/local/opt/openssl@1.1/include"' >> ~/.bash_profile
 echo 'export PKG_CONFIG_PATH="/usr/local/opt/openssl@1.1/lib/pkgconfig"' >> ~/.bash_profile
 ```
 
 ### Python
 
-Hokusai is currently tested on Python 3.9.10 so we recommend using that Python version.
+Hokusai is currently tested on Python 3.10 so we recommend using that Python version.
 
 If you use Pyenv to install Python, you should see an output similar to this:
 
 ```
-pyenv install 3.9.10
-
-    python-build: use openssl from homebrew
-    python-build: use readline from homebrew
-
-    Downloading Python-3.9.10.tar.xz...
-    -> https://www.python.org/ftp/python/3.9.10/Python-3.9.10.tar.xz
-    Installing Python-3.9.10...
-    python-build: use tcl-tk from homebrew
-    python-build: use readline from homebrew
-    python-build: use zlib from xcode sdk
-
-    Installed Python-3.9.10 to $HOME/.pyenv/versions/3.9.10
+$ pyenv install 3.10
+python-build: use openssl@1.1 from homebrew
+python-build: use readline from homebrew
+Downloading Python-3.10.13.tar.xz...
+-> https://www.python.org/ftp/python/3.10.13/Python-3.10.13.tar.xz
+Installing Python-3.10.13...
+python-build: use tcl-tk from homebrew
+python-build: use readline from homebrew
+python-build: use ncurses from homebrew
+python-build: use zlib from xcode sdk
+Installed Python-3.10.13 to /Users/jxu/.pyenv/versions/3.10.13
 ```
 
 With the desired Python version installed, activate it globally:
 
 ```
-pyenv global 3.9.10
+pyenv global 3.10
 ```
 
 Note: If you want to create a PyInstaller distribution, Python must be installed with development libraries. Use the environment variable `PYTHON_CONFIGURE_OPTS="--enable-framework"` on Darwin and `PYTHON_CONFIGURE_OPTS="--enable-shared"` on Linux when running `pyenv install`.
 
 ### Virtualenv
 
 We recommend using a virtual environment to isolate Hokusai's dependencies from that of other projects on your local environment.
@@ -199,14 +197,15 @@
 ### Poetry
 
 Use [Poetry](https://python-poetry.org/) to install Hokusai's dependencies as well as Hokusai itself in [editable mode](https://pip-python3.readthedocs.io/en/latest/reference/pip_install.html#editable-installs). Please see [this guide](https://python-poetry.org/docs/basic-usage/) for working with Poetry.
 
 Install Poetry:
 
 ```
+pip install --upgrade pip
 pip install poetry
 ```
 
 Install dependencies and Hokusai in editable mode:
 
 ```
 poetry install
@@ -227,24 +226,24 @@
 ```
 brew install minikube
 minikube start --kubernetes-version=<version of your Kubernetes clusters, example: v1.2.3>
 ```
 
 ### Run tests
 
-To run unit and smoke tests:
+To run unit tests:
 
 ```
 make test
 ```
 
 To run integration tests:
 
 ```
-make integration
+make integration-local
 ```
 
 Only specific modules, TestClasses, or even methods:
 
 ```
 python -m unittest test.unit.test_module.TestClass.test_method
 ```
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: hokusai Version: 2.1.1 Summary: Artsy Docker
+Metadata-Version: 2.1 Name: hokusai Version: 2.2.0 Summary: Artsy Docker
 development toolkit Home-page: http://github.com/artsy/hokusai License: MIT
 Author: Isac Petruzzi Author-email: isac@artsymail.com Maintainer: Jian-Feng Xu
 Maintainer-email: jian-feng@artsymail.com Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Dist: Jinja2
 (==3.1.1) Requires-Dist: MarkupSafe (==2.1.1) Requires-Dist: PyYAML (==6.0.1)
-Requires-Dist: boto3 (==1.21.28) Requires-Dist: click (==8.1.0) Requires-Dist:
-click-repl (==0.2.0) Requires-Dist: packaging (==21.3) Requires-Dist: prompt-
-toolkit (==3.0.28) Requires-Dist: termcolor (==1.1.0) Project-URL: Repository,
-http://github.com/artsy/hokusai Description-Content-Type: text/markdown ##
-HOKUSAI [![CircleCI](https://circleci.com/gh/artsy/hokusai/tree/
+Requires-Dist: boto3 (>=1.34.25,<2.0.0) Requires-Dist: click (==8.1.0)
+Requires-Dist: click-repl (==0.2.0) Requires-Dist: packaging (==21.3) Requires-
+Dist: prompt-toolkit (==3.0.28) Requires-Dist: termcolor (==1.1.0) Project-URL:
+Repository, http://github.com/artsy/hokusai Description-Content-Type: text/
+markdown ## HOKUSAI [![CircleCI](https://circleci.com/gh/artsy/hokusai/tree/
 main.svg?style=svg)](https://circleci.com/gh/artsy/hokusai/tree/main)
 _[_h_o_k_u_s_a_i_._j_p_g_]Hokusai is a Docker + Kubernetes CLI for application developers.
 Hokusai "dockerizes" applications and manages their lifecycle throughout
 development, testing, and release cycles. Hokusai wraps calls to [Kubectl]
 (https://kubernetes.io/), [Docker](https://www.docker.com/), [Docker-Compose]
 (https://docs.docker.com/compose/) and [Git](https://git-scm.com/) with a CLI,
 and defines a CI workflow. Hokusai currently only supports Kubernetes
@@ -73,59 +73,60 @@
 use brew-installed `openssl` and `readline` libraries, and xcode-installed
 `zlib` library. And make sure these libraries are correctly linked. Like so:
 ``` brew install openssl readline zlib echo 'export PATH="/usr/local/opt/
 openssl@1.1/bin:$PATH"' >> ~/.bash_profile echo 'export LDFLAGS="-L/usr/local/
 opt/openssl@1.1/lib"' >> ~/.bash_profile echo 'export CPPFLAGS="-I/usr/local/
 opt/openssl@1.1/include"' >> ~/.bash_profile echo 'export PKG_CONFIG_PATH="/
 usr/local/opt/openssl@1.1/lib/pkgconfig"' >> ~/.bash_profile ``` ### Python
-Hokusai is currently tested on Python 3.9.10 so we recommend using that Python
+Hokusai is currently tested on Python 3.10 so we recommend using that Python
 version. If you use Pyenv to install Python, you should see an output similar
-to this: ``` pyenv install 3.9.10 python-build: use openssl from homebrew
-python-build: use readline from homebrew Downloading Python-3.9.10.tar.xz... -
-> https://www.python.org/ftp/python/3.9.10/Python-3.9.10.tar.xz Installing
-Python-3.9.10... python-build: use tcl-tk from homebrew python-build: use
-readline from homebrew python-build: use zlib from xcode sdk Installed Python-
-3.9.10 to $HOME/.pyenv/versions/3.9.10 ``` With the desired Python version
-installed, activate it globally: ``` pyenv global 3.9.10 ``` Note: If you want
-to create a PyInstaller distribution, Python must be installed with development
-libraries. Use the environment variable `PYTHON_CONFIGURE_OPTS="--enable-
-framework"` on Darwin and `PYTHON_CONFIGURE_OPTS="--enable-shared"` on Linux
-when running `pyenv install`. ### Virtualenv We recommend using a virtual
-environment to isolate Hokusai's dependencies from that of other projects on
-your local environment. The Pyenv install comes with [pyenv-virtualenv](https:/
-/github.com/pyenv/pyenv-virtualenv) which can be used to create virtual
-environments. ### Poetry Use [Poetry](https://python-poetry.org/) to install
-Hokusai's dependencies as well as Hokusai itself in [editable mode](https://
-pip-python3.readthedocs.io/en/latest/reference/pip_install.html#editable-
-installs). Please see [this guide](https://python-poetry.org/docs/basic-usage/
-) for working with Poetry. Install Poetry: ``` pip install poetry ``` Install
+to this: ``` $ pyenv install 3.10 python-build: use openssl@1.1 from homebrew
+python-build: use readline from homebrew Downloading Python-3.10.13.tar.xz... -
+> https://www.python.org/ftp/python/3.10.13/Python-3.10.13.tar.xz Installing
+Python-3.10.13... python-build: use tcl-tk from homebrew python-build: use
+readline from homebrew python-build: use ncurses from homebrew python-build:
+use zlib from xcode sdk Installed Python-3.10.13 to /Users/jxu/.pyenv/versions/
+3.10.13 ``` With the desired Python version installed, activate it globally:
+``` pyenv global 3.10 ``` Note: If you want to create a PyInstaller
+distribution, Python must be installed with development libraries. Use the
+environment variable `PYTHON_CONFIGURE_OPTS="--enable-framework"` on Darwin and
+`PYTHON_CONFIGURE_OPTS="--enable-shared"` on Linux when running `pyenv
+install`. ### Virtualenv We recommend using a virtual environment to isolate
+Hokusai's dependencies from that of other projects on your local environment.
+The Pyenv install comes with [pyenv-virtualenv](https://github.com/pyenv/pyenv-
+virtualenv) which can be used to create virtual environments. ### Poetry Use
+[Poetry](https://python-poetry.org/) to install Hokusai's dependencies as well
+as Hokusai itself in [editable mode](https://pip-python3.readthedocs.io/en/
+latest/reference/pip_install.html#editable-installs). Please see [this guide]
+(https://python-poetry.org/docs/basic-usage/) for working with Poetry. Install
+Poetry: ``` pip install --upgrade pip pip install poetry ``` Install
 dependencies and Hokusai in editable mode: ``` poetry install ``` To update
 dependencies: ``` poetry lock ``` ## Testing ### Install Minikube [Minikube]
 (https://minikube.sigs.k8s.io/docs/start/) is used for integration tests. ```
 brew install minikube minikube start --kubernetes-version= ``` ### Run tests To
-run unit and smoke tests: ``` make test ``` To run integration tests: ``` make
-integration ``` Only specific modules, TestClasses, or even methods: ``` python
--m unittest test.unit.test_module.TestClass.test_method ``` Tip: Set `DEBUG=1`
-environment variable to print boto logging ## Distributing Hokusai ### Beta
-Release Merging a branch into `main` automatically creates a beta version
-useful for testing. A [script](./scripts/update_version_file.sh) that runs in
-CI automatically generates a Beta version number and writes it into [VERSION]
-(./hokusai/VERSION) file. The version number is based on the combination of the
-latest canonical version found in [RELEASE_VERSION](./hokusai/RELEASE_VERSION)
-file and the latest Git commit in `main` branch. [VERSION](./hokusai/VERSION)
-file in version control has just a dummy number (e.g. 999.999.999). To install
-the beta: #### MacOS ``` $ brew uninstall hokusai $ brew uninstall hokusai-beta
-$ brew update $ brew tap artsy/formulas $ brew install hokusai-beta ``` ####
-Linux ``` curl -sSL https://raw.githubusercontent.com/artsy/hokusai/main/get-
-hokusai.sh | sudo bash -s beta ``` ### Official Release To create an official
-release, such as `v1.2.3`, perform the following: - Create a branch named
-`prepare-v1.2.3` and make the following changes: - Bump canonical version in
-[RELEASE_VERSION](./hokusai/RELEASE_VERSION) file. - Upate [CHANGELOG](./
-CHANGELOG.md). - Open a PR to merge into `main`. Please see [past PRs](https://
-github.com/artsy/hokusai/
+run unit tests: ``` make test ``` To run integration tests: ``` make
+integration-local ``` Only specific modules, TestClasses, or even methods: ```
+python -m unittest test.unit.test_module.TestClass.test_method ``` Tip: Set
+`DEBUG=1` environment variable to print boto logging ## Distributing Hokusai
+### Beta Release Merging a branch into `main` automatically creates a beta
+version useful for testing. A [script](./scripts/update_version_file.sh) that
+runs in CI automatically generates a Beta version number and writes it into
+[VERSION](./hokusai/VERSION) file. The version number is based on the
+combination of the latest canonical version found in [RELEASE_VERSION](./
+hokusai/RELEASE_VERSION) file and the latest Git commit in `main` branch.
+[VERSION](./hokusai/VERSION) file in version control has just a dummy number
+(e.g. 999.999.999). To install the beta: #### MacOS ``` $ brew uninstall
+hokusai $ brew uninstall hokusai-beta $ brew update $ brew tap artsy/formulas $
+brew install hokusai-beta ``` #### Linux ``` curl -sSL https://
+raw.githubusercontent.com/artsy/hokusai/main/get-hokusai.sh | sudo bash -s beta
+``` ### Official Release To create an official release, such as `v1.2.3`,
+perform the following: - Create a branch named `prepare-v1.2.3` and make the
+following changes: - Bump canonical version in [RELEASE_VERSION](./hokusai/
+RELEASE_VERSION) file. - Upate [CHANGELOG](./CHANGELOG.md). - Open a PR to
+merge into `main`. Please see [past PRs](https://github.com/artsy/hokusai/
 pulls?q=is%3Apr+Release+is%3Aclosed+%22prepare+version%22) for example. - [Open
 a PR](https://github.com/artsy/hokusai/compare/release...main?expand=1) to
 merge `main` into `release`. Please see [past PRs](https://github.com/artsy/
 hokusai/pulls?q=is%3Apr+is%3Aclosed+%22release+version%22) for example. A CI
 [script](./scripts/update_version_file.sh) will copy the version in
 [RELEASE_VERSION](./hokusai/RELEASE_VERSION) file to [VERSION](./hokusai/
 VERSION) file. ## The Name The project is named for the great Japanese artist
```

