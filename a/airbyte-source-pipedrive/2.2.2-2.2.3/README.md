# Comparing `tmp/airbyte-source-pipedrive-2.2.2.tar.gz` & `tmp/airbyte_source_pipedrive-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-pipedrive-2.2.2.tar", last modified: Thu Feb  1 13:53:32 2024, max compression
+gzip compressed data, was "airbyte_source_pipedrive-2.2.3.tar", max compression
```

## Comparing `airbyte-source-pipedrive-2.2.2.tar` & `airbyte_source_pipedrive-2.2.3.tar`

### file list

```diff
@@ -1,55 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 13:53:32.887150 airbyte-source-pipedrive-2.2.2/
--rw-r--r--   0 root         (0) root         (0)     4165 2024-02-01 13:53:32.887150 airbyte-source-pipedrive-2.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4043 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 13:53:32.887150 airbyte-source-pipedrive-2.2.2/airbyte_source_pipedrive.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4165 2024-02-01 13:53:32.000000 airbyte-source-pipedrive-2.2.2/airbyte_source_pipedrive.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1773 2024-02-01 13:53:32.000000 airbyte-source-pipedrive-2.2.2/airbyte_source_pipedrive.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 13:53:32.000000 airbyte-source-pipedrive-2.2.2/airbyte_source_pipedrive.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-02-01 13:53:32.000000 airbyte-source-pipedrive-2.2.2/airbyte_source_pipedrive.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-02-01 13:53:32.000000 airbyte-source-pipedrive-2.2.2/airbyte_source_pipedrive.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-02-01 13:53:32.000000 airbyte-source-pipedrive-2.2.2/airbyte_source_pipedrive.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 13:53:32.879150 airbyte-source-pipedrive-2.2.2/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2338 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     7631 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       79 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       79 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)      676 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4085 2024-02-01 13:53:32.887150 airbyte-source-pipedrive-2.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      897 2024-02-01 13:53:30.000000 airbyte-source-pipedrive-2.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 13:53:32.879150 airbyte-source-pipedrive-2.2.2/source_pipedrive/
--rw-r--r--   0 root         (0) root         (0)      130 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1982 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/extractor.py
--rw-r--r--   0 root         (0) root         (0)    11123 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      239 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 13:53:32.887150 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/
--rw-r--r--   0 root         (0) root         (0)     5269 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/activities.json
--rw-r--r--   0 root         (0) root         (0)     1862 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/activity_fields.json
--rw-r--r--   0 root         (0) root         (0)      758 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/activity_types.json
--rw-r--r--   0 root         (0) root         (0)      501 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/currencies.json
--rw-r--r--   0 root         (0) root         (0)     2308 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/deal_fields.json
--rw-r--r--   0 root         (0) root         (0)     1422 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/deal_products.json
--rw-r--r--   0 root         (0) root         (0)     3908 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/deals.json
--rw-r--r--   0 root         (0) root         (0)     2016 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/files.json
--rw-r--r--   0 root         (0) root         (0)      762 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/filters.json
--rw-r--r--   0 root         (0) root         (0)     1985 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/goals.json
--rw-r--r--   0 root         (0) root         (0)      372 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/lead_labels.json
--rw-r--r--   0 root         (0) root         (0)     1229 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/leads.json
--rw-r--r--   0 root         (0) root         (0)     2388 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/mail.json
--rw-r--r--   0 root         (0) root         (0)     1966 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/notes.json
--rw-r--r--   0 root         (0) root         (0)     2272 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/organization_fields.json
--rw-r--r--   0 root         (0) root         (0)     4589 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/organizations.json
--rw-r--r--   0 root         (0) root         (0)      372 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/permission_sets.json
--rw-r--r--   0 root         (0) root         (0)     1828 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/person_fields.json
--rw-r--r--   0 root         (0) root         (0)     4611 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/persons.json
--rw-r--r--   0 root         (0) root         (0)      709 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/pipelines.json
--rw-r--r--   0 root         (0) root         (0)     1847 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/product_fields.json
--rw-r--r--   0 root         (0) root         (0)     1730 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/products.json
--rw-r--r--   0 root         (0) root         (0)      573 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/roles.json
--rw-r--r--   0 root         (0) root         (0)      921 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/stages.json
--rw-r--r--   0 root         (0) root         (0)     1293 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/users.json
--rw-r--r--   0 root         (0) root         (0)      478 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/source_pipedrive/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 13:53:32.887150 airbyte-source-pipedrive-2.2.2/unit_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/unit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1200 2024-02-01 13:41:32.000000 airbyte-source-pipedrive-2.2.2/unit_tests/test_extractor.py
+-rw-r--r--   0        0        0     4550 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/README.md
+-rw-r--r--   0        0        0      732 2024-05-31 08:27:42.290608 airbyte_source_pipedrive-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0      130 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/__init__.py
+-rw-r--r--   0        0        0     1982 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/extractor.py
+-rw-r--r--   0        0        0    11123 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/manifest.yaml
+-rw-r--r--   0        0        0      239 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/run.py
+-rw-r--r--   0        0        0     5269 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/activities.json
+-rw-r--r--   0        0        0     1862 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/activity_fields.json
+-rw-r--r--   0        0        0      758 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/activity_types.json
+-rw-r--r--   0        0        0      501 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/currencies.json
+-rw-r--r--   0        0        0     2308 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/deal_fields.json
+-rw-r--r--   0        0        0     1422 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/deal_products.json
+-rw-r--r--   0        0        0     3908 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/deals.json
+-rw-r--r--   0        0        0     2016 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/files.json
+-rw-r--r--   0        0        0      762 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/filters.json
+-rw-r--r--   0        0        0     1985 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/goals.json
+-rw-r--r--   0        0        0      372 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/lead_labels.json
+-rw-r--r--   0        0        0     1229 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/leads.json
+-rw-r--r--   0        0        0     2388 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/mail.json
+-rw-r--r--   0        0        0     1966 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/notes.json
+-rw-r--r--   0        0        0     2272 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/organization_fields.json
+-rw-r--r--   0        0        0     4589 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/organizations.json
+-rw-r--r--   0        0        0      372 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/permission_sets.json
+-rw-r--r--   0        0        0     1828 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/person_fields.json
+-rw-r--r--   0        0        0     4611 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/persons.json
+-rw-r--r--   0        0        0      709 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/pipelines.json
+-rw-r--r--   0        0        0     1847 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/product_fields.json
+-rw-r--r--   0        0        0     1730 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/products.json
+-rw-r--r--   0        0        0      573 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/roles.json
+-rw-r--r--   0        0        0      921 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/stages.json
+-rw-r--r--   0        0        0     1293 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/users.json
+-rw-r--r--   0        0        0      478 2024-05-31 07:56:51.000000 airbyte_source_pipedrive-2.2.3/source_pipedrive/source.py
+-rw-r--r--   0        0        0     5261 1970-01-01 00:00:00.000000 airbyte_source_pipedrive-2.2.3/PKG-INFO
```

### Comparing `airbyte-source-pipedrive-2.2.2/PKG-INFO` & `airbyte_source_pipedrive-2.2.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,91 @@
-Metadata-Version: 2.1
-Name: airbyte-source-pipedrive
-Version: 2.2.2
-Summary: Source implementation for Pipedrive.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Provides-Extra: tests
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
+# Pipedrive source connector
 
-# Pipedrive Source
 
-This is the repository for the Pipedrive configuration based source connector.
+This is the repository for the Pipedrive source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/pipedrive).
 
+## Local development
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/pipedrive)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_pipedrive/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source pipedrive test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-pipedrive spec
+poetry run source-pipedrive check --config secrets/config.json
+poetry run source-pipedrive discover --config secrets/config.json
+poetry run source-pipedrive read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-pipedrive build
 ```
 
-An image will be built with the tag `airbyte/source-pipedrive:dev`.
+An image will be available on your host with the tag `airbyte/source-pipedrive:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-pipedrive:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-pipedrive:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pipedrive:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pipedrive:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-pipedrive:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-pipedrive test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-pipedrive test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/pipedrive.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/pipedrive.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-pipedrive-2.2.2/README.md` & `airbyte_source_pipedrive-2.2.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,110 @@
-# Pipedrive Source
+Metadata-Version: 2.1
+Name: airbyte-source-pipedrive
+Version: 2.2.3
+Summary: Source implementation for Pipedrive.
+Home-page: https://airbyte.com
+License: MIT
+Author: Airbyte
+Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (>=0,<1)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/pipedrive
+Project-URL: Repository, https://github.com/airbytehq/airbyte
+Description-Content-Type: text/markdown
 
-This is the repository for the Pipedrive configuration based source connector.
+# Pipedrive source connector
+
+
+This is the repository for the Pipedrive source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/pipedrive).
 
 ## Local development
 
-#### Create credentials
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/pipedrive)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_pipedrive/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source pipedrive test creds`
-and place them into `secrets/config.json`.
 
-### Locally running the connector docker image
+### Locally running the connector
+```
+poetry run source-pipedrive spec
+poetry run source-pipedrive check --config secrets/config.json
+poetry run source-pipedrive discover --config secrets/config.json
+poetry run source-pipedrive read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-pipedrive build
 ```
 
-An image will be built with the tag `airbyte/source-pipedrive:dev`.
+An image will be available on your host with the tag `airbyte/source-pipedrive:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-pipedrive:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-pipedrive:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pipedrive:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pipedrive:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-pipedrive:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-pipedrive test
 ```
 
 ### Customizing acceptance Tests
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-## Dependency Management
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
 
-### Publishing a new version of the connector
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-pipedrive test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/pipedrive.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/pipedrive.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/extractor.py` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/extractor.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/manifest.yaml` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/activities.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/activities.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/activity_fields.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/activity_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/activity_types.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/activity_types.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/deal_fields.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/deal_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/deal_products.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/deal_products.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/deals.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/deals.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/files.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/files.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/filters.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/filters.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/goals.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/goals.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/leads.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/leads.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/mail.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/mail.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/notes.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/notes.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/organization_fields.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/organization_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/organizations.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/organizations.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/person_fields.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/person_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/persons.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/persons.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/pipelines.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/pipelines.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/product_fields.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/product_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/products.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/roles.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/roles.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/stages.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/stages.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-pipedrive-2.2.2/source_pipedrive/schemas/users.json` & `airbyte_source_pipedrive-2.2.3/source_pipedrive/schemas/users.json`

 * *Files identical despite different names*

