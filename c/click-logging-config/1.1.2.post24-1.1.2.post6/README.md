# Comparing `tmp/click_logging_config-1.1.2.post24.tar.gz` & `tmp/click_logging_config-1.1.2.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_logging_config-1.1.2.post24.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "click_logging_config-1.1.2.post6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `click_logging_config-1.1.2.post24.tar` & `click_logging_config-1.1.2.post6.tar`

### file list

```diff
@@ -1,50 +1,43 @@
--rw-r--r--   0        0        0      103 2024-05-31 12:26:46.889392 click_logging_config-1.1.2.post24/.flake8
--rw-r--r--   0        0        0     2207 2024-05-31 12:26:46.889392 click_logging_config-1.1.2.post24/.gitignore
--rw-r--r--   0        0        0     3188 2024-05-31 12:26:46.889392 click_logging_config-1.1.2.post24/.gitlab-ci.yml
--rw-r--r--   0        0        0     1392 2024-05-31 12:26:46.889392 click_logging_config-1.1.2.post24/.gitlab-ci/build.yml
--rw-r--r--   0        0        0      236 2024-05-31 12:26:46.889392 click_logging_config-1.1.2.post24/.gitlab-ci/build_harness.yml
--rw-r--r--   0        0        0     1635 2024-05-31 12:26:46.889392 click_logging_config-1.1.2.post24/.gitlab-ci/docker.yml
--rw-r--r--   0        0        0     1313 2024-05-31 12:26:46.889392 click_logging_config-1.1.2.post24/.gitlab-ci/gitlab_runner_workaround.yml
--rw-r--r--   0        0        0     1685 2024-05-31 12:26:46.889392 click_logging_config-1.1.2.post24/.gitlab-ci/publish.yml
--rw-r--r--   0        0        0      243 2024-05-31 12:26:46.889392 click_logging_config-1.1.2.post24/.gitlab-ci/pyenv.yml
--rw-r--r--   0        0        0     1358 2024-05-31 12:26:46.890392 click_logging_config-1.1.2.post24/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1103 2024-05-31 12:26:46.890392 click_logging_config-1.1.2.post24/LICENSE.txt
--rw-r--r--   0        0        0      108 2024-05-31 12:26:46.890392 click_logging_config-1.1.2.post24/Makefile
--rw-r--r--   0        0        0     7432 2024-05-31 12:26:46.890392 click_logging_config-1.1.2.post24/README.rst
--rw-r--r--   0        0        0       13 2024-05-31 12:27:05.869379 click_logging_config-1.1.2.post24/click_logging_config/VERSION
--rw-r--r--   0        0        0      319 2024-05-31 12:26:46.890392 click_logging_config-1.1.2.post24/click_logging_config/__init__.py
--rw-r--r--   0        0        0     4896 2024-05-31 12:26:46.890392 click_logging_config-1.1.2.post24/click_logging_config/_click.py
--rw-r--r--   0        0        0      735 2024-05-31 12:26:46.890392 click_logging_config-1.1.2.post24/click_logging_config/_default_values.py
--rw-r--r--   0        0        0     7437 2024-05-31 12:26:46.890392 click_logging_config-1.1.2.post24/click_logging_config/_logging.py
--rw-r--r--   0        0        0      941 2024-05-31 12:26:46.890392 click_logging_config-1.1.2.post24/click_logging_config/_version.py
--rw-r--r--   0        0        0        0 2024-05-31 12:26:46.923392 click_logging_config-1.1.2.post24/click_logging_config/py.typed
--rw-r--r--   0        0        0     2078 2024-05-31 12:26:46.891392 click_logging_config-1.1.2.post24/docker/ci/Dockerfile
--rw-r--r--   0        0        0     1064 2024-05-31 12:26:46.891392 click_logging_config-1.1.2.post24/docker/ci/Dockerfile-apt-lock
--rw-r--r--   0        0        0      261 2024-05-31 12:26:46.891392 click_logging_config-1.1.2.post24/docker/ci/README.md
--rw-r--r--   0        0        0       24 2024-05-31 12:26:46.891392 click_logging_config-1.1.2.post24/docker/ci/apt1_requirements.lock
--rw-r--r--   0        0        0        5 2024-05-31 12:26:46.891392 click_logging_config-1.1.2.post24/docker/ci/apt1_requirements.txt
--rw-r--r--   0        0        0      311 2024-05-31 12:26:46.891392 click_logging_config-1.1.2.post24/docker/ci/apt2_requirements.lock
--rw-r--r--   0        0        0      160 2024-05-31 12:26:46.891392 click_logging_config-1.1.2.post24/docker/ci/apt2_requirements.txt
--rwxr-xr-x   0        0        0      855 2024-05-31 12:26:46.891392 click_logging_config-1.1.2.post24/docker/ci/get_versions.sh
--rw-r--r--   0        0        0       35 2024-05-31 12:26:46.891392 click_logging_config-1.1.2.post24/docker/ci/pyenv-python-versions
--rw-r--r--   0        0        0       46 2024-05-31 12:26:46.891392 click_logging_config-1.1.2.post24/docker/ci/requirements-dev.txt
--rw-r--r--   0        0        0     1250 2024-05-31 12:26:46.891392 click_logging_config-1.1.2.post24/docker/ci/tasks.py
--rw-r--r--   0        0        0     2027 2024-05-31 12:26:46.891392 click_logging_config-1.1.2.post24/pyproject.toml
--rw-r--r--   0        0        0      282 2024-05-31 12:26:46.891392 click_logging_config-1.1.2.post24/setup.cfg
--rw-r--r--   0        0        0      432 2024-05-31 12:26:46.891392 click_logging_config-1.1.2.post24/sonar-project.properties
--rw-r--r--   0        0        0      218 2024-05-31 12:26:46.892392 click_logging_config-1.1.2.post24/tests/__init__.py
--rw-r--r--   0        0        0      218 2024-05-31 12:26:46.892392 click_logging_config-1.1.2.post24/tests/ci/__init__.py
--rw-r--r--   0        0        0      218 2024-05-31 12:26:46.892392 click_logging_config-1.1.2.post24/tests/ci/integration_tests/__init__.py
--rw-r--r--   0        0        0     1256 2024-05-31 12:26:46.892392 click_logging_config-1.1.2.post24/tests/ci/integration_tests/conftest.py
--rw-r--r--   0        0        0     6454 2024-05-31 12:26:46.892392 click_logging_config-1.1.2.post24/tests/ci/integration_tests/test_logging_options.py
--rw-r--r--   0        0        0        0 2024-05-31 12:26:46.927392 click_logging_config-1.1.2.post24/tests/ci/support/__init__.py
--rw-r--r--   0        0        0      352 2024-05-31 12:26:46.892392 click_logging_config-1.1.2.post24/tests/ci/support/click_runner.py
--rw-r--r--   0        0        0      552 2024-05-31 12:26:46.892392 click_logging_config-1.1.2.post24/tests/ci/support/directory.py
--rw-r--r--   0        0        0      218 2024-05-31 12:26:46.892392 click_logging_config-1.1.2.post24/tests/ci/unit_tests/__init__.py
--rw-r--r--   0        0        0     1975 2024-05-31 12:26:46.893392 click_logging_config-1.1.2.post24/tests/ci/unit_tests/test_decorators.py
--rw-r--r--   0        0        0     1356 2024-05-31 12:26:46.893392 click_logging_config-1.1.2.post24/tests/ci/unit_tests/test_logging_configuration.py
--rw-r--r--   0        0        0     6314 2024-05-31 12:26:46.893392 click_logging_config-1.1.2.post24/tests/ci/unit_tests/test_logging_decorator.py
--rw-r--r--   0        0        0    13982 2024-05-31 12:26:46.893392 click_logging_config-1.1.2.post24/tests/ci/unit_tests/test_logging_state.py
--rw-r--r--   0        0        0     1530 2024-05-31 12:26:46.893392 click_logging_config-1.1.2.post24/tests/ci/unit_tests/test_version.py
--rw-r--r--   0        0        0      218 2024-05-31 12:26:46.893392 click_logging_config-1.1.2.post24/tests/manual/__init__.py
--rw-r--r--   0        0        0     8775 1970-01-01 00:00:00.000000 click_logging_config-1.1.2.post24/PKG-INFO
+-rw-r--r--   0        0        0      103 2024-01-03 18:19:26.255616 click_logging_config-1.1.2.post6/.flake8
+-rw-r--r--   0        0        0     2189 2024-01-03 18:19:26.255616 click_logging_config-1.1.2.post6/.gitignore
+-rw-r--r--   0        0        0     8242 2024-01-03 18:19:26.255616 click_logging_config-1.1.2.post6/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1358 2024-01-03 18:19:26.255616 click_logging_config-1.1.2.post6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1103 2024-01-03 18:19:26.255616 click_logging_config-1.1.2.post6/LICENSE.txt
+-rw-r--r--   0        0        0      108 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/Makefile
+-rw-r--r--   0        0        0     7432 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/README.rst
+-rw-r--r--   0        0        0       12 2024-01-03 18:19:41.744749 click_logging_config-1.1.2.post6/click_logging_config/VERSION
+-rw-r--r--   0        0        0      319 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/click_logging_config/__init__.py
+-rw-r--r--   0        0        0     4896 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/click_logging_config/_click.py
+-rw-r--r--   0        0        0      735 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/click_logging_config/_default_values.py
+-rw-r--r--   0        0        0     7437 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/click_logging_config/_logging.py
+-rw-r--r--   0        0        0      941 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/click_logging_config/_version.py
+-rw-r--r--   0        0        0        0 2024-01-03 18:19:26.280616 click_logging_config-1.1.2.post6/click_logging_config/py.typed
+-rw-r--r--   0        0        0     2012 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/docker/ci/Dockerfile
+-rw-r--r--   0        0        0     1064 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/docker/ci/Dockerfile-apt-lock
+-rw-r--r--   0        0        0      261 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/docker/ci/README.md
+-rw-r--r--   0        0        0       24 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/docker/ci/apt1_requirements.lock
+-rw-r--r--   0        0        0        5 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/docker/ci/apt1_requirements.txt
+-rw-r--r--   0        0        0      311 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/docker/ci/apt2_requirements.lock
+-rw-r--r--   0        0        0      160 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/docker/ci/apt2_requirements.txt
+-rwxr-xr-x   0        0        0      855 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/docker/ci/get_versions.sh
+-rw-r--r--   0        0        0       35 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/docker/ci/python-versions
+-rw-r--r--   0        0        0       46 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/docker/ci/requirements-dev.txt
+-rw-r--r--   0        0        0     1250 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/docker/ci/tasks.py
+-rw-r--r--   0        0        0     1989 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/pyproject.toml
+-rw-r--r--   0        0        0      282 2024-01-03 18:19:26.256616 click_logging_config-1.1.2.post6/setup.cfg
+-rw-r--r--   0        0        0      218 2024-01-03 18:19:26.257616 click_logging_config-1.1.2.post6/tests/__init__.py
+-rw-r--r--   0        0        0      218 2024-01-03 18:19:26.257616 click_logging_config-1.1.2.post6/tests/ci/__init__.py
+-rw-r--r--   0        0        0      218 2024-01-03 18:19:26.257616 click_logging_config-1.1.2.post6/tests/ci/integration_tests/__init__.py
+-rw-r--r--   0        0        0     1256 2024-01-03 18:19:26.257616 click_logging_config-1.1.2.post6/tests/ci/integration_tests/conftest.py
+-rw-r--r--   0        0        0     6454 2024-01-03 18:19:26.257616 click_logging_config-1.1.2.post6/tests/ci/integration_tests/test_logging_options.py
+-rw-r--r--   0        0        0        0 2024-01-03 18:19:26.283616 click_logging_config-1.1.2.post6/tests/ci/support/__init__.py
+-rw-r--r--   0        0        0      352 2024-01-03 18:19:26.257616 click_logging_config-1.1.2.post6/tests/ci/support/click_runner.py
+-rw-r--r--   0        0        0      552 2024-01-03 18:19:26.257616 click_logging_config-1.1.2.post6/tests/ci/support/directory.py
+-rw-r--r--   0        0        0      218 2024-01-03 18:19:26.257616 click_logging_config-1.1.2.post6/tests/ci/unit_tests/__init__.py
+-rw-r--r--   0        0        0     1975 2024-01-03 18:19:26.257616 click_logging_config-1.1.2.post6/tests/ci/unit_tests/test_decorators.py
+-rw-r--r--   0        0        0     1356 2024-01-03 18:19:26.257616 click_logging_config-1.1.2.post6/tests/ci/unit_tests/test_logging_configuration.py
+-rw-r--r--   0        0        0     6314 2024-01-03 18:19:26.257616 click_logging_config-1.1.2.post6/tests/ci/unit_tests/test_logging_decorator.py
+-rw-r--r--   0        0        0    13982 2024-01-03 18:19:26.257616 click_logging_config-1.1.2.post6/tests/ci/unit_tests/test_logging_state.py
+-rw-r--r--   0        0        0     1530 2024-01-03 18:19:26.257616 click_logging_config-1.1.2.post6/tests/ci/unit_tests/test_version.py
+-rw-r--r--   0        0        0      218 2024-01-03 18:19:26.257616 click_logging_config-1.1.2.post6/tests/manual/__init__.py
+-rw-r--r--   0        0        0     8770 1970-01-01 00:00:00.000000 click_logging_config-1.1.2.post6/PKG-INFO
```

### Comparing `click_logging_config-1.1.2.post24/.gitignore` & `click_logging_config-1.1.2.post6/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -142,9 +142,7 @@
 *.orig
 .idea/
 .pypirc
 # folder created by hadolint codequality reports
 reports/
 
 *_py
-
-.python-version*
```

### Comparing `click_logging_config-1.1.2.post24/.pre-commit-config.yaml` & `click_logging_config-1.1.2.post6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `click_logging_config-1.1.2.post24/LICENSE.txt` & `click_logging_config-1.1.2.post6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `click_logging_config-1.1.2.post24/README.rst` & `click_logging_config-1.1.2.post6/README.rst`

 * *Files identical despite different names*

### Comparing `click_logging_config-1.1.2.post24/click_logging_config/_click.py` & `click_logging_config-1.1.2.post6/click_logging_config/_click.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,10 +134,10 @@
 
             return ctx.invoke(
                 f,
                 *args,
                 **kwargs,
             )
 
-        return typing.cast(FC, functools.update_wrapper(wrapper, f))
+        return functools.update_wrapper(typing.cast(FC, wrapper), f)
 
     return decorator
```

### Comparing `click_logging_config-1.1.2.post24/click_logging_config/_default_values.py` & `click_logging_config-1.1.2.post6/click_logging_config/_default_values.py`

 * *Files identical despite different names*

### Comparing `click_logging_config-1.1.2.post24/click_logging_config/_logging.py` & `click_logging_config-1.1.2.post6/click_logging_config/_logging.py`

 * *Files identical despite different names*

### Comparing `click_logging_config-1.1.2.post24/click_logging_config/_version.py` & `click_logging_config-1.1.2.post6/click_logging_config/_version.py`

 * *Files identical despite different names*

### Comparing `click_logging_config-1.1.2.post24/docker/ci/Dockerfile` & `click_logging_config-1.1.2.post6/docker/ci/Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -35,22 +35,21 @@
     https://raw.githubusercontent.com/pyenv/pyenv-installer/master/bin/pyenv-installer \
     > /pyenv-installer"
 
 
 # python:3.8-slim
 FROM python@sha256:f8a12edddd4fb9c9fd38cd7147c5861a596dee5a4852b6bded3d1d6e2c8987bd
 
-ARG python_version
 ARG requirements_lock=/tmp/apt_requirements.lock
 ARG venv_path
 
 COPY docker/ci/apt2_requirements.lock "${requirements_lock}"
 
 COPY --from=pyenv /pyenv-installer /pyenv-installer
-COPY docker/ci/pyenv-python-versions /pyenv-python-versions
+COPY docker/ci/python-versions /python-versions
 
 ENV PYENV_ROOT="/root/.pyenv"
 
 RUN /bin/bash -c \
   "set -ex; \
   apt-get update; \
   xargs -a \"${requirements_lock}\" \
@@ -58,12 +57,12 @@
       -y \
       --no-install-recommends; \
   rm -rf /var/lib/apt/lists/*; \
   git config --global user.email \"you@example.com\"; \
   git config --global user.name \"Your Name\"; \
   source /pyenv-installer; \
   command -v pyenv >/dev/null || export PATH=\"\${PYENV_ROOT}/bin:\${PATH}\"; \
-  for x in \$(cat /pyenv-python-versions | grep \"${python_version}\"); do \
+  for x in \$(cat /python-versions); do \
     pyenv install \${x}; \
   done"
 
 COPY --from=venv "${venv_path}" "${venv_path}"
```

### Comparing `click_logging_config-1.1.2.post24/docker/ci/Dockerfile-apt-lock` & `click_logging_config-1.1.2.post6/docker/ci/Dockerfile-apt-lock`

 * *Files identical despite different names*

### Comparing `click_logging_config-1.1.2.post24/docker/ci/get_versions.sh` & `click_logging_config-1.1.2.post6/docker/ci/get_versions.sh`

 * *Files identical despite different names*

### Comparing `click_logging_config-1.1.2.post24/docker/ci/tasks.py` & `click_logging_config-1.1.2.post6/docker/ci/tasks.py`

 * *Files identical despite different names*

### Comparing `click_logging_config-1.1.2.post24/pyproject.toml` & `click_logging_config-1.1.2.post6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 [build-system]
 build-backend = "flit_core.buildapi"
-requires = ["flit_core >=3.2,<4"]
+requires = ["flit_core >=2,<4"]
 
 
-[project]
-authors = [{ name = "Russell Smiley", email = "russell@bytingchipmunk.com" }]
+[tool.flit.metadata]
+author = "Russell Smiley"
+author-email = "russell@bytingchipmunk.com"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Typing :: Typed",
 ]
-dynamic = ["description", "version"]
-name = "click_logging_config"
-readme = "README.rst"
+description-file = "README.rst"
+home-page = "https://gitlab.com/ci-cd-devops/click_logging_config"
+module = "click_logging_config"
 
 # Drop support for EOL Python versions
 # https://devguide.python.org/versions/
 requires-python = ">=3.8"
 
-dependencies = [
+requires = [
     "click >=8.1.3, <9",
-    "json_log_formatter >=1.0, <2",
+    "json_log_formatter >=0.5.1, <1",
     "pendulum >=3.0, <4",
-    "pydantic >=1.10.2, <3",
-    "pytz >=2024.1",
+    "pydantic >=1.10.2, <2",
+    "pytz >=2022.6",
 ]
 
 
-[project.urls]
-Source = "https://gitlab.com/ci-cd-devops/click_logging_config"
-
-
-[project.optional-dependencies]
+[tool.flit.metadata.requires-extra]
 dev = [
-    "build_harness >=2.4.0, <3",
+    "build_harness >=2, <3",
     "invoke >=2.2.0, <3",
     # NOTE: currently need low 2.17 release until build-harness updates it's
     #       pre-commit dependency range.
     "pre_commit >=2.17, <4",
-    "types-pytz >=2024.1.0",
+    "types-pytz >=2023.3.1.1",
 ]
 doc = [
     "sphinx <7.2.6; python_version < '3.9'",
     "sphinx >=7.2.6, <8; python_version >= '3.9'",
     "sphinx_rtd_theme >=2.0, <3",
 ]
 test = [
```

### Comparing `click_logging_config-1.1.2.post24/tests/ci/integration_tests/conftest.py` & `click_logging_config-1.1.2.post6/tests/ci/integration_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `click_logging_config-1.1.2.post24/tests/ci/integration_tests/test_logging_options.py` & `click_logging_config-1.1.2.post6/tests/ci/integration_tests/test_logging_options.py`

 * *Files identical despite different names*

### Comparing `click_logging_config-1.1.2.post24/tests/ci/support/directory.py` & `click_logging_config-1.1.2.post6/tests/ci/support/directory.py`

 * *Files identical despite different names*

### Comparing `click_logging_config-1.1.2.post24/tests/ci/unit_tests/test_decorators.py` & `click_logging_config-1.1.2.post6/tests/ci/unit_tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `click_logging_config-1.1.2.post24/tests/ci/unit_tests/test_logging_configuration.py` & `click_logging_config-1.1.2.post6/tests/ci/unit_tests/test_logging_configuration.py`

 * *Files identical despite different names*

### Comparing `click_logging_config-1.1.2.post24/tests/ci/unit_tests/test_logging_decorator.py` & `click_logging_config-1.1.2.post6/tests/ci/unit_tests/test_logging_decorator.py`

 * *Files identical despite different names*

### Comparing `click_logging_config-1.1.2.post24/tests/ci/unit_tests/test_logging_state.py` & `click_logging_config-1.1.2.post6/tests/ci/unit_tests/test_logging_state.py`

 * *Files identical despite different names*

### Comparing `click_logging_config-1.1.2.post24/tests/ci/unit_tests/test_version.py` & `click_logging_config-1.1.2.post6/tests/ci/unit_tests/test_version.py`

 * *Files identical despite different names*

### Comparing `click_logging_config-1.1.2.post24/PKG-INFO` & `click_logging_config-1.1.2.post6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: click_logging_config
-Version: 1.1.2.post24
+Version: 1.1.2.post6
 Summary: Quick and easy logging parameters for click commands.
-Author-email: Russell Smiley <russell@bytingchipmunk.com>
+Home-page: https://gitlab.com/ci-cd-devops/click_logging_config
+Author: Russell Smiley
+Author-email: russell@bytingchipmunk.com
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
 Requires-Dist: click >=8.1.3, <9
-Requires-Dist: json_log_formatter >=1.0, <2
+Requires-Dist: json_log_formatter >=0.5.1, <1
 Requires-Dist: pendulum >=3.0, <4
-Requires-Dist: pydantic >=1.10.2, <3
-Requires-Dist: pytz >=2024.1
-Requires-Dist: build_harness >=2.4.0, <3 ; extra == "dev"
+Requires-Dist: pydantic >=1.10.2, <2
+Requires-Dist: pytz >=2022.6
+Requires-Dist: build_harness >=2, <3 ; extra == "dev"
 Requires-Dist: invoke >=2.2.0, <3 ; extra == "dev"
 Requires-Dist: pre_commit >=2.17, <4 ; extra == "dev"
-Requires-Dist: types-pytz >=2024.1.0 ; extra == "dev"
+Requires-Dist: types-pytz >=2023.3.1.1 ; extra == "dev"
 Requires-Dist: sphinx <7.2.6 ; extra == "doc" and ( python_version < '3.9')
 Requires-Dist: sphinx >=7.2.6, <8 ; extra == "doc" and ( python_version >= '3.9')
 Requires-Dist: sphinx_rtd_theme >=2.0, <3 ; extra == "doc"
 Requires-Dist: pytest >=7.4.3, <8 ; extra == "test"
 Requires-Dist: pytest-cov >=4.1, <5 ; extra == "test"
 Requires-Dist: pytest-mock >=3.12.0, <4 ; extra == "test"
-Project-URL: Source, https://gitlab.com/ci-cd-devops/click_logging_config
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 
 click-logging-config
 ====================
```

