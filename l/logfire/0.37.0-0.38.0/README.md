# Comparing `tmp/logfire-0.37.0.tar.gz` & `tmp/logfire-0.38.0.tar.gz`

## Comparing `logfire-0.37.0.tar` & `logfire-0.38.0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.37.0/Makefile
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/__main__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/cli.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/exceptions.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/propagate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/py.typed
--rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/testing.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/version.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/__init__.py
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/ast_utils.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/async_.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/auth.py
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/backfill.py
--rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/cli.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/collect_system_info.py
--rw-r--r--   0        0        0    56043 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/config.py
--rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/config_params.py
--rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/constants.py
--rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/formatter.py
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/instrument.py
--rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/json_encoder.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/json_formatter.py
--rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/json_schema.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/json_types.py
--rw-r--r--   0        0        0    63477 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/main.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/metrics.py
--rw-r--r--   0        0        0     8756 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/scrubbing.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/stack_info.py
--rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/tracer.py
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/utils.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/auto_trace/__init__.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/auto_trace/import_hook.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/auto_trace/rewrite_ast.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/auto_trace/types.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/exporters/__init__.py
--rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/exporters/console.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/exporters/fallback.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/exporters/file.py
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/exporters/otlp.py
--rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/exporters/processor_wrapper.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/exporters/remove_pending.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/exporters/wrapper.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/asyncpg.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/django.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/executors.py
--rw-r--r--   0        0        0    10656 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/fastapi.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/httpx.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/psycopg.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/requests.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/llm_providers/anthropic.py
--rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/llm_providers/llm_provider.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/llm_providers/openai.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/_internal/integrations/llm_providers/types.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/integrations/__init__.py
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/integrations/logging.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/integrations/loguru.py
--rw-r--r--   0        0        0    19169 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/integrations/pydantic.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 logfire-0.37.0/logfire/integrations/structlog.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/__init__.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/conftest.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/module_used_for_tests.py
--rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_auto_trace.py
--rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_backfill.py
--rw-r--r--   0        0        0    47077 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_cli.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_collect_package_resources.py
--rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_configure.py
--rw-r--r--   0        0        0    29388 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_console_exporter.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_formatter.py
--rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_json_args.py
--rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_json_args_formatting.py
--rw-r--r--   0        0        0   107358 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_logfire.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_loguru.py
--rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_metrics.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_no_production.py
--rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_pydantic_plugin.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_sampling.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_secret_scrubbing.py
--rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_slow_async_callbacks.py
--rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_source_code_extraction.py
--rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_stdlib_logging.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_structlog.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_testing.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/test_utils.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/auto_trace_samples/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/auto_trace_samples/foo.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/auto_trace_samples/simple_nesting.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/exporters/test_fallback_exporter.py
--rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/exporters/test_file_exporter.py
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/exporters/test_otlp_session.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/exporters/test_remove_pending.py
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/exporters/test_retry_fewer_spans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/import_used_for_tests/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/import_used_for_tests/slow_async_callbacks_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/import_used_for_tests/a/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/import_used_for_tests/a/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/__init__.py
--rw-r--r--   0        0        0    24476 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_anthropic.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_asgi.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_asyncpg.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_django.py
--rw-r--r--   0        0        0    44449 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_fastapi.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_flask.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_httpx.py
--rw-r--r--   0        0        0    44244 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_openai.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_psycopg.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_requests.py
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_sqlalchemy.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_starlette.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/test_wsgi.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/__init__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/manage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_app/models.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_app/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.37.0/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.37.0/LICENSE
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 logfire-0.37.0/README.md
--rw-r--r--   0        0        0     8521 2020-02-02 00:00:00.000000 logfire-0.37.0/pyproject.toml
--rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 logfire-0.37.0/PKG-INFO
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.38.0/Makefile
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/__main__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/cli.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/exceptions.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/propagate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/py.typed
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/testing.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/version.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/__init__.py
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/ast_utils.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/async_.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/auth.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/backfill.py
+-rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/cli.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/collect_system_info.py
+-rw-r--r--   0        0        0    56682 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/config.py
+-rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/config_params.py
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/constants.py
+-rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/formatter.py
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/instrument.py
+-rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/json_encoder.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/json_formatter.py
+-rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/json_schema.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/json_types.py
+-rw-r--r--   0        0        0    64101 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/main.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/metrics.py
+-rw-r--r--   0        0        0     8756 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/scrubbing.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/stack_info.py
+-rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/tracer.py
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/utils.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/auto_trace/__init__.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/auto_trace/import_hook.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/auto_trace/rewrite_ast.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/auto_trace/types.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/exporters/__init__.py
+-rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/exporters/console.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/exporters/fallback.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/exporters/file.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/exporters/otlp.py
+-rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/exporters/processor_wrapper.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/exporters/remove_pending.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/exporters/wrapper.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/__init__.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/asyncpg.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/django.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/executors.py
+-rw-r--r--   0        0        0    10656 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/fastapi.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/httpx.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/psycopg.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/requests.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/llm_providers/anthropic.py
+-rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/llm_providers/llm_provider.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/llm_providers/openai.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/_internal/integrations/llm_providers/types.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/integrations/__init__.py
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/integrations/logging.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/integrations/loguru.py
+-rw-r--r--   0        0        0    19169 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/integrations/pydantic.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 logfire-0.38.0/logfire/integrations/structlog.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/__init__.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/conftest.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/module_used_for_tests.py
+-rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_auto_trace.py
+-rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_backfill.py
+-rw-r--r--   0        0        0    47077 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_cli.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_collect_package_resources.py
+-rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_configure.py
+-rw-r--r--   0        0        0    29388 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_console_exporter.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_formatter.py
+-rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_json_args.py
+-rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_json_args_formatting.py
+-rw-r--r--   0        0        0   108461 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_logfire.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_loguru.py
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_metrics.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_no_production.py
+-rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_pydantic_plugin.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_sampling.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_secret_scrubbing.py
+-rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_slow_async_callbacks.py
+-rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_source_code_extraction.py
+-rw-r--r--   0        0        0    12433 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_stdlib_logging.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_structlog.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_testing.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/auto_trace_samples/__init__.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/auto_trace_samples/foo.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/auto_trace_samples/simple_nesting.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/exporters/test_fallback_exporter.py
+-rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/exporters/test_file_exporter.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/exporters/test_otlp_session.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/exporters/test_remove_pending.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/exporters/test_retry_fewer_spans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/import_used_for_tests/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/import_used_for_tests/slow_async_callbacks_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/import_used_for_tests/a/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/import_used_for_tests/a/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/__init__.py
+-rw-r--r--   0        0        0    24476 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_anthropic.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_asgi.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_asyncpg.py
+-rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_django.py
+-rw-r--r--   0        0        0    44449 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_fastapi.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_flask.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_httpx.py
+-rw-r--r--   0        0        0    44244 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_openai.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_psycopg.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_requests.py
+-rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_sqlalchemy.py
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_starlette.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/test_wsgi.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/__init__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_app/models.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_app/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.38.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.38.0/LICENSE
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 logfire-0.38.0/README.md
+-rw-r--r--   0        0        0     8521 2020-02-02 00:00:00.000000 logfire-0.38.0/pyproject.toml
+-rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 logfire-0.38.0/PKG-INFO
```

### Comparing `logfire-0.37.0/Makefile` & `logfire-0.38.0/Makefile`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/__init__.py` & `logfire-0.38.0/logfire/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/propagate.py` & `logfire-0.38.0/logfire/propagate.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/testing.py` & `logfire-0.38.0/logfire/testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/ast_utils.py` & `logfire-0.38.0/logfire/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/async_.py` & `logfire-0.38.0/logfire/_internal/async_.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/auth.py` & `logfire-0.38.0/logfire/_internal/auth.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/backfill.py` & `logfire-0.38.0/logfire/_internal/backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/cli.py` & `logfire-0.38.0/logfire/_internal/cli.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/config.py` & `logfire-0.38.0/logfire/_internal/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 from .exporters.file import FileSpanExporter
 from .exporters.otlp import OTLPExporterHttpSession, RetryFewerSpansSpanExporter
 from .exporters.processor_wrapper import SpanProcessorWrapper
 from .exporters.remove_pending import RemovePendingSpansExporter
 from .integrations.executors import instrument_executors
 from .metrics import ProxyMeterProvider, configure_metrics
 from .scrubbing import Scrubber, ScrubCallback
+from .stack_info import get_user_frame_and_stacklevel
 from .tracer import PendingSpanProcessor, ProxyTracerProvider
 from .utils import UnexpectedResponse, ensure_data_dir_exists, get_version, read_toml_file, suppress_instrumentation
 
 CREDENTIALS_FILENAME = 'logfire_credentials.json'
 """Default base URL for the Logfire API."""
 COMMON_REQUEST_HEADERS = {'User-Agent': f'logfire/{VERSION}'}
 """Common request headers for requests to the Logfire API."""
@@ -705,30 +706,39 @@
         """Get a tracer provider from this `LogfireConfig`.
 
         This is used internally and should not be called by users of the SDK.
 
         Returns:
             The tracer provider.
         """
-        if not self._initialized:
-            return self.initialize()
+        self.warn_if_not_initialized('No logs or spans will be created')
         return self._tracer_provider
 
     def get_meter_provider(self) -> ProxyMeterProvider:
         """Get a meter provider from this `LogfireConfig`.
 
         This is used internally and should not be called by users of the SDK.
 
         Returns:
             The meter provider.
         """
-        if not self._initialized:  # pragma: no cover
-            self.initialize()
+        self.warn_if_not_initialized('No metrics will be created')
         return self._meter_provider
 
+    def warn_if_not_initialized(self, message: str):
+        env_var_name = 'LOGFIRE_IGNORE_NO_CONFIG'
+        if not self._initialized and not os.environ.get(env_var_name):
+            _frame, stacklevel = get_user_frame_and_stacklevel()
+            warnings.warn(
+                f'{message} until `logfire.configure()` has been called. '
+                f'Set the environment variable {env_var_name}=1 to suppress this warning.',
+                category=LogfireNotConfiguredWarning,
+                stacklevel=stacklevel,
+            )
+
     @cached_property
     def meter(self) -> metrics.Meter:
         """Get a meter from this `LogfireConfig`.
 
         This is used internally and should not be called by users of the SDK.
 
         Returns:
@@ -1219,7 +1229,11 @@
     # Project names are limited to 50 characters, but the backend may also add 9 characters
     # if the project name already exists, so we limit it to 41 characters.
     return re.sub(r'[^a-zA-Z0-9]', '', name).lower()[:41] or 'untitled'
 
 
 def default_project_name():
     return sanitize_project_name(os.path.basename(os.getcwd()))
+
+
+class LogfireNotConfiguredWarning(UserWarning):
+    pass
```

### Comparing `logfire-0.37.0/logfire/_internal/config_params.py` & `logfire-0.38.0/logfire/_internal/config_params.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/constants.py` & `logfire-0.38.0/logfire/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/formatter.py` & `logfire-0.38.0/logfire/_internal/formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/instrument.py` & `logfire-0.38.0/logfire/_internal/instrument.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/json_encoder.py` & `logfire-0.38.0/logfire/_internal/json_encoder.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/json_formatter.py` & `logfire-0.38.0/logfire/_internal/json_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/json_schema.py` & `logfire-0.38.0/logfire/_internal/json_schema.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/json_types.py` & `logfire-0.38.0/logfire/_internal/json_types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/main.py` & `logfire-0.38.0/logfire/_internal/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -791,14 +791,17 @@
             min_duration: An optional minimum duration in seconds for which a function must run before it's traced.
                 The default is `0`, which means all functions are traced from the beginning.
                 Otherwise, the first time(s) each function is called, it will be timed but not traced.
                 Only after the function has run for at least `min_duration` will it be traced in subsequent calls.
         """
         install_auto_tracing(self, modules, check_imported_modules=check_imported_modules, min_duration=min_duration)
 
+    def _warn_if_not_initialized_for_instrumentation(self):
+        self.config.warn_if_not_initialized('Instrumentation will have no effect')
+
     def instrument_fastapi(
         self,
         app: FastAPI,
         *,
         request_attributes_mapper: Callable[
             [
                 Request | WebSocket,
@@ -846,14 +849,15 @@
                 This context manager doesn't take into account threads or other concurrency.
                 Calling this method will immediately apply the instrumentation
                 without waiting for the context manager to be opened,
                 i.e. it's not necessary to use this as a context manager.
         """
         from .integrations.fastapi import instrument_fastapi
 
+        self._warn_if_not_initialized_for_instrumentation()
         return instrument_fastapi(
             self,
             app,
             request_attributes_mapper=request_attributes_mapper,
             excluded_urls=excluded_urls,
             use_opentelemetry_instrumentation=use_opentelemetry_instrumentation,
             **opentelemetry_kwargs,
@@ -918,14 +922,15 @@
                 Use of this context manager is optional.
         """
         import openai
 
         from .integrations.llm_providers.llm_provider import instrument_llm_provider
         from .integrations.llm_providers.openai import get_endpoint_config, is_async_client, on_response
 
+        self._warn_if_not_initialized_for_instrumentation()
         return instrument_llm_provider(
             self,
             openai_client or (openai.OpenAI, openai.AsyncOpenAI),
             suppress_other_instrumentation,
             'OpenAI',
             get_endpoint_config,
             on_response,
@@ -991,39 +996,42 @@
                 Use of this context manager is optional.
         """
         import anthropic
 
         from .integrations.llm_providers.anthropic import get_endpoint_config, is_async_client, on_response
         from .integrations.llm_providers.llm_provider import instrument_llm_provider
 
+        self._warn_if_not_initialized_for_instrumentation()
         return instrument_llm_provider(
             self,
             anthropic_client or (anthropic.Anthropic, anthropic.AsyncAnthropic),
             suppress_other_instrumentation,
             'Anthropic',
             get_endpoint_config,
             on_response,
             is_async_client,
         )
 
     def instrument_asyncpg(self):
         """Instrument the `asyncpg` module so that spans are automatically created for each query."""
         from .integrations.asyncpg import instrument_asyncpg
 
+        self._warn_if_not_initialized_for_instrumentation()
         return instrument_asyncpg()
 
     def instrument_httpx(self, **kwargs: Any):
         """Instrument the `httpx` module so that spans are automatically created for each request.
 
         Uses the
         [OpenTelemetry HTTPX Instrumentation](https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/httpx/httpx.html)
         library, specifically `HTTPXClientInstrumentor().instrument()`, to which it passes `**kwargs`.
         """
         from .integrations.httpx import instrument_httpx
 
+        self._warn_if_not_initialized_for_instrumentation()
         return instrument_httpx(**kwargs)
 
     def instrument_django(
         self,
         is_sql_commentor_enabled: bool | None = None,
         request_hook: Callable[[Span, HttpRequest], None] | None = None,
         response_hook: Callable[[Span, HttpRequest, HttpResponse], None] | None = None,
@@ -1057,14 +1065,15 @@
 
             **kwargs: Additional keyword arguments to pass to the OpenTelemetry `instrument` method,
                 for future compatibility.
 
         """
         from .integrations.django import instrument_django
 
+        self._warn_if_not_initialized_for_instrumentation()
         return instrument_django(
             is_sql_commentor_enabled=is_sql_commentor_enabled,
             request_hook=request_hook,
             response_hook=response_hook,
             excluded_urls=excluded_urls,
             **kwargs,
         )
@@ -1075,14 +1084,15 @@
         Args:
             excluded_urls: A string containing a comma-delimited list of regexes used to exclude URLs from tracking
             **kwargs: Additional keyword arguments to pass to the OpenTelemetry `instrument` methods,
                 particularly `request_hook` and `response_hook`.
         """
         from .integrations.requests import instrument_requests
 
+        self._warn_if_not_initialized_for_instrumentation()
         return instrument_requests(excluded_urls=excluded_urls, **kwargs)
 
     def instrument_psycopg(self, conn_or_module: Any = None, **kwargs: Any):
         """Instrument a `psycopg` connection or module so that spans are automatically created for each query.
 
         Uses the OpenTelemetry instrumentation libraries for
         [`psycopg`](https://opentelemetry-python-contrib.readthedocs.io/en/latest/instrumentation/psycopg/psycopg.html)
@@ -1098,14 +1108,15 @@
                 - A `psycopg` or `psycopg2` connection.
 
             **kwargs: Additional keyword arguments to pass to the OpenTelemetry `instrument` methods,
                 particularly `enable_commenter` and `commenter_options`.
         """
         from .integrations.psycopg import instrument_psycopg
 
+        self._warn_if_not_initialized_for_instrumentation()
         return instrument_psycopg(conn_or_module, **kwargs)
 
     def metric_counter(self, name: str, *, unit: str = '', description: str = '') -> Counter:
         """Create a counter metric.
 
         A counter is a cumulative metric that represents a single numerical value that only ever goes up.
```

### Comparing `logfire-0.37.0/logfire/_internal/metrics.py` & `logfire-0.38.0/logfire/_internal/metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/scrubbing.py` & `logfire-0.38.0/logfire/_internal/scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/stack_info.py` & `logfire-0.38.0/logfire/_internal/stack_info.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/tracer.py` & `logfire-0.38.0/logfire/_internal/tracer.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/utils.py` & `logfire-0.38.0/logfire/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/auto_trace/__init__.py` & `logfire-0.38.0/logfire/_internal/auto_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/auto_trace/import_hook.py` & `logfire-0.38.0/logfire/_internal/auto_trace/import_hook.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/auto_trace/rewrite_ast.py` & `logfire-0.38.0/logfire/_internal/auto_trace/rewrite_ast.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/auto_trace/types.py` & `logfire-0.38.0/logfire/_internal/auto_trace/types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/exporters/console.py` & `logfire-0.38.0/logfire/_internal/exporters/console.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/exporters/fallback.py` & `logfire-0.38.0/logfire/_internal/exporters/fallback.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/exporters/file.py` & `logfire-0.38.0/logfire/_internal/exporters/file.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/exporters/otlp.py` & `logfire-0.38.0/logfire/_internal/exporters/otlp.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/exporters/processor_wrapper.py` & `logfire-0.38.0/logfire/_internal/exporters/processor_wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/exporters/remove_pending.py` & `logfire-0.38.0/logfire/_internal/exporters/remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/exporters/wrapper.py` & `logfire-0.38.0/logfire/_internal/exporters/wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/integrations/executors.py` & `logfire-0.38.0/logfire/_internal/integrations/executors.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/integrations/fastapi.py` & `logfire-0.38.0/logfire/_internal/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/integrations/psycopg.py` & `logfire-0.38.0/logfire/_internal/integrations/psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/integrations/llm_providers/anthropic.py` & `logfire-0.38.0/logfire/_internal/integrations/llm_providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/integrations/llm_providers/llm_provider.py` & `logfire-0.38.0/logfire/_internal/integrations/llm_providers/llm_provider.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/_internal/integrations/llm_providers/openai.py` & `logfire-0.38.0/logfire/_internal/integrations/llm_providers/openai.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/integrations/logging.py` & `logfire-0.38.0/logfire/integrations/logging.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/integrations/loguru.py` & `logfire-0.38.0/logfire/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/integrations/pydantic.py` & `logfire-0.38.0/logfire/integrations/pydantic.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/logfire/integrations/structlog.py` & `logfire-0.38.0/logfire/integrations/structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/conftest.py` & `logfire-0.38.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_auto_trace.py` & `logfire-0.38.0/tests/test_auto_trace.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_backfill.py` & `logfire-0.38.0/tests/test_backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_cli.py` & `logfire-0.38.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_collect_package_resources.py` & `logfire-0.38.0/tests/test_collect_package_resources.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_configure.py` & `logfire-0.38.0/tests/test_configure.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_console_exporter.py` & `logfire-0.38.0/tests/test_console_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_formatter.py` & `logfire-0.38.0/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_json_args.py` & `logfire-0.38.0/tests/test_json_args.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_json_args_formatting.py` & `logfire-0.38.0/tests/test_json_args_formatting.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_logfire.py` & `logfire-0.38.0/tests/test_logfire.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from opentelemetry.sdk.trace import ReadableSpan
 from opentelemetry.sdk.trace.export import SimpleSpanProcessor
 from pydantic import BaseModel
 from pydantic_core import ValidationError
 
 import logfire
 from logfire import Logfire, suppress_instrumentation
-from logfire._internal.config import LogfireConfig, configure
+from logfire._internal.config import LogfireConfig, LogfireNotConfiguredWarning, configure
 from logfire._internal.constants import (
     ATTRIBUTES_MESSAGE_KEY,
     ATTRIBUTES_MESSAGE_TEMPLATE_KEY,
     ATTRIBUTES_SPAN_TYPE_KEY,
     ATTRIBUTES_TAGS_KEY,
     LEVEL_NUMBERS,
     NULL_ARGS_KEY,
@@ -890,77 +890,101 @@
             SimpleSpanProcessor(exporter1),
         ],
     )
 
     logfire = Logfire(config=config)
     logfire1 = logfire.with_tags('tag1', 'tag2')
 
+    with pytest.warns(LogfireNotConfiguredWarning) as warnings:
+        with logfire.span('root'):
+            with logfire.span('child'):
+                logfire.info('test1')
+                logfire1.info('test2')
+
+    assert str(warnings[0].message) == (
+        'No logs or spans will be created until `logfire.configure()` has been called. '
+        'Set the environment variable LOGFIRE_IGNORE_NO_CONFIG=1 to suppress this warning.'
+    )
+    assert warnings[0].lineno == inspect.currentframe().f_lineno - 9  # type: ignore
+
+    with pytest.warns(LogfireNotConfiguredWarning) as warnings:
+        logfire.instrument_django()
+
+    assert str(warnings[0].message) == (
+        'Instrumentation will have no effect until `logfire.configure()` has been '
+        'called. Set the environment variable LOGFIRE_IGNORE_NO_CONFIG=1 to suppress '
+        'this warning.'
+    )
+    assert warnings[0].lineno == inspect.currentframe().f_lineno - 7  # type: ignore
+
+    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot([])
+    assert exporter1.exported_spans_as_dict(_include_pending_spans=True) == snapshot([])
+
+    config.initialize()
     with logfire.span('root'):
         with logfire.span('child'):
             logfire.info('test1')
             logfire1.info('test2')
 
-    assert exporter.exported_spans_as_dict(_include_pending_spans=True) == snapshot([])
-
     assert exporter1.exported_spans_as_dict(_include_pending_spans=True) == snapshot(
         [
             {
                 'name': 'root (pending)',
                 'context': {'trace_id': 1, 'span_id': 2, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-                'start_time': 1000000000,
-                'end_time': 1000000000,
+                'start_time': 5000000000,
+                'end_time': 5000000000,
                 'attributes': {
                     'code.filepath': 'test_logfire.py',
                     'code.lineno': 123,
                     'code.function': 'test_logfire_with_its_own_config',
                     'logfire.msg_template': 'root',
                     'logfire.msg': 'root',
                     'logfire.span_type': 'pending_span',
                     'logfire.pending_parent_id': '0000000000000000',
                 },
             },
             {
                 'name': 'child (pending)',
                 'context': {'trace_id': 1, 'span_id': 4, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-                'start_time': 2000000000,
-                'end_time': 2000000000,
+                'start_time': 6000000000,
+                'end_time': 6000000000,
                 'attributes': {
                     'code.filepath': 'test_logfire.py',
                     'code.lineno': 123,
                     'code.function': 'test_logfire_with_its_own_config',
                     'logfire.msg_template': 'child',
                     'logfire.msg': 'child',
                     'logfire.span_type': 'pending_span',
                     'logfire.pending_parent_id': '0000000000000001',
                 },
             },
             {
                 'name': 'test1',
                 'context': {'trace_id': 1, 'span_id': 5, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-                'start_time': 3000000000,
-                'end_time': 3000000000,
+                'start_time': 7000000000,
+                'end_time': 7000000000,
                 'attributes': {
                     'logfire.span_type': 'log',
                     'logfire.level_num': 9,
                     'logfire.msg_template': 'test1',
                     'logfire.msg': 'test1',
                     'code.filepath': 'test_logfire.py',
                     'code.lineno': 123,
                     'code.function': 'test_logfire_with_its_own_config',
                 },
             },
             {
                 'name': 'test2',
                 'context': {'trace_id': 1, 'span_id': 6, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
-                'start_time': 4000000000,
-                'end_time': 4000000000,
+                'start_time': 8000000000,
+                'end_time': 8000000000,
                 'attributes': {
                     'logfire.span_type': 'log',
                     'logfire.level_num': 9,
                     'logfire.msg_template': 'test2',
                     'logfire.msg': 'test2',
                     'code.filepath': 'test_logfire.py',
                     'code.lineno': 123,
@@ -968,31 +992,31 @@
                     'logfire.tags': ('tag1', 'tag2'),
                 },
             },
             {
                 'name': 'child',
                 'context': {'trace_id': 1, 'span_id': 3, 'is_remote': False},
                 'parent': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
-                'start_time': 2000000000,
-                'end_time': 5000000000,
+                'start_time': 6000000000,
+                'end_time': 9000000000,
                 'attributes': {
                     'code.filepath': 'test_logfire.py',
                     'code.lineno': 123,
                     'code.function': 'test_logfire_with_its_own_config',
                     'logfire.msg_template': 'child',
                     'logfire.span_type': 'span',
                     'logfire.msg': 'child',
                 },
             },
             {
                 'name': 'root',
                 'context': {'trace_id': 1, 'span_id': 1, 'is_remote': False},
                 'parent': None,
-                'start_time': 1000000000,
-                'end_time': 6000000000,
+                'start_time': 5000000000,
+                'end_time': 10000000000,
                 'attributes': {
                     'code.filepath': 'test_logfire.py',
                     'code.lineno': 123,
                     'code.function': 'test_logfire_with_its_own_config',
                     'logfire.msg_template': 'root',
                     'logfire.span_type': 'span',
                     'logfire.msg': 'root',
```

### Comparing `logfire-0.37.0/tests/test_loguru.py` & `logfire-0.38.0/tests/test_loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_metrics.py` & `logfire-0.38.0/tests/test_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import json
-import subprocess
 from typing import Any, cast
 
 import pytest
 from dirty_equals._numeric import IsInt
 from inline_snapshot import snapshot
 from opentelemetry.metrics import CallbackOptions, Observation
 from opentelemetry.sdk.metrics.export import AggregationTemporality, InMemoryMetricReader, MetricsData
@@ -318,33 +317,12 @@
                     'is_monotonic': False,
                 },
             }
         ]
     )
 
 
-def test_metrics_without_configure():
-    # Ensure that methods like logfire.metric_counter() can be called without calling logfire.configure().
-    # language=python
-    code = """
-import logfire
-
-config = logfire.DEFAULT_LOGFIRE_INSTANCE._config
-
-def initialize():
-    # Just check that initialize() is called without actually starting metric exporters etc.
-    config._initialized = True
-
-config.initialize = initialize
-
-assert not config._initialized
-logfire.metric_counter('foo')
-assert config._initialized
-    """
-    subprocess.check_call(['python', '-c', code])
-
-
 def get_collected_metrics(metrics_reader: InMemoryMetricReader) -> list[dict[str, Any]]:
     exported_metrics = json.loads(cast(MetricsData, metrics_reader.get_metrics_data()).to_json())  # type: ignore
     [resource_metric] = exported_metrics['resource_metrics']
     [scope_metric] = resource_metric['scope_metrics']
     return scope_metric['metrics']
```

### Comparing `logfire-0.37.0/tests/test_no_production.py` & `logfire-0.38.0/tests/test_no_production.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_pydantic_plugin.py` & `logfire-0.38.0/tests/test_pydantic_plugin.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_sampling.py` & `logfire-0.38.0/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_secret_scrubbing.py` & `logfire-0.38.0/tests/test_secret_scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_slow_async_callbacks.py` & `logfire-0.38.0/tests/test_slow_async_callbacks.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_source_code_extraction.py` & `logfire-0.38.0/tests/test_source_code_extraction.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_stdlib_logging.py` & `logfire-0.38.0/tests/test_stdlib_logging.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_structlog.py` & `logfire-0.38.0/tests/test_structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_testing.py` & `logfire-0.38.0/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/test_utils.py` & `logfire-0.38.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/utils.py` & `logfire-0.38.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/exporters/test_fallback_exporter.py` & `logfire-0.38.0/tests/exporters/test_fallback_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/exporters/test_file_exporter.py` & `logfire-0.38.0/tests/exporters/test_file_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/exporters/test_otlp_session.py` & `logfire-0.38.0/tests/exporters/test_otlp_session.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/exporters/test_remove_pending.py` & `logfire-0.38.0/tests/exporters/test_remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/exporters/test_retry_fewer_spans.py` & `logfire-0.38.0/tests/exporters/test_retry_fewer_spans.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/import_used_for_tests/slow_async_callbacks_example.py` & `logfire-0.38.0/tests/import_used_for_tests/slow_async_callbacks_example.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/otel_integrations/test_anthropic.py` & `logfire-0.38.0/tests/otel_integrations/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/otel_integrations/test_asgi.py` & `logfire-0.38.0/tests/otel_integrations/test_asgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/otel_integrations/test_asyncpg.py` & `logfire-0.38.0/tests/otel_integrations/test_asyncpg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/otel_integrations/test_django.py` & `logfire-0.38.0/tests/otel_integrations/test_django.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from django.http import HttpResponse
 from django.test import Client
 from inline_snapshot import snapshot
 
+import logfire
 from logfire.testing import TestExporter
 
 
 def test_good_route(client: Client, exporter: TestExporter):
+    logfire.instrument_django()
     response: HttpResponse = client.get(  # type: ignore
         '/django_test_app/123/?very_long_query_param_name=very+long+query+param+value&foo=1'
     )
     assert response.status_code == 200
     assert response.content == b'item_id: 123'
 
     # TODO route and target should consistently start with /, including in the name/message
@@ -37,14 +39,15 @@
                 },
             }
         ]
     )
 
 
 def test_error_route(client: Client, exporter: TestExporter):
+    logfire.instrument_django()
     response: HttpResponse = client.get('/django_test_app/bad/?foo=1')  # type: ignore
     assert response.status_code == 400
 
     assert exporter.exported_spans_as_dict() == snapshot(
         [
             {
                 'name': 'GET django_test_app/bad/',
@@ -80,14 +83,15 @@
                 ],
             }
         ]
     )
 
 
 def test_no_matching_route(client: Client, exporter: TestExporter):
+    logfire.instrument_django()
     response: HttpResponse = client.get('/django_test_app/nowhere/?foo=1')  # type: ignore
     assert response.status_code == 404
 
     assert exporter.exported_spans_as_dict() == snapshot(
         [
             {
                 'name': 'GET',
```

### Comparing `logfire-0.37.0/tests/otel_integrations/test_fastapi.py` & `logfire-0.38.0/tests/otel_integrations/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/otel_integrations/test_flask.py` & `logfire-0.38.0/tests/otel_integrations/test_flask.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/otel_integrations/test_httpx.py` & `logfire-0.38.0/tests/otel_integrations/test_httpx.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/otel_integrations/test_openai.py` & `logfire-0.38.0/tests/otel_integrations/test_openai.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/otel_integrations/test_psycopg.py` & `logfire-0.38.0/tests/otel_integrations/test_psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/otel_integrations/test_requests.py` & `logfire-0.38.0/tests/otel_integrations/test_requests.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/otel_integrations/test_sqlalchemy.py` & `logfire-0.38.0/tests/otel_integrations/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/otel_integrations/test_starlette.py` & `logfire-0.38.0/tests/otel_integrations/test_starlette.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/otel_integrations/test_wsgi.py` & `logfire-0.38.0/tests/otel_integrations/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/otel_integrations/django_test_project/manage.py` & `logfire-0.38.0/tests/otel_integrations/django_test_project/manage.py`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/tests/otel_integrations/django_test_project/django_test_site/settings.py` & `logfire-0.38.0/tests/otel_integrations/django_test_project/django_test_site/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 For the full list of settings and their values, see
 https://docs.djangoproject.com/en/5.0/ref/settings/
 """
 
 from pathlib import Path
 from typing import Any
 
-import logfire
-
 # Build paths inside the project like this: BASE_DIR / 'subdir'.
 BASE_DIR = Path(__file__).resolve().parent.parent
 
 
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/5.0/howto/deployment/checklist/
 
@@ -122,10 +120,7 @@
 
 # Default primary key field type
 # https://docs.djangoproject.com/en/5.0/ref/settings/#default-auto-field
 
 DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'
 
 LOGGING_CONFIG = None
-
-
-logfire.instrument_django()
```

### Comparing `logfire-0.37.0/LICENSE` & `logfire-0.38.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/README.md` & `logfire-0.38.0/README.md`

 * *Files identical despite different names*

### Comparing `logfire-0.37.0/pyproject.toml` & `logfire-0.38.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "logfire"
-version = "0.37.0"
+version = "0.38.0"
 description = "The best Python observability tool! 🪵🔥"
 authors = [
     { name = "Pydantic Team", email = "engineering@pydantic.dev" },
     { name = "Samuel Colvin", email = "samuel@pydantic.dev" },
     { name = "Hasan Ramezani", email = "hasan@pydantic.dev" },
     { name = "Adrian Garcia Badaracco", email = "adrian@pydantic.dev" },
     { name = "David Montague", email = "david@pydantic.dev" },
```

### Comparing `logfire-0.37.0/PKG-INFO` & `logfire-0.38.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: logfire
-Version: 0.37.0
+Version: 0.38.0
 Summary: The best Python observability tool! 🪵🔥
 Author-email: Pydantic Team <engineering@pydantic.dev>, Samuel Colvin <samuel@pydantic.dev>, Hasan Ramezani <hasan@pydantic.dev>, Adrian Garcia Badaracco <adrian@pydantic.dev>, David Montague <david@pydantic.dev>, Marcelo Trylesinski <marcelo@pydantic.dev>, David Hewitt <david.hewitt@pydantic.dev>, Alex Hall <alex@pydantic.dev>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
```

