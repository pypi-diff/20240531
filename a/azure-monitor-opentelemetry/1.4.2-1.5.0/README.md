# Comparing `tmp/azure-monitor-opentelemetry-1.4.2.tar.gz` & `tmp/azure-monitor-opentelemetry-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-monitor-opentelemetry-1.4.2.tar", last modified: Tue May 14 23:27:18 2024, max compression
+gzip compressed data, was "azure-monitor-opentelemetry-1.5.0.tar", last modified: Fri May 31 18:16:12 2024, max compression
```

## Comparing `azure-monitor-opentelemetry-1.4.2.tar` & `azure-monitor-opentelemetry-1.5.0.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.336917 azure-monitor-opentelemetry-1.4.2/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11093 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      199 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/MANIFEST.in
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8273 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/NOTICE.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20095 2024-05-14 23:27:18.336917 azure-monitor-opentelemetry-1.4.2/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19172 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.320917 azure-monitor-opentelemetry-1.4.2/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.320917 azure-monitor-opentelemetry-1.4.2/azure/monitor/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.320917 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      480 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.324917 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_autoinstrumentation/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      305 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_autoinstrumentation/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1560 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_autoinstrumentation/configurator.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3140 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_autoinstrumentation/distro.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8768 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_configure.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1893 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_constants.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.324917 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_diagnostics/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_diagnostics/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3611 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_diagnostics/diagnostic_logging.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2282 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_diagnostics/status_logger.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      709 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_types.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.324917 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_utils/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2065 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_utils/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5914 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_utils/configurations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      325 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_version.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      193 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.324917 azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20095 2024-05-14 23:27:18.000000 azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3081 2024-05-14 23:27:18.000000 azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-14 23:27:18.000000 azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      295 2024-05-14 23:27:18.000000 azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/entry_points.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-14 23:27:18.000000 azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      481 2024-05-14 23:27:18.000000 azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-05-14 23:27:18.000000 azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      135 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/pyproject.toml
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.324917 azure-monitor-opentelemetry-1.4.2/samples/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5377 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.328917 azure-monitor-opentelemetry-1.4.2/samples/logging/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1285 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/logging/basic.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      845 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/logging/correlated_logs.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      634 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/logging/custom_properties.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      818 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/logging/exception_logs.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/logging/logs_with_traces.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.328917 azure-monitor-opentelemetry-1.4.2/samples/metrics/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      904 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/metrics/attributes.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1579 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/metrics/instruments.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.328917 azure-monitor-opentelemetry-1.4.2/samples/tracing/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      542 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/azure_core.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      740 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/db_psycopg2.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.316917 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.328917 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.332917 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      157 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/admin.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      240 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/apps.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.332917 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/migrations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/migrations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      151 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/models.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      154 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/tests.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      262 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/urls.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      626 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/views.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1130 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/manage.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.332917 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      871 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/asgi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3404 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/settings.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      820 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/urls.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      837 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/wsgi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2096 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/filter_spans.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1217 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/http_fastapi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1088 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/http_flask.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1302 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/http_requests.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1106 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/http_urllib.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1087 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/http_urllib3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      834 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/instrumentation_options.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1005 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/manually_instrumented.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1306 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/modify_spans.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      801 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/sampling.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      548 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/samples/tracing/simple.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-05-14 23:27:18.336917 azure-monitor-opentelemetry-1.4.2/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3719 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.332917 azure-monitor-opentelemetry-1.4.2/tests/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.332917 azure-monitor-opentelemetry-1.4.2/tests/autoinstrumentation/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2454 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/autoinstrumentation/test_configurator.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6167 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/autoinstrumentation/test_distro.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      515 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/conftest.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.332917 azure-monitor-opentelemetry-1.4.2/tests/diagnostics/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6878 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/diagnostics/test_diagnostic_logging.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5886 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/diagnostics/test_status_logger.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.332917 azure-monitor-opentelemetry-1.4.2/tests/exporter/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1365 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/exporter/test_exporter.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.336917 azure-monitor-opentelemetry-1.4.2/tests/instrumentation/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      764 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_django.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      849 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_fastapi.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      839 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_flask.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      953 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_psycopg2.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      774 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_requests.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      764 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_urllib.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      769 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_urllib3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17585 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/test_configure.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-14 23:27:18.336917 azure-monitor-opentelemetry-1.4.2/tests/utils/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10091 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/utils/test_configurations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4396 2024-05-14 23:25:35.000000 azure-monitor-opentelemetry-1.4.2/tests/utils/test_utils.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.609822 azure-monitor-opentelemetry-1.5.0/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11297 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      199 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8273 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/NOTICE.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20319 2024-05-31 18:16:12.609822 azure-monitor-opentelemetry-1.5.0/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19396 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.593822 azure-monitor-opentelemetry-1.5.0/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.593822 azure-monitor-opentelemetry-1.5.0/azure/monitor/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/azure/monitor/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.597822 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      480 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.597822 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_autoinstrumentation/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      305 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_autoinstrumentation/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1560 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_autoinstrumentation/configurator.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3140 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_autoinstrumentation/distro.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9711 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_configure.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1941 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_constants.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.597822 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_diagnostics/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_diagnostics/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3611 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_diagnostics/diagnostic_logging.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2282 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_diagnostics/status_logger.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      709 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_types.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.597822 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_utils/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2065 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_utils/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6022 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_utils/configurations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      325 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_version.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      193 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.597822 azure-monitor-opentelemetry-1.5.0/azure_monitor_opentelemetry.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20319 2024-05-31 18:16:12.000000 azure-monitor-opentelemetry-1.5.0/azure_monitor_opentelemetry.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3113 2024-05-31 18:16:12.000000 azure-monitor-opentelemetry-1.5.0/azure_monitor_opentelemetry.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-31 18:16:12.000000 azure-monitor-opentelemetry-1.5.0/azure_monitor_opentelemetry.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      295 2024-05-31 18:16:12.000000 azure-monitor-opentelemetry-1.5.0/azure_monitor_opentelemetry.egg-info/entry_points.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-31 18:16:12.000000 azure-monitor-opentelemetry-1.5.0/azure_monitor_opentelemetry.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      481 2024-05-31 18:16:12.000000 azure-monitor-opentelemetry-1.5.0/azure_monitor_opentelemetry.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-05-31 18:16:12.000000 azure-monitor-opentelemetry-1.5.0/azure_monitor_opentelemetry.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      135 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/pyproject.toml
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.597822 azure-monitor-opentelemetry-1.5.0/samples/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5586 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.601822 azure-monitor-opentelemetry-1.5.0/samples/logging/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1285 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/logging/basic.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      845 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/logging/correlated_logs.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      634 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/logging/custom_properties.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      818 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/logging/exception_logs.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      847 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/logging/logs_with_traces.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.601822 azure-monitor-opentelemetry-1.5.0/samples/metrics/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      904 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/metrics/attributes.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1579 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/metrics/instruments.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1237 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/metrics/live_metrics.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.601822 azure-monitor-opentelemetry-1.5.0/samples/tracing/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      542 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/azure_core.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      740 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/db_psycopg2.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.589822 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.601822 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.605822 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/example/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/example/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      157 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/example/admin.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      240 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/example/apps.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.605822 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/example/migrations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/example/migrations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      151 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/example/models.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      154 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/example/tests.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      262 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/example/urls.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      626 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/example/views.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1130 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/manage.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.605822 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/sample/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       94 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/sample/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      871 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/sample/asgi.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3404 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/sample/settings.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      820 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/sample/urls.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      837 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/sample/wsgi.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2096 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/filter_spans.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1217 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/http_fastapi.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1088 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/http_flask.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1302 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/http_requests.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1106 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/http_urllib.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1087 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/http_urllib3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      834 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/instrumentation_options.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1005 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/manually_instrumented.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1306 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/modify_spans.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      801 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/sampling.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      548 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/samples/tracing/simple.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-05-31 18:16:12.609822 azure-monitor-opentelemetry-1.5.0/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3719 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.605822 azure-monitor-opentelemetry-1.5.0/tests/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.605822 azure-monitor-opentelemetry-1.5.0/tests/autoinstrumentation/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2454 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/tests/autoinstrumentation/test_configurator.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6167 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/tests/autoinstrumentation/test_distro.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      515 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/tests/conftest.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.605822 azure-monitor-opentelemetry-1.5.0/tests/diagnostics/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6878 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/tests/diagnostics/test_diagnostic_logging.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5886 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/tests/diagnostics/test_status_logger.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.605822 azure-monitor-opentelemetry-1.5.0/tests/exporter/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1365 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/tests/exporter/test_exporter.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.609822 azure-monitor-opentelemetry-1.5.0/tests/instrumentation/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      764 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/tests/instrumentation/test_django.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      849 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/tests/instrumentation/test_fastapi.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      839 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/tests/instrumentation/test_flask.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      953 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/tests/instrumentation/test_psycopg2.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      774 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/tests/instrumentation/test_requests.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      764 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/tests/instrumentation/test_urllib.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      769 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/tests/instrumentation/test_urllib3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19751 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/tests/test_configure.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-31 18:16:12.609822 azure-monitor-opentelemetry-1.5.0/tests/utils/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10162 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/tests/utils/test_configurations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4396 2024-05-31 18:14:20.000000 azure-monitor-opentelemetry-1.5.0/tests/utils/test_utils.py
```

### Comparing `azure-monitor-opentelemetry-1.4.2/CHANGELOG.md` & `azure-monitor-opentelemetry-1.5.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,29 @@
 # Release History
 
+## 1.5.0 (2024-05-31)
+
+### Features Added
+
+- Enable live metrics feature
+    ([#35566](https://github.com/Azure/azure-sdk-for-python/pull/35566))
+
 ## 1.4.2 (2024-05-20)
 
 ### Features Added
 
 - Add diagnostics for sdk detection and backoff
     ([#35610](https://github.com/Azure/azure-sdk-for-python/pull/35610))
 
+### Breaking Changes
+
+### Bugs Fixed
+
+### Other Changes
+
 ## 1.4.1 (2024-04-25)
 
 ### Features Added
 
 - Enable sampling for attach
     ([#35218](https://github.com/Azure/azure-sdk-for-python/pull/35218))
```

### Comparing `azure-monitor-opentelemetry-1.4.2/LICENSE` & `azure-monitor-opentelemetry-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/NOTICE.txt` & `azure-monitor-opentelemetry-1.5.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/PKG-INFO` & `azure-monitor-opentelemetry-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-monitor-opentelemetry
-Version: 1.4.2
+Version: 1.5.0
 Summary: Microsoft Azure Monitor Opentelemetry Distro Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -79,14 +79,15 @@
 ### Usage
 
 You can use `configure_azure_monitor` to set up instrumentation for your app to Azure Monitor. `configure_azure_monitor` supports the following optional arguments. All pass-in parameters take priority over any related environment variables.
 
 | Parameter | Description | Environment Variable |
 |-------------------|----------------------------------------------------|----------------------|
 | `connection_string` | The [connection string][connection_string_doc] for your Application Insights resource. The connection string will be automatically populated from the `APPLICATIONINSIGHTS_CONNECTION_STRING` environment variable if not explicitly passed in. | `APPLICATIONINSIGHTS_CONNECTION_STRING` |
+| `enable_live_metrics` | Enable [live metrics][application_insights_live_metrics] feature. Defaults to `False`. | `N/A` |
 | `logger_name` | The name of the [Python logger][python_logger] under which telemetry is collected. | `N/A` |
 | `instrumentation_options` | A nested dictionary that determines which instrumentations to enable or disable. Instrumentations are referred to by their [Library Names](#officially-supported-instrumentations). For example, `{"azure_sdk": {"enabled": False}, "flask": {"enabled": False}, "django": {"enabled": True}}` will disable Azure Core Tracing and the Flask instrumentation but leave Django and the other default instrumentations enabled. The `OTEL_PYTHON_DISABLED_INSTRUMENTATIONS` environment variable explained below can also be used to disable instrumentations. | `N/A` |
 | `resource` | Specifies the OpenTelemetry [Resource][ot_spec_resource] associated with your application. Passed in [Resource Attributes][ot_spec_resource_attributes] take priority over default attributes and those from [Resource Detectors][ot_python_resource_detectors]. | [OTEL_SERVICE_NAME][ot_spec_service_name], [OTEL_RESOURCE_ATTRIBUTES][ot_spec_resource_attributes], [OTEL_EXPERIMENTAL_RESOURCE_DETECTORS][ot_python_resource_detectors] |
 | `span_processors` | A list of [span processors][ot_span_processor] that will perform processing on each of your spans before they are exported. Useful for filtering/modifying telemetry. | `N/A` |
 
 You can configure further with [OpenTelemetry environment variables][ot_env_vars].
 
@@ -229,14 +230,15 @@
 <!-- LINKS -->
 [azure_core_tracing_opentelemetry_plugin]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/core/azure-core-tracing-opentelemetry
 [azure_core_tracing_opentelemetry_plugin_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/tracing/azure_core.py
 [azure_monitor_enable_docs]: https://learn.microsoft.com/azure/azure-monitor/app/opentelemetry-enable?tabs=python
 [azure_monitor_opentelemetry_exporters]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter#microsoft-opentelemetry-exporter-for-azure-monitor
 [azure_portal]: https://portal.azure.com
 [azure_sub]: https://azure.microsoft.com/free/
+[application_insights_live_metrics]: https://learn.microsoft.com/azure/azure-monitor/app/live-stream
 [application_insights_namespace]: https://learn.microsoft.com/azure/azure-monitor/app/app-insights-overview
 [application_insights_sampling]: https://learn.microsoft.com/azure/azure-monitor/app/sampling
 [connection_string_doc]: https://learn.microsoft.com/azure/azure-monitor/app/sdk-connection-string
 [distro_feature_request]: https://github.com/Azure/azure-sdk-for-python/issues/new
 [exporter_configuration_docs]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter#configuration
 [ot_env_vars]: https://opentelemetry.io/docs/reference/specification/sdk-environment-variables/
 [ot_instrumentations]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation
```

### Comparing `azure-monitor-opentelemetry-1.4.2/README.md` & `azure-monitor-opentelemetry-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 ### Usage
 
 You can use `configure_azure_monitor` to set up instrumentation for your app to Azure Monitor. `configure_azure_monitor` supports the following optional arguments. All pass-in parameters take priority over any related environment variables.
 
 | Parameter | Description | Environment Variable |
 |-------------------|----------------------------------------------------|----------------------|
 | `connection_string` | The [connection string][connection_string_doc] for your Application Insights resource. The connection string will be automatically populated from the `APPLICATIONINSIGHTS_CONNECTION_STRING` environment variable if not explicitly passed in. | `APPLICATIONINSIGHTS_CONNECTION_STRING` |
+| `enable_live_metrics` | Enable [live metrics][application_insights_live_metrics] feature. Defaults to `False`. | `N/A` |
 | `logger_name` | The name of the [Python logger][python_logger] under which telemetry is collected. | `N/A` |
 | `instrumentation_options` | A nested dictionary that determines which instrumentations to enable or disable. Instrumentations are referred to by their [Library Names](#officially-supported-instrumentations). For example, `{"azure_sdk": {"enabled": False}, "flask": {"enabled": False}, "django": {"enabled": True}}` will disable Azure Core Tracing and the Flask instrumentation but leave Django and the other default instrumentations enabled. The `OTEL_PYTHON_DISABLED_INSTRUMENTATIONS` environment variable explained below can also be used to disable instrumentations. | `N/A` |
 | `resource` | Specifies the OpenTelemetry [Resource][ot_spec_resource] associated with your application. Passed in [Resource Attributes][ot_spec_resource_attributes] take priority over default attributes and those from [Resource Detectors][ot_python_resource_detectors]. | [OTEL_SERVICE_NAME][ot_spec_service_name], [OTEL_RESOURCE_ATTRIBUTES][ot_spec_resource_attributes], [OTEL_EXPERIMENTAL_RESOURCE_DETECTORS][ot_python_resource_detectors] |
 | `span_processors` | A list of [span processors][ot_span_processor] that will perform processing on each of your spans before they are exported. Useful for filtering/modifying telemetry. | `N/A` |
 
 You can configure further with [OpenTelemetry environment variables][ot_env_vars].
 
@@ -206,14 +207,15 @@
 <!-- LINKS -->
 [azure_core_tracing_opentelemetry_plugin]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/core/azure-core-tracing-opentelemetry
 [azure_core_tracing_opentelemetry_plugin_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/tracing/azure_core.py
 [azure_monitor_enable_docs]: https://learn.microsoft.com/azure/azure-monitor/app/opentelemetry-enable?tabs=python
 [azure_monitor_opentelemetry_exporters]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter#microsoft-opentelemetry-exporter-for-azure-monitor
 [azure_portal]: https://portal.azure.com
 [azure_sub]: https://azure.microsoft.com/free/
+[application_insights_live_metrics]: https://learn.microsoft.com/azure/azure-monitor/app/live-stream
 [application_insights_namespace]: https://learn.microsoft.com/azure/azure-monitor/app/app-insights-overview
 [application_insights_sampling]: https://learn.microsoft.com/azure/azure-monitor/app/sampling
 [connection_string_doc]: https://learn.microsoft.com/azure/azure-monitor/app/sdk-connection-string
 [distro_feature_request]: https://github.com/Azure/azure-sdk-for-python/issues/new
 [exporter_configuration_docs]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter#configuration
 [ot_env_vars]: https://opentelemetry.io/docs/reference/specification/sdk-environment-variables/
 [ot_instrumentations]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation
```

### Comparing `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_autoinstrumentation/configurator.py` & `azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_autoinstrumentation/configurator.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_autoinstrumentation/distro.py` & `azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_autoinstrumentation/distro.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_configure.py` & `azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_configure.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,46 +2,52 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License in the project root for
 # license information.
 # --------------------------------------------------------------------------
 from logging import getLogger
 from typing import Dict, cast
 
-from opentelemetry._logs import get_logger_provider, set_logger_provider
+from opentelemetry._logs import set_logger_provider
 from opentelemetry.instrumentation.dependencies import (
     get_dist_dependency_conflicts,
 )
 from opentelemetry.instrumentation.instrumentor import ( # type: ignore
     BaseInstrumentor,
 )
 from opentelemetry.metrics import set_meter_provider
 from opentelemetry.sdk._logs import LoggerProvider, LoggingHandler
 from opentelemetry.sdk._logs.export import BatchLogRecordProcessor
 from opentelemetry.sdk.metrics import MeterProvider
 from opentelemetry.sdk.metrics.export import PeriodicExportingMetricReader
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
-from opentelemetry.trace import get_tracer_provider, set_tracer_provider
+from opentelemetry.trace import set_tracer_provider
 from pkg_resources import iter_entry_points  # type: ignore
 
 from azure.core.settings import settings
 from azure.core.tracing.ext.opentelemetry_span import OpenTelemetrySpan
 from azure.monitor.opentelemetry._constants import (
     _ALL_SUPPORTED_INSTRUMENTED_LIBRARIES,
     _AZURE_SDK_INSTRUMENTATION_NAME,
     DISABLE_LOGGING_ARG,
     DISABLE_METRICS_ARG,
     DISABLE_TRACING_ARG,
+    ENABLE_LIVE_METRICS_ARG,
     LOGGER_NAME_ARG,
     RESOURCE_ARG,
     SAMPLING_RATIO_ARG,
     SPAN_PROCESSORS_ARG,
 )
 from azure.monitor.opentelemetry._types import ConfigurationValue
+from azure.monitor.opentelemetry.exporter._quickpulse import enable_live_metrics  # pylint: disable=import-error,no-name-in-module
+from azure.monitor.opentelemetry.exporter._quickpulse._processor import (  # pylint: disable=import-error,no-name-in-module
+    _QuickpulseLogRecordProcessor,
+    _QuickpulseSpanProcessor,
+)
 from azure.monitor.opentelemetry.exporter import (  # pylint: disable=import-error,no-name-in-module
     ApplicationInsightsSampler,
     AzureMonitorLogExporter,
     AzureMonitorMetricExporter,
     AzureMonitorTraceExporter,
 )
 from azure.monitor.opentelemetry.exporter._utils import _is_attach_enabled # pylint: disable=import-error,no-name-in-module
@@ -74,74 +80,87 @@
      `{"azure_sdk": {"enabled": False}, "flask": {"enabled": False}, "django": {"enabled": True}}`
      will disable Azure Core Tracing and the Flask instrumentation but leave Django and the other default
      instrumentations enabled.
     :keyword ~opentelemetry.sdk.resources.Resource resource: OpenTelemetry Resource object. Passed in Resource
      Attributes take priority over default attributes and those from Resource Detectors.
     :keyword list[~opentelemetry.sdk.trace.SpanProcessor] span_processors: List of `SpanProcessor` objects
      to process every span prior to exporting. Will be run sequentially.
+    :keyword bool enable_live_metrics: Boolean value to determine whether to enable live metrics feature.
+     Defaults to `False`.
     :keyword str storage_directory: Storage directory in which to store retry files. Defaults to
      `<tempfile.gettempdir()>/Microsoft/AzureMonitor/opentelemetry-python-<your-instrumentation-key>`.
     :rtype: None
     """
 
     _send_attach_warning()
 
     configurations = _get_configurations(**kwargs)
 
     disable_tracing = configurations[DISABLE_TRACING_ARG]
     disable_logging = configurations[DISABLE_LOGGING_ARG]
     disable_metrics = configurations[DISABLE_METRICS_ARG]
+    enable_live_metrics_config = configurations[ENABLE_LIVE_METRICS_ARG]
 
     # Setup tracing pipeline
     if not disable_tracing:
         _setup_tracing(configurations)
 
     # Setup logging pipeline
     if not disable_logging:
         _setup_logging(configurations)
 
     # Setup metrics pipeline
     if not disable_metrics:
         _setup_metrics(configurations)
 
+    # Setup live metrics
+    if enable_live_metrics_config:
+        _setup_live_metrics(configurations)
+
     # Setup instrumentations
     # Instrumentations need to be setup last so to use the global providers
     # instanstiated in the other setup steps
     _setup_instrumentations(configurations)
 
 
 def _setup_tracing(configurations: Dict[str, ConfigurationValue]):
     resource: Resource = configurations[RESOURCE_ARG] # type: ignore
     sampling_ratio = configurations[SAMPLING_RATIO_ARG]
     tracer_provider = TracerProvider(
         sampler=ApplicationInsightsSampler(sampling_ratio=cast(float, sampling_ratio)),
         resource=resource
     )
-    set_tracer_provider(tracer_provider)
     for span_processor in configurations[SPAN_PROCESSORS_ARG]: # type: ignore
-        get_tracer_provider().add_span_processor(span_processor) # type: ignore
+        tracer_provider.add_span_processor(span_processor) # type: ignore
+    if configurations.get(ENABLE_LIVE_METRICS_ARG):
+        qsp = _QuickpulseSpanProcessor()
+        tracer_provider.add_span_processor(qsp)
     trace_exporter = AzureMonitorTraceExporter(**configurations)
     bsp = BatchSpanProcessor(
         trace_exporter,
     )
-    get_tracer_provider().add_span_processor(bsp) # type: ignore
+    tracer_provider.add_span_processor(bsp)
+    set_tracer_provider(tracer_provider)
     if _is_instrumentation_enabled(configurations, _AZURE_SDK_INSTRUMENTATION_NAME):
         settings.tracing_implementation = OpenTelemetrySpan
 
 
 def _setup_logging(configurations: Dict[str, ConfigurationValue]):
     resource: Resource = configurations[RESOURCE_ARG] # type: ignore
     logger_provider = LoggerProvider(resource=resource)
-    set_logger_provider(logger_provider)
+    if configurations.get(ENABLE_LIVE_METRICS_ARG):
+        qlp = _QuickpulseLogRecordProcessor()
+        logger_provider.add_log_record_processor(qlp)
     log_exporter = AzureMonitorLogExporter(**configurations)
     log_record_processor = BatchLogRecordProcessor(
         log_exporter,
     )
-    get_logger_provider().add_log_record_processor(log_record_processor) # type: ignore
-    handler = LoggingHandler(logger_provider=get_logger_provider())
+    logger_provider.add_log_record_processor(log_record_processor)
+    set_logger_provider(logger_provider)
+    handler = LoggingHandler(logger_provider=logger_provider)
     logger_name: str = configurations[LOGGER_NAME_ARG] # type: ignore
     getLogger(logger_name).addHandler(handler)
 
 
 def _setup_metrics(configurations: Dict[str, ConfigurationValue]):
     resource: Resource = configurations[RESOURCE_ARG] # type: ignore
     metric_exporter = AzureMonitorMetricExporter(**configurations)
@@ -149,14 +168,18 @@
     meter_provider = MeterProvider(
         metric_readers=[reader],
         resource=resource
     )
     set_meter_provider(meter_provider)
 
 
+def _setup_live_metrics(configurations):
+    enable_live_metrics(**configurations)
+
+
 def _setup_instrumentations(configurations: Dict[str, ConfigurationValue]):
     # use pkg_resources for now until https://github.com/open-telemetry/opentelemetry-python/pull/3168 is merged
     for entry_point in iter_entry_points(
         "opentelemetry_instrumentor"
     ):
         lib_name = entry_point.name
         if lib_name not in _ALL_SUPPORTED_INSTRUMENTED_LIBRARIES:
```

### Comparing `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_constants.py` & `azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from azure.monitor.opentelemetry.exporter._constants import (  # pylint: disable=import-error,no-name-in-module
     _AZURE_MONITOR_DISTRO_VERSION_ARG,
 )
 
 # --------------------Configuration------------------------------------------
 
 CONNECTION_STRING_ARG = "connection_string"
+ENABLE_LIVE_METRICS_ARG = "enable_live_metrics"
 DISABLE_AZURE_CORE_TRACING_ARG = "disable_azure_core_tracing"
 DISABLE_LOGGING_ARG = "disable_logging"
 DISABLE_METRICS_ARG = "disable_metrics"
 DISABLE_TRACING_ARG = "disable_tracing"
 DISTRO_VERSION_ARG = _AZURE_MONITOR_DISTRO_VERSION_ARG
 LOGGER_NAME_ARG = "logger_name"
 INSTRUMENTATION_OPTIONS_ARG = "instrumentation_options"
```

### Comparing `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_diagnostics/diagnostic_logging.py` & `azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_diagnostics/diagnostic_logging.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_diagnostics/status_logger.py` & `azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_diagnostics/status_logger.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_types.py` & `azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_types.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_utils/__init__.py` & `azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/azure/monitor/opentelemetry/_utils/configurations.py` & `azure-monitor-opentelemetry-1.5.0/azure/monitor/opentelemetry/_utils/configurations.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     _AZURE_VM_RESOURCE_DETECTOR_NAME,
     _FULLY_SUPPORTED_INSTRUMENTED_LIBRARIES,
     _PREVIEW_INSTRUMENTED_LIBRARIES,
     DISABLE_LOGGING_ARG,
     DISABLE_METRICS_ARG,
     DISABLE_TRACING_ARG,
     DISTRO_VERSION_ARG,
+    ENABLE_LIVE_METRICS_ARG,
     INSTRUMENTATION_OPTIONS_ARG,
     LOGGER_NAME_ARG,
     RESOURCE_ARG,
     SAMPLING_RATIO_ARG,
     SPAN_PROCESSORS_ARG,
 )
 from azure.monitor.opentelemetry._types import ConfigurationValue
@@ -64,14 +65,15 @@
     _default_disable_metrics(configurations)
     _default_disable_tracing(configurations)
     _default_logger_name(configurations)
     _default_resource(configurations)
     _default_sampling_ratio(configurations)
     _default_instrumentation_options(configurations)
     _default_span_processors(configurations)
+    _default_enable_live_metrics(configurations)
 
     return configurations
 
 
 def _default_disable_logging(configurations):
     default = False
     if OTEL_LOGS_EXPORTER in environ:
@@ -93,16 +95,15 @@
     if OTEL_TRACES_EXPORTER in environ:
         if environ[OTEL_TRACES_EXPORTER].lower().strip() == "none":
             default = True
     configurations[DISABLE_TRACING_ARG] = default
 
 
 def _default_logger_name(configurations):
-    if LOGGER_NAME_ARG not in configurations:
-        configurations[LOGGER_NAME_ARG] = ""
+    configurations.setdefault(LOGGER_NAME_ARG, "")
 
 
 def _default_resource(configurations):
     environ.setdefault(
         OTEL_EXPERIMENTAL_RESOURCE_DETECTORS,
         ",".join(_SUPPORTED_RESOURCE_DETECTORS)
     )
@@ -143,16 +144,19 @@
         options.update(instrumentation_options.get(lib_name, {}))
         merged_instrumentation_options[lib_name] = options
 
     configurations[INSTRUMENTATION_OPTIONS_ARG] = merged_instrumentation_options
 
 
 def _default_span_processors(configurations):
-    if SPAN_PROCESSORS_ARG not in configurations:
-        configurations[SPAN_PROCESSORS_ARG] = []
+    configurations.setdefault(SPAN_PROCESSORS_ARG, [])
+
+
+def _default_enable_live_metrics(configurations):
+    configurations.setdefault(ENABLE_LIVE_METRICS_ARG, False)
 
 
 def _get_otel_disabled_instrumentations():
     disabled_instrumentation = environ.get(
         OTEL_PYTHON_DISABLED_INSTRUMENTATIONS, ""
     )
     disabled_instrumentation = disabled_instrumentation.split(",")
```

### Comparing `azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/PKG-INFO` & `azure-monitor-opentelemetry-1.5.0/azure_monitor_opentelemetry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-monitor-opentelemetry
-Version: 1.4.2
+Version: 1.5.0
 Summary: Microsoft Azure Monitor Opentelemetry Distro Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry
 Author: Microsoft Corporation
 Author-email: ascl@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -79,14 +79,15 @@
 ### Usage
 
 You can use `configure_azure_monitor` to set up instrumentation for your app to Azure Monitor. `configure_azure_monitor` supports the following optional arguments. All pass-in parameters take priority over any related environment variables.
 
 | Parameter | Description | Environment Variable |
 |-------------------|----------------------------------------------------|----------------------|
 | `connection_string` | The [connection string][connection_string_doc] for your Application Insights resource. The connection string will be automatically populated from the `APPLICATIONINSIGHTS_CONNECTION_STRING` environment variable if not explicitly passed in. | `APPLICATIONINSIGHTS_CONNECTION_STRING` |
+| `enable_live_metrics` | Enable [live metrics][application_insights_live_metrics] feature. Defaults to `False`. | `N/A` |
 | `logger_name` | The name of the [Python logger][python_logger] under which telemetry is collected. | `N/A` |
 | `instrumentation_options` | A nested dictionary that determines which instrumentations to enable or disable. Instrumentations are referred to by their [Library Names](#officially-supported-instrumentations). For example, `{"azure_sdk": {"enabled": False}, "flask": {"enabled": False}, "django": {"enabled": True}}` will disable Azure Core Tracing and the Flask instrumentation but leave Django and the other default instrumentations enabled. The `OTEL_PYTHON_DISABLED_INSTRUMENTATIONS` environment variable explained below can also be used to disable instrumentations. | `N/A` |
 | `resource` | Specifies the OpenTelemetry [Resource][ot_spec_resource] associated with your application. Passed in [Resource Attributes][ot_spec_resource_attributes] take priority over default attributes and those from [Resource Detectors][ot_python_resource_detectors]. | [OTEL_SERVICE_NAME][ot_spec_service_name], [OTEL_RESOURCE_ATTRIBUTES][ot_spec_resource_attributes], [OTEL_EXPERIMENTAL_RESOURCE_DETECTORS][ot_python_resource_detectors] |
 | `span_processors` | A list of [span processors][ot_span_processor] that will perform processing on each of your spans before they are exported. Useful for filtering/modifying telemetry. | `N/A` |
 
 You can configure further with [OpenTelemetry environment variables][ot_env_vars].
 
@@ -229,14 +230,15 @@
 <!-- LINKS -->
 [azure_core_tracing_opentelemetry_plugin]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/core/azure-core-tracing-opentelemetry
 [azure_core_tracing_opentelemetry_plugin_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/tracing/azure_core.py
 [azure_monitor_enable_docs]: https://learn.microsoft.com/azure/azure-monitor/app/opentelemetry-enable?tabs=python
 [azure_monitor_opentelemetry_exporters]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter#microsoft-opentelemetry-exporter-for-azure-monitor
 [azure_portal]: https://portal.azure.com
 [azure_sub]: https://azure.microsoft.com/free/
+[application_insights_live_metrics]: https://learn.microsoft.com/azure/azure-monitor/app/live-stream
 [application_insights_namespace]: https://learn.microsoft.com/azure/azure-monitor/app/app-insights-overview
 [application_insights_sampling]: https://learn.microsoft.com/azure/azure-monitor/app/sampling
 [connection_string_doc]: https://learn.microsoft.com/azure/azure-monitor/app/sdk-connection-string
 [distro_feature_request]: https://github.com/Azure/azure-sdk-for-python/issues/new
 [exporter_configuration_docs]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry-exporter#configuration
 [ot_env_vars]: https://opentelemetry.io/docs/reference/specification/sdk-environment-variables/
 [ot_instrumentations]: https://github.com/open-telemetry/opentelemetry-python-contrib/tree/main/instrumentation
```

### Comparing `azure-monitor-opentelemetry-1.4.2/azure_monitor_opentelemetry.egg-info/SOURCES.txt` & `azure-monitor-opentelemetry-1.5.0/azure_monitor_opentelemetry.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 samples/logging/basic.py
 samples/logging/correlated_logs.py
 samples/logging/custom_properties.py
 samples/logging/exception_logs.py
 samples/logging/logs_with_traces.py
 samples/metrics/attributes.py
 samples/metrics/instruments.py
+samples/metrics/live_metrics.py
 samples/tracing/azure_core.py
 samples/tracing/db_psycopg2.py
 samples/tracing/filter_spans.py
 samples/tracing/http_fastapi.py
 samples/tracing/http_flask.py
 samples/tracing/http_requests.py
 samples/tracing/http_urllib.py
```

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/README.md` & `azure-monitor-opentelemetry-1.5.0/samples/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 |[logging/correlated_logs.py][correlated_logs] | Produce logs correlated with spans |
 |[logging/custom_properties.py][custom_properties] | Add custom propterties to logs |
 |[logging/exception_logs.py][exception_logs] | Produce exception logs |
 |[logging/logs_with_traces.py][logs_with_traces] | Produce correlated logs inside an instrumented http library's distributed tracing |
 |[logging/basic.py][logging_basic] | Produce logs |
 |[metrics/attributes.py][attributes] | Add attributes to custom metrics counters |
 |[metrics/instruments.py][instruments] | Create observable instruments |
+|[metrics/live_metrics.py][live_metrics] | Live metrics feature |
 |[tracing/django/sample/manage.py][django] | Instrument a django app |
 |[tracing/db_psycopg2.py][db_psycopg2] | Instrument the PsycoPG2 library |
 |[tracing/http_fastapi.py][http_fastapi] | Instrument a FastAPI app |
 |[tracing/http_flask.py][http_flask] | Instrument a Flask app |
 |[tracing/http_requests.py][http_requests] | Instrument the Requests library |
 |[tracing/http_urllib.py][http_urllib] | Instrument the URLLib library |
 |[tracing/http_urllib3.py][http_urllib3] | Instrument the URLLib library |
@@ -64,14 +65,15 @@
 [correlated_logs]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/logging/correlated_logs.py
 [custom_properties]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/logging/custom_properties.py
 [exception_logs]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/logging/exception_logs.py
 [logs_with_traces]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/logging/logs_with_traces.py
 [logging_basic]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/logging/basic.py
 [attributes]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/metrics/attributes.py
 [instruments]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/metrics/instruments.py
+[instruments]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/metrics/live_metrics.py
 [django]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/tracing/django/sample/manage.py
 [db_psycopg2]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/tracing/db_psycopg2.py
 [http_fastapi]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/tracing/http_fastapi.py
 [http_flask]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/tracing/http_flask.py
 [http_requests]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/tracing/http_requests.py
 [http_urllib]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/tracing/http_urllib.py
 [http_urllib3]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/monitor/azure-monitor-opentelemetry/samples/tracing/http_urllib3.py
```

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/logging/basic.py` & `azure-monitor-opentelemetry-1.5.0/samples/logging/basic.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/logging/correlated_logs.py` & `azure-monitor-opentelemetry-1.5.0/samples/logging/correlated_logs.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/logging/custom_properties.py` & `azure-monitor-opentelemetry-1.5.0/samples/logging/custom_properties.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/logging/exception_logs.py` & `azure-monitor-opentelemetry-1.5.0/samples/logging/exception_logs.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/logging/logs_with_traces.py` & `azure-monitor-opentelemetry-1.5.0/samples/logging/logs_with_traces.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/metrics/attributes.py` & `azure-monitor-opentelemetry-1.5.0/samples/metrics/attributes.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/metrics/instruments.py` & `azure-monitor-opentelemetry-1.5.0/samples/metrics/instruments.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/azure_core.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/azure_core.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/db_psycopg2.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/db_psycopg2.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/example/views.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/example/views.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/manage.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/manage.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/asgi.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/sample/asgi.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/settings.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/sample/settings.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/urls.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/sample/urls.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/django/sample/sample/wsgi.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/django/sample/sample/wsgi.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/filter_spans.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/filter_spans.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/http_fastapi.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/http_fastapi.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/http_flask.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/http_flask.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/http_requests.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/http_requests.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/http_urllib.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/http_urllib.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/http_urllib3.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/http_urllib3.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/instrumentation_options.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/instrumentation_options.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/manually_instrumented.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/manually_instrumented.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/modify_spans.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/modify_spans.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/sampling.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/sampling.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/samples/tracing/simple.py` & `azure-monitor-opentelemetry-1.5.0/samples/tracing/simple.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/setup.py` & `azure-monitor-opentelemetry-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     package_data={
         "pytyped": ["py.typed"],
     },
     python_requires=">=3.8",
     install_requires=[
         "azure-core<2.0.0,>=1.28.0",
         "azure-core-tracing-opentelemetry~=1.0.0b11",
-        "azure-monitor-opentelemetry-exporter~=1.0.0b25",
+        "azure-monitor-opentelemetry-exporter~=1.0.0b26",
         "opentelemetry-instrumentation-django~=0.42b0",
         "opentelemetry-instrumentation-fastapi~=0.42b0",
         "opentelemetry-instrumentation-flask~=0.42b0",
         "opentelemetry-instrumentation-psycopg2~=0.42b0",
         "opentelemetry-instrumentation-requests~=0.42b0",
         "opentelemetry-instrumentation-urllib~=0.42b0",
         "opentelemetry-instrumentation-urllib3~=0.42b0",
```

### Comparing `azure-monitor-opentelemetry-1.4.2/tests/autoinstrumentation/test_configurator.py` & `azure-monitor-opentelemetry-1.5.0/tests/autoinstrumentation/test_configurator.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/tests/autoinstrumentation/test_distro.py` & `azure-monitor-opentelemetry-1.5.0/tests/autoinstrumentation/test_distro.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/tests/conftest.py` & `azure-monitor-opentelemetry-1.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/tests/diagnostics/test_diagnostic_logging.py` & `azure-monitor-opentelemetry-1.5.0/tests/diagnostics/test_diagnostic_logging.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/tests/diagnostics/test_status_logger.py` & `azure-monitor-opentelemetry-1.5.0/tests/diagnostics/test_status_logger.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/tests/exporter/test_exporter.py` & `azure-monitor-opentelemetry-1.5.0/tests/exporter/test_exporter.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_django.py` & `azure-monitor-opentelemetry-1.5.0/tests/instrumentation/test_django.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_fastapi.py` & `azure-monitor-opentelemetry-1.5.0/tests/instrumentation/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_flask.py` & `azure-monitor-opentelemetry-1.5.0/tests/instrumentation/test_flask.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_psycopg2.py` & `azure-monitor-opentelemetry-1.5.0/tests/instrumentation/test_psycopg2.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_requests.py` & `azure-monitor-opentelemetry-1.5.0/tests/instrumentation/test_requests.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_urllib.py` & `azure-monitor-opentelemetry-1.5.0/tests/instrumentation/test_urllib.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/tests/instrumentation/test_urllib3.py` & `azure-monitor-opentelemetry-1.5.0/tests/instrumentation/test_urllib3.py`

 * *Files identical despite different names*

### Comparing `azure-monitor-opentelemetry-1.4.2/tests/test_configure.py` & `azure-monitor-opentelemetry-1.5.0/tests/test_configure.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from opentelemetry.sdk.resources import Resource
 
 from azure.core.tracing.ext.opentelemetry_span import OpenTelemetrySpan
 from azure.monitor.opentelemetry._configure import (
     _send_attach_warning,
     _setup_instrumentations,
+    _setup_live_metrics,
     _setup_logging,
     _setup_metrics,
     _setup_tracing,
     configure_azure_monitor,
 )
 from azure.monitor.opentelemetry._diagnostics.diagnostic_logging import _DISTRO_DETECTS_ATTACH
 
@@ -35,44 +36,52 @@
     @patch(
         "azure.monitor.opentelemetry._configure._send_attach_warning",
     )
     @patch(
         "azure.monitor.opentelemetry._configure._setup_instrumentations",
     )
     @patch(
+        "azure.monitor.opentelemetry._configure._setup_live_metrics",
+    )
+    @patch(
         "azure.monitor.opentelemetry._configure._setup_metrics",
     )
     @patch(
         "azure.monitor.opentelemetry._configure._setup_logging",
     )
     @patch(
         "azure.monitor.opentelemetry._configure._setup_tracing",
     )
     def test_configure_azure_monitor(
         self,
         tracing_mock,
         logging_mock,
         metrics_mock,
+        live_metrics_mock,
         instrumentation_mock,
         detect_attach_mock,
     ):
         kwargs = {
             "connection_string": "test_cs",
         }
         configure_azure_monitor(**kwargs)
         tracing_mock.assert_called_once()
         logging_mock.assert_called_once()
         metrics_mock.assert_called_once()
+        live_metrics_mock.assert_not_called()
         instrumentation_mock.assert_called_once()
         detect_attach_mock.assert_called_once()
 
     @patch(
         "azure.monitor.opentelemetry._configure._setup_instrumentations",
     )
     @patch(
+        "azure.monitor.opentelemetry._configure._setup_live_metrics",
+    )
+    @patch(
         "azure.monitor.opentelemetry._configure._setup_metrics",
     )
     @patch(
         "azure.monitor.opentelemetry._configure._setup_logging",
     )
     @patch(
         "azure.monitor.opentelemetry._configure._setup_tracing",
@@ -82,14 +91,15 @@
     )
     def test_configure_azure_monitor_disable_tracing(
         self,
         config_mock,
         tracing_mock,
         logging_mock,
         metrics_mock,
+        live_metrics_mock,
         instrumentation_mock,
     ):
         configurations = {
             "connection_string": "test_cs",
             "disable_tracing": True,
             "disable_logging": False,
             "disable_metrics": False,
@@ -100,27 +110,32 @@
                 "django": {
                     "enabled": False
                 },
                 "requests": {
                     "enabled": False
                 },
             },
+            "enable_live_metrics": False,
             "resource": TEST_RESOURCE,
         }
         config_mock.return_value = configurations
         configure_azure_monitor()
         tracing_mock.assert_not_called()
         logging_mock.assert_called_once_with(configurations)
         metrics_mock.assert_called_once_with(configurations)
+        live_metrics_mock.assert_not_called()
         instrumentation_mock.assert_called_once_with(configurations)
 
     @patch(
         "azure.monitor.opentelemetry._configure._setup_instrumentations",
     )
     @patch(
+        "azure.monitor.opentelemetry._configure._setup_live_metrics",
+    )
+    @patch(
         "azure.monitor.opentelemetry._configure._setup_metrics",
     )
     @patch(
         "azure.monitor.opentelemetry._configure._setup_logging",
     )
     @patch(
         "azure.monitor.opentelemetry._configure._setup_tracing",
@@ -130,34 +145,40 @@
     )
     def test_configure_azure_monitor_disable_logging(
         self,
         config_mock,
         tracing_mock,
         logging_mock,
         metrics_mock,
+        live_metrics_mock,
         instrumentation_mock,
     ):
         configurations = {
             "connection_string": "test_cs",
             "disable_tracing": False,
             "disable_logging": True,
             "disable_metrics": False,
+            "enable_live_metrics": False,
             "resource": TEST_RESOURCE,
         }
         config_mock.return_value = configurations
         configure_azure_monitor()
         tracing_mock.assert_called_once_with(configurations)
         logging_mock.assert_not_called()
         metrics_mock.assert_called_once_with(configurations)
+        live_metrics_mock.assert_not_called()
         instrumentation_mock.assert_called_once_with(configurations)
 
     @patch(
         "azure.monitor.opentelemetry._configure._setup_instrumentations",
     )
     @patch(
+        "azure.monitor.opentelemetry._configure._setup_live_metrics",
+    )
+    @patch(
         "azure.monitor.opentelemetry._configure._setup_metrics",
     )
     @patch(
         "azure.monitor.opentelemetry._configure._setup_logging",
     )
     @patch(
         "azure.monitor.opentelemetry._configure._setup_tracing",
@@ -167,67 +188,108 @@
     )
     def test_configure_azure_monitor_disable_metrics(
         self,
         config_mock,
         tracing_mock,
         logging_mock,
         metrics_mock,
+        live_metrics_mock,
         instrumentation_mock,
     ):
         configurations = {
             "connection_string": "test_cs",
             "disable_tracing": False,
             "disable_logging": False,
             "disable_metrics": True,
+            "enable_live_metrics": False,
             "resource": TEST_RESOURCE,
         }
         config_mock.return_value = configurations
         configure_azure_monitor()
         tracing_mock.assert_called_once_with(configurations)
         logging_mock.assert_called_once_with(configurations)
         metrics_mock.assert_not_called()
+        live_metrics_mock.assert_not_called()
+        instrumentation_mock.assert_called_once_with(configurations)
+
+    @patch(
+        "azure.monitor.opentelemetry._configure._setup_instrumentations",
+    )
+    @patch(
+        "azure.monitor.opentelemetry._configure._setup_live_metrics",
+    )
+    @patch(
+        "azure.monitor.opentelemetry._configure._setup_metrics",
+    )
+    @patch(
+        "azure.monitor.opentelemetry._configure._setup_logging",
+    )
+    @patch(
+        "azure.monitor.opentelemetry._configure._setup_tracing",
+    )
+    @patch(
+        "azure.monitor.opentelemetry._configure._get_configurations",
+    )
+    def test_configure_azure_monitor_enable_live_metrics(
+        self,
+        config_mock,
+        tracing_mock,
+        logging_mock,
+        metrics_mock,
+        live_metrics_mock,
+        instrumentation_mock,
+    ):
+        configurations = {
+            "connection_string": "test_cs",
+            "disable_tracing": False,
+            "disable_logging": False,
+            "disable_metrics": False,
+            "enable_live_metrics": True,
+            "resource": TEST_RESOURCE,
+        }
+        config_mock.return_value = configurations
+        configure_azure_monitor()
+        tracing_mock.assert_called_once_with(configurations)
+        logging_mock.assert_called_once_with(configurations)
+        metrics_mock.assert_called_once_with(configurations)
+        live_metrics_mock.assert_called_once_with(configurations)
         instrumentation_mock.assert_called_once_with(configurations)
 
     @patch(
         "azure.monitor.opentelemetry._configure.settings",
     )
     @patch(
         "azure.monitor.opentelemetry._configure.BatchSpanProcessor",
     )
     @patch(
         "azure.monitor.opentelemetry._configure.AzureMonitorTraceExporter",
     )
     @patch(
-        "azure.monitor.opentelemetry._configure.get_tracer_provider",
-    )
-    @patch(
         "azure.monitor.opentelemetry._configure.set_tracer_provider",
     )
     @patch(
         "azure.monitor.opentelemetry._configure.TracerProvider",
         autospec=True,
     )
     @patch(
         "azure.monitor.opentelemetry._configure.ApplicationInsightsSampler",
     )
     def test_setup_tracing(
         self,
         sampler_mock,
         tp_mock,
         set_tracer_provider_mock,
-        get_tracer_provider_mock,
         trace_exporter_mock,
         bsp_mock,
         azure_core_mock,
     ):
         sampler_init_mock = Mock()
         sampler_mock.return_value = sampler_init_mock
         tp_init_mock = Mock()
         tp_mock.return_value = tp_init_mock
-        get_tracer_provider_mock.return_value = tp_init_mock
         trace_exp_init_mock = Mock()
         trace_exporter_mock.return_value = trace_exp_init_mock
         bsp_init_mock = Mock()
         bsp_mock.return_value = bsp_init_mock
         custom_sp = Mock()
 
         configurations = {
@@ -242,15 +304,14 @@
         _setup_tracing(configurations)
         sampler_mock.assert_called_once_with(sampling_ratio=0.5)
         tp_mock.assert_called_once_with(
             sampler=sampler_init_mock,
             resource=TEST_RESOURCE
         )
         set_tracer_provider_mock.assert_called_once_with(tp_init_mock)
-        get_tracer_provider_mock.assert_called()
         trace_exporter_mock.assert_called_once_with(**configurations)
         bsp_mock.assert_called_once_with(trace_exp_init_mock)
         self.assertEqual(tp_init_mock.add_span_processor.call_count, 2)
         tp_init_mock.add_span_processor.assert_has_calls([call(custom_sp), call(bsp_init_mock)])
         self.assertEqual(
             azure_core_mock.tracing_implementation, OpenTelemetrySpan
         )
@@ -264,36 +325,31 @@
     @patch(
         "azure.monitor.opentelemetry._configure.BatchLogRecordProcessor",
     )
     @patch(
         "azure.monitor.opentelemetry._configure.AzureMonitorLogExporter",
     )
     @patch(
-        "azure.monitor.opentelemetry._configure.get_logger_provider",
-    )
-    @patch(
         "azure.monitor.opentelemetry._configure.set_logger_provider",
     )
     @patch(
         "azure.monitor.opentelemetry._configure.LoggerProvider",
         autospec=True,
     )
     def test_setup_logging(
         self,
         lp_mock,
         set_logger_provider_mock,
-        get_logger_provider_mock,
         log_exporter_mock,
         blrp_mock,
         logging_handler_mock,
         get_logger_mock,
     ):
         lp_init_mock = Mock()
         lp_mock.return_value = lp_init_mock
-        get_logger_provider_mock.return_value = lp_init_mock
         log_exp_init_mock = Mock()
         log_exporter_mock.return_value = log_exp_init_mock
         blrp_init_mock = Mock()
         blrp_mock.return_value = blrp_init_mock
         logging_handler_init_mock = Mock()
         logging_handler_mock.return_value = logging_handler_init_mock
         logger_mock = Mock()
@@ -304,15 +360,14 @@
             "logger_name": "test",
             "resource": TEST_RESOURCE,
         }
         _setup_logging(configurations)
 
         lp_mock.assert_called_once_with(resource=TEST_RESOURCE)
         set_logger_provider_mock.assert_called_once_with(lp_init_mock)
-        get_logger_provider_mock.assert_called()
         log_exporter_mock.assert_called_once_with(**configurations)
         blrp_mock.assert_called_once_with(
             log_exp_init_mock,
         )
         lp_init_mock.add_log_record_processor.assert_called_once_with(
             blrp_init_mock
         )
@@ -360,14 +415,29 @@
             metric_readers=[reader_init_mock],
             resource=TEST_RESOURCE
         )
         set_meter_provider_mock.assert_called_once_with(mp_init_mock)
         metric_exporter_mock.assert_called_once_with(**configurations)
         reader_mock.assert_called_once_with(metric_exp_init_mock)
 
+    @patch(
+        "azure.monitor.opentelemetry._configure.enable_live_metrics",
+    )
+    def test_setup_live_metrics(
+        self,
+        enable_live_metrics_mock,
+    ):
+        configurations = {
+            "connection_string": "test_cs",
+            "resource": TEST_RESOURCE,
+        }
+        _setup_live_metrics(configurations)
+
+        enable_live_metrics_mock.assert_called_once_with(**configurations)
+
     @patch("azure.monitor.opentelemetry._configure._ALL_SUPPORTED_INSTRUMENTED_LIBRARIES", ("test_instr2"))
     @patch("azure.monitor.opentelemetry._configure._is_instrumentation_enabled")
     @patch("azure.monitor.opentelemetry._configure.get_dist_dependency_conflicts")
     @patch("azure.monitor.opentelemetry._configure.iter_entry_points")
     def test_setup_instrumentations_lib_not_supported(
         self,
         iter_mock,
```

### Comparing `azure-monitor-opentelemetry-1.4.2/tests/utils/test_configurations.py` & `azure-monitor-opentelemetry-1.5.0/tests/utils/test_configurations.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         })
         self.assertEqual(configurations["resource"].attributes, TEST_DEFAULT_RESOURCE.attributes)
         self.assertEqual(environ[OTEL_EXPERIMENTAL_RESOURCE_DETECTORS], "azure_app_service,azure_vm")
         resource_create_mock.assert_called_once_with()
         self.assertEqual(configurations["sampling_ratio"], 1.0)
         self.assertTrue("credential" not in configurations)
         self.assertTrue("storage_directory" not in configurations)
+        self.assertEqual(configurations["enable_live_metrics"], False)
 
     @patch.dict(
         "os.environ",
         {
             OTEL_PYTHON_DISABLED_INSTRUMENTATIONS: "flask , requests,fastapi,azure_sdk",
             SAMPLING_RATIO_ENV_VAR: "0.5",
             OTEL_TRACES_EXPORTER: "None",
```

### Comparing `azure-monitor-opentelemetry-1.4.2/tests/utils/test_utils.py` & `azure-monitor-opentelemetry-1.5.0/tests/utils/test_utils.py`

 * *Files identical despite different names*

