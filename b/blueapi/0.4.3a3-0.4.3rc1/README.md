# Comparing `tmp/blueapi-0.4.3a3.tar.gz` & `tmp/blueapi-0.4.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueapi-0.4.3a3.tar", last modified: Fri May 17 08:26:32 2024, max compression
+gzip compressed data, was "blueapi-0.4.3rc1.tar", last modified: Fri May 31 16:27:18 2024, max compression
```

## Comparing `blueapi-0.4.3a3.tar` & `blueapi-0.4.3rc1.tar`

### file list

```diff
@@ -1,200 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.561314 blueapi-0.4.3a3/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.533314 blueapi-0.4.3a3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.533314 blueapi-0.4.3a3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.529314 blueapi-0.4.3a3/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.533314 blueapi-0.4.3a3/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.533314 blueapi-0.4.3a3/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     2722 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.537314 blueapi-0.4.3a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/workflows/_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/workflows/_container.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/workflows/_dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/workflows/_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/workflows/_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/workflows/_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/workflows/_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/workflows/_tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/workflows/asyncapi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/workflows/backstage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/workflows/helm.yml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.github/workflows/periodic.yml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.537314 blueapi-0.4.3a3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17015 2024-05-17 08:26:32.561314 blueapi-0.4.3a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/catalog-info.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/codecov.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      312 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/container-startup.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.537314 blueapi-0.4.3a3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.537314 blueapi-0.4.3a3/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/explanations/architecture.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.541314 blueapi-0.4.3a3/docs/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/explanations/decisions/0001-record-architecture-decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/explanations/decisions/0002-switched-to-python-copier-template.md
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/explanations/decisions/0003-no-queues.rst
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/explanations/decisions/0004-api-case.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/explanations/decisions/COPYME
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/explanations/decisions.md
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/explanations/events.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/explanations/lifecycle.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/explanations/type_validators.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/explanations.md
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/genindex.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.541314 blueapi-0.4.3a3/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/how-to/add-plans-and-devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/how-to/configure-app.rst
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/how-to/contribute.md
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/how-to/run-cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9815 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/how-to/write-plans.rst
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/how-to.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.541314 blueapi-0.4.3a3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)   236122 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/images/blueapi-architecture.png
--rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/images/blueapi-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   386340 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/images/blueapi.png
--rw-r--r--   0 runner    (1001) docker     (127)   304331 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/images/bluesky-events.png
--rw-r--r--   0 runner    (1001) docker     (127)    16967 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/images/debug-vscode.png
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.545314 blueapi-0.4.3a3/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/reference/asyncapi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/reference/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/reference/messaging-spec.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/reference/openapi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/reference/rest-spec.rst
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/reference.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.545314 blueapi-0.4.3a3/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/tutorials/dev-run.rst
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/tutorials/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/tutorials/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/docs/tutorials.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.529314 blueapi-0.4.3a3/helm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.545314 blueapi-0.4.3a3/helm/blueapi/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/helm/blueapi/.helmignore
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/helm/blueapi/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.545314 blueapi-0.4.3a3/helm/blueapi/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/helm/blueapi/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/helm/blueapi/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/helm/blueapi/templates/configmap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/helm/blueapi/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/helm/blueapi/templates/ingress.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/helm/blueapi/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/helm/blueapi/templates/serviceaccount.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.545314 blueapi-0.4.3a3/helm/blueapi/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/helm/blueapi/templates/tests/test-ping.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/helm/blueapi/values.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 08:26:32.561314 blueapi-0.4.3a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.529314 blueapi-0.4.3a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.549314 blueapi-0.4.3a3/src/blueapi/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-17 08:26:32.000000 blueapi-0.4.3a3/src/blueapi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.549314 blueapi-0.4.3a3/src/blueapi/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/cli/event_bus_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/cli/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/cli/updates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.549314 blueapi-0.4.3a3/src/blueapi/core/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/core/bluesky_event_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/core/bluesky_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/core/device_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/core/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.553314 blueapi-0.4.3a3/src/blueapi/messaging/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/messaging/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/messaging/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/messaging/stomptemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/messaging/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.553314 blueapi-0.4.3a3/src/blueapi/service/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/service/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/service/handler_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/service/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/service/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/service/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/service/subprocess_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.553314 blueapi-0.4.3a3/src/blueapi/startup/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/startup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/startup/example_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/startup/example_plans.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/startup/simmotor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.553314 blueapi-0.4.3a3/src/blueapi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/utils/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/utils/invalid_config_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/utils/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/utils/thread_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.553314 blueapi-0.4.3a3/src/blueapi/worker/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/worker/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/worker/multithread.py
--rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/worker/reworker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/worker/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/src/blueapi/worker/worker_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.561314 blueapi-0.4.3a3/src/blueapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17015 2024-05-17 08:26:32.000000 blueapi-0.4.3a3/src/blueapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-17 08:26:32.000000 blueapi-0.4.3a3/src/blueapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:26:32.000000 blueapi-0.4.3a3/src/blueapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-17 08:26:32.000000 blueapi-0.4.3a3/src/blueapi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-17 08:26:32.000000 blueapi-0.4.3a3/src/blueapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 08:26:32.000000 blueapi-0.4.3a3/src/blueapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.557314 blueapi-0.4.3a3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.557314 blueapi-0.4.3a3/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/core/fake_device_module.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/core/fake_plan_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/core/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/core/test_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.557314 blueapi-0.4.3a3/tests/example_yaml/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/example_yaml/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/example_yaml/nested_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/example_yaml/override_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/example_yaml/rest_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/example_yaml/valid_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/example_yaml/valid_stomp_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.557314 blueapi-0.4.3a3/tests/messaging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/messaging/test_stomptemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/messaging/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.557314 blueapi-0.4.3a3/tests/service/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/service/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/service/test_openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/service/test_rest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/service/test_subprocess_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.561314 blueapi-0.4.3a3/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/utils/hasall.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/utils/lacksall.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/utils/test_base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/utils/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/utils/test_thread_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:26:32.561314 blueapi-0.4.3a3/tests/worker/
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/worker/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-05-17 08:26:26.000000 blueapi-0.4.3a3/tests/worker/test_reworker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.548254 blueapi-0.4.3rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.524253 blueapi-0.4.3rc1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.524253 blueapi-0.4.3rc1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.516254 blueapi-0.4.3rc1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.524253 blueapi-0.4.3rc1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.524253 blueapi-0.4.3rc1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2722 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.524253 blueapi-0.4.3rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/workflows/_container.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/workflows/_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/workflows/asyncapi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/workflows/backstage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/workflows/helm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.github/workflows/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.524253 blueapi-0.4.3rc1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-05-31 16:27:18.548254 blueapi-0.4.3rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/catalog-info.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/codecov.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/container-startup.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.528254 blueapi-0.4.3rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.528254 blueapi-0.4.3rc1/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/explanations/architecture.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.528254 blueapi-0.4.3rc1/docs/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/explanations/decisions/0001-record-architecture-decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/explanations/decisions/0002-switched-to-python-copier-template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/explanations/decisions/0003-no-queues.md
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/explanations/decisions/0004-api-case.md
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/explanations/decisions/COPYME
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/explanations/decisions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/explanations/events.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/explanations/lifecycle.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/explanations/type_validators.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/explanations.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/genindex.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.528254 blueapi-0.4.3rc1/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/how-to/add-plans-and-devices.md
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/how-to/configure-app.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/how-to/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/how-to/run-cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/how-to/run-container.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/how-to/write-plans.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/how-to.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.532254 blueapi-0.4.3rc1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   236122 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/images/blueapi-architecture.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/images/blueapi-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   386340 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/images/blueapi.png
+-rw-r--r--   0 runner    (1001) docker     (127)   304331 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/images/bluesky-events.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16967 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/images/debug-vscode.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.532254 blueapi-0.4.3rc1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/reference/asyncapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/reference/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/reference/messaging-spec.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13612 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/reference/openapi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/reference/rest-spec.md
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/reference.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.532254 blueapi-0.4.3rc1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/tutorials/dev-run.md
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/tutorials/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/tutorials/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/docs/tutorials.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.520254 blueapi-0.4.3rc1/helm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.532254 blueapi-0.4.3rc1/helm/blueapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/helm/blueapi/.helmignore
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/helm/blueapi/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.532254 blueapi-0.4.3rc1/helm/blueapi/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/helm/blueapi/templates/NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/helm/blueapi/templates/_helpers.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/helm/blueapi/templates/configmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/helm/blueapi/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/helm/blueapi/templates/ingress.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/helm/blueapi/templates/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/helm/blueapi/templates/serviceaccount.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.536254 blueapi-0.4.3rc1/helm/blueapi/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/helm/blueapi/templates/tests/test-ping.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/helm/blueapi/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 16:27:18.548254 blueapi-0.4.3rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.520254 blueapi-0.4.3rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.536254 blueapi-0.4.3rc1/src/blueapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-31 16:27:18.000000 blueapi-0.4.3rc1/src/blueapi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.536254 blueapi-0.4.3rc1/src/blueapi/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/cli/event_bus_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/cli/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/cli/updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5235 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.536254 blueapi-0.4.3rc1/src/blueapi/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/core/bluesky_event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/core/bluesky_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/core/device_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/core/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.540253 blueapi-0.4.3rc1/src/blueapi/messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/messaging/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/messaging/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/messaging/stomptemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/messaging/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.540253 blueapi-0.4.3rc1/src/blueapi/service/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/service/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/service/handler_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/service/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/service/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/service/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/service/subprocess_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.540253 blueapi-0.4.3rc1/src/blueapi/startup/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/startup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/startup/example_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/startup/example_plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/startup/simmotor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.540253 blueapi-0.4.3rc1/src/blueapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/utils/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/utils/invalid_config_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/utils/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/utils/thread_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.540253 blueapi-0.4.3rc1/src/blueapi/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/worker/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/worker/multithread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13532 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/worker/reworker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/worker/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/src/blueapi/worker/worker_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.548254 blueapi-0.4.3rc1/src/blueapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17016 2024-05-31 16:27:18.000000 blueapi-0.4.3rc1/src/blueapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-31 16:27:18.000000 blueapi-0.4.3rc1/src/blueapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 16:27:18.000000 blueapi-0.4.3rc1/src/blueapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 16:27:18.000000 blueapi-0.4.3rc1/src/blueapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-31 16:27:18.000000 blueapi-0.4.3rc1/src/blueapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 16:27:18.000000 blueapi-0.4.3rc1/src/blueapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.544254 blueapi-0.4.3rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.544254 blueapi-0.4.3rc1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/core/fake_device_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/core/fake_device_module_failing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/core/fake_plan_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11828 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/core/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/core/test_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.544254 blueapi-0.4.3rc1/tests/example_yaml/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/example_yaml/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/example_yaml/nested_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/example_yaml/override_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/example_yaml/rest_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/example_yaml/valid_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/example_yaml/valid_stomp_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.544254 blueapi-0.4.3rc1/tests/messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/messaging/test_stomptemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/messaging/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.544254 blueapi-0.4.3rc1/tests/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/service/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/service/test_openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/service/test_rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/service/test_subprocess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.544254 blueapi-0.4.3rc1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/utils/hasall.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/utils/lacksall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/utils/test_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/utils/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/utils/test_thread_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 16:27:18.548254 blueapi-0.4.3rc1/tests/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/worker/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12971 2024-05-31 16:27:14.000000 blueapi-0.4.3rc1/tests/worker/test_reworker.py
```

### Comparing `blueapi-0.4.3a3/.devcontainer/devcontainer.json` & `blueapi-0.4.3rc1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/.github/CONTRIBUTING.md` & `blueapi-0.4.3rc1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/.github/actions/install_requirements/action.yml` & `blueapi-0.4.3rc1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/.github/dependabot.yml` & `blueapi-0.4.3rc1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/.github/pages/make_switcher.py` & `blueapi-0.4.3rc1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/.github/workflows/_check.yml` & `blueapi-0.4.3rc1/.github/workflows/_check.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/.github/workflows/_container.yml` & `blueapi-0.4.3rc1/.github/workflows/_container.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/.github/workflows/_dist.yml` & `blueapi-0.4.3rc1/.github/workflows/_dist.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/.github/workflows/_docs.yml` & `blueapi-0.4.3rc1/.github/workflows/_docs.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/.github/workflows/_release.yml` & `blueapi-0.4.3rc1/.github/workflows/_release.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/.github/workflows/_test.yml` & `blueapi-0.4.3rc1/.github/workflows/_test.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/.github/workflows/ci.yml` & `blueapi-0.4.3rc1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/.github/workflows/helm.yml` & `blueapi-0.4.3rc1/.github/workflows/helm.yml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/.gitignore` & `blueapi-0.4.3rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/.pre-commit-config.yaml` & `blueapi-0.4.3rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/.vscode/launch.json` & `blueapi-0.4.3rc1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/Dockerfile` & `blueapi-0.4.3rc1/Dockerfile`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/LICENSE` & `blueapi-0.4.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/PKG-INFO` & `blueapi-0.4.3rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapi
-Version: 0.4.3a3
+Version: 0.4.3rc1
 Summary: Lightweight bluesky-as-a-service wrapper application. Also usable as a library.
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `blueapi-0.4.3a3/README.md` & `blueapi-0.4.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/catalog-info.yaml` & `blueapi-0.4.3rc1/catalog-info.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/docs/conf.py` & `blueapi-0.4.3rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/docs/explanations/architecture.rst` & `blueapi-0.4.3rc1/docs/explanations/architecture.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,34 @@
-Architecture
-============
+# Architecture
+
 
 Blueapi performs a number of tasks:
 
-* Managing the Bluesky RunEngine_, giving it instructions and handling its errors. Traditionally this job has been done by a human with an IPython_ terminal, so it requires automating.
+* Managing the Bluesky [RunEngine](https://nsls-ii.github.io/bluesky/run_engine_api.html), giving it instructions and handling its errors. Traditionally this job has been done by a human with an [IPython](https://ipython.org/) terminal, so it requires automating.
 * Maintaining a registry of plans and devices. In the aforementioned IPython_ case, these would have just been global variables.
 * Communicating with the outside world, accepting instructions to run plans, providing updates on plan progress etc.
 
 These responsibilities are kept separate in the codebase to ensure a clean, maintainable architecture.
 
-Key Components
---------------
+## Key Components
 
-.. figure:: ../images/blueapi-architecture.png
-    :width: 600px
-    :align: center
 
-    main components
+![blueapi architecture main components](../images/blueapi-architecture.png)
 
 
-The ``BlueskyContext`` Object
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+### The `BlueskyContext` Object
 
 Holds registries of plans and devices as well as a number of helper methods for 
 registering en-masse from a normal Python module. 
 
+### The Worker Object
 
-The Worker Object
-^^^^^^^^^^^^^^^^^
-
-Wraps the Bluesky ``RunEngine`` and accepts requests to run plans. The requests include the name 
+Wraps the Bluesky `RunEngine` and accepts requests to run plans. The requests include the name 
 of the plan and a dictionary of parameters to pass. The worker validates the parameters against
-the known expectations of the plan, passes it to the ``RunEngine`` and handles any errors.
+the known expectations of the plan, passes it to the `RunEngine` and handles any errors.
 
 
-The Service Object
-^^^^^^^^^^^^^^^^^^
+### The Service Object
 
 Handles communications and the API layer. This object holds a reference to the worker 
 can interrogate it/give it instructions in response to messages it recieves from the message
 bus. It can also forward the various events generated by the worker to topics on the bus.
-
-
-.. _RunEngine: https://nsls-ii.github.io/bluesky/run_engine_api.html
-.. _IPython: https://ipython.org/
```

### Comparing `blueapi-0.4.3a3/docs/explanations/decisions/0002-switched-to-python-copier-template.md` & `blueapi-0.4.3rc1/docs/explanations/decisions/0002-switched-to-python-copier-template.md`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/docs/explanations/events.rst` & `blueapi-0.4.3rc1/docs/explanations/events.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,51 @@
-Events Emitted by the Worker
-============================
+# Events Emitted by the Worker
 
-Blueapi adds new events on top of the `bluesky event model`_.
+Blueapi adds new events on top of the [`bluesky event model`](https://blueskyproject.io/event-model/main/index.html).
 
-Reasons
--------
+## Reasons
 
-Since the ``RunEngine`` is traditionally used by a human in front of an IPython terminal, it
+
+Since the `RunEngine` is traditionally used by a human in front of an IPython terminal, it
 sometimes assumes intuitive behaviour. The worker replaces the human and so must fill in the
 gaps.
 
 The base engine programatically emits data events conforming to the `bluesky event model`_. These
 are meant to be handled by other subscribing code (e.g. databroker) and are decoupled from concerns such as whether
 a plan has started, finished, paused, errored etc. See the example below:
 
-.. figure:: ../images/bluesky-events.png
-    :width: 600px
-    :align: center
-
-    sequence of event emission compared to plan start/finish, in a complicated case
+![sequence of event emission compared to plan start/finish, in a complicated case](../images/bluesky-events.png)
 
-Note the gap between the start of the plan and the issue of the first `run start document`_, and the similar gap
+Note the gap between the start of the plan and the issue of the first [`run start document`](https://blueskyproject.io/event-model/main/user/explanations/data-model.html#run-start-document), and the similar gap
 for the stop document vs end of the plan, thsse are typically used for setup and cleanup. 
 Also note that a plan can produce an arbitrary number of runs. This decoupling is fine in an IPython terminal
 because a human user can see when a plan has started, can see when it's finished and can see which runs are
 associated with which plans.
 
-New Events
-----------
+## New Events
 
 For the case of automation, we introduce a new set of events outside of the event model, specifically
-pertaining to the running of the plan and state of the ``RunEngine``. At a mimimum, an event is emitted
+pertaining to the running of the plan and state of the `RunEngine`. At a mimimum, an event is emitted
 every time the engine:
 
 * Starts a new plan
 * Completes a plan
 * Fails/errors
 
 In the latter case, information about the error is also included.
 
 
-Correlation ID
---------------
+## Correlation ID
+
 
 When controlling plans programatically, it can be useful to verify that event model documents really are related to 
 the plan you just asked the worker to run. The worker will therefore bundle a correlation ID into the headers of
 messages containing documents.
 
-.. seealso:: `Microsoft Playbook on Correlation IDs`_
+see also [`Microsoft Playbook on Correlation IDs`](https://microsoft.github.io/code-with-engineering-playbook/observability/correlation-id/)
 
 ActiveMQ will give this header a different name depending on the protocol you use.
 
-.. list-table:: Correlation ID Headers
-   :widths: 25 25
-   :header-rows: 1
-
-   * - Protocol
-     - Header name
-   * - JMS
-     - jms_correlationID
-   * - STOMP
-     - correlation-id
-
-.. _`bluesky event model`: https://blueskyproject.io/event-model/main/index.html
-.. _`run start document`: https://blueskyproject.io/event-model/main/user/explanations/data-model.html#run-start-document
-.. _`Microsoft Playbook on Correlation IDs`: https://microsoft.github.io/code-with-engineering-playbook/observability/correlation-id/
+| Protocol | Header name      |
+|----------|------------------|
+| JMS      | jms_correlationID|
+| STOMP    | correlation-id   |
```

### Comparing `blueapi-0.4.3a3/docs/explanations/lifecycle.rst` & `blueapi-0.4.3rc1/docs/explanations/lifecycle.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-Lifecycle of a Plan
-===================
+# Lifecycle of a Plan
 
 The following demonstrates exactly what the code does with a plan through its lifecycle 
 of being written, loaded and run. Take the following plan.
-
-.. code:: python
-
+```
     from typing import Any, List, Mapping, Optional, Union
     
     import bluesky.plans as bp
     from blueapi.core import MsgGenerator
     from dls_bluesky_core.core import inject
     from bluesky.protocols import Readable
     
@@ -38,102 +35,94 @@
             MsgGenerator: _description_
     
         Yields:
             Iterator[MsgGenerator]: _description_
         """
     
         yield from bp.count(detectors, num, delay=delay, md=metadata)
+```
 
 
-
-Loading and Registration
-------------------------
+## Loading and Registration
 
 Blueapi will load this plan into its context if configured to load either this module or a module that 
-imports it. The ``BlueskyContext`` will go through all global variables in the module and register them
+imports it. The `BlueskyContext` will go through all global variables in the module and register them
 if it detects that they are plans.
 
 At the point of registration it will inspect the plan's parameters and their type hints, from which it
-will build a pydantic_ model of the parameters to validate against. In other words, it will build something
+will build a [pydantic](https://docs.pydantic.dev/) model of the parameters to validate against. In other words, it will build something
 like this:
 
 
-.. code:: python
-
+```
     from pydantic import BaseModel
 
     class CountParameters(BaseModel):
         detectors: List[Readable] = ["det"]
         num: int = 1
         delay: Optional[Union[float, List[float]]] = None
         metadata: Optional[Mapping[str, Any]] = None
 
         class Config:
             arbitrary_types_allowed = True
             validate_all = True
 
-.. note:: 
-    
     This is for illustrative purposes only, this code is not actually generated, but an object
     resembling this class is constructed in memory.
     The default arguments will be validated by the context to inject the "det" device when the
     plan is run. The existence of the "det" default device is not checked until this time.
+```
 
 The model is also stored in the context.
 
 
-Startup
--------
+## Startup
 
 On startup, the context is passed to the worker, which is passed to the service.
-The worker also holds a reference to the ``RunEngine`` that can run the plan.
+The worker also holds a reference to the `RunEngine` that can run the plan.
 
 
-Request
--------
+## Request
 
 A user can send a request to run the plan to the service, which includes values for the parameters.
 It takes the form of JSON and may look something like this:
-
-.. code:: json
-
+```
     {
         "name": "count",
         "params": {
             "detectors": [
             "andor",
             "pilatus"
             ],
             "num": 3,
             "delay": 0.1
         }
     }
+```
 
-The ``Service`` receives the request and passes it to the worker, which holds it in an internal queue
+The `Service` receives the request and passes it to the worker, which holds it in an internal queue
 and executes it as soon as it can. 
 
 
-Validation
-----------
+## Validation
 
 The pydantic model from earlier, as well as the plan function itself, is loaded out of the registry
 The parameter values in the request are validated against the model, this includes looking up devices
-with names ``andor`` and ``pilatus`` or, if detectors was not passed ``det``.
+with names `andor` and `pilatus` or, if detectors was not passed `det`.
 
+See also [type validators](./type_validators.md)
 
-.. seealso:: `./type_validators`
 
-Execution
----------
+## Execution
 
 The validated parameter values are then passed to the plan function, which is passed to the RunEngine.
-The plan is executed. While it is running, the ``Worker`` will publish
+The plan is executed. While it is running, the `Worker` will publish
 
-* Changes to the state of the ``RunEngine``
+* Changes to the state of the `RunEngine`
 * Changes to any device statuses running within a plan (e.g. when a motor changes position)
-* Event model documents emitted by the ``RunEngine``
+* Event model documents emitted by the `RunEngine`
 * When a plan starts, finishes or fails.
 
 If an error occurs during any of the stages from "Request" onwards it is sent back to the user
 over the message bus.
 
-.. _pydantic: https://docs.pydantic.dev/
+
```

### Comparing `blueapi-0.4.3a3/docs/explanations/type_validators.rst` & `blueapi-0.4.3rc1/docs/explanations/type_validators.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,96 +1,88 @@
-Type Validators
-===============
+# Type Validators
 
-Requirement
------------
-
-Blueapi takes the parameters of a plan and internally creates a pydantic_ model for future validation e.g.
-
-.. code:: python
+## Requirement
 
+Blueapi takes the parameters of a plan and internally creates a [pydantic](https://docs.pydantic.dev/) model for future validation e.g.
+``` 
     def my_plan(a: int, b: str = "b") -> Plan
         ...
 
     # Internally becomes something like
 
     class MyPlanModel(BaseModel):
         a: int
         b: str = "b"
+```
 
 
 That way, when the plan parameters are sent in JSON form, they can be parsed and validated by pydantic.
 However, it must also cover the case where a plan doesn't take a simple dictionary, list or primitive but
 instead a device, such as a detector.
 
-.. code:: python
-
+```
     def my_plan(a: int, b: Readable) -> Plan:
         ...
-
+```
 
 An Ophyd object cannot be passed over the network as JSON because it has state.
-Instead, a string is passed, representing an ID of the object known to the ``BlueskyContext``.
+Instead, a string is passed, representing an ID of the object known to the `BlueskyContext`.
 At the time a plan's parameters are validated, blueapi must take all the strings that are supposed
 to be devices and look them up against the context. For example with the request:
 
-.. code:: json
-
+``` 
     {
         "name": "count",
         "params": {
             "detectors": [
             "andor",
             "pilatus"
             ],
             "num": 3,
             "delay": 0.1
         }
     }
+```
+
+`andor` and `pilatus` should be looked up and replaced with Ophyd objects.
 
-``andor`` and ``pilatus`` should be looked up and replaced with Ophyd objects.
 
+## Solution
 
-Solution
---------
 When the context loads available plans, it iterates through the type signature
 and replaces any reference to a bluesky protocol (or instance of a protocol)
 with a new class that extends the original type. Defining a class validator on
 this new type allows it to check that the string being deserialised is the ID of
 a device of the correct type.
 
 These new intermediate types are used only in the deserialisation process. The
 object returned from validator method is not checked by pydantic so it can be
 the actual instance and the plan never sees the runtime generated reference
 type, only the type it was expecting.
 
-.. note:: This uses the fact that the new types generated at runtime have access to
+> **_NOTE:_** This uses the fact that the new types generated at runtime have access to
     the context that required them via their closure. This circumvents the usual
     problem of pydantic validation not being able to access external state when
     validating or deserialising.
 
-.. code:: python
-
+```
     def my_plan(a: int, b: Readable) -> Plan:
         ...
 
     # Becomes
 
     class MyPlanModel(BaseModel):
         a: int
         b: Reference[Readable]
+```
 
 
-This also allows ``Readable`` to be placed at various type levels. For example:
-
-.. code:: python
-
+This also allows `Readable` to be placed at various type levels. For example:
+``` 
     def my_weird_plan(
         a: Readable,
         b: List[Readable],
         c: Dict[str, Readable],
         d: List[List[Readable]],
         e: List[Dict[str, Set[Readable]]]) -> Plan:
         ...
-
-
-.. _pydantic: https://docs.pydantic.dev/
+```
```

### Comparing `blueapi-0.4.3a3/docs/how-to/add-plans-and-devices.rst` & `blueapi-0.4.3rc1/docs/how-to/add-plans-and-devices.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,118 +1,103 @@
-Add Plans and Devices to your Blueapi Environment
-=================================================
+# Add Plans and Devices to your Blueapi Environment
 
 Custom plans and devices, tailored to individual experimental environments, can be added via configuration. In both cases the relevant code must be in your Python path, for example, part of a library installed in your Python environment. For editing and tweaking you can use an editable install, see below.
 
-Home of Code
-------------
+## Home of Code
 
 The code can be in any pip-installable package, such as:
 
 * A package on pypi
 * A Github repository
-* A local directory with a ``pyproject.toml`` file or similar.
+* A local directory with a `pyproject.toml` file or similar.
 
-The easiest place to put the code is a repository created with the `python-copier-template`_. Which can then become any of the above.
+The easiest place to put the code is a repository created with the [`python-copier-template`](https://diamondlightsource.github.io/python-copier-template/main/index.html). Which can then become any of the above.
 
-.. seealso:: Guide to setting up a new Python project with an environment and a standard set of tools: `Create a new repo from the template`_
+See also: Guide to setting up a new Python project with an environment and a standard set of tools: [`Create a new repo from the template`](https://diamondlightsource.github.io/python-copier-template/main/tutorials/create-new.html)
 
 For development purposes this code should be installed into your environment with 
 
-.. code:: shell
-
+``` 
   pip install -e path/to/package
+```
 
-Format
-------
+## Format
 
 Plans in Python files look like this:
 
-.. note:: The type annotations (e.g. ``: str``, ``: int``, ``-> MsgGenerator``) are required as blueapi uses them to generate an API!
-
-You can define as many plans as you like in a single Python file or spread them over multiple files.
-
-.. code:: python
-
+> **_NOTE:_** The type annotations (e.g. `: str`, `: int`, `-> MsgGenerator`) are required as blueapi uses them to generate an API!  You can define as many plans as you like in a single Python file or spread them over multiple files.
+``` 
     from bluesky.protocols import Readable, Movable
     from blueapi.core import MsgGenerator
     from typing import Mapping, Any
 
     def my_plan(
         detector: Readable, 
         motor: Movable, 
         steps: int, 
         sample_name: str, 
         extra_metadata: Mapping[str, Any]) -> MsgGenerator:
         
         # logic goes here
         ...
+```
 
+Devices are made using the [dodal](https://github.com/DiamondLightSource/dodal) style available through factory functions like this:
 
-Devices are made using the dodal_ style available through factory functions like this:
-
-.. note:: The return type annotation ``-> MyTypeOfDetector`` is required as blueapi uses it to determine that this function creates a device. Meaning you can have a Python file where only some functions create devices and they will be automatically picked up.
+> **_NOTE:_** The return type annotation `-> MyTypeOfDetector` is required as blueapi uses it to determine that this function creates a device. Meaning you can have a Python file where only some functions create devices and they will be automatically picked up.
 
 Similarly, these functions can be organized per-preference into files.
-
-.. code:: python
-
+``` 
     from my_facility_devices import MyTypeOfDetector
 
     def my_detector(name: str) -> MyTypeOfDetector:
         return MyTypeOfDetector(name, {"other_config": "foo"})
+```
 
 
-.. seealso:: dodal_ for many more examples
+See also: dodal for many more examples
 
 An extra function to create the device is used to preserve side-effect-free imports. Each device must have its own factory function.
 
 
-Configuration
--------------
+## Configuration
+
 
-.. seealso:: `./configure-app`
+See also: [configure app](./configure-app.md)
 
 First determine the import path of your code. If you were going to import it in a Python file, what would you put?
 For example:
-
-.. code:: python
-
+``` 
     import my_plan_library.tomography.plans
+```
 
 You would add the following into your configuration file:
-
-.. code:: yaml
-
+``` 
     env:
       sources:
         - kind: dodal
           # note, this code does not have to be inside dodal just because it uses
           # the dodal kind. The module referenced contains a dodal-style function
           # for initializing a particular device e.g. MyTypeOfDetector in my_lab.
           module: dodal.my_beamline  
         - kind: planFunctions
           module: my_plan_library.tomography.plans
+```
 
 
 You can have as many sources for plans and devices as are needed.
 
 
-Scratch Area on Kubernetes
---------------------------
+## Scratch Area on Kubernetes
 
-Sometimes in-the-loop development of plans and devices may be required. If running blueapi out of a virtual environment local packages can be installed with ``pip install -e path/to/package``, but there is also a way to support editable packages on Kubernetes with a shared filesystem.
+Sometimes in-the-loop development of plans and devices may be required. If running blueapi out of a virtual environment local packages can be installed with `pip install -e path/to/package`, but there is also a way to support editable packages on Kubernetes with a shared filesystem.
 
 Blueapi can be configured to install editable Python packages from a chosen directory, the helm chart can mount this directory from the
-host machine, include the following in your ``values.yaml``:
-
-.. code:: yaml
-
+host machine, include the following in your `values.yaml`:
+``` 
   scratch:
     hostPath: path/to/scratch/area  # e.g. /dls_sw/<my_beamline>/software/blueapi/scratch
 
-You can then clone projects into the scratch directory and blueapi will automatically incorporate them on startup. You must still include configuration to load the plans and devices from specific modules within those packages, see above. 
+```
 
+You can then clone projects into the scratch directory and blueapi will automatically incorporate them on startup. You must still include configuration to load the plans and devices from specific modules within those packages, see above. 
 
-.. _dodal: https://github.com/DiamondLightSource/dodal
-.. _`python-copier-template`: https://diamondlightsource.github.io/python-copier-template/main/index.html
-.. _`Create a new repo from the template`: https://diamondlightsource.github.io/python-copier-template/main/tutorials/create-new.html
```

### Comparing `blueapi-0.4.3a3/docs/how-to/configure-app.rst` & `blueapi-0.4.3rc1/docs/how-to/configure-app.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-Configure the application
-=========================
+# Configure the application
 
 By default, configuration options are ingested from pydantic BaseModels,
 however the option exists to override these by defining a yaml file which
-can be passed to the ``blueapi`` command.
+can be passed to the `blueapi` command.
 
-An example of this yaml file is found in ``config/defaults.yaml``, which follows
-the schema defined in ``src/blueapi/config.py`` in the ``ApplicationConfig`` 
+An example of this yaml file is found in `config/defaults.yaml`, which follows
+the schema defined in `src/blueapi/config.py` in the `ApplicationConfig` 
 object.
 
 To set your own application configuration, edit this file (or write your own)
 and simply pass it to the CLI by typing::
 
-    $ blueapi --config path/to/file.yaml
+``` blueapi --config path/to/file.yaml ```
 
-where ``path/to/file.yaml`` is the relative path to the configuration file you
+where `path/to/file.yaml` is the relative path to the configuration file you
 wish to use. Then, any subsequent calls to child commands of blueapi will
 use this file.
```

### Comparing `blueapi-0.4.3a3/docs/how-to/run-cli.rst` & `blueapi-0.4.3rc1/docs/how-to/run-cli.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,39 @@
-Control the Worker via the CLI
-==============================
+# Control the Worker via the CLI
 
 The worker comes with a minimal CLI client for basic control. It should be noted that this is 
 a test/development/debugging tool and not meant for production!
 
-.. seealso:: 
-    You must have access to the ``blueapi`` command either via the container or pip installing.
     `./run-container` and `../tutorials/installation`
 
 
-.. seealso:: 
-    In a developer environment, the worker can also be run from vscode: `../tutorials/dev-run`.
 
 
-Basic Introspection
--------------------
+## Basic Introspection
 
 The worker can tell you which plans and devices are available via:
-
-.. code:: shell
-
+``` 
     blueapi controller plans
     blueapi controller devices
 
-By default, the CLI will talk to the worker via a message broker on ``tcp://localhost:61613``,
+By default, the CLI will talk to the worker via a message broker on `tcp://localhost:61613`,
 but you can customize this.
 
-.. code:: shell
-
+```
     blueapi controller -h my.host -p 61614 plans
+```
 
-Running Plans
--------------
+## Running Plans
 
 You can run a plan and pass arbitrary JSON parameters.
-
-.. code:: shell
-
+``` 
     # Run the sleep plan
     blueapi controller run sleep '{"time": 5.0}'
 
     # Run the count plan
     blueapi controller run count '{"detectors": ["current_det", "image_det"]}'
+```
 
 The command will block until the plan is finished and will forward error/status messages 
 from the server.
 
-.. seealso:: Full reference: `../reference/cli`
+See also [Full CLI reference](../reference/cli.md)
```

### Comparing `blueapi-0.4.3a3/docs/how-to/write-plans.rst` & `blueapi-0.4.3rc1/docs/how-to/write-plans.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,97 +1,79 @@
-Writing Bluesky plans for Blueapi
-=================================
+# Writing Bluesky plans for Blueapi
 
-.. warning::
-    Please read the following completely and carefully, as you risk losing data if plans are written incorrectly!
 
 For an introduction to bluesky plans and general forms/advice, `see the bluesky documentation <https://nsls-ii.github.io/bluesky/plans.html>`__. Blueapi has some additional requirements, which are explained below.
 
-Plans
-~~~~~
+## Plans
 
-While the bluesky project uses ``plan`` in a general sense to refer to any ``Iterable`` of ``Msg``\ s which may be run by the ``RunEngine``, blueapi distinguishes between a ``plan`` and a ``stub``. This distinction is made to allow for a subset of ``stub``\ s to be exposed and run, as ``stub``\ s may not make sense to run alone.
+While the bluesky project uses `plan` in a general sense to refer to any `Iterable` of `Msg`\ s which may be run by the `RunEngine`, blueapi distinguishes between a `plan` and a `stub`. This distinction is made to allow for a subset of `stub`\ s to be exposed and run, as `stub`\ s may not make sense to run alone.
 
-Generally, a ``plan`` includes at least one ``open_run`` and ``close_run`` and is a complete description of an experiment. If it does not, it is a ``stub``. This distinction is made in the bluesky core library between the ``plan``\ s and ``plan_stub``\ s modules.
+Generally, a `plan` includes at least one `open_run` and `close_run` and is a complete description of an experiment. If it does not, it is a `stub`. This distinction is made in the bluesky core library between the `plan`\ s and `plan_stub`\ s modules.
 
-Type Annotations
-^^^^^^^^^^^^^^^^
+## Type Annotations
 
-To be imported into the blueapi context, ``plan``\ s and ``stub``\ s must be the in the form of a ``PlanGenerator``: any function that return a ``MsgGenerator`` (a python ``Generator`` that yields ``Msg``\ s). ``PlanGenerator`` and ``MsgGenerator`` types are available to import from ``dodal``.
-
-.. note::
-    ``PlanGenerator``\ s must be annotated with the return type ``MsgGenerator`` to be added to the blueapi context.
-
-.. code:: python
+To be imported into the blueapi context, `plan`\ s and `stub`\ s must be the in the form of a `PlanGenerator`: any function that return a `MsgGenerator` (a python `Generator` that yields `Msg`\ s). `PlanGenerator` and `MsgGenerator` types are available to import from `dodal`.
 
+``` 
    def foo() -> MsgGenerator:
        # The minimum PlanGenerator acceptable to blueapi
        yield from {}
+```
 
-.. note::
-    ``PlanGenerator`` arguments must be annotated to enable blueapi to generate their schema
+> **_NOTE:_** `PlanGenerator` arguments must be annotated to enable blueapi to generate their schema
 
 **Input annotations should be as broad as possible**, the least specific implementation that is sufficient to accomplish the requirements of the plan.
 
-For example, if a plan is written to drive a specific implementation of Movable, but never calls any methods on the device and only yields bluesky ``'set'`` Msgs, it can be generalised to instead use the base protocol ``Movable``.
-
-.. code:: python
+For example, if a plan is written to drive a specific implementation of Movable, but never calls any methods on the device and only yields bluesky `'set'` Msgs, it can be generalised to instead use the base protocol `Movable`.
 
+```
    def move_to_each_position(axis: Movable) -> MsgGenerator:
        # Originally written for SpecificImplementationMovable
        for _ in range(i):
            yield from abs_set(axis, location)
+```
 
-Allowed Argument Types
-^^^^^^^^^^^^^^^^^^^^^^
+## Allowed Argument Types
 
-When added to the blueapi context, ``PlanGenerator``\ s are formalised into their schema- `a Pydantic BaseModel <https://docs.pydantic.dev/1.10/usage/models/>`__ with the expected argument types and their defaults. 
+When added to the blueapi context, `PlanGenerator`\ s are formalised into their schema- `a Pydantic BaseModel <https://docs.pydantic.dev/1.10/usage/models/>`__ with the expected argument types and their defaults. 
 
-Therefore, ``PlanGenerator``\ s must only take as arguments `those types which are valid Pydantic fields <https://docs.pydantic.dev/1.10/usage/types/>`__ or Device types which implement ``BLUESKY_PROTOCOLS`` defined in dodal, which are fetched from the context at runtime.
+Therefore, `PlanGenerator`\ s must only take as arguments `those types which are valid Pydantic fields <https://docs.pydantic.dev/1.10/usage/types/>`__ or Device types which implement `BLUESKY_PROTOCOLS` defined in dodal, which are fetched from the context at runtime.
 
-.. note::
+    Allowed argument types for Pydantic BaseModels include the primitives, types that extend `BaseModel` and `dict`\ s, `list`\ s  and other `sequence`\ s of supported types. Blueapi will deserialise these types from JSON, so `dict`\ s should use `str` keys.
 
-    Allowed argument types for Pydantic BaseModels include the primitives, types that extend ``BaseModel`` and ``dict``\ s, ``list``\ s  and other ``sequence``\ s of supported types. Blueapi will deserialise these types from JSON, so ``dict``\ s should use ``str`` keys.
-
-Injecting defaults
-^^^^^^^^^^^^^^^^^^
+## Injecting defaults
 
 Often when writing a plan, it is known which device the plan will mostly or always be run with, but at the time of writing the plan the device object has not been instantiated: dodal defines device factory functions, but these cannot be injected as default arguments to plans.
 
-Dodal defines an ``inject`` function which bypasses the type checking of the constructed schemas, defering to the blueapi contexting fetching of the device when the plan is imported. This allows defaulting devices, so long as there is a device of that name in the context which conforms to the type annotation.
-
-.. code:: python
+Dodal defines an `inject` function which bypasses the type checking of the constructed schemas, defering to the blueapi contexting fetching of the device when the plan is imported. This allows defaulting devices, so long as there is a device of that name in the context which conforms to the type annotation.
 
+``` 
    def touch_synchrotron(sync: Synchrotron = inject("synchrotron")) -> MsgGenerator:
        # There is only one Synchrotron device, so we know which one it will always be.
        # If there is no device named "synchrotron" in the blueapi context, it will except.
        sync.specific_function()
        yield from {}
+```
 
-Metadata
-^^^^^^^^
+### Metadata
 
 The bluesky event model allows for rich structured metadata to be attached to a scan. To enable this to be used consistently, blueapi encourages a standard form.
 
-.. note::
-
-    Plans **should** include ``metadata`` as their final argument, if they do it **must** have the type Optional[Mapping[str, Any]], `and a default of None <https://stackoverflow.com/questions/26320899/why-is-the-empty-dictionary-a-dangerous-default-value-in-python>`__\, with the plan defaulting to an empty dict if passed ``None``. If the plan calls to a stub/plan which takes metadata, the plan **must** pass down its metadata, which may be a differently named argument.
-
-.. code:: python
+> **_NOTE:_** Plans **should** include `metadata` as their final argument, if they do it **must** have the type Optional[Mapping[str, Any]], `and a default of None <https://stackoverflow.com/questions/26320899/why-is-the-empty-dictionary-a-dangerous-default-value-in-python>`__\, with the plan defaulting to an empty dict if passed `None`. If the plan calls to a stub/plan which takes metadata, the plan **must** pass down its metadata, which may be a differently named argument.
 
+```
    def pass_metadata(x: Movable, metadata: Optional[Mapping[str, Any]] = None) -> MsgGenerator:
        yield from bp.count{[x], md=metadata or {}}
+```
 
-Docstrings
-^^^^^^^^^^
+## Docstrings
 
 Blueapi plan schemas include includes the docstrings of imported Plans. **These should therefore explain as much about the scan as cannot be ascertained from its arguments and name**. This may include units of arguments (e.g. seconds or microseconds), its purpose in the function, the purpose of the plan etc.
 
-.. code:: python
-
+``` 
    def temp_pressure_snapshot(
        detectors: List[Readable],
        temperature: Movable = inject("sample_temperature"),
        pressure: Movable = inject("sample_pressure"),
        target_temperature: float = 273.0,
        target_pressure: float = 10**5,
        metadata: Optional[Mapping[str, Any]] = None,
@@ -110,83 +92,73 @@
        Returns:
            MsgGenerator: Plan
        Yields:
            Iterator[MsgGenerator]: Bluesky messages
        """
        yield from move({temperature: target_temperature, pressure: target_pressure})
        yield from count(detectors, 1, metadata or {})
+```
 
-Decorators
-^^^^^^^^^^
-
-Dodal defines a decorator for configuring any ``ophyd-async`` devices- which will be the majority of devices at Diamond- to write to a common location. 
-
-.. warning::
+### Decorators
 
-    **This is an absolute requirement to write data onto the Diamond Filesystem**.
+Dodal defines a decorator for configuring any `ophyd-async` devices- which will be the majority of devices at Diamond- to write to a common location. 
 
-    This decorator must be used every time a new data collection is intended to begin. For an example, see below.
-
-.. code:: python
+> **_NOTE:_** **This is an absolute requirement to write data onto the Diamond Filesystem**.  This decorator must be used every time a new data collection is intended to begin. For an example, see below.
 
+```
    @attach_metadata
    def ophyd_async_snapshot(
        detectors: List[Readable],
        metadata: Optional[Mapping[str, Any]] = None,
-   ) -> MsgGenerator:
-       """
+###    ) -> MsgGenerator:
        Configures a number of devices, which may be Ophyd-Async detectors and require
        knowledge of where to write their files, then takes a snapshot with them.
        Args:
            detectors (List[Readable]): Devices, maybe including Ophyd-Async detectors.
        Returns:
            MsgGenerator: Plan
        Yields:
-           Iterator[MsgGenerator]: Bluesky messages
-       """
+###            Iterator[MsgGenerator]: Bluesky messages
        yield from count(detectors, 1, metadata or {})
 
    def repeated_snapshot(
        detectors: List[Readable],
        metadata: Optional[Mapping[str, Any]] = None,
-   ) -> MsgGenerator:
-       """
+###    ) -> MsgGenerator:
        Configures a number of devices, which may be Ophyd-Async detectors and require
        knowledge of where to write their files, then takes multiple snapshot with them.
        Args:
            detectors (List[Readable]): Devices, maybe including Ophyd-Async detectors.
        Returns:
            MsgGenerator: Plan
        Yields:
-           Iterator[MsgGenerator]: Bluesky messages
-       """
+###            Iterator[MsgGenerator]: Bluesky messages
        @attach_metadata
        def inner_function():
            yield from count(detectors, 1, metadata or {})
 
 
        for _ in range(5):
            yield from inner_function()
+```
 
-Stubs
-~~~~~
+### Stubs
 
 Some functionality in your plans may make sense to factor out to allow re-use. These pieces of functionality may or may not make sense outside of the context of a plan. Some will, such as nudging a motor, but others may not, such as waiting to consume data from the previous position, or opening a run without an equivalent closure.
 
-To enable blueapi to expose the stubs that it makes sense to, but not the others, blueapi will only expose a subset of ``MsgGenerator``\ s under the following conditions:
-
-| ``__init__.py`` in directory has ``__exports__``: List[str]: only
-  those named in ``__exports__``
-| ``__init__.py`` in directory has ``__all__``: List[str] but no
-  ``__exports__``: only those named in ``__all__``
+To enable blueapi to expose the stubs that it makes sense to, but not the others, blueapi will only expose a subset of `MsgGenerator`\ s under the following conditions:
 
-This allows other python packages (such as ``plans``) to access every function in ``__all__``, while only allowing a subset to be called from blueapi as standalone.
+| `__init__.py` in directory has `__exports__`: List[str]: only
+  those named in `__exports__`
+| `__init__.py` in directory has `__all__`: List[str] but no
+  `__exports__`: only those named in `__all__`
 
-.. code:: python
+This allows other python packages (such as `plans`) to access every function in `__all__`, while only allowing a subset to be called from blueapi as standalone.
 
+``` 
     # Rehomes all of the beamline's devices. May require to be run standalone
     from .package import rehome_devices
     # Awaits a standard callback from analysis. Should not be run standalone
     from .package import await_callback
 
     # Exported from the module for use by other modules
     __all__ = [
@@ -194,7 +166,8 @@
         "await_callback",
     ]
 
     # Imported by instances of blueapi and allowed to be run
     __exports__ = [
         "rehome_devices",
     ]
+```
```

### Comparing `blueapi-0.4.3a3/docs/images/blueapi-architecture.png` & `blueapi-0.4.3rc1/docs/images/blueapi-architecture.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/docs/images/blueapi-logo.svg` & `blueapi-0.4.3rc1/docs/images/blueapi-logo.svg`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/docs/images/blueapi.png` & `blueapi-0.4.3rc1/docs/images/blueapi.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/docs/images/bluesky-events.png` & `blueapi-0.4.3rc1/docs/images/bluesky-events.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/docs/images/debug-vscode.png` & `blueapi-0.4.3rc1/docs/images/debug-vscode.png`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/docs/index.md` & `blueapi-0.4.3rc1/docs/index.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,62 @@
----
-html_theme.sidebar_secondary.remove: true
----
+# How the documentation is structured
 
 ```{include} ../README.md
 :end-before: <!-- README only content
 ```
 
-[concept]: images/blueapi.png
-
-How the documentation is structured
------------------------------------
-
 Documentation is split into [four categories](https://diataxis.fr), also accessible from links in the top bar.
 
+- Tutorials - Tutorials for installation and typical usage. New users start here.
+- How-To-s - Practical step-by-step guides for the more experienced user.
+- Explanations - Explanations of how it works and why it works that way.
+- Reference - Technical reference material including APIs and release notes.
 <!-- https://sphinx-design.readthedocs.io/en/latest/grids.html -->
 
 ::::{grid} 2
 :gutter: 4
 
 :::{grid-item-card} {material-regular}`directions_walk;2em`
+
 ```{toctree}
 :maxdepth: 2
 tutorials
 ```
+
 +++
 Tutorials for installation and typical usage. New users start here.
 :::
 
 :::{grid-item-card} {material-regular}`directions;2em`
+
 ```{toctree}
 :maxdepth: 2
 how-to
 ```
+
 +++
 Practical step-by-step guides for the more experienced user.
 :::
 
 :::{grid-item-card} {material-regular}`info;2em`
+
 ```{toctree}
 :maxdepth: 2
 explanations
 ```
+
 +++
 Explanations of how it works and why it works that way.
 :::
 
 :::{grid-item-card} {material-regular}`menu_book;2em`
+
 ```{toctree}
 :maxdepth: 2
 reference
 ```
+
 +++
 Technical reference material including APIs and release notes.
 :::
 
 ::::
```

### Comparing `blueapi-0.4.3a3/docs/reference/asyncapi.yaml` & `blueapi-0.4.3rc1/docs/reference/asyncapi.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/docs/reference/openapi.yaml` & `blueapi-0.4.3rc1/docs/reference/openapi.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/docs/tutorials/installation.md` & `blueapi-0.4.3rc1/docs/tutorials/installation.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 # Installation
 
 ## Check your version of python
 
 You will need python 3.8 or later. You can check your version of python by
 typing into a terminal:
-
-```
-$ python3 --version
+``` 
+python3 --version
 ```
 
 ## Create a virtual environment
 
 It is recommended that you install into a “virtual environment” so this
 installation will not interfere with any existing Python software:
-
-```
-$ python3 -m venv /path/to/venv
-$ source /path/to/venv/bin/activate
+``` 
+python3 -m venv /path/to/venv
+source /path/to/venv/bin/activate
 ```
 
 ## Installing the library
 
 You can now use `pip` to install the library and its dependencies:
-
-```
-$ python3 -m pip install blueapi
+``` 
+python3 -m pip install blueapi
 ```
 
 If you require a feature that is not currently released you can also install
 from github:
-
-```
-$ python3 -m pip install git+https://github.com/DiamondLightSource/blueapi.git
+``` 
+python3 -m pip install git+https://github.com/DiamondLightSource/blueapi.git
 ```
 
 The library should now be installed and the commandline interface on your path.
 You can check the version that has been installed by typing:
-
-```
-$ blueapi --version
+``` 
+blueapi --version
 ```
```

### Comparing `blueapi-0.4.3a3/helm/blueapi/Chart.yaml` & `blueapi-0.4.3rc1/helm/blueapi/Chart.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/helm/blueapi/templates/_helpers.tpl` & `blueapi-0.4.3rc1/helm/blueapi/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/helm/blueapi/templates/deployment.yaml` & `blueapi-0.4.3rc1/helm/blueapi/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/helm/blueapi/templates/ingress.yaml` & `blueapi-0.4.3rc1/helm/blueapi/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/helm/blueapi/templates/tests/test-ping.yaml` & `blueapi-0.4.3rc1/helm/blueapi/templates/tests/test-ping.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/helm/blueapi/values.yaml` & `blueapi-0.4.3rc1/helm/blueapi/values.yaml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/pyproject.toml` & `blueapi-0.4.3rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/cli/cli.py` & `blueapi-0.4.3rc1/src/blueapi/cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import logging
 from collections import deque
 from functools import wraps
 from pathlib import Path
 from pprint import pprint
 
 import click
+from pydantic import ValidationError
 from requests.exceptions import ConnectionError
 
 from blueapi import __version__
-from blueapi.cli.event_bus_client import EventBusClient
+from blueapi.cli.event_bus_client import BlueskyRemoteError, EventBusClient
 from blueapi.config import ApplicationConfig, ConfigLoader
 from blueapi.core import DataEvent
 from blueapi.messaging import MessageContext
 from blueapi.messaging.stomptemplate import StompMessagingTemplate
 from blueapi.service.main import start
 from blueapi.service.model import WorkerTask
 from blueapi.service.openapi import (
@@ -176,29 +177,39 @@
     config: ApplicationConfig = obj["config"]
     client: BlueapiRestClient = obj["rest_client"]
 
     logger = logging.getLogger(__name__)
     if config.stomp is not None:
         _message_template = StompMessagingTemplate.autoconfigured(config.stomp)
     else:
-        raise RuntimeError(
-            "Cannot run plans without Stomp configuration to track progress"
-        )
+        pprint("ERROR: Cannot run plans without Stomp configuration to track progress")
+        return
     event_bus_client = EventBusClient(_message_template)
     finished_event: deque[WorkerEvent] = deque()
 
     def store_finished_event(event: WorkerEvent) -> None:
         if event.is_complete():
             finished_event.append(event)
 
     parameters = parameters or "{}"
-    task = Task(name=name, params=json.loads(parameters))
-
-    resp = client.create_task(task)
-    task_id = resp.task_id
+    task_id = ""
+    parsed_params = json.loads(parameters) if isinstance(parameters, str) else {}
+    try:
+        task = Task(name=name, params=parsed_params)
+        resp = client.create_task(task)
+        task_id = resp.task_id
+    except ValidationError as e:
+        pprint(f"failed to validate the task parameters, {task_id}, error: {e}")
+        return
+    except BlueskyRemoteError as e:
+        pprint(f"server error with this message: {e}")
+        return
+    except ValueError:
+        pprint("task could not run")
+        return
 
     with event_bus_client:
         event_bus_client.subscribe_to_topics(task_id, on_event=store_finished_event)
         updated = client.update_worker_task(WorkerTask(task_id=task_id))
 
         event_bus_client.wait_for_complete(timeout=timeout)
```

### Comparing `blueapi-0.4.3a3/src/blueapi/cli/event_bus_client.py` & `blueapi-0.4.3rc1/src/blueapi/cli/event_bus_client.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/cli/rest.py` & `blueapi-0.4.3rc1/src/blueapi/cli/rest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections.abc import Callable, Mapping
+from http import HTTPStatus
 from typing import Any, Literal, TypeVar
 
 import requests
 from pydantic import parse_obj_as
 
 from blueapi.config import RestConfig
 from blueapi.service.model import (
@@ -16,14 +17,23 @@
 from blueapi.worker import Task, TrackableTask, WorkerState
 
 from .event_bus_client import BlueskyRemoteError
 
 T = TypeVar("T")
 
 
+def get_status_message(code: int) -> str:
+    """Returns the standard description for a given HTTP status code."""
+    try:
+        message = HTTPStatus(code).phrase
+        return message
+    except ValueError:
+        return "Unknown Status Code"
+
+
 def _is_exception(response: requests.Response) -> bool:
     return response.status_code >= 400
 
 
 class BlueapiRestClient:
     _config: RestConfig
 
@@ -103,14 +113,18 @@
         data: Mapping[str, Any] | None = None,
         method="GET",
         raise_if: Callable[[requests.Response], bool] = _is_exception,
     ) -> T:
         url = self._url(suffix)
         response = requests.request(method, url, json=data)
         if raise_if(response):
-            raise BlueskyRemoteError(str(response))
+            message = get_status_message(response.status_code)
+            error_message = f"""Response failed with text: {response.text},
+            with error code: {response.status_code}
+            which corresponds to {message}"""
+            raise BlueskyRemoteError(error_message)
         deserialized = parse_obj_as(target_type, response.json())
         return deserialized
 
     def _url(self, suffix: str) -> str:
         base_url = f"{self._config.protocol}://{self._config.host}:{self._config.port}"
         return f"{base_url}{suffix}"
```

### Comparing `blueapi-0.4.3a3/src/blueapi/cli/updates.py` & `blueapi-0.4.3rc1/src/blueapi/cli/updates.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/config.py` & `blueapi-0.4.3rc1/src/blueapi/config.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/core/__init__.py` & `blueapi-0.4.3rc1/src/blueapi/core/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/core/bluesky_types.py` & `blueapi-0.4.3rc1/src/blueapi/core/bluesky_types.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/core/context.py` & `blueapi-0.4.3rc1/src/blueapi/core/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 from dataclasses import dataclass, field
 from importlib import import_module
 from inspect import Parameter, signature
 from types import ModuleType, UnionType
 from typing import Any, Generic, TypeVar, Union, get_args, get_origin, get_type_hints
 
 from bluesky.run_engine import RunEngine
+from dodal.utils import make_all_devices
+from ophyd_async.core import NotConnected
 from pydantic import create_model
 from pydantic.fields import FieldInfo, ModelField
 
 from blueapi.config import EnvironmentConfig, SourceKind
-from blueapi.utils import (
-    BlueapiPlanModelConfig,
-    load_module_all,
-)
+from blueapi.utils import BlueapiPlanModelConfig, load_module_all
 
 from .bluesky_types import (
     BLUESKY_PROTOCOLS,
     Device,
     HasName,
     Plan,
     PlanGenerator,
@@ -100,19 +99,27 @@
             if is_bluesky_plan_generator(obj):
                 self.plan(obj)
 
     def with_device_module(self, module: ModuleType) -> None:
         self.with_dodal_module(module)
 
     def with_dodal_module(self, module: ModuleType, **kwargs) -> None:
-        from dodal.utils import make_all_devices
+        devices, exceptions = make_all_devices(module, **kwargs)
 
-        for device in make_all_devices(module, **kwargs).values():
+        for device in devices.values():
             self.device(device)
 
+        # If exceptions have occurred, we log them but we do not make blueapi
+        # fall over
+        if len(exceptions) > 0:
+            LOGGER.warning(
+                f"{len(exceptions)} exceptions occurred while instantiating devices"
+            )
+            LOGGER.exception(NotConnected(exceptions))
+
     def plan(self, plan: PlanGenerator) -> PlanGenerator:
         """
         Register the argument as a plan in the context. Can be used as a decorator e.g.
         @ctx.plan
         def my_plan(a: int, b: str):
             ...
```

### Comparing `blueapi-0.4.3a3/src/blueapi/core/device_lookup.py` & `blueapi-0.4.3rc1/src/blueapi/core/device_lookup.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/core/event.py` & `blueapi-0.4.3rc1/src/blueapi/core/event.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/messaging/base.py` & `blueapi-0.4.3rc1/src/blueapi/messaging/base.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/messaging/stomptemplate.py` & `blueapi-0.4.3rc1/src/blueapi/messaging/stomptemplate.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/messaging/utils.py` & `blueapi-0.4.3rc1/src/blueapi/messaging/utils.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/service/handler.py` & `blueapi-0.4.3rc1/src/blueapi/service/handler.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/service/handler_base.py` & `blueapi-0.4.3rc1/src/blueapi/service/handler_base.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/service/main.py` & `blueapi-0.4.3rc1/src/blueapi/service/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,20 +141,31 @@
     request: Request,
     response: Response,
     task: Task = Body(..., example=Task(name="count", params={"detectors": ["x"]})),  # noqa: B008
     handler: BlueskyHandler = Depends(get_handler),
 ):
     """Submit a task to the worker."""
     try:
+        plan_model = handler.get_plan(task.name)
         task_id: str = handler.submit_task(task)
         response.headers["Location"] = f"{request.url}/{task_id}"
         return TaskResponse(task_id=task_id)
     except ValidationError as e:
+        errors = e.errors()
+        formatted_errors = "; ".join(
+            [f"{err['loc'][0]}: {err['msg']}" for err in errors]
+        )
+        error_detail_response = f"""
+        Input validation failed: {formatted_errors},
+        suppplied params {task.params},
+        do not match the expected params: {plan_model.parameter_schema}
+        """
         raise HTTPException(
-            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=e.errors()
+            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+            detail=error_detail_response,
         ) from e
 
 
 @app.delete("/tasks/{task_id}", status_code=status.HTTP_200_OK)
 def delete_submitted_task(
     task_id: str,
     handler: BlueskyHandler = Depends(get_handler),
```

### Comparing `blueapi-0.4.3a3/src/blueapi/service/model.py` & `blueapi-0.4.3rc1/src/blueapi/service/model.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/service/openapi.py` & `blueapi-0.4.3rc1/src/blueapi/service/openapi.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/service/subprocess_handler.py` & `blueapi-0.4.3rc1/src/blueapi/service/subprocess_handler.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/startup/example_devices.py` & `blueapi-0.4.3rc1/src/blueapi/startup/example_devices.py`

 * *Files 22% similar despite different names*

```diff
@@ -68,7 +68,14 @@
         name=name,
         motor=x,
         motor_field="x",
         center=0.0,
         Imax=1,
         labels={"detectors"},
     )
+
+
+def unplugged_motor(name="unplugged_motor") -> SynAxisWithMotionEvents:
+    raise TimeoutError(
+        "This device is supposed to fail, blueapi "
+        "will mark it as not present and start up regardless"
+    )
```

### Comparing `blueapi-0.4.3a3/src/blueapi/startup/example_plans.py` & `blueapi-0.4.3rc1/src/blueapi/startup/example_plans.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/startup/simmotor.py` & `blueapi-0.4.3rc1/src/blueapi/startup/simmotor.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/utils/base_model.py` & `blueapi-0.4.3rc1/src/blueapi/utils/base_model.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/utils/modules.py` & `blueapi-0.4.3rc1/src/blueapi/utils/modules.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/utils/serialization.py` & `blueapi-0.4.3rc1/src/blueapi/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/utils/thread_exception.py` & `blueapi-0.4.3rc1/src/blueapi/utils/thread_exception.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/worker/__init__.py` & `blueapi-0.4.3rc1/src/blueapi/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/worker/event.py` & `blueapi-0.4.3rc1/src/blueapi/worker/event.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/worker/multithread.py` & `blueapi-0.4.3rc1/src/blueapi/worker/multithread.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/worker/reworker.py` & `blueapi-0.4.3rc1/src/blueapi/worker/reworker.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/worker/task.py` & `blueapi-0.4.3rc1/src/blueapi/worker/task.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi/worker/worker.py` & `blueapi-0.4.3rc1/src/blueapi/worker/worker.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/src/blueapi.egg-info/PKG-INFO` & `blueapi-0.4.3rc1/src/blueapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueapi
-Version: 0.4.3a3
+Version: 0.4.3rc1
 Summary: Lightweight bluesky-as-a-service wrapper application. Also usable as a library.
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `blueapi-0.4.3a3/src/blueapi.egg-info/SOURCES.txt` & `blueapi-0.4.3rc1/src/blueapi.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -34,44 +34,44 @@
 docs/conf.py
 docs/explanations.md
 docs/genindex.md
 docs/how-to.md
 docs/index.md
 docs/reference.md
 docs/tutorials.md
-docs/explanations/architecture.rst
+docs/explanations/architecture.md
 docs/explanations/decisions.md
-docs/explanations/events.rst
-docs/explanations/lifecycle.rst
-docs/explanations/type_validators.rst
+docs/explanations/events.md
+docs/explanations/lifecycle.md
+docs/explanations/type_validators.md
 docs/explanations/decisions/0001-record-architecture-decisions.md
 docs/explanations/decisions/0002-switched-to-python-copier-template.md
-docs/explanations/decisions/0003-no-queues.rst
-docs/explanations/decisions/0004-api-case.rst
+docs/explanations/decisions/0003-no-queues.md
+docs/explanations/decisions/0004-api-case.md
 docs/explanations/decisions/COPYME
-docs/how-to/add-plans-and-devices.rst
-docs/how-to/configure-app.rst
+docs/how-to/add-plans-and-devices.md
+docs/how-to/configure-app.md
 docs/how-to/contribute.md
-docs/how-to/run-cli.rst
-docs/how-to/run-container.rst
-docs/how-to/write-plans.rst
+docs/how-to/run-cli.md
+docs/how-to/run-container.md
+docs/how-to/write-plans.md
 docs/images/blueapi-architecture.png
 docs/images/blueapi-logo.svg
 docs/images/blueapi.png
 docs/images/bluesky-events.png
 docs/images/debug-vscode.png
 docs/reference/api.md
 docs/reference/asyncapi.yaml
-docs/reference/cli.rst
-docs/reference/messaging-spec.rst
+docs/reference/cli.md
+docs/reference/messaging-spec.md
 docs/reference/openapi.yaml
-docs/reference/rest-spec.rst
-docs/tutorials/dev-run.rst
+docs/reference/rest-spec.md
+docs/tutorials/dev-run.md
 docs/tutorials/installation.md
-docs/tutorials/quickstart.rst
+docs/tutorials/quickstart.md
 helm/blueapi/.helmignore
 helm/blueapi/Chart.yaml
 helm/blueapi/values.yaml
 helm/blueapi/templates/NOTES.txt
 helm/blueapi/templates/_helpers.tpl
 helm/blueapi/templates/configmap.yaml
 helm/blueapi/templates/deployment.yaml
@@ -132,14 +132,15 @@
 src/blueapi/worker/worker_errors.py
 tests/__init__.py
 tests/conftest.py
 tests/test_cli.py
 tests/test_config.py
 tests/core/__init__.py
 tests/core/fake_device_module.py
+tests/core/fake_device_module_failing.py
 tests/core/fake_plan_module.py
 tests/core/test_context.py
 tests/core/test_event.py
 tests/example_yaml/config.yaml
 tests/example_yaml/nested_config.yaml
 tests/example_yaml/override_config.yaml
 tests/example_yaml/rest_config.yaml
```

### Comparing `blueapi-0.4.3a3/tests/conftest.py` & `blueapi-0.4.3rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/tests/core/fake_device_module.py` & `blueapi-0.4.3rc1/tests/core/fake_device_module.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/tests/core/test_context.py` & `blueapi-0.4.3rc1/tests/core/test_context.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from unittest.mock import patch
 
 import pytest
 from bluesky.protocols import Descriptor, Movable, Readable, Reading, SyncOrAsync
 from dls_bluesky_core.core import MsgGenerator, PlanGenerator, inject
 from ophyd.sim import SynAxis, SynGauss
 from pydantic import ValidationError, parse_obj_as
+from pytest import LogCaptureFixture
 
 from blueapi.config import EnvironmentConfig, Source, SourceKind
 from blueapi.core import BlueskyContext, is_bluesky_compatible_device
 from blueapi.core.context import DefaultFactory
 
 SIM_MOTOR_NAME = "sim"
 ALT_MOTOR_NAME = "alt"
@@ -170,23 +171,39 @@
         "motor_x",
         "motor_y",
         "motor_bundle_a",
         "motor_bundle_b",
     } == empty_context.devices.keys()
 
 
+def test_add_failing_deivces_from_module(
+    caplog: LogCaptureFixture, empty_context: BlueskyContext
+) -> None:
+    import tests.core.fake_device_module_failing as device_module
+
+    caplog.set_level(10)
+    empty_context.with_device_module(device_module)
+    logs = caplog.get_records("call")
+
+    assert any("TimeoutError: FooBar" in log.message for log in logs)
+    assert len(empty_context.devices.keys()) == 0
+
+
 def test_extra_kwargs_in_with_dodal_module_passed_to_make_all_devices(
     empty_context: BlueskyContext,
 ) -> None:
     """
     Note that this functionality is currently used by hyperion.
     """
     import tests.core.fake_device_module as device_module
 
-    with patch("dodal.utils.make_all_devices") as mock_make_all_devices:
+    with patch(
+        "blueapi.core.context.make_all_devices",
+        return_value=({}, {}),
+    ) as mock_make_all_devices:
         empty_context.with_dodal_module(
             device_module, some_argument=1, another_argument="two"
         )
 
         mock_make_all_devices.assert_called_once_with(
             device_module, some_argument=1, another_argument="two"
         )
```

### Comparing `blueapi-0.4.3a3/tests/core/test_event.py` & `blueapi-0.4.3rc1/tests/core/test_event.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/tests/messaging/test_stomptemplate.py` & `blueapi-0.4.3rc1/tests/messaging/test_stomptemplate.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/tests/messaging/test_utils.py` & `blueapi-0.4.3rc1/tests/messaging/test_utils.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/tests/service/test_handler.py` & `blueapi-0.4.3rc1/tests/service/test_handler.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/tests/service/test_openapi.py` & `blueapi-0.4.3rc1/tests/service/test_openapi.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/tests/service/test_rest_api.py` & `blueapi-0.4.3rc1/tests/service/test_rest_api.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/tests/service/test_subprocess_handler.py` & `blueapi-0.4.3rc1/tests/service/test_subprocess_handler.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/tests/test_cli.py` & `blueapi-0.4.3rc1/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,17 +178,16 @@
         and str(result.exception) == "Message bus needs to be configured"
     )
 
 
 def test_cannot_run_plans_without_stomp_config(runner: CliRunner):
     result = runner.invoke(main, ["controller", "run", "sleep", '{"time": 5}'])
     assert (
-        isinstance(result.exception, RuntimeError)
-        and str(result.exception)
-        == "Cannot run plans without Stomp configuration to track progress"
+        "Cannot run plans without Stomp configuration to track progress"
+        in result.output
     )
 
 
 @pytest.mark.stomp
 def test_valid_stomp_config_for_listener(runner: CliRunner):
     result = runner.invoke(
         main,
@@ -197,12 +196,7 @@
             "tests/example_yaml/valid_stomp_config.yaml",
             "controller",
             "listen",
         ],
         input="\n",
     )
     assert result.exit_code == 0
-
-
-def test_invalid_condition_for_run(runner: CliRunner):
-    result = runner.invoke(main, ["controller", "run", "sleep", '{"time": 5}'])
-    assert type(result.exception) is RuntimeError
```

### Comparing `blueapi-0.4.3a3/tests/test_config.py` & `blueapi-0.4.3rc1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/tests/utils/test_thread_exception.py` & `blueapi-0.4.3rc1/tests/utils/test_thread_exception.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/tests/worker/devices.py` & `blueapi-0.4.3rc1/tests/worker/devices.py`

 * *Files identical despite different names*

### Comparing `blueapi-0.4.3a3/tests/worker/test_reworker.py` & `blueapi-0.4.3rc1/tests/worker/test_reworker.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,15 +289,15 @@
 
 
 def begin_task_and_wait_until_complete(
     worker: Worker,
     task_id: str,
     timeout: float = 5.0,
 ) -> list[WorkerEvent]:
-    events: "Future[list[WorkerEvent]]" = take_events(
+    events: Future[list[WorkerEvent]] = take_events(
         worker.worker_events,
         lambda event: event.is_complete(),
     )
 
     worker.begin_task(task_id)
     return events.result(timeout=timeout)
 
@@ -351,15 +351,15 @@
 ) -> None:
     event_streams: list[EventStream[Any, int]] = [
         worker.data_events,
         worker.worker_events,
     ]
 
     count = itertools.count()
-    events: "Future[list[Any]]" = take_events_from_streams(
+    events: Future[list[Any]] = take_events_from_streams(
         event_streams,
         lambda _: next(count) >= len(expected_events) - 1,
     )
 
     task_id = worker.submit_task(task)
     worker.begin_task(task_id)
     results = events.result(timeout=timeout)
@@ -376,40 +376,40 @@
 
 E = TypeVar("E")
 
 
 def take_n_events(
     stream: EventStream[E, Any],
     num: int,
-) -> "Future[list[E]]":
+) -> Future[list[E]]:
     count = itertools.count()
     return take_events(stream, lambda _: next(count) >= num)
 
 
 def take_events(
     stream: EventStream[E, Any],
     cutoff_predicate: Callable[[E], bool],
-) -> "Future[list[E]]":
+) -> Future[list[E]]:
     events: list[E] = []
-    future: "Future[list[E]]" = Future()
+    future: Future[list[E]] = Future()
 
     def on_event(event: E, event_id: str | None) -> None:
         events.append(event)
         if cutoff_predicate(event):
             future.set_result(events)
 
     sub = stream.subscribe(on_event)
     future.add_done_callback(lambda _: stream.unsubscribe(sub))
     return future
 
 
 def take_events_from_streams(
     streams: list[EventStream[Any, int]],
     cutoff_predicate: Callable[[Any], bool],
-) -> "Future[list[Any]]":
+) -> Future[list[Any]]:
     """Returns a collated list of futures for events in numerous event streams.
 
     The support for generic and algebraic types doesn't appear to extend to
     taking an arbitrary list of concrete types with single but differing
     generic arguments while also maintaining the generality of the argument
     types.
 
@@ -422,15 +422,15 @@
             EventStream[DataEvent, int],
             EventStream[ProgressEvent, int]
         ]
     ]
 
     """
     events: list[Any] = []
-    future: "Future[list[Any]]" = Future()
+    future: Future[list[Any]] = Future()
 
     def on_event(event: Any, event_id: str | None) -> None:
         print(event)
         events.append(event)
         if cutoff_predicate(event):
             future.set_result(events)
```

