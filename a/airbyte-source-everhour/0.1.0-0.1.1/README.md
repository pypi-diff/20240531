# Comparing `tmp/airbyte-source-everhour-0.1.0.tar.gz` & `tmp/airbyte_source_everhour-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-everhour-0.1.0.tar", last modified: Tue Jan 30 17:36:06 2024, max compression
+gzip compressed data, was "airbyte_source_everhour-0.1.1.tar", max compression
```

## Comparing `airbyte-source-everhour-0.1.0.tar` & `airbyte_source_everhour-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 17:36:06.611291 airbyte-source-everhour-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     4204 2024-01-30 17:36:06.611291 airbyte-source-everhour-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4025 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 17:36:06.611291 airbyte-source-everhour-0.1.0/airbyte_source_everhour.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4204 2024-01-30 17:36:06.000000 airbyte-source-everhour-0.1.0/airbyte_source_everhour.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      950 2024-01-30 17:36:06.000000 airbyte-source-everhour-0.1.0/airbyte_source_everhour.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-30 17:36:06.000000 airbyte-source-everhour-0.1.0/airbyte_source_everhour.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-01-30 17:36:06.000000 airbyte-source-everhour-0.1.0/airbyte_source_everhour.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-30 17:36:06.000000 airbyte-source-everhour-0.1.0/airbyte_source_everhour.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2024-01-30 17:36:06.000000 airbyte-source-everhour-0.1.0/airbyte_source_everhour.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 17:36:06.607291 airbyte-source-everhour-0.1.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)      914 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/integration_tests/catalog.json
--rw-r--r--   0 root         (0) root         (0)     1347 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       93 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       27 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       63 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4066 2024-01-30 17:36:06.611291 airbyte-source-everhour-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      912 2024-01-30 17:36:04.000000 airbyte-source-everhour-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 17:36:06.611291 airbyte-source-everhour-0.1.0/source_everhour/
--rw-r--r--   0 root         (0) root         (0)      128 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/source_everhour/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2319 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/source_everhour/everhour.yaml
--rw-r--r--   0 root         (0) root         (0)      236 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/source_everhour/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 17:36:06.611291 airbyte-source-everhour-0.1.0/source_everhour/schemas/
--rw-r--r--   0 root         (0) root         (0)      999 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/source_everhour/schemas/clients.json
--rw-r--r--   0 root         (0) root         (0)     1185 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/source_everhour/schemas/projects.json
--rw-r--r--   0 root         (0) root         (0)     1108 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/source_everhour/schemas/tasks.json
--rw-r--r--   0 root         (0) root         (0)     2277 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/source_everhour/schemas/time.json
--rw-r--r--   0 root         (0) root         (0)     1892 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/source_everhour/schemas/time_records.json
--rw-r--r--   0 root         (0) root         (0)     2228 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/source_everhour/schemas/users.json
--rw-r--r--   0 root         (0) root         (0)      477 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/source_everhour/source.py
--rw-r--r--   0 root         (0) root         (0)      481 2024-01-30 17:32:07.000000 airbyte-source-everhour-0.1.0/source_everhour/spec.yaml
+-rw-r--r--   0        0        0     4532 2024-05-31 11:49:54.000000 airbyte_source_everhour-0.1.1/README.md
+-rw-r--r--   0        0        0      755 2024-05-31 12:16:17.207208 airbyte_source_everhour-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      128 2024-05-31 11:49:54.000000 airbyte_source_everhour-0.1.1/source_everhour/__init__.py
+-rw-r--r--   0        0        0     2319 2024-05-31 11:49:54.000000 airbyte_source_everhour-0.1.1/source_everhour/everhour.yaml
+-rw-r--r--   0        0        0      236 2024-05-31 11:49:54.000000 airbyte_source_everhour-0.1.1/source_everhour/run.py
+-rw-r--r--   0        0        0      999 2024-05-31 11:49:54.000000 airbyte_source_everhour-0.1.1/source_everhour/schemas/clients.json
+-rw-r--r--   0        0        0     1185 2024-05-31 11:49:54.000000 airbyte_source_everhour-0.1.1/source_everhour/schemas/projects.json
+-rw-r--r--   0        0        0     1108 2024-05-31 11:49:54.000000 airbyte_source_everhour-0.1.1/source_everhour/schemas/tasks.json
+-rw-r--r--   0        0        0     2277 2024-05-31 11:49:54.000000 airbyte_source_everhour-0.1.1/source_everhour/schemas/time.json
+-rw-r--r--   0        0        0     1892 2024-05-31 11:49:54.000000 airbyte_source_everhour-0.1.1/source_everhour/schemas/time_records.json
+-rw-r--r--   0        0        0     2228 2024-05-31 11:49:54.000000 airbyte_source_everhour-0.1.1/source_everhour/schemas/users.json
+-rw-r--r--   0        0        0      477 2024-05-31 11:49:54.000000 airbyte_source_everhour-0.1.1/source_everhour/source.py
+-rw-r--r--   0        0        0      481 2024-05-31 11:49:54.000000 airbyte_source_everhour-0.1.1/source_everhour/spec.yaml
+-rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 airbyte_source_everhour-0.1.1/PKG-INFO
```

### Comparing `airbyte-source-everhour-0.1.0/PKG-INFO` & `airbyte_source_everhour-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,91 @@
-Metadata-Version: 2.1
-Name: airbyte-source-everhour
-Version: 0.1.0
-Summary: Source implementation for Everhour.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
+# Everhour source connector
 
-# Everhour Source
 
-This is the repository for the Everhour configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/everhour).
+This is the repository for the Everhour source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/everhour).
 
+## Local development
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/everhour)
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/everhour)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_everhour/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source everhour test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-everhour spec
+poetry run source-everhour check --config secrets/config.json
+poetry run source-everhour discover --config secrets/config.json
+poetry run source-everhour read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-everhour build
 ```
 
-An image will be built with the tag `airbyte/source-everhour:dev`.
+An image will be available on your host with the tag `airbyte/source-everhour:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-everhour:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-everhour:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-everhour:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-everhour:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-everhour:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-everhour test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-everhour test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/everhour.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/everhour.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-everhour-0.1.0/source_everhour/everhour.yaml` & `airbyte_source_everhour-0.1.1/source_everhour/everhour.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-everhour-0.1.0/source_everhour/schemas/clients.json` & `airbyte_source_everhour-0.1.1/source_everhour/schemas/clients.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-everhour-0.1.0/source_everhour/schemas/projects.json` & `airbyte_source_everhour-0.1.1/source_everhour/schemas/projects.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-everhour-0.1.0/source_everhour/schemas/tasks.json` & `airbyte_source_everhour-0.1.1/source_everhour/schemas/tasks.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-everhour-0.1.0/source_everhour/schemas/time.json` & `airbyte_source_everhour-0.1.1/source_everhour/schemas/time.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-everhour-0.1.0/source_everhour/schemas/time_records.json` & `airbyte_source_everhour-0.1.1/source_everhour/schemas/time_records.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-everhour-0.1.0/source_everhour/schemas/users.json` & `airbyte_source_everhour-0.1.1/source_everhour/schemas/users.json`

 * *Files identical despite different names*

