# Comparing `tmp/nestipy-0.3.8.tar.gz` & `tmp/nestipy-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy-0.3.8.tar", max compression
+gzip compressed data, was "nestipy-0.3.9.tar", max compression
```

## Comparing `nestipy-0.3.8.tar` & `nestipy-0.3.9.tar`

### file list

```diff
@@ -1,207 +1,207 @@
--rw-r--r--   0        0        0     1054 2024-05-31 11:28:39.663237 nestipy-0.3.8/LICENSE
--rw-r--r--   0        0        0     1906 2024-05-31 11:28:39.663237 nestipy-0.3.8/README.md
--rw-r--r--   0        0        0      707 2024-05-31 11:28:51.295233 nestipy-0.3.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/__init__.py
--rw-r--r--   0        0        0     1251 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/__init__.py
--rw-r--r--   0        0        0     1489 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      652 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
--rw-r--r--   0        0        0     1005 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/config/__init__.py
--rw-r--r--   0        0        0      246 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/decorator/__init__.py
--rw-r--r--   0        0        0     2957 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/decorator/class_.py
--rw-r--r--   0        0        0     1204 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/decorator/method.py
--rw-r--r--   0        0        0      367 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/exception/__init__.py
--rw-r--r--   0        0        0      732 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/exception/decorator.py
--rw-r--r--   0        0        0      433 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/exception/http.py
--rw-r--r--   0        0        0      364 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/exception/interface.py
--rw-r--r--   0        0        0     2531 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/exception/message.py
--rw-r--r--   0        0        0      113 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/exception/meta.py
--rw-r--r--   0        0        0     1686 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/exception/status.py
--rw-r--r--   0        0        0      164 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/guards/__init__.py
--rw-r--r--   0        0        0      326 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/guards/can_activate.py
--rw-r--r--   0        0        0      332 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/guards/decorator.py
--rw-r--r--   0        0        0       45 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/guards/meta.py
--rw-r--r--   0        0        0      971 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/helpers/__init__.py
--rw-r--r--   0        0        0      208 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/http_/__init__.py
--rw-r--r--   0        0        0     4503 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/http_/multipart.py
--rw-r--r--   0        0        0     5299 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/http_/request.py
--rw-r--r--   0        0        0     5321 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/http_/response.py
--rw-r--r--   0        0        0      478 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/http_/test.py
--rw-r--r--   0        0        0     1403 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/http_/upload_file.py
--rw-r--r--   0        0        0      303 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/http_/websocket.py
--rw-r--r--   0        0        0      199 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/interceptor/__init__.py
--rw-r--r--   0        0        0      489 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/interceptor/decorator.py
--rw-r--r--   0        0        0      352 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/interceptor/interface.py
--rw-r--r--   0        0        0       52 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/interceptor/meta.py
--rw-r--r--   0        0        0       54 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/logger.py
--rw-r--r--   0        0        0      248 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/middleware/__init__.py
--rw-r--r--   0        0        0      695 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/middleware/cors.py
--rw-r--r--   0        0        0      323 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/middleware/interface.py
--rw-r--r--   0        0        0      100 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/middleware/meta.py
--rw-r--r--   0        0        0     3276 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/middleware/session.py
--rw-r--r--   0        0        0      167 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/template/__init__.py
--rw-r--r--   0        0        0      274 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/template/decorator.py
--rw-r--r--   0        0        0      627 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/template/interface.py
--rw-r--r--   0        0        0      109 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/template/meta.py
--rw-r--r--   0        0        0     1590 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/utils.py
--rw-r--r--   0        0        0      933 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/core/__init__.py
--rw-r--r--   0        0        0     1179 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16492 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
--rw-r--r--   0        0        0     1929 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/__pycache__/factory.cpython-311.pyc
--rw-r--r--   0        0        0     1567 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0      212 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/adapter/__init__.py
--rw-r--r--   0        0        0     4224 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/adapter/blacksheep_adapter.py
--rw-r--r--   0        0        0     3803 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/adapter/fastapi_adapter.py
--rw-r--r--   0        0        0     5666 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/adapter/http_adapter.py
--rw-r--r--   0        0        0      418 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/constant.py
--rw-r--r--   0        0        0        0 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/context/__init__.py
--rw-r--r--   0        0        0     1741 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/context/argument_host.py
--rw-r--r--   0        0        0     1613 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/context/execution_context.py
--rw-r--r--   0        0        0      526 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/context/graphql_argument_host.py
--rw-r--r--   0        0        0      369 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/context/http_argument_host.py
--rw-r--r--   0        0        0      556 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/context/websocket_argument_host.py
--rw-r--r--   0        0        0      730 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/discover.py
--rw-r--r--   0        0        0       90 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/exception/__init__.py
--rw-r--r--   0        0        0     4040 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/exception/processor.py
--rw-r--r--   0        0        0       75 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/guards/__init__.py
--rw-r--r--   0        0        0     2164 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/guards/processor.py
--rw-r--r--   0        0        0     4566 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/instance_loader.py
--rw-r--r--   0        0        0       82 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/interceptor/__init__.py
--rw-r--r--   0        0        0     2569 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/interceptor/processor.py
--rw-r--r--   0        0        0        0 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/meta/__init__.py
--rw-r--r--   0        0        0      380 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/meta/controller_metadata_creator.py
--rw-r--r--   0        0        0     4040 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/meta/metadata_creator.py
--rw-r--r--   0        0        0      771 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/meta/module_metadata_creator.py
--rw-r--r--   0        0        0      374 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/meta/provider_metadata_creator.py
--rw-r--r--   0        0        0      162 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/middleware/__init__.py
--rw-r--r--   0        0        0     3973 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/middleware/executor.py
--rw-r--r--   0        0        0     8913 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/nestipy_application.py
--rw-r--r--   0        0        0     1317 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/nestipy_factory.py
--rw-r--r--   0        0        0       64 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/on_destroy.py
--rw-r--r--   0        0        0       60 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/on_init.py
--rw-r--r--   0        0        0       89 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/platform/__init__.py
--rw-r--r--   0        0        0      608 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3199 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
--rw-r--r--   0        0        0     7185 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
--rw-r--r--   0        0        0     7397 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/router/__init__.py
--rw-r--r--   0        0        0     2879 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/router/route_explorer.py
--rw-r--r--   0        0        0      510 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/router/route_extractor.py
--rw-r--r--   0        0        0     7497 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/router/router_proxy.py
--rw-r--r--   0        0        0      184 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/template/__init__.py
--rw-r--r--   0        0        0     1004 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/template/minimal_jinja.py
--rw-r--r--   0        0        0     1457 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/template/processor.py
--rw-r--r--   0        0        0      231 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/dynamic_module/__init__.py
--rw-r--r--   0        0        0     3512 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/dynamic_module/builder.py
--rw-r--r--   0        0        0      139 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/dynamic_module/module/__init__.py
--rw-r--r--   0        0        0      517 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/dynamic_module/module/consumer.py
--rw-r--r--   0        0        0      251 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/dynamic_module/module/interface.py
--rw-r--r--   0        0        0      282 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/__init__.py
--rw-r--r--   0        0        0     1533 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/decorator.py
--rw-r--r--   0        0        0     2244 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/graphql_adapter.py
--rw-r--r--   0        0        0     1768 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/graphql_asgi.py
--rw-r--r--   0        0        0     1871 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/graphql_explorer.py
--rw-r--r--   0        0        0      584 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/graphql_module.py
--rw-r--r--   0        0        0     4315 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/graphql_proxy.py
--rw-r--r--   0        0        0      289 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/meta.py
--rw-r--r--   0        0        0     1531 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/playground/graphql-playground-default.html
--rw-r--r--   0        0        0     3486 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/playground/graphql-playground-graphiql.html
--rw-r--r--   0        0        0      704 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/pubsub.py
--rw-r--r--   0        0        0      648 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/strawberry/__init__.py
--rw-r--r--   0        0        0     2103 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/strawberry/strawberry_adapter.py
--rw-r--r--   0        0        0     1588 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/strawberry/strawberry_asgi.py
--rw-r--r--   0        0        0      110 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/test.py
--rw-r--r--   0        0        0      848 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/__init__.py
--rw-r--r--   0        0        0      449 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/annotation.py
--rw-r--r--   0        0        0    10665 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/container.py
--rw-r--r--   0        0        0      831 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/context_container.py
--rw-r--r--   0        0        0     5718 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/dependency.py
--rw-r--r--   0        0        0      602 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/meta.py
--rw-r--r--   0        0        0     3013 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/middleware.py
--rw-r--r--   0        0        0      877 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/provider.py
--rw-r--r--   0        0        0       57 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/utils.py
--rw-r--r--   0        0        0      458 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/__init__.py
--rw-r--r--   0        0        0     1748 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/class_.py
--rw-r--r--   0        0        0      508 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/container.py
--rw-r--r--   0        0        0      710 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/decorator.py
--rw-r--r--   0        0        0     1004 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/dependency.py
--rw-r--r--   0        0        0      236 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/module.py
--rw-r--r--   0        0        0       88 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/provider_token.py
--rw-r--r--   0        0        0      688 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/reflect.py
--rw-r--r--   0        0        0      107 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/route.py
--rw-r--r--   0        0        0     1165 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/openapi/__init__.py
--rw-r--r--   0        0        0       49 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/openapi/constant.py
--rw-r--r--   0        0        0     4451 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/openapi/decorator.py
--rw-r--r--   0        0        0     1587 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/document_builder.py
--rw-r--r--   0        0        0      580 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/explorer.py
--rw-r--r--   0        0        0       44 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/__init__.py
--rw-r--r--   0        0        0     4684 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/common.py
--rw-r--r--   0        0        0     1325 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/__init__.py
--rw-r--r--   0        0        0     1757 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/common.py
--rw-r--r--   0        0        0     1855 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/contents.py
--rw-r--r--   0        0        0      633 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/generate.py
--rw-r--r--   0        0        0     3196 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/jinja.py
--rw-r--r--   0        0        0     1894 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/md.py
--rw-r--r--   0        0        0     3065 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/texts.py
--rw-r--r--   0        0        0    21375 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/__init__.py
--rw-r--r--   0        0        0     4250 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/examples.py
--rw-r--r--   0        0        0      103 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/README.md
--rw-r--r--   0        0        0        0 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/__init__.py
--rw-r--r--   0        0        0      890 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/layout.html
--rw-r--r--   0        0        0      610 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-parameters.html
--rw-r--r--   0        0        0      730 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-responses.html
--rw-r--r--   0        0        0      135 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-schemas.html
--rw-r--r--   0        0        0      322 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-security-schemes.html
--rw-r--r--   0        0        0      284 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/content-examples.html
--rw-r--r--   0        0        0      207 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/external-docs.html
--rw-r--r--   0        0        0      571 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/info.html
--rw-r--r--   0        0        0      873 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/path-items.html
--rw-r--r--   0        0        0        0 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-auth.html
--rw-r--r--   0        0        0      480 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-body.html
--rw-r--r--   0        0        0      492 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-parameters.html
--rw-r--r--   0        0        0     1335 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-responses.html
--rw-r--r--   0        0        0      929 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/schema-repr.html
--rw-r--r--   0        0        0      224 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/servers.html
--rw-r--r--   0        0        0      227 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/tags.html
--rw-r--r--   0        0        0      429 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/type.html
--rw-r--r--   0        0        0      286 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/README.md
--rw-r--r--   0        0        0        0 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/__init__.py
--rw-r--r--   0        0        0      889 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/layout.html
--rw-r--r--   0        0        0      933 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-parameters.html
--rw-r--r--   0        0        0      843 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-responses.html
--rw-r--r--   0        0        0      135 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-schemas.html
--rw-r--r--   0        0        0      561 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-security-schemes.html
--rw-r--r--   0        0        0      383 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/content-examples.html
--rw-r--r--   0        0        0      326 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/external-docs.html
--rw-r--r--   0        0        0      817 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/info.html
--rw-r--r--   0        0        0     1007 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/path-items.html
--rw-r--r--   0        0        0        0 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-auth.html
--rw-r--r--   0        0        0      616 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-body.html
--rw-r--r--   0        0        0      857 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-parameters.html
--rw-r--r--   0        0        0     2250 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-responses.html
--rw-r--r--   0        0        0     1155 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/schema-repr.html
--rw-r--r--   0        0        0      475 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/servers.html
--rw-r--r--   0        0        0      227 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/tags.html
--rw-r--r--   0        0        0      638 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/type.html
--rw-r--r--   0        0        0      170 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/README.md
--rw-r--r--   0        0        0      548 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/layout.html
--rw-r--r--   0        0        0      670 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/partial/schema-repr.html
--rw-r--r--   0        0        0      156 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/README.md
--rw-r--r--   0        0        0      754 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/layout.html
--rw-r--r--   0        0        0      670 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/partial/schema-repr.html
--rw-r--r--   0        0        0        0 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/utils/__init__.py
--rw-r--r--   0        0        0     2844 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/utils/source.py
--rw-r--r--   0        0        0      878 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/utils/web.py
--rw-r--r--   0        0        0     9579 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/v2.py
--rw-r--r--   0        0        0     9667 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/v3.py
--rw-r--r--   0        0        0     1323 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/swagger.html
--rw-r--r--   0        0        0     2707 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/swagger_module.py
--rw-r--r--   0        0        0     2676 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/test.py
--rw-r--r--   0        0        0      220 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/types_/__init__.py
--rw-r--r--   0        0        0      393 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/types_/handler.py
--rw-r--r--   0        0        0      123 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/types_/http.py
--rw-r--r--   0        0        0      309 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/websocket/__init__.py
--rw-r--r--   0        0        0     3323 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/websocket/adapter.py
--rw-r--r--   0        0        0      716 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/websocket/decorator.py
--rw-r--r--   0        0        0     4556 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/websocket/proxy.py
--rw-r--r--   0        0        0      316 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/websocket/socket_request.py
--rw-r--r--   0        0        0     2896 1970-01-01 00:00:00.000000 nestipy-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-05-31 11:36:23.591349 nestipy-0.3.9/LICENSE
+-rw-r--r--   0        0        0     1906 2024-05-31 11:36:23.591349 nestipy-0.3.9/README.md
+-rw-r--r--   0        0        0      707 2024-05-31 11:36:37.847283 nestipy-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/__init__.py
+-rw-r--r--   0        0        0     1251 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/__init__.py
+-rw-r--r--   0        0        0     1489 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      652 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
+-rw-r--r--   0        0        0     1005 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/config/__init__.py
+-rw-r--r--   0        0        0      246 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/decorator/__init__.py
+-rw-r--r--   0        0        0     2957 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/decorator/class_.py
+-rw-r--r--   0        0        0     1204 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/decorator/method.py
+-rw-r--r--   0        0        0      367 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/exception/__init__.py
+-rw-r--r--   0        0        0      732 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/exception/decorator.py
+-rw-r--r--   0        0        0      433 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/exception/http.py
+-rw-r--r--   0        0        0      364 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/exception/interface.py
+-rw-r--r--   0        0        0     2531 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/exception/message.py
+-rw-r--r--   0        0        0      113 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/exception/meta.py
+-rw-r--r--   0        0        0     1686 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/exception/status.py
+-rw-r--r--   0        0        0      164 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/guards/__init__.py
+-rw-r--r--   0        0        0      326 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/guards/can_activate.py
+-rw-r--r--   0        0        0      332 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/guards/decorator.py
+-rw-r--r--   0        0        0       45 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/guards/meta.py
+-rw-r--r--   0        0        0      971 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/helpers/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/http_/__init__.py
+-rw-r--r--   0        0        0     4718 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/http_/multipart.py
+-rw-r--r--   0        0        0     5399 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/http_/request.py
+-rw-r--r--   0        0        0     5321 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/http_/response.py
+-rw-r--r--   0        0        0      478 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/http_/test.py
+-rw-r--r--   0        0        0     1594 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/http_/upload_file.py
+-rw-r--r--   0        0        0      303 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/http_/websocket.py
+-rw-r--r--   0        0        0      199 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/interceptor/__init__.py
+-rw-r--r--   0        0        0      489 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/interceptor/decorator.py
+-rw-r--r--   0        0        0      352 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/interceptor/interface.py
+-rw-r--r--   0        0        0       52 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/interceptor/meta.py
+-rw-r--r--   0        0        0       54 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/logger.py
+-rw-r--r--   0        0        0      248 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/middleware/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/middleware/cors.py
+-rw-r--r--   0        0        0      323 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/middleware/interface.py
+-rw-r--r--   0        0        0      100 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/middleware/meta.py
+-rw-r--r--   0        0        0     3276 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/middleware/session.py
+-rw-r--r--   0        0        0      167 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/template/__init__.py
+-rw-r--r--   0        0        0      274 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/template/decorator.py
+-rw-r--r--   0        0        0      627 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/template/interface.py
+-rw-r--r--   0        0        0      109 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/template/meta.py
+-rw-r--r--   0        0        0     1590 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/common/utils.py
+-rw-r--r--   0        0        0      933 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/__init__.py
+-rw-r--r--   0        0        0     1179 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16492 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
+-rw-r--r--   0        0        0     1929 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/__pycache__/factory.cpython-311.pyc
+-rw-r--r--   0        0        0     1567 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0      212 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/adapter/__init__.py
+-rw-r--r--   0        0        0     4224 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/adapter/blacksheep_adapter.py
+-rw-r--r--   0        0        0     3803 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/adapter/fastapi_adapter.py
+-rw-r--r--   0        0        0     5666 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/adapter/http_adapter.py
+-rw-r--r--   0        0        0      418 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/constant.py
+-rw-r--r--   0        0        0        0 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/context/__init__.py
+-rw-r--r--   0        0        0     1741 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/context/argument_host.py
+-rw-r--r--   0        0        0     1613 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/context/execution_context.py
+-rw-r--r--   0        0        0      526 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/context/graphql_argument_host.py
+-rw-r--r--   0        0        0      369 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/context/http_argument_host.py
+-rw-r--r--   0        0        0      556 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/context/websocket_argument_host.py
+-rw-r--r--   0        0        0      730 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/discover.py
+-rw-r--r--   0        0        0       90 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/exception/__init__.py
+-rw-r--r--   0        0        0     4040 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/exception/processor.py
+-rw-r--r--   0        0        0       75 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/guards/__init__.py
+-rw-r--r--   0        0        0     2164 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/guards/processor.py
+-rw-r--r--   0        0        0     4566 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/instance_loader.py
+-rw-r--r--   0        0        0       82 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/interceptor/__init__.py
+-rw-r--r--   0        0        0     2569 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/interceptor/processor.py
+-rw-r--r--   0        0        0        0 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/meta/__init__.py
+-rw-r--r--   0        0        0      380 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/meta/controller_metadata_creator.py
+-rw-r--r--   0        0        0     4040 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/meta/metadata_creator.py
+-rw-r--r--   0        0        0      771 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/meta/module_metadata_creator.py
+-rw-r--r--   0        0        0      374 2024-05-31 11:36:23.607349 nestipy-0.3.9/src/nestipy/core/meta/provider_metadata_creator.py
+-rw-r--r--   0        0        0      162 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/middleware/__init__.py
+-rw-r--r--   0        0        0     3973 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/middleware/executor.py
+-rw-r--r--   0        0        0     9120 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/nestipy_application.py
+-rw-r--r--   0        0        0     1317 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/nestipy_factory.py
+-rw-r--r--   0        0        0       64 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/on_destroy.py
+-rw-r--r--   0        0        0       60 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/on_init.py
+-rw-r--r--   0        0        0       89 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/platform/__init__.py
+-rw-r--r--   0        0        0      608 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3199 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
+-rw-r--r--   0        0        0     7185 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
+-rw-r--r--   0        0        0     7397 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/router/__init__.py
+-rw-r--r--   0        0        0     3235 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/router/route_explorer.py
+-rw-r--r--   0        0        0      510 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/router/route_extractor.py
+-rw-r--r--   0        0        0     7497 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/router/router_proxy.py
+-rw-r--r--   0        0        0      184 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/template/__init__.py
+-rw-r--r--   0        0        0     1004 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/template/minimal_jinja.py
+-rw-r--r--   0        0        0     1457 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/core/template/processor.py
+-rw-r--r--   0        0        0      231 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/dynamic_module/__init__.py
+-rw-r--r--   0        0        0     3512 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/dynamic_module/builder.py
+-rw-r--r--   0        0        0      139 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/dynamic_module/module/__init__.py
+-rw-r--r--   0        0        0      517 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/dynamic_module/module/consumer.py
+-rw-r--r--   0        0        0      251 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/dynamic_module/module/interface.py
+-rw-r--r--   0        0        0      282 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/graphql/__init__.py
+-rw-r--r--   0        0        0     1533 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/graphql/decorator.py
+-rw-r--r--   0        0        0     2244 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/graphql/graphql_adapter.py
+-rw-r--r--   0        0        0     1768 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/graphql/graphql_asgi.py
+-rw-r--r--   0        0        0     1871 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/graphql/graphql_explorer.py
+-rw-r--r--   0        0        0      584 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/graphql/graphql_module.py
+-rw-r--r--   0        0        0     4315 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/graphql/graphql_proxy.py
+-rw-r--r--   0        0        0      289 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/graphql/meta.py
+-rw-r--r--   0        0        0     1531 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/graphql/playground/graphql-playground-default.html
+-rw-r--r--   0        0        0     3486 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/graphql/playground/graphql-playground-graphiql.html
+-rw-r--r--   0        0        0      704 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/graphql/pubsub.py
+-rw-r--r--   0        0        0      648 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/graphql/strawberry/__init__.py
+-rw-r--r--   0        0        0     2103 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/graphql/strawberry/strawberry_adapter.py
+-rw-r--r--   0        0        0     1588 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/graphql/strawberry/strawberry_asgi.py
+-rw-r--r--   0        0        0      110 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/graphql/test.py
+-rw-r--r--   0        0        0      848 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/ioc/__init__.py
+-rw-r--r--   0        0        0      449 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/ioc/annotation.py
+-rw-r--r--   0        0        0    10665 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/ioc/container.py
+-rw-r--r--   0        0        0      831 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/ioc/context_container.py
+-rw-r--r--   0        0        0     5718 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/ioc/dependency.py
+-rw-r--r--   0        0        0      602 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/ioc/meta.py
+-rw-r--r--   0        0        0     3013 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/ioc/middleware.py
+-rw-r--r--   0        0        0      877 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/ioc/provider.py
+-rw-r--r--   0        0        0       57 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/ioc/utils.py
+-rw-r--r--   0        0        0      458 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/metadata/__init__.py
+-rw-r--r--   0        0        0     1748 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/metadata/class_.py
+-rw-r--r--   0        0        0      508 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/metadata/container.py
+-rw-r--r--   0        0        0      710 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/metadata/decorator.py
+-rw-r--r--   0        0        0     1004 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/metadata/dependency.py
+-rw-r--r--   0        0        0      236 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/metadata/module.py
+-rw-r--r--   0        0        0       88 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/metadata/provider_token.py
+-rw-r--r--   0        0        0      688 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/metadata/reflect.py
+-rw-r--r--   0        0        0      107 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/metadata/route.py
+-rw-r--r--   0        0        0     1165 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/constant.py
+-rw-r--r--   0        0        0     4451 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/decorator.py
+-rw-r--r--   0        0        0     1587 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/document_builder.py
+-rw-r--r--   0        0        0      580 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/explorer.py
+-rw-r--r--   0        0        0       44 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/__init__.py
+-rw-r--r--   0        0        0     4684 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/common.py
+-rw-r--r--   0        0        0     1325 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/__init__.py
+-rw-r--r--   0        0        0     1757 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/common.py
+-rw-r--r--   0        0        0     1855 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/contents.py
+-rw-r--r--   0        0        0      633 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/generate.py
+-rw-r--r--   0        0        0     3196 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/jinja.py
+-rw-r--r--   0        0        0     1894 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/md.py
+-rw-r--r--   0        0        0     3065 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/texts.py
+-rw-r--r--   0        0        0    21375 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/__init__.py
+-rw-r--r--   0        0        0     4250 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/examples.py
+-rw-r--r--   0        0        0      103 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/README.md
+-rw-r--r--   0        0        0        0 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/__init__.py
+-rw-r--r--   0        0        0      890 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/layout.html
+-rw-r--r--   0        0        0      610 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-parameters.html
+-rw-r--r--   0        0        0      730 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-responses.html
+-rw-r--r--   0        0        0      135 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-schemas.html
+-rw-r--r--   0        0        0      322 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-security-schemes.html
+-rw-r--r--   0        0        0      284 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/content-examples.html
+-rw-r--r--   0        0        0      207 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/external-docs.html
+-rw-r--r--   0        0        0      571 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/info.html
+-rw-r--r--   0        0        0      873 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/path-items.html
+-rw-r--r--   0        0        0        0 2024-05-31 11:36:23.611348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-auth.html
+-rw-r--r--   0        0        0      480 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-body.html
+-rw-r--r--   0        0        0      492 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-parameters.html
+-rw-r--r--   0        0        0     1335 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-responses.html
+-rw-r--r--   0        0        0      929 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/schema-repr.html
+-rw-r--r--   0        0        0      224 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/servers.html
+-rw-r--r--   0        0        0      227 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/tags.html
+-rw-r--r--   0        0        0      429 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/type.html
+-rw-r--r--   0        0        0      286 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/README.md
+-rw-r--r--   0        0        0        0 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/__init__.py
+-rw-r--r--   0        0        0      889 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/layout.html
+-rw-r--r--   0        0        0      933 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-parameters.html
+-rw-r--r--   0        0        0      843 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-responses.html
+-rw-r--r--   0        0        0      135 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-schemas.html
+-rw-r--r--   0        0        0      561 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-security-schemes.html
+-rw-r--r--   0        0        0      383 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/content-examples.html
+-rw-r--r--   0        0        0      326 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/external-docs.html
+-rw-r--r--   0        0        0      817 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/info.html
+-rw-r--r--   0        0        0     1007 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/path-items.html
+-rw-r--r--   0        0        0        0 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-auth.html
+-rw-r--r--   0        0        0      616 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-body.html
+-rw-r--r--   0        0        0      857 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-parameters.html
+-rw-r--r--   0        0        0     2250 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-responses.html
+-rw-r--r--   0        0        0     1155 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/schema-repr.html
+-rw-r--r--   0        0        0      475 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/servers.html
+-rw-r--r--   0        0        0      227 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/tags.html
+-rw-r--r--   0        0        0      638 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/type.html
+-rw-r--r--   0        0        0      170 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/README.md
+-rw-r--r--   0        0        0      548 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/layout.html
+-rw-r--r--   0        0        0      670 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/partial/schema-repr.html
+-rw-r--r--   0        0        0      156 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/README.md
+-rw-r--r--   0        0        0      754 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/layout.html
+-rw-r--r--   0        0        0      670 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/partial/schema-repr.html
+-rw-r--r--   0        0        0        0 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/utils/__init__.py
+-rw-r--r--   0        0        0     2844 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/utils/source.py
+-rw-r--r--   0        0        0      878 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/utils/web.py
+-rw-r--r--   0        0        0     9579 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/v2.py
+-rw-r--r--   0        0        0     9666 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/openapi_docs/v3.py
+-rw-r--r--   0        0        0      917 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/swagger.html
+-rw-r--r--   0        0        0     2877 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/swagger_module.py
+-rw-r--r--   0        0        0     3063 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/openapi/test.py
+-rw-r--r--   0        0        0      220 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/types_/__init__.py
+-rw-r--r--   0        0        0      393 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/types_/handler.py
+-rw-r--r--   0        0        0      123 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/types_/http.py
+-rw-r--r--   0        0        0      309 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/websocket/__init__.py
+-rw-r--r--   0        0        0     3323 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/websocket/adapter.py
+-rw-r--r--   0        0        0      716 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/websocket/decorator.py
+-rw-r--r--   0        0        0     4556 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/websocket/proxy.py
+-rw-r--r--   0        0        0      316 2024-05-31 11:36:23.615348 nestipy-0.3.9/src/nestipy/websocket/socket_request.py
+-rw-r--r--   0        0        0     2896 1970-01-01 00:00:00.000000 nestipy-0.3.9/PKG-INFO
```

### Comparing `nestipy-0.3.8/LICENSE` & `nestipy-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/README.md` & `nestipy-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/pyproject.toml` & `nestipy-0.3.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nestipy"
-version = "0.3.8"
+version = "0.3.9"
 description = "Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS"
 authors = ["tsiresymila <tsiresymila@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "nestipy", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `nestipy-0.3.8/src/nestipy/common/__init__.py` & `nestipy-0.3.9/src/nestipy/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/common/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.3.9/src/nestipy/common/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/common/__pycache__/http_method.cpython-311.pyc` & `nestipy-0.3.9/src/nestipy/common/__pycache__/http_method.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/common/config/__init__.py` & `nestipy-0.3.9/src/nestipy/common/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/common/decorator/class_.py` & `nestipy-0.3.9/src/nestipy/common/decorator/class_.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/common/decorator/method.py` & `nestipy-0.3.9/src/nestipy/common/decorator/method.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/common/exception/decorator.py` & `nestipy-0.3.9/src/nestipy/common/exception/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/common/exception/message.py` & `nestipy-0.3.9/src/nestipy/common/exception/message.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/common/exception/status.py` & `nestipy-0.3.9/src/nestipy/common/exception/status.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/common/helpers/__init__.py` & `nestipy-0.3.9/src/nestipy/common/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/common/http_/multipart.py` & `nestipy-0.3.9/src/nestipy/common/http_/multipart.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import json
 import re
 from collections import defaultdict
 from email.utils import decode_rfc2231
 from functools import lru_cache
 from typing import Any
 from urllib.parse import unquote, parse_qsl as _parse_qsl
 
@@ -112,12 +113,17 @@
             post_data = form_part[line_index:-4].lstrip(b"\r\n")
             if file_name:
                 form_file = UploadFile(
                     content_type=content_type, filename=file_name, file_data=post_data, headers=dict(headers)
                 )
                 fields[field_name].append(form_file)
             elif post_data:
-                fields[field_name].append(post_data.decode(content_charset))
+                try:
+                    decoded = json.loads(post_data.decode(content_charset))
+                except Exception as e:
+                    print(e)
+                    decoded = post_data.decode(content_charset)
+                fields[field_name].append(decoded)
             else:
                 fields[field_name].append(None)
 
     return {k: v if len(v) > 1 else v[0] for k, v in fields.items()}
```

### Comparing `nestipy-0.3.8/src/nestipy/common/http_/request.py` & `nestipy-0.3.9/src/nestipy/common/http_/request.py`

 * *Files 9% similar despite different names*

```diff
@@ -105,57 +105,57 @@
     @session.setter
     def session(self, session: dict):
         self._session = session
 
     def set_body(self, body: str):
         self._body = body
 
-    async def body(self) -> str:
+    async def body(self, encoding='utf-8') -> str:
         if self._body is None:
             body = b""
             while True:
                 message = await self.receive()
                 body += message.get("body", b"")
                 if not message.get("more_body", False):
                     break
             self._body = body
-        return self._body.decode()
+        return self._body.decode(encoding or 'utf-8')
 
     async def files(self) -> list[UploadFile]:
         form_data = await self.starlette_request.form()
         return form_data.getlist('files')
 
-    async def json(self) -> dict:
+    async def json(self, encoding='utf-8') -> dict:
         if self._json is None:
-            body = await self.body()
+            body = await self.body(encoding)
             try:
                 self._json = ujson.loads('{}' if body == '' else body)
             except ujson.JSONDecodeError:
                 self._json = {}
         return self._json
 
     @property
     def content_type(self) -> tuple[str, dict[str, str]]:
         _content_type = self.headers.get("content-type", "")
         return parse_content_header(
             _content_type
         )
 
-    async def form(self) -> dict:
+    async def form(self, encoding='utf-8') -> dict:
         if self._form is None:
             content_type, options = self.content_type
             if content_type == "multipart/form-data":
                 self._form = parse_multipart_form(
-                    body=(await self.body()).encode(),
+                    body=(await self.body(encoding)).encode(),
                     boundary=options.get("boundary", "").encode(),
-                    multipart_form_part_limit=1000,
+                    multipart_form_part_limit=1000000,
                 )
             elif content_type == "application/x-www-form-urlencoded":
                 self._form = parse_url_encoded_form_data(
-                    (await self.body()).encode(),
+                    (await self.body(encoding)).encode(),
                 )
             else:
                 self._form = None
         return self._form
 
     @property
     def cookies(self) -> dict[str, str]:
```

### Comparing `nestipy-0.3.8/src/nestipy/common/http_/response.py` & `nestipy-0.3.9/src/nestipy/common/http_/response.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/common/middleware/cors.py` & `nestipy-0.3.9/src/nestipy/common/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/common/middleware/session.py` & `nestipy-0.3.9/src/nestipy/common/middleware/session.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/common/template/interface.py` & `nestipy-0.3.9/src/nestipy/common/template/interface.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/common/utils.py` & `nestipy-0.3.9/src/nestipy/common/utils.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/__init__.py` & `nestipy-0.3.9/src/nestipy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.3.9/src/nestipy/core/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/__pycache__/app_context.cpython-311.pyc` & `nestipy-0.3.9/src/nestipy/core/__pycache__/app_context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/__pycache__/factory.cpython-311.pyc` & `nestipy-0.3.9/src/nestipy/core/__pycache__/factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/__pycache__/utils.cpython-311.pyc` & `nestipy-0.3.9/src/nestipy/core/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/adapter/blacksheep_adapter.py` & `nestipy-0.3.9/src/nestipy/core/adapter/blacksheep_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/adapter/fastapi_adapter.py` & `nestipy-0.3.9/src/nestipy/core/adapter/fastapi_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/adapter/http_adapter.py` & `nestipy-0.3.9/src/nestipy/core/adapter/http_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/context/argument_host.py` & `nestipy-0.3.9/src/nestipy/core/context/argument_host.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/context/execution_context.py` & `nestipy-0.3.9/src/nestipy/core/context/execution_context.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/context/graphql_argument_host.py` & `nestipy-0.3.9/src/nestipy/core/context/graphql_argument_host.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/context/websocket_argument_host.py` & `nestipy-0.3.9/src/nestipy/core/context/websocket_argument_host.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/discover.py` & `nestipy-0.3.9/src/nestipy/core/discover.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/exception/processor.py` & `nestipy-0.3.9/src/nestipy/core/exception/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/guards/processor.py` & `nestipy-0.3.9/src/nestipy/core/guards/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/instance_loader.py` & `nestipy-0.3.9/src/nestipy/core/instance_loader.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/interceptor/processor.py` & `nestipy-0.3.9/src/nestipy/core/interceptor/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/meta/metadata_creator.py` & `nestipy-0.3.9/src/nestipy/core/meta/metadata_creator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/meta/module_metadata_creator.py` & `nestipy-0.3.9/src/nestipy/core/meta/module_metadata_creator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/middleware/executor.py` & `nestipy-0.3.9/src/nestipy/core/middleware/executor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/nestipy_application.py` & `nestipy-0.3.9/src/nestipy/core/nestipy_application.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import dataclasses
 import os.path
 import traceback
-from typing import Type, Callable, Literal, Union, Any, TYPE_CHECKING
+from typing import Type, Callable, Literal, Union, Any, TYPE_CHECKING, Optional, Dict
 
-from openapidocs.v3 import PathItem
+from openapidocs.v3 import PathItem, Schema, Reference
 
 from nestipy.common.http_ import Response, Request
 from nestipy.common.logger import logger
 from nestipy.common.middleware import NestipyMiddleware
 from nestipy.common.template import TemplateEngine, TemplateKey
 from nestipy.common.utils import uniq_list
 from nestipy.core.template import MinimalJinjaTemplateEngine
@@ -40,14 +40,15 @@
     adapter: HttpAdapter = None
     cors: bool = None
 
 
 class NestipyApplication:
     _root_module: Type = None
     _openapi_paths = {}
+    _openapi_schemas = {}
 
     def __init__(self, config: NestipyApplicationConfig = None):
         config = config if config is not None else NestipyApplicationConfig()
         # self._http_adapter: HttpServer = FastAPIAdapter()
         self._http_adapter: HttpAdapter = config.adapter if config.adapter is not None else FastApiAdapter()
         self._graphql_builder = StrawberryAdapter()
         self._router_proxy = RouterProxy(self._http_adapter)
@@ -99,15 +100,15 @@
         module_metadata_maker.create()
 
     async def _setup(self):
         try:
             modules = self._get_modules(self._root_module)
             graphql_module_instance = await self.instance_loader.create_instances(modules)
             # create and register route to platform adapter
-            self._openapi_paths = self._router_proxy.apply_routes(modules)
+            self._openapi_paths, self._openapi_schemas = self._router_proxy.apply_routes(modules)
             # check if graphql is enabled
             if graphql_module_instance is not None:
                 GraphqlProxy(self._http_adapter, self._graphql_builder).apply_resolvers(
                     graphql_module_instance,
                     modules
                 )
             if self._http_adapter.get_io_adapter() is not None:
@@ -130,14 +131,17 @@
 
     def get_graphql_adapter(self) -> GraphqlAdapter:
         return self._graphql_builder
 
     def get_openapi_paths(self) -> dict[Any, PathItem]:
         return self._openapi_paths
 
+    def get_open_api_schemas(self) -> Optional[Dict[str, Union[Schema, Reference]]]:
+        return self._openapi_schemas
+
     async def __call__(self, scope: dict, receive: Callable, send: Callable):
         if scope.get('type') == 'lifespan':
             await self._setup()
         await self.get_adapter()(scope, receive, send)
 
     def use(self, *middleware: Union[Type[NestipyMiddleware], Callable]):
         for m in middleware:
```

### Comparing `nestipy-0.3.8/src/nestipy/core/nestipy_factory.py` & `nestipy-0.3.9/src/nestipy/core/nestipy_factory.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.3.9/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc` & `nestipy-0.3.9/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc` & `nestipy-0.3.9/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc` & `nestipy-0.3.9/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/router/route_explorer.py` & `nestipy-0.3.9/src/nestipy/core/router/route_explorer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from inspect import isfunction, getmembers
 from typing import List, Type, Union
 
-from nestipy.ioc import MiddlewareContainer
-from nestipy.metadata import ModuleMetadata, Reflect, RouteKey
 from openapidocs.v3 import Parameter, ParameterLocation
 
 from nestipy.common.utils import deep_merge
+from nestipy.ioc import MiddlewareContainer
+from nestipy.metadata import ModuleMetadata, Reflect, RouteKey
 from nestipy.openapi.explorer import OpenApiExplorer
 from .route_extractor import RouteParamsExtractor
 
 
 class RouteExplorer:
     _middleware_container: MiddlewareContainer
     _openapi_scanner = OpenApiExplorer()
@@ -26,15 +26,15 @@
         for controller in controllers:
             controller_routes = ins.explore_controller(controller)
             routes = routes + controller_routes
         return routes
 
     def explore_controller(self, controller: Type) -> List[dict]:
 
-        docs = self._openapi_scanner.explore(controller)
+        docs, schemas = self._openapi_scanner.explore(controller)
         routes = []
         # need to extract middleware, guards, exception_handler,
         controller_path = self._normalize_path(Reflect.get_metadata(controller, RouteKey.path, ''))
         for method_name, _ in getmembers(controller, isfunction):
             if method_name.startswith("__"):
                 continue
             method = getattr(controller, method_name)
@@ -42,28 +42,39 @@
             if path is not None:
                 method_path = self._normalize_path(path)
                 path = f"/{self._normalize_path(f'{controller_path}/{method_path}')}"
                 request_method = Reflect.get_metadata(method, RouteKey.method)
 
                 # openapi docs
                 params = RouteParamsExtractor.extract_params(path)
-                parameters = [Parameter(name=name, in_=ParameterLocation.PATH, required=True, description='Route path',
-                                        allow_empty_value=False)
-                              for name in params.keys()]
-                method_docs = deep_merge(self._openapi_scanner.explore(method), {'parameters': parameters})
+                parameters = [
+                    Parameter(
+                        name=name,
+                        in_=ParameterLocation.PATH,
+                        required=True,
+                        description='Route path',
+                        allow_empty_value=False
+                    )
+                    for name in params.keys()
+                ]
+                method_deps, method_schemas = self._openapi_scanner.explore(method)
+                method_docs = deep_merge(method_deps, {'parameters': parameters})
+                merged_docs = deep_merge(docs, method_docs)
+                merger_schemas = deep_merge(schemas, method_schemas)
                 path_docs = deep_merge(
                     {'tags': [controller.__name__.replace('Controller', '')]},
-                    deep_merge(docs, method_docs)
+                    merged_docs
                 )
                 path_docs['tags'] = [path_docs['tags'][0]]
 
                 # en open api
 
                 route_info = {
                     'path': path,
                     'request_method': request_method,
                     'method_name': method_name,
                     'controller': controller,
-                    'openapi': path_docs  # openapi docs
+                    'openapi': path_docs,  # openapi docs
+                    'schemas': merger_schemas,
                 }
                 routes.append(route_info)
         return routes
```

### Comparing `nestipy-0.3.8/src/nestipy/core/router/router_proxy.py` & `nestipy-0.3.9/src/nestipy/core/router/router_proxy.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/template/minimal_jinja.py` & `nestipy-0.3.9/src/nestipy/core/template/minimal_jinja.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/core/template/processor.py` & `nestipy-0.3.9/src/nestipy/core/template/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/dynamic_module/builder.py` & `nestipy-0.3.9/src/nestipy/dynamic_module/builder.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/dynamic_module/module/consumer.py` & `nestipy-0.3.9/src/nestipy/dynamic_module/module/consumer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/graphql/decorator.py` & `nestipy-0.3.9/src/nestipy/graphql/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/graphql/graphql_adapter.py` & `nestipy-0.3.9/src/nestipy/graphql/graphql_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/graphql/graphql_asgi.py` & `nestipy-0.3.9/src/nestipy/graphql/graphql_asgi.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/graphql/graphql_explorer.py` & `nestipy-0.3.9/src/nestipy/graphql/graphql_explorer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/graphql/graphql_module.py` & `nestipy-0.3.9/src/nestipy/graphql/graphql_module.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/graphql/graphql_proxy.py` & `nestipy-0.3.9/src/nestipy/graphql/graphql_proxy.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/graphql/playground/graphql-playground-default.html` & `nestipy-0.3.9/src/nestipy/graphql/playground/graphql-playground-default.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/graphql/playground/graphql-playground-graphiql.html` & `nestipy-0.3.9/src/nestipy/graphql/playground/graphql-playground-graphiql.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/graphql/pubsub.py` & `nestipy-0.3.9/src/nestipy/graphql/pubsub.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/graphql/strawberry/__init__.py` & `nestipy-0.3.9/src/nestipy/graphql/strawberry/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/graphql/strawberry/strawberry_adapter.py` & `nestipy-0.3.9/src/nestipy/graphql/strawberry/strawberry_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/graphql/strawberry/strawberry_asgi.py` & `nestipy-0.3.9/src/nestipy/graphql/strawberry/strawberry_asgi.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/ioc/__init__.py` & `nestipy-0.3.9/src/nestipy/ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/ioc/container.py` & `nestipy-0.3.9/src/nestipy/ioc/container.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/ioc/context_container.py` & `nestipy-0.3.9/src/nestipy/ioc/context_container.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/ioc/dependency.py` & `nestipy-0.3.9/src/nestipy/ioc/dependency.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/ioc/meta.py` & `nestipy-0.3.9/src/nestipy/ioc/meta.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/ioc/middleware.py` & `nestipy-0.3.9/src/nestipy/ioc/middleware.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/ioc/provider.py` & `nestipy-0.3.9/src/nestipy/ioc/provider.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/metadata/class_.py` & `nestipy-0.3.9/src/nestipy/metadata/class_.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/metadata/decorator.py` & `nestipy-0.3.9/src/nestipy/metadata/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/metadata/dependency.py` & `nestipy-0.3.9/src/nestipy/metadata/dependency.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/metadata/reflect.py` & `nestipy-0.3.9/src/nestipy/metadata/reflect.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/__init__.py` & `nestipy-0.3.9/src/nestipy/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/decorator.py` & `nestipy-0.3.9/src/nestipy/openapi/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/document_builder.py` & `nestipy-0.3.9/src/nestipy/openapi/document_builder.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/explorer.py` & `nestipy-0.3.9/src/nestipy/openapi/explorer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/common.py` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/common.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/__init__.py` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/common.py` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/common.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/contents.py` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/contents.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/generate.py` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/generate.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/jinja.py` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/jinja.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/md.py` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/md.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/texts.py` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/texts.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/__init__.py` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/examples.py` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/examples.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/layout.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/layout.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-parameters.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-parameters.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-responses.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-responses.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/info.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/info.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/path-items.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/path-items.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-responses.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-responses.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/schema-repr.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/layout.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/layout.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-parameters.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-parameters.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-responses.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-responses.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-security-schemes.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-security-schemes.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/info.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/info.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/path-items.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/path-items.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-body.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-body.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-parameters.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-parameters.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-responses.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-responses.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/schema-repr.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/type.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/type.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/layout.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/layout.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/partial/schema-repr.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/layout.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/layout.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/partial/schema-repr.html` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/utils/source.py` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/utils/source.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/utils/web.py` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/utils/web.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/v2.py` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/v2.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/v3.py` & `nestipy-0.3.9/src/nestipy/openapi/openapi_docs/v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 https://swagger.io/specification/
 """
 from abc import ABC
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
-from .common import OpenAPIRoot, normalize_dict
-
 from .common import OpenAPIElement
+from .common import OpenAPIRoot, normalize_dict
 
 
 class ParameterLocation(Enum):
     QUERY = "query"
     HEADER = "header"
     PATH = "path"
     COOKIE = "cookie"
```

### Comparing `nestipy-0.3.8/src/nestipy/openapi/swagger_module.py` & `nestipy-0.3.9/src/nestipy/openapi/swagger_module.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,17 @@
         else:
             return json_data
 
     @classmethod
     def _create_document(cls, app: "NestipyApplication", config: OpenAPI) -> _Document:
         paths = app.get_openapi_paths()
         config.paths = paths
+        schemas = app.get_open_api_schemas()
+        if "schemas" in schemas:
+            config.components.schemas = {**config.components.schemas, **schemas["schemas"]}
         serializer = Serializer()
         json = serializer.to_json(config)
         document_json = ujson.dumps(
             cls.remove_null(ujson.loads(json)), allow_nan=False,
             indent=4
         )
         document_yml = serializer.to_yaml(config)
```

### Comparing `nestipy-0.3.8/src/nestipy/openapi/test.py` & `nestipy-0.3.9/src/nestipy/openapi/test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .openapi_docs.common import Serializer
-from .openapi_docs.v3 import OpenAPI, Info, Response, Components, Schema, SecuritySchemeType
-from .openapi_docs.v3 import PathItem, Operation, SecurityRequirement, ValueType
-from .openapi_docs.v3 import Tag, HTTPSecurity, APIKeySecurity, ParameterLocation, Parameter
+from openapi_docs.common import Serializer
+from openapi_docs.v3 import OpenAPI, Info, Response, Components, Schema, SecuritySchemeType, MediaType
+from openapi_docs.v3 import PathItem, Operation, SecurityRequirement, ValueType
+from openapi_docs.v3 import Tag, HTTPSecurity, APIKeySecurity, ParameterLocation, Parameter, RequestBody
 
 open_api = OpenAPI(
     info=Info(
         title='Test openapi',
         description='This is the description',
         version='v1'
     ),
@@ -37,15 +37,25 @@
                         name='test3',
                         in_=ParameterLocation.HEADER
                     ),
                     Parameter(
                         name='test3',
                         in_=ParameterLocation.HEADER
                     )
-                ]
+                ],
+                request_body=RequestBody(
+                    required=True,
+                    content={
+                        "application/json": MediaType(
+                            schema=Schema(
+                                ref="#/components/schemas/User"
+                            )
+                        )
+                    },
+                )
             )
         )
     },
     components=Components(
         schemas={
             'User': Schema(
                 type=ValueType.OBJECT,
```

### Comparing `nestipy-0.3.8/src/nestipy/websocket/adapter.py` & `nestipy-0.3.9/src/nestipy/websocket/adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/websocket/decorator.py` & `nestipy-0.3.9/src/nestipy/websocket/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/src/nestipy/websocket/proxy.py` & `nestipy-0.3.9/src/nestipy/websocket/proxy.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.8/PKG-INFO` & `nestipy-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nestipy
-Version: 0.3.8
+Version: 0.3.9
 Summary: Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS
 Author: tsiresymila
 Author-email: tsiresymila@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nestipy Version: 0.3.8 Summary: Nestipy is a Python
+Metadata-Version: 2.1 Name: nestipy Version: 0.3.9 Summary: Nestipy is a Python
 framework built on top of BlackSheep that follows the modular architecture of
 NestJS Author: tsiresymila Author-email: tsiresymila@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Dist: aiofiles (>=23.2.1,<24.0.0) Requires-Dist: blacksheep (>=2.0.7,<3.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0) Requires-Dist: minijinja
```

