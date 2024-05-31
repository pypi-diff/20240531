# Comparing `tmp/nestipy-0.3.7.tar.gz` & `tmp/nestipy-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy-0.3.7.tar", max compression
+gzip compressed data, was "nestipy-0.3.8.tar", max compression
```

## Comparing `nestipy-0.3.7.tar` & `nestipy-0.3.8.tar`

### file list

```diff
@@ -1,207 +1,207 @@
--rw-r--r--   0        0        0     1054 2024-05-28 13:14:17.462167 nestipy-0.3.7/LICENSE
--rw-r--r--   0        0        0     1906 2024-05-28 13:14:17.462167 nestipy-0.3.7/README.md
--rw-r--r--   0        0        0      681 2024-05-28 13:14:27.866151 nestipy-0.3.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/__init__.py
--rw-r--r--   0        0        0     1251 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/__init__.py
--rw-r--r--   0        0        0     1489 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      652 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
--rw-r--r--   0        0        0     1005 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/config/__init__.py
--rw-r--r--   0        0        0      246 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/decorator/__init__.py
--rw-r--r--   0        0        0     2957 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/decorator/class_.py
--rw-r--r--   0        0        0     1204 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/decorator/method.py
--rw-r--r--   0        0        0      367 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/exception/__init__.py
--rw-r--r--   0        0        0      732 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/exception/decorator.py
--rw-r--r--   0        0        0      433 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/exception/http.py
--rw-r--r--   0        0        0      364 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/exception/interface.py
--rw-r--r--   0        0        0     2531 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/exception/message.py
--rw-r--r--   0        0        0      113 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/exception/meta.py
--rw-r--r--   0        0        0     1686 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/exception/status.py
--rw-r--r--   0        0        0      164 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/guards/__init__.py
--rw-r--r--   0        0        0      326 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/guards/can_activate.py
--rw-r--r--   0        0        0      332 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/guards/decorator.py
--rw-r--r--   0        0        0       45 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/guards/meta.py
--rw-r--r--   0        0        0      971 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/helpers/__init__.py
--rw-r--r--   0        0        0      208 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/http_/__init__.py
--rw-r--r--   0        0        0     4503 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/http_/multipart.py
--rw-r--r--   0        0        0     5299 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/http_/request.py
--rw-r--r--   0        0        0     5321 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/http_/response.py
--rw-r--r--   0        0        0      478 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/http_/test.py
--rw-r--r--   0        0        0     1403 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/http_/upload_file.py
--rw-r--r--   0        0        0      303 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/http_/websocket.py
--rw-r--r--   0        0        0      199 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/interceptor/__init__.py
--rw-r--r--   0        0        0      489 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/interceptor/decorator.py
--rw-r--r--   0        0        0      352 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/interceptor/interface.py
--rw-r--r--   0        0        0       52 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/interceptor/meta.py
--rw-r--r--   0        0        0       54 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/logger.py
--rw-r--r--   0        0        0      248 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/middleware/__init__.py
--rw-r--r--   0        0        0      695 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/middleware/cors.py
--rw-r--r--   0        0        0      323 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/middleware/interface.py
--rw-r--r--   0        0        0      100 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/middleware/meta.py
--rw-r--r--   0        0        0     3276 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/middleware/session.py
--rw-r--r--   0        0        0      167 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/template/__init__.py
--rw-r--r--   0        0        0      274 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/template/decorator.py
--rw-r--r--   0        0        0      627 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/template/interface.py
--rw-r--r--   0        0        0      109 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/template/meta.py
--rw-r--r--   0        0        0     1590 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/common/utils.py
--rw-r--r--   0        0        0      933 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/__init__.py
--rw-r--r--   0        0        0     1179 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    16492 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
--rw-r--r--   0        0        0     1929 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/__pycache__/factory.cpython-311.pyc
--rw-r--r--   0        0        0     1567 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0      212 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/adapter/__init__.py
--rw-r--r--   0        0        0     4224 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/adapter/blacksheep_adapter.py
--rw-r--r--   0        0        0     3803 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/adapter/fastapi_adapter.py
--rw-r--r--   0        0        0     5666 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/adapter/http_adapter.py
--rw-r--r--   0        0        0      418 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/constant.py
--rw-r--r--   0        0        0        0 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/context/__init__.py
--rw-r--r--   0        0        0     1741 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/context/argument_host.py
--rw-r--r--   0        0        0     1613 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/context/execution_context.py
--rw-r--r--   0        0        0      526 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/context/graphql_argument_host.py
--rw-r--r--   0        0        0      369 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/context/http_argument_host.py
--rw-r--r--   0        0        0      556 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/context/websocket_argument_host.py
--rw-r--r--   0        0        0      730 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/discover.py
--rw-r--r--   0        0        0       90 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/exception/__init__.py
--rw-r--r--   0        0        0     4040 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/exception/processor.py
--rw-r--r--   0        0        0       75 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/guards/__init__.py
--rw-r--r--   0        0        0     2164 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/guards/processor.py
--rw-r--r--   0        0        0     4566 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/instance_loader.py
--rw-r--r--   0        0        0       82 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/interceptor/__init__.py
--rw-r--r--   0        0        0     2569 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/interceptor/processor.py
--rw-r--r--   0        0        0        0 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/meta/__init__.py
--rw-r--r--   0        0        0      380 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/meta/controller_metadata_creator.py
--rw-r--r--   0        0        0     4040 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/meta/metadata_creator.py
--rw-r--r--   0        0        0      771 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/meta/module_metadata_creator.py
--rw-r--r--   0        0        0      374 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/meta/provider_metadata_creator.py
--rw-r--r--   0        0        0      162 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/middleware/__init__.py
--rw-r--r--   0        0        0     3973 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/middleware/executor.py
--rw-r--r--   0        0        0     8913 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/nestipy_application.py
--rw-r--r--   0        0        0     1317 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/nestipy_factory.py
--rw-r--r--   0        0        0       64 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/on_destroy.py
--rw-r--r--   0        0        0       60 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/on_init.py
--rw-r--r--   0        0        0       89 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/platform/__init__.py
--rw-r--r--   0        0        0      608 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3199 2024-05-28 13:14:17.478167 nestipy-0.3.7/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
--rw-r--r--   0        0        0     7185 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
--rw-r--r--   0        0        0     7397 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
--rw-r--r--   0        0        0        0 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/router/__init__.py
--rw-r--r--   0        0        0     2879 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/router/route_explorer.py
--rw-r--r--   0        0        0      510 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/router/route_extractor.py
--rw-r--r--   0        0        0     7389 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/router/router_proxy.py
--rw-r--r--   0        0        0      184 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/template/__init__.py
--rw-r--r--   0        0        0     1004 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/template/minimal_jinja.py
--rw-r--r--   0        0        0     1457 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/core/template/processor.py
--rw-r--r--   0        0        0      231 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/dynamic_module/__init__.py
--rw-r--r--   0        0        0     3512 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/dynamic_module/builder.py
--rw-r--r--   0        0        0      139 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/dynamic_module/module/__init__.py
--rw-r--r--   0        0        0      517 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/dynamic_module/module/consumer.py
--rw-r--r--   0        0        0      251 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/dynamic_module/module/interface.py
--rw-r--r--   0        0        0      282 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/__init__.py
--rw-r--r--   0        0        0     1533 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/decorator.py
--rw-r--r--   0        0        0     2244 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/graphql_adapter.py
--rw-r--r--   0        0        0     1768 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/graphql_asgi.py
--rw-r--r--   0        0        0     1871 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/graphql_explorer.py
--rw-r--r--   0        0        0      584 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/graphql_module.py
--rw-r--r--   0        0        0     4315 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/graphql_proxy.py
--rw-r--r--   0        0        0      289 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/meta.py
--rw-r--r--   0        0        0     1531 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/playground/graphql-playground-default.html
--rw-r--r--   0        0        0     3486 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/playground/graphql-playground-graphiql.html
--rw-r--r--   0        0        0      704 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/pubsub.py
--rw-r--r--   0        0        0      648 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/strawberry/__init__.py
--rw-r--r--   0        0        0     2103 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/strawberry/strawberry_adapter.py
--rw-r--r--   0        0        0     1588 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/strawberry/strawberry_asgi.py
--rw-r--r--   0        0        0      110 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/graphql/test.py
--rw-r--r--   0        0        0      848 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/__init__.py
--rw-r--r--   0        0        0      449 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/annotation.py
--rw-r--r--   0        0        0    10665 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/container.py
--rw-r--r--   0        0        0      831 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/context_container.py
--rw-r--r--   0        0        0     5679 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/dependency.py
--rw-r--r--   0        0        0      602 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/meta.py
--rw-r--r--   0        0        0     3013 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/middleware.py
--rw-r--r--   0        0        0      877 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/provider.py
--rw-r--r--   0        0        0       57 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/ioc/utils.py
--rw-r--r--   0        0        0      458 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/__init__.py
--rw-r--r--   0        0        0     1748 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/class_.py
--rw-r--r--   0        0        0      508 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/container.py
--rw-r--r--   0        0        0      710 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/decorator.py
--rw-r--r--   0        0        0     1004 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/dependency.py
--rw-r--r--   0        0        0      236 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/module.py
--rw-r--r--   0        0        0       88 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/provider_token.py
--rw-r--r--   0        0        0      688 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/reflect.py
--rw-r--r--   0        0        0      107 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/metadata/route.py
--rw-r--r--   0        0        0     1133 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/__init__.py
--rw-r--r--   0        0        0       49 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/constant.py
--rw-r--r--   0        0        0     3227 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/decorator.py
--rw-r--r--   0        0        0     1587 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/document_builder.py
--rw-r--r--   0        0        0      424 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/explorer.py
--rw-r--r--   0        0        0       44 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/__init__.py
--rw-r--r--   0        0        0     4684 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/common.py
--rw-r--r--   0        0        0     1325 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/__init__.py
--rw-r--r--   0        0        0     1757 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/common.py
--rw-r--r--   0        0        0     1855 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/contents.py
--rw-r--r--   0        0        0      633 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/generate.py
--rw-r--r--   0        0        0     3196 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/jinja.py
--rw-r--r--   0        0        0     1894 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/md.py
--rw-r--r--   0        0        0     3065 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/texts.py
--rw-r--r--   0        0        0    21375 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/__init__.py
--rw-r--r--   0        0        0     4250 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/examples.py
--rw-r--r--   0        0        0      103 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/README.md
--rw-r--r--   0        0        0        0 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/__init__.py
--rw-r--r--   0        0        0      890 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/layout.html
--rw-r--r--   0        0        0      610 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-parameters.html
--rw-r--r--   0        0        0      730 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-responses.html
--rw-r--r--   0        0        0      135 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-schemas.html
--rw-r--r--   0        0        0      322 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-security-schemes.html
--rw-r--r--   0        0        0      284 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/content-examples.html
--rw-r--r--   0        0        0      207 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/external-docs.html
--rw-r--r--   0        0        0      571 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/info.html
--rw-r--r--   0        0        0      873 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/path-items.html
--rw-r--r--   0        0        0        0 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-auth.html
--rw-r--r--   0        0        0      480 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-body.html
--rw-r--r--   0        0        0      492 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-parameters.html
--rw-r--r--   0        0        0     1335 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-responses.html
--rw-r--r--   0        0        0      929 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/schema-repr.html
--rw-r--r--   0        0        0      224 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/servers.html
--rw-r--r--   0        0        0      227 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/tags.html
--rw-r--r--   0        0        0      429 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/type.html
--rw-r--r--   0        0        0      286 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/README.md
--rw-r--r--   0        0        0        0 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/__init__.py
--rw-r--r--   0        0        0      889 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/layout.html
--rw-r--r--   0        0        0      933 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-parameters.html
--rw-r--r--   0        0        0      843 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-responses.html
--rw-r--r--   0        0        0      135 2024-05-28 13:14:17.482167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-schemas.html
--rw-r--r--   0        0        0      561 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-security-schemes.html
--rw-r--r--   0        0        0      383 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/content-examples.html
--rw-r--r--   0        0        0      326 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/external-docs.html
--rw-r--r--   0        0        0      817 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/info.html
--rw-r--r--   0        0        0     1007 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/path-items.html
--rw-r--r--   0        0        0        0 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-auth.html
--rw-r--r--   0        0        0      616 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-body.html
--rw-r--r--   0        0        0      857 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-parameters.html
--rw-r--r--   0        0        0     2250 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-responses.html
--rw-r--r--   0        0        0     1155 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/schema-repr.html
--rw-r--r--   0        0        0      475 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/servers.html
--rw-r--r--   0        0        0      227 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/tags.html
--rw-r--r--   0        0        0      638 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/type.html
--rw-r--r--   0        0        0      170 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/README.md
--rw-r--r--   0        0        0      548 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/layout.html
--rw-r--r--   0        0        0      670 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/partial/schema-repr.html
--rw-r--r--   0        0        0      156 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/README.md
--rw-r--r--   0        0        0      754 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/layout.html
--rw-r--r--   0        0        0      670 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/partial/schema-repr.html
--rw-r--r--   0        0        0        0 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/utils/__init__.py
--rw-r--r--   0        0        0     2844 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/utils/source.py
--rw-r--r--   0        0        0      878 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/utils/web.py
--rw-r--r--   0        0        0     9579 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/v2.py
--rw-r--r--   0        0        0     9667 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/openapi_docs/v3.py
--rw-r--r--   0        0        0     1323 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/swagger.html
--rw-r--r--   0        0        0     2707 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/swagger_module.py
--rw-r--r--   0        0        0     2676 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/openapi/test.py
--rw-r--r--   0        0        0      220 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/types_/__init__.py
--rw-r--r--   0        0        0      393 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/types_/handler.py
--rw-r--r--   0        0        0      123 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/types_/http.py
--rw-r--r--   0        0        0      309 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/websocket/__init__.py
--rw-r--r--   0        0        0     3323 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/websocket/adapter.py
--rw-r--r--   0        0        0      716 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/websocket/decorator.py
--rw-r--r--   0        0        0     4556 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/websocket/proxy.py
--rw-r--r--   0        0        0      316 2024-05-28 13:14:17.486167 nestipy-0.3.7/src/nestipy/websocket/socket_request.py
--rw-r--r--   0        0        0     2846 1970-01-01 00:00:00.000000 nestipy-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-05-31 11:28:39.663237 nestipy-0.3.8/LICENSE
+-rw-r--r--   0        0        0     1906 2024-05-31 11:28:39.663237 nestipy-0.3.8/README.md
+-rw-r--r--   0        0        0      707 2024-05-31 11:28:51.295233 nestipy-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/__init__.py
+-rw-r--r--   0        0        0     1251 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/__init__.py
+-rw-r--r--   0        0        0     1489 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      652 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/__pycache__/http_method.cpython-311.pyc
+-rw-r--r--   0        0        0     1005 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/config/__init__.py
+-rw-r--r--   0        0        0      246 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/decorator/__init__.py
+-rw-r--r--   0        0        0     2957 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/decorator/class_.py
+-rw-r--r--   0        0        0     1204 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/decorator/method.py
+-rw-r--r--   0        0        0      367 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/exception/__init__.py
+-rw-r--r--   0        0        0      732 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/exception/decorator.py
+-rw-r--r--   0        0        0      433 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/exception/http.py
+-rw-r--r--   0        0        0      364 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/exception/interface.py
+-rw-r--r--   0        0        0     2531 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/exception/message.py
+-rw-r--r--   0        0        0      113 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/exception/meta.py
+-rw-r--r--   0        0        0     1686 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/exception/status.py
+-rw-r--r--   0        0        0      164 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/guards/__init__.py
+-rw-r--r--   0        0        0      326 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/guards/can_activate.py
+-rw-r--r--   0        0        0      332 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/guards/decorator.py
+-rw-r--r--   0        0        0       45 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/guards/meta.py
+-rw-r--r--   0        0        0      971 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/helpers/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/http_/__init__.py
+-rw-r--r--   0        0        0     4503 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/http_/multipart.py
+-rw-r--r--   0        0        0     5299 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/http_/request.py
+-rw-r--r--   0        0        0     5321 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/http_/response.py
+-rw-r--r--   0        0        0      478 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/http_/test.py
+-rw-r--r--   0        0        0     1403 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/http_/upload_file.py
+-rw-r--r--   0        0        0      303 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/http_/websocket.py
+-rw-r--r--   0        0        0      199 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/interceptor/__init__.py
+-rw-r--r--   0        0        0      489 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/interceptor/decorator.py
+-rw-r--r--   0        0        0      352 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/interceptor/interface.py
+-rw-r--r--   0        0        0       52 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/interceptor/meta.py
+-rw-r--r--   0        0        0       54 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/logger.py
+-rw-r--r--   0        0        0      248 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/middleware/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/middleware/cors.py
+-rw-r--r--   0        0        0      323 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/middleware/interface.py
+-rw-r--r--   0        0        0      100 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/middleware/meta.py
+-rw-r--r--   0        0        0     3276 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/middleware/session.py
+-rw-r--r--   0        0        0      167 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/template/__init__.py
+-rw-r--r--   0        0        0      274 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/template/decorator.py
+-rw-r--r--   0        0        0      627 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/template/interface.py
+-rw-r--r--   0        0        0      109 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/template/meta.py
+-rw-r--r--   0        0        0     1590 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/common/utils.py
+-rw-r--r--   0        0        0      933 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/core/__init__.py
+-rw-r--r--   0        0        0     1179 2024-05-31 11:28:39.675237 nestipy-0.3.8/src/nestipy/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16492 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/__pycache__/app_context.cpython-311.pyc
+-rw-r--r--   0        0        0     1929 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/__pycache__/factory.cpython-311.pyc
+-rw-r--r--   0        0        0     1567 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0      212 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/adapter/__init__.py
+-rw-r--r--   0        0        0     4224 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/adapter/blacksheep_adapter.py
+-rw-r--r--   0        0        0     3803 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/adapter/fastapi_adapter.py
+-rw-r--r--   0        0        0     5666 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/adapter/http_adapter.py
+-rw-r--r--   0        0        0      418 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/constant.py
+-rw-r--r--   0        0        0        0 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/context/__init__.py
+-rw-r--r--   0        0        0     1741 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/context/argument_host.py
+-rw-r--r--   0        0        0     1613 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/context/execution_context.py
+-rw-r--r--   0        0        0      526 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/context/graphql_argument_host.py
+-rw-r--r--   0        0        0      369 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/context/http_argument_host.py
+-rw-r--r--   0        0        0      556 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/context/websocket_argument_host.py
+-rw-r--r--   0        0        0      730 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/discover.py
+-rw-r--r--   0        0        0       90 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/exception/__init__.py
+-rw-r--r--   0        0        0     4040 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/exception/processor.py
+-rw-r--r--   0        0        0       75 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/guards/__init__.py
+-rw-r--r--   0        0        0     2164 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/guards/processor.py
+-rw-r--r--   0        0        0     4566 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/instance_loader.py
+-rw-r--r--   0        0        0       82 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/interceptor/__init__.py
+-rw-r--r--   0        0        0     2569 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/interceptor/processor.py
+-rw-r--r--   0        0        0        0 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/meta/__init__.py
+-rw-r--r--   0        0        0      380 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/meta/controller_metadata_creator.py
+-rw-r--r--   0        0        0     4040 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/meta/metadata_creator.py
+-rw-r--r--   0        0        0      771 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/meta/module_metadata_creator.py
+-rw-r--r--   0        0        0      374 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/meta/provider_metadata_creator.py
+-rw-r--r--   0        0        0      162 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/middleware/__init__.py
+-rw-r--r--   0        0        0     3973 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/middleware/executor.py
+-rw-r--r--   0        0        0     8913 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/nestipy_application.py
+-rw-r--r--   0        0        0     1317 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/nestipy_factory.py
+-rw-r--r--   0        0        0       64 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/on_destroy.py
+-rw-r--r--   0        0        0       60 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/on_init.py
+-rw-r--r--   0        0        0       89 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/platform/__init__.py
+-rw-r--r--   0        0        0      608 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3199 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc
+-rw-r--r--   0        0        0     7185 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc
+-rw-r--r--   0        0        0     7397 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/router/__init__.py
+-rw-r--r--   0        0        0     2879 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/router/route_explorer.py
+-rw-r--r--   0        0        0      510 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/router/route_extractor.py
+-rw-r--r--   0        0        0     7497 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/router/router_proxy.py
+-rw-r--r--   0        0        0      184 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/template/__init__.py
+-rw-r--r--   0        0        0     1004 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/template/minimal_jinja.py
+-rw-r--r--   0        0        0     1457 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/core/template/processor.py
+-rw-r--r--   0        0        0      231 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/dynamic_module/__init__.py
+-rw-r--r--   0        0        0     3512 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/dynamic_module/builder.py
+-rw-r--r--   0        0        0      139 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/dynamic_module/module/__init__.py
+-rw-r--r--   0        0        0      517 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/dynamic_module/module/consumer.py
+-rw-r--r--   0        0        0      251 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/dynamic_module/module/interface.py
+-rw-r--r--   0        0        0      282 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/__init__.py
+-rw-r--r--   0        0        0     1533 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/decorator.py
+-rw-r--r--   0        0        0     2244 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/graphql_adapter.py
+-rw-r--r--   0        0        0     1768 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/graphql_asgi.py
+-rw-r--r--   0        0        0     1871 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/graphql_explorer.py
+-rw-r--r--   0        0        0      584 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/graphql_module.py
+-rw-r--r--   0        0        0     4315 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/graphql_proxy.py
+-rw-r--r--   0        0        0      289 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/meta.py
+-rw-r--r--   0        0        0     1531 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/playground/graphql-playground-default.html
+-rw-r--r--   0        0        0     3486 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/playground/graphql-playground-graphiql.html
+-rw-r--r--   0        0        0      704 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/pubsub.py
+-rw-r--r--   0        0        0      648 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/strawberry/__init__.py
+-rw-r--r--   0        0        0     2103 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/strawberry/strawberry_adapter.py
+-rw-r--r--   0        0        0     1588 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/strawberry/strawberry_asgi.py
+-rw-r--r--   0        0        0      110 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/graphql/test.py
+-rw-r--r--   0        0        0      848 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/__init__.py
+-rw-r--r--   0        0        0      449 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/annotation.py
+-rw-r--r--   0        0        0    10665 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/container.py
+-rw-r--r--   0        0        0      831 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/context_container.py
+-rw-r--r--   0        0        0     5718 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/dependency.py
+-rw-r--r--   0        0        0      602 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/meta.py
+-rw-r--r--   0        0        0     3013 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/middleware.py
+-rw-r--r--   0        0        0      877 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/provider.py
+-rw-r--r--   0        0        0       57 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/ioc/utils.py
+-rw-r--r--   0        0        0      458 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/__init__.py
+-rw-r--r--   0        0        0     1748 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/class_.py
+-rw-r--r--   0        0        0      508 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/container.py
+-rw-r--r--   0        0        0      710 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/decorator.py
+-rw-r--r--   0        0        0     1004 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/dependency.py
+-rw-r--r--   0        0        0      236 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/module.py
+-rw-r--r--   0        0        0       88 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/provider_token.py
+-rw-r--r--   0        0        0      688 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/reflect.py
+-rw-r--r--   0        0        0      107 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/metadata/route.py
+-rw-r--r--   0        0        0     1165 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/openapi/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/openapi/constant.py
+-rw-r--r--   0        0        0     4451 2024-05-31 11:28:39.679237 nestipy-0.3.8/src/nestipy/openapi/decorator.py
+-rw-r--r--   0        0        0     1587 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/document_builder.py
+-rw-r--r--   0        0        0      580 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/explorer.py
+-rw-r--r--   0        0        0       44 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/__init__.py
+-rw-r--r--   0        0        0     4684 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/common.py
+-rw-r--r--   0        0        0     1325 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/__init__.py
+-rw-r--r--   0        0        0     1757 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/common.py
+-rw-r--r--   0        0        0     1855 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/contents.py
+-rw-r--r--   0        0        0      633 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/generate.py
+-rw-r--r--   0        0        0     3196 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/jinja.py
+-rw-r--r--   0        0        0     1894 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/md.py
+-rw-r--r--   0        0        0     3065 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/texts.py
+-rw-r--r--   0        0        0    21375 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/__init__.py
+-rw-r--r--   0        0        0     4250 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/examples.py
+-rw-r--r--   0        0        0      103 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/README.md
+-rw-r--r--   0        0        0        0 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/__init__.py
+-rw-r--r--   0        0        0      890 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/layout.html
+-rw-r--r--   0        0        0      610 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-parameters.html
+-rw-r--r--   0        0        0      730 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-responses.html
+-rw-r--r--   0        0        0      135 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-schemas.html
+-rw-r--r--   0        0        0      322 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-security-schemes.html
+-rw-r--r--   0        0        0      284 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/content-examples.html
+-rw-r--r--   0        0        0      207 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/external-docs.html
+-rw-r--r--   0        0        0      571 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/info.html
+-rw-r--r--   0        0        0      873 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/path-items.html
+-rw-r--r--   0        0        0        0 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-auth.html
+-rw-r--r--   0        0        0      480 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-body.html
+-rw-r--r--   0        0        0      492 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-parameters.html
+-rw-r--r--   0        0        0     1335 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-responses.html
+-rw-r--r--   0        0        0      929 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/schema-repr.html
+-rw-r--r--   0        0        0      224 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/servers.html
+-rw-r--r--   0        0        0      227 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/tags.html
+-rw-r--r--   0        0        0      429 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/type.html
+-rw-r--r--   0        0        0      286 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/README.md
+-rw-r--r--   0        0        0        0 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/__init__.py
+-rw-r--r--   0        0        0      889 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/layout.html
+-rw-r--r--   0        0        0      933 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-parameters.html
+-rw-r--r--   0        0        0      843 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-responses.html
+-rw-r--r--   0        0        0      135 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-schemas.html
+-rw-r--r--   0        0        0      561 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-security-schemes.html
+-rw-r--r--   0        0        0      383 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/content-examples.html
+-rw-r--r--   0        0        0      326 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/external-docs.html
+-rw-r--r--   0        0        0      817 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/info.html
+-rw-r--r--   0        0        0     1007 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/path-items.html
+-rw-r--r--   0        0        0        0 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-auth.html
+-rw-r--r--   0        0        0      616 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-body.html
+-rw-r--r--   0        0        0      857 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-parameters.html
+-rw-r--r--   0        0        0     2250 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-responses.html
+-rw-r--r--   0        0        0     1155 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/schema-repr.html
+-rw-r--r--   0        0        0      475 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/servers.html
+-rw-r--r--   0        0        0      227 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/tags.html
+-rw-r--r--   0        0        0      638 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/type.html
+-rw-r--r--   0        0        0      170 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/README.md
+-rw-r--r--   0        0        0      548 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/layout.html
+-rw-r--r--   0        0        0      670 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/partial/schema-repr.html
+-rw-r--r--   0        0        0      156 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/README.md
+-rw-r--r--   0        0        0      754 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/layout.html
+-rw-r--r--   0        0        0      670 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/partial/schema-repr.html
+-rw-r--r--   0        0        0        0 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/utils/__init__.py
+-rw-r--r--   0        0        0     2844 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/utils/source.py
+-rw-r--r--   0        0        0      878 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/utils/web.py
+-rw-r--r--   0        0        0     9579 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/v2.py
+-rw-r--r--   0        0        0     9667 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/openapi_docs/v3.py
+-rw-r--r--   0        0        0     1323 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/swagger.html
+-rw-r--r--   0        0        0     2707 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/swagger_module.py
+-rw-r--r--   0        0        0     2676 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/openapi/test.py
+-rw-r--r--   0        0        0      220 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/types_/__init__.py
+-rw-r--r--   0        0        0      393 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/types_/handler.py
+-rw-r--r--   0        0        0      123 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/types_/http.py
+-rw-r--r--   0        0        0      309 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/websocket/__init__.py
+-rw-r--r--   0        0        0     3323 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/websocket/adapter.py
+-rw-r--r--   0        0        0      716 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/websocket/decorator.py
+-rw-r--r--   0        0        0     4556 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/websocket/proxy.py
+-rw-r--r--   0        0        0      316 2024-05-31 11:28:39.683237 nestipy-0.3.8/src/nestipy/websocket/socket_request.py
+-rw-r--r--   0        0        0     2896 1970-01-01 00:00:00.000000 nestipy-0.3.8/PKG-INFO
```

### Comparing `nestipy-0.3.7/LICENSE` & `nestipy-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/README.md` & `nestipy-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/pyproject.toml` & `nestipy-0.3.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "nestipy"
-version = "0.3.7"
+version = "0.3.8"
 description = "Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS"
 authors = ["tsiresymila <tsiresymila@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "nestipy", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pyee = "^11.1.0"
 snakecase = "^1.0.1"
 python-socketio = "^5.11.1"
 blacksheep = "^2.0.7"
 aiofiles = "^23.2.1"
 fastapi = "^0.110.0"
-uvicorn = { extras = ["standard"], version = "^0.29.0" }
 strawberry-graphql = "^0.225.0"
 ujson = "^5.9.0"
 minijinja = "^2.0.1"
+python-multipart = "^0.0.9"
+uvicorn = {extras = ["standard"], version = "^0.30.0"}
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nestipy-0.3.7/src/nestipy/common/__init__.py` & `nestipy-0.3.8/src/nestipy/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/common/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.3.8/src/nestipy/common/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/common/__pycache__/http_method.cpython-311.pyc` & `nestipy-0.3.8/src/nestipy/common/__pycache__/http_method.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/common/config/__init__.py` & `nestipy-0.3.8/src/nestipy/common/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/common/decorator/class_.py` & `nestipy-0.3.8/src/nestipy/common/decorator/class_.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/common/decorator/method.py` & `nestipy-0.3.8/src/nestipy/common/decorator/method.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/common/exception/decorator.py` & `nestipy-0.3.8/src/nestipy/common/exception/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/common/exception/message.py` & `nestipy-0.3.8/src/nestipy/common/exception/message.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/common/exception/status.py` & `nestipy-0.3.8/src/nestipy/common/exception/status.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/common/helpers/__init__.py` & `nestipy-0.3.8/src/nestipy/common/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/common/http_/multipart.py` & `nestipy-0.3.8/src/nestipy/common/http_/multipart.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/common/http_/request.py` & `nestipy-0.3.8/src/nestipy/common/http_/request.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/common/http_/response.py` & `nestipy-0.3.8/src/nestipy/common/http_/response.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/common/http_/upload_file.py` & `nestipy-0.3.8/src/nestipy/common/http_/upload_file.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/common/middleware/cors.py` & `nestipy-0.3.8/src/nestipy/common/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/common/middleware/session.py` & `nestipy-0.3.8/src/nestipy/common/middleware/session.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/common/template/interface.py` & `nestipy-0.3.8/src/nestipy/common/template/interface.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/common/utils.py` & `nestipy-0.3.8/src/nestipy/common/utils.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/__init__.py` & `nestipy-0.3.8/src/nestipy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.3.8/src/nestipy/core/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/__pycache__/app_context.cpython-311.pyc` & `nestipy-0.3.8/src/nestipy/core/__pycache__/app_context.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/__pycache__/factory.cpython-311.pyc` & `nestipy-0.3.8/src/nestipy/core/__pycache__/factory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/__pycache__/utils.cpython-311.pyc` & `nestipy-0.3.8/src/nestipy/core/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/adapter/blacksheep_adapter.py` & `nestipy-0.3.8/src/nestipy/core/adapter/blacksheep_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/adapter/fastapi_adapter.py` & `nestipy-0.3.8/src/nestipy/core/adapter/fastapi_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/adapter/http_adapter.py` & `nestipy-0.3.8/src/nestipy/core/adapter/http_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/context/argument_host.py` & `nestipy-0.3.8/src/nestipy/core/context/argument_host.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/context/execution_context.py` & `nestipy-0.3.8/src/nestipy/core/context/execution_context.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/context/graphql_argument_host.py` & `nestipy-0.3.8/src/nestipy/core/context/graphql_argument_host.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/context/websocket_argument_host.py` & `nestipy-0.3.8/src/nestipy/core/context/websocket_argument_host.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/discover.py` & `nestipy-0.3.8/src/nestipy/core/discover.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/exception/processor.py` & `nestipy-0.3.8/src/nestipy/core/exception/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/guards/processor.py` & `nestipy-0.3.8/src/nestipy/core/guards/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/instance_loader.py` & `nestipy-0.3.8/src/nestipy/core/instance_loader.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/interceptor/processor.py` & `nestipy-0.3.8/src/nestipy/core/interceptor/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/meta/metadata_creator.py` & `nestipy-0.3.8/src/nestipy/core/meta/metadata_creator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/meta/module_metadata_creator.py` & `nestipy-0.3.8/src/nestipy/core/meta/module_metadata_creator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/middleware/executor.py` & `nestipy-0.3.8/src/nestipy/core/middleware/executor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/nestipy_application.py` & `nestipy-0.3.8/src/nestipy/core/nestipy_application.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/nestipy_factory.py` & `nestipy-0.3.8/src/nestipy/core/nestipy_factory.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc` & `nestipy-0.3.8/src/nestipy/core/platform/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc` & `nestipy-0.3.8/src/nestipy/core/platform/__pycache__/platform.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc` & `nestipy-0.3.8/src/nestipy/core/platform/__pycache__/platform_fastapi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc` & `nestipy-0.3.8/src/nestipy/core/platform/__pycache__/platform_litestar.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/router/route_explorer.py` & `nestipy-0.3.8/src/nestipy/core/router/route_explorer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/router/router_proxy.py` & `nestipy-0.3.8/src/nestipy/core/router/router_proxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,43 +28,44 @@
 class RouterProxy:
     def __init__(self, router: HttpAdapter):
         self.router = router
         self._template_processor = TemplateRendererProcessor(router)
 
     def apply_routes(self, modules: list[Union[Type, object]]):
         json_paths = {}
+        json_schemas = {}
         for module_ref in modules:
             routes = RouteExplorer.explore(module_ref)
             for route in routes:
                 path = route['path']
                 methods = route['request_method']
                 method_name = route['method_name']
                 controller = route['controller']
                 handler = self.create_request_handler(module_ref, controller, method_name)
                 for method in methods:
                     getattr(self.router, method.lower())(path, handler, route)
 
                     # OPEN API REGISTER
-                    if path in json_paths.keys():
+                    if path in json_paths:
                         route_path = json_paths[path]
                     else:
                         route_path = {}
-                    if "responses" not in route['openapi'].keys():
-                        continue
-
+                    # if "responses" not in route['openapi'].keys():
+                    #     continue
+                    json_schemas = {**json_schemas, **route['schemas']}
                     if 'no_swagger' not in route['openapi'].keys():
                         route_path[method.lower()] = Operation(
                             **route['openapi'],
                             summary=snakecase_to_camelcase(method_name)
                         )
                         json_paths[path] = route_path
         paths = {}
         for path, op in json_paths.items():
             paths[path] = PathItem(**op)
-        return paths
+        return paths, json_schemas
 
     def create_request_handler(
             self,
             module_ref: Type,
             controller: Union[object, Type],
             method_name: str
     ) -> CallableHandler:
```

### Comparing `nestipy-0.3.7/src/nestipy/core/template/minimal_jinja.py` & `nestipy-0.3.8/src/nestipy/core/template/minimal_jinja.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/core/template/processor.py` & `nestipy-0.3.8/src/nestipy/core/template/processor.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/dynamic_module/builder.py` & `nestipy-0.3.8/src/nestipy/dynamic_module/builder.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/dynamic_module/module/consumer.py` & `nestipy-0.3.8/src/nestipy/dynamic_module/module/consumer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/graphql/decorator.py` & `nestipy-0.3.8/src/nestipy/graphql/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/graphql/graphql_adapter.py` & `nestipy-0.3.8/src/nestipy/graphql/graphql_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/graphql/graphql_asgi.py` & `nestipy-0.3.8/src/nestipy/graphql/graphql_asgi.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/graphql/graphql_explorer.py` & `nestipy-0.3.8/src/nestipy/graphql/graphql_explorer.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/graphql/graphql_module.py` & `nestipy-0.3.8/src/nestipy/graphql/graphql_module.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/graphql/graphql_proxy.py` & `nestipy-0.3.8/src/nestipy/graphql/graphql_proxy.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/graphql/playground/graphql-playground-default.html` & `nestipy-0.3.8/src/nestipy/graphql/playground/graphql-playground-default.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/graphql/playground/graphql-playground-graphiql.html` & `nestipy-0.3.8/src/nestipy/graphql/playground/graphql-playground-graphiql.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/graphql/pubsub.py` & `nestipy-0.3.8/src/nestipy/graphql/pubsub.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/graphql/strawberry/__init__.py` & `nestipy-0.3.8/src/nestipy/graphql/strawberry/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/graphql/strawberry/strawberry_adapter.py` & `nestipy-0.3.8/src/nestipy/graphql/strawberry/strawberry_adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/graphql/strawberry/strawberry_asgi.py` & `nestipy-0.3.8/src/nestipy/graphql/strawberry/strawberry_asgi.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/ioc/__init__.py` & `nestipy-0.3.8/src/nestipy/ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/ioc/container.py` & `nestipy-0.3.8/src/nestipy/ioc/container.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/ioc/context_container.py` & `nestipy-0.3.8/src/nestipy/ioc/context_container.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/ioc/dependency.py` & `nestipy-0.3.8/src/nestipy/ioc/dependency.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import is_dataclass
 from typing import Any, Type, Optional
 
-from nestipy.metadata import CtxDepKey
 from pydantic import BaseModel
 
+from nestipy.metadata import CtxDepKey
 from .annotation import ParamAnnotation, TypeAnnotatedCallable
 from .context_container import RequestContextContainer
 
 
 class TypeAnnotated:
 
     def __init__(self, metadata: ParamAnnotation):
@@ -37,25 +37,30 @@
     return _request_context.execution_context.get_response()
 
 
 def to_valid_value(value: Any, _type_ref: Type):
     if is_dataclass(_type_ref):
         return _type_ref(**value)
     elif issubclass(_type_ref, BaseModel):
-        return _type_ref.model_validate(value)
+        return _type_ref(**value)
     return value
 
 
-async def body_callback(_name: str, _token: Optional[str], _type_ref: Type, _request_context: RequestContextContainer):
+async def body_callback(
+        _name: str,
+        encoding: Optional[str],
+        _type_ref: Type,
+        _request_context: RequestContextContainer
+):
     req = _request_context.execution_context.get_request()
-    form_data = await req.form()
+    form_data = await req.form(encoding)
     if form_data is not None:
         return to_valid_value(form_data, _type_ref)
     else:
-        return to_valid_value(await req.json(), _type_ref)
+        return to_valid_value(await req.json(encoding), _type_ref)
 
 
 def _get_request_param_value(
         key: str,
         _type_ref: Type, _request_context: RequestContextContainer,
         token: Optional[str] = None
 ):
```

### Comparing `nestipy-0.3.7/src/nestipy/ioc/meta.py` & `nestipy-0.3.8/src/nestipy/ioc/meta.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/ioc/middleware.py` & `nestipy-0.3.8/src/nestipy/ioc/middleware.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/ioc/provider.py` & `nestipy-0.3.8/src/nestipy/ioc/provider.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/metadata/class_.py` & `nestipy-0.3.8/src/nestipy/metadata/class_.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/metadata/decorator.py` & `nestipy-0.3.8/src/nestipy/metadata/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/metadata/dependency.py` & `nestipy-0.3.8/src/nestipy/metadata/dependency.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/metadata/reflect.py` & `nestipy-0.3.8/src/nestipy/metadata/reflect.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/__init__.py` & `nestipy-0.3.8/src/nestipy/openapi/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 
 from pydantic import create_model
 
 from .decorator import ApiBearerAuth, ApiBasicAuth, ApiSecurity, NoSwagger
-from .decorator import ApiResponse, ApiCreatedResponse, ApiOkResponse, ApiNotFoundResponse
+from .decorator import ApiResponse, ApiCreatedResponse, ApiOkResponse, ApiNotFoundResponse, ApiConsumer
 from .decorator import ApiTags, ApiId, ApiBody, ApiParameter
 from .document_builder import DocumentBuilder
 from .swagger_module import SwaggerModule
 
 
 def ApiSchema(cls):
     data_cls = dataclass(cls)
@@ -42,9 +42,10 @@
     "ApiTags",
     "ApiId",
     "ApiBody",
     "ApiParameter",
     "ApiBearerAuth",
     "ApiBasicAuth",
     "ApiSecurity",
-    "NoSwagger"
+    "NoSwagger",
+    "ApiConsumer"
 ]
```

### Comparing `nestipy-0.3.7/src/nestipy/openapi/decorator.py` & `nestipy-0.3.8/src/nestipy/openapi/decorator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,119 @@
 import dataclasses
-from typing import Union, Optional, Any, Type
+import inspect
+from enum import Enum
+from typing import Union, Optional, Any, Type, Callable
 
 from pydantic import TypeAdapter, BaseModel
 
 from nestipy.metadata import SetMetadata
 from .openapi_docs.v3 import RequestBody, Response, Parameter
 from .openapi_docs.v3 import SecurityRequirement, MediaType, Schema
 
 
-def ApiBody(body: Union[BaseModel, Type] = None, consumer: str = 'application/json'):
+class ApiConsumer(Enum):
+    JSON = "application/json"
+    MULTIPART = "multipart/form-data"
+    X_WWW_FORM_URLENCODED = "application/x-www-form-urlencoded"
+
+
+def _dict_to_dataclass(data: dict[str, Any], cls: Any) -> Any:
+    field_names = {field.name for field in dataclasses.fields(cls)}
+    filtered_data = {key: value for key, value in data.items() if key in field_names}
+    return cls(**filtered_data)
+
+
+def _get_json_of_body(body: Union[BaseModel, Type]):
     content: dict = {}
+    ref_template = "#/components/schemas/{model}"
     if dataclasses.is_dataclass(body):
-        content: dict = TypeAdapter(body).json_schema()
-    elif isinstance(body, BaseModel):
-        content: dict = body.model_json_schema()
+        content: dict = TypeAdapter(body).json_schema(ref_template=ref_template)
+    elif inspect.isclass(body) and issubclass(body, BaseModel):
+        content: dict = body.model_json_schema(ref_template=ref_template)
+    return content
+
+
+def _create_decorator_to_add_schema_ref(decorator: callable, content: dict):
+    if "$defs" not in content:
+        return decorator
+
+    def update_decorator(cls: Union[Type, Callable]):
+        new_cls = decorator(cls)
+        class_decorated = SetMetadata(key='__openapi__schemas', as_dict=True, data=content["$defs"])(new_cls)
+        return class_decorated
+
+    return update_decorator
+
+
+def ApiBody(body: Union[BaseModel, Type] = None, consumer: ApiConsumer = ApiConsumer.JSON):
+    content = _get_json_of_body(body)
     body = RequestBody(
         required=True,
         content={
-            consumer: MediaType(
-                schema=Schema(**content)
+            consumer.value: MediaType(
+                schema=_dict_to_dataclass(content, Schema),
+            )
+        },
+    )
+    decorator = SetMetadata(key='__openapi__request_body', data=body)
+    return _create_decorator_to_add_schema_ref(decorator, content)
+
+
+def ApiResponse(
+        status: int,
+        response: Union[BaseModel, Type] = None,
+        description: str = None,
+        example: Any = None,
+        consumer: ApiConsumer = ApiConsumer.JSON
+):
+    content = _get_json_of_body(response)
+    response_body = Response(
+        description=description,
+        content={
+            consumer.value: MediaType(
+                schema=_dict_to_dataclass(content, Schema),
+                example=example
             )
         },
     )
-    return SetMetadata(key='__openapi__request_body', data=body)
+    return _ApiResponse(status, response_body)
 
 
-def ApiResponse(status: int, response: Response):
+def _ApiResponse(status: int, response: Response):
     return SetMetadata(key='__openapi__responses', data={status: response}, as_dict=True)
 
 
 def NoSwagger():
     return SetMetadata(key='__openapi__no_swagger', data=True)
 
 
-def ApiOkResponse(description: Optional[str] = None, schema: Schema = None, example: Any = None):
+def ApiOkResponse(schema: Union[BaseModel, Type] = None, description: Optional[str] = None, example: Any = None):
     return ApiResponse(
         status=200,
-        response=Response(
-            description or 'Success response',
-            content={
-                'application/json': MediaType(
-                    schema=schema or Schema(),
-                    example=example
-                )
-            }
-        )
+        description=description,
+        response=schema,
+        example=example
     )
 
 
-def ApiCreatedResponse(description: Optional[str] = None, schema: Schema = None, example: Any = None):
+def ApiCreatedResponse(schema: Union[BaseModel, Type] = None, description: Optional[str] = None, example: Any = None):
     return ApiResponse(
         status=201,
-        response=Response(
-            description or 'Success response',
-            content={
-                'application/json': MediaType(
-                    schema=schema or Schema(),
-                    example=example
-                )
-            }
-        )
+        description=description,
+        response=schema,
+        example=example
     )
 
 
-def ApiNotFoundResponse(description: Optional[str] = None, schema: Schema = None, example: Any = None):
+def ApiNotFoundResponse(schema: Union[BaseModel, Type] = None, description: Optional[str] = None, example: Any = None):
     return ApiResponse(
         status=404,
-        response=Response(
-            description or 'Not Found',
-            content={
-                'application/json': MediaType(
-                    schema=schema or Schema(),
-                    example=example
-                )
-            }
-        )
+        description=description,
+        response=schema,
+        example=example
     )
 
 
 def ApiParameter(param: Parameter):
     return SetMetadata(key='__openapi__parameters', data=[param], as_list=True)
```

### Comparing `nestipy-0.3.7/src/nestipy/openapi/document_builder.py` & `nestipy-0.3.8/src/nestipy/openapi/document_builder.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/common.py` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/common.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/__init__.py` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/common.py` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/common.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/contents.py` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/contents.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/generate.py` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/generate.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/jinja.py` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/jinja.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/md.py` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/md.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/texts.py` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/texts.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/__init__.py` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/examples.py` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/examples.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/layout.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/layout.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-parameters.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-parameters.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-responses.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/components-responses.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/info.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/info.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/path-items.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/path-items.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-responses.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/request-responses.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/schema-repr.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_markdown/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/layout.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/layout.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-parameters.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-parameters.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-responses.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-responses.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-security-schemes.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/components-security-schemes.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/info.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/info.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/path-items.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/path-items.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-body.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-body.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-parameters.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-parameters.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-responses.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/request-responses.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/schema-repr.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/type.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_mkdocs/partial/type.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/layout.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/layout.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/partial/schema-repr.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_api/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/layout.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/layout.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/partial/schema-repr.html` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/mk/v3/views_plantuml_schemas/partial/schema-repr.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/utils/source.py` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/utils/source.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/utils/web.py` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/utils/web.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/v2.py` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/v2.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/openapi_docs/v3.py` & `nestipy-0.3.8/src/nestipy/openapi/openapi_docs/v3.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/swagger.html` & `nestipy-0.3.8/src/nestipy/openapi/swagger.html`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/swagger_module.py` & `nestipy-0.3.8/src/nestipy/openapi/swagger_module.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/openapi/test.py` & `nestipy-0.3.8/src/nestipy/openapi/test.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/websocket/adapter.py` & `nestipy-0.3.8/src/nestipy/websocket/adapter.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/websocket/decorator.py` & `nestipy-0.3.8/src/nestipy/websocket/decorator.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/src/nestipy/websocket/proxy.py` & `nestipy-0.3.8/src/nestipy/websocket/proxy.py`

 * *Files identical despite different names*

### Comparing `nestipy-0.3.7/PKG-INFO` & `nestipy-0.3.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: nestipy
-Version: 0.3.7
+Version: 0.3.8
 Summary: Nestipy is a Python framework built on top of BlackSheep that follows the modular architecture of NestJS
 Author: tsiresymila
 Author-email: tsiresymila@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: blacksheep (>=2.0.7,<3.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: minijinja (>=2.0.1,<3.0.0)
 Requires-Dist: pyee (>=11.1.0,<12.0.0)
+Requires-Dist: python-multipart (>=0.0.9,<0.0.10)
 Requires-Dist: python-socketio (>=5.11.1,<6.0.0)
 Requires-Dist: snakecase (>=1.0.1,<2.0.0)
 Requires-Dist: strawberry-graphql (>=0.225.0,<0.226.0)
 Requires-Dist: ujson (>=5.9.0,<6.0.0)
-Requires-Dist: uvicorn[standard] (>=0.29.0,<0.30.0)
+Requires-Dist: uvicorn[standard] (>=0.30.0,<0.31.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a target="_blank"><img src="https://raw.githubusercontent.com/nestipy/nestipy/release-v1/nestipy.png" width="200" alt="Nestipy Logo" /></a></p>
 <p align="center">
     <a href="https://pypi.org/project/nestipy">
         <img src="https://img.shields.io/pypi/v/nestipy?color=%2334D058&label=pypi%20package" alt="Version">
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: nestipy Version: 0.3.7 Summary: Nestipy is a Python
+Metadata-Version: 2.1 Name: nestipy Version: 0.3.8 Summary: Nestipy is a Python
 framework built on top of BlackSheep that follows the modular architecture of
 NestJS Author: tsiresymila Author-email: tsiresymila@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Dist: aiofiles (>=23.2.1,<24.0.0) Requires-Dist: blacksheep (>=2.0.7,<3.0.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0) Requires-Dist: minijinja
 (>=2.0.1,<3.0.0) Requires-Dist: pyee (>=11.1.0,<12.0.0) Requires-Dist: python-
-socketio (>=5.11.1,<6.0.0) Requires-Dist: snakecase (>=1.0.1,<2.0.0) Requires-
-Dist: strawberry-graphql (>=0.225.0,<0.226.0) Requires-Dist: ujson
-(>=5.9.0,<6.0.0) Requires-Dist: uvicorn[standard] (>=0.29.0,<0.30.0)
-Description-Content-Type: text/markdown
+multipart (>=0.0.9,<0.0.10) Requires-Dist: python-socketio (>=5.11.1,<6.0.0)
+Requires-Dist: snakecase (>=1.0.1,<2.0.0) Requires-Dist: strawberry-graphql
+(>=0.225.0,<0.226.0) Requires-Dist: ujson (>=5.9.0,<6.0.0) Requires-Dist:
+uvicorn[standard] (>=0.30.0,<0.31.0) Description-Content-Type: text/markdown
                                 [Nestipy Logo]
                           _[_V_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_L_i_c_e_n_s_e_]
 ## Description
 Nestipy is a Python framework built on top of FastAPI that follows the modular
 architecture of NestJS
 Under the hood, Nestipy makes use of _F_a_s_t_A_P_I, but also provides compatibility
 with a wide range of other libraries, like _B_l_a_c_k_s_h_e_e_p, allowing for easy use of
```

