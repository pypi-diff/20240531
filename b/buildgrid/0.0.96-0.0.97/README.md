# Comparing `tmp/buildgrid-0.0.96.tar.gz` & `tmp/buildgrid-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildgrid-0.0.96.tar", last modified: Tue May 28 15:29:20 2024, max compression
+gzip compressed data, was "buildgrid-0.0.97.tar", last modified: Fri May 31 13:15:02 2024, max compression
```

## Comparing `buildgrid-0.0.96.tar` & `buildgrid-0.0.97.tar`

### file list

```diff
@@ -1,498 +1,498 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.743185 buildgrid-0.0.96/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-05-28 15:28:48.000000 buildgrid-0.0.96/BuildGrid.doap
--rw-rw-rw-   0 root         (0) root         (0)     9648 2024-05-28 15:28:48.000000 buildgrid-0.0.96/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    11338 2024-05-28 15:28:48.000000 buildgrid-0.0.96/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      500 2024-05-28 15:28:48.000000 buildgrid-0.0.96/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7030 2024-05-28 15:29:20.743185 buildgrid-0.0.96/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2932 2024-05-28 15:28:48.000000 buildgrid-0.0.96/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.632186 buildgrid-0.0.96/buildgrid/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.634186 buildgrid-0.0.96/buildgrid/_app/
--rw-rw-rw-   0 root         (0) root         (0)      621 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5675 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.637186 buildgrid-0.0.96/buildgrid/_app/commands/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6755 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_actioncache.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_browser_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     3170 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_capabilities.py
--rw-rw-rw-   0 root         (0) root         (0)    10608 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_cas.py
--rw-rw-rw-   0 root         (0) root         (0)     8817 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)    12570 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     2840 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_janitor.py
--rw-rw-rw-   0 root         (0) root         (0)     4842 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_logstream.py
--rw-rw-rw-   0 root         (0) root         (0)    11215 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_operation.py
--rw-rw-rw-   0 root         (0) root         (0)     8166 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/cmd_server.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/commands/rpc_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.638186 buildgrid-0.0.96/buildgrid/_app/settings/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   110867 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     8691 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/reference.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.638186 buildgrid-0.0.96/buildgrid/_app/settings/schemas/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.639186 buildgrid-0.0.96/buildgrid/_app/settings/schemas/caches/
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/caches/lru-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/caches/mirrored-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      676 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/caches/with-cache.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.640185 buildgrid-0.0.96/buildgrid/_app/settings/schemas/clients/
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/clients/asset-client.yaml
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2785 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.640185 buildgrid-0.0.96/buildgrid/_app/settings/schemas/connections/
--rw-rw-rw-   0 root         (0) root         (0)      403 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/connections/redis.yaml
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/connections/sql.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.641186 buildgrid-0.0.96/buildgrid/_app/settings/schemas/misc/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/misc/channel.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.641186 buildgrid-0.0.96/buildgrid/_app/settings/schemas/scheduler/
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/scheduler/memory.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3907 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/scheduler/sql.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.643185 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      971 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/bots.yaml
--rw-rw-rw-   0 root         (0) root         (0)      343 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/bytestream.yaml
--rw-rw-rw-   0 root         (0) root         (0)      273 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/cas.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1557 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/execution.yaml
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/platform-queues.yml
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/s3-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/write-once-action-cache.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.646185 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/disk.yaml
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/lru.yaml
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/operations_sql_storage.yaml
--rw-rw-rw-   0 root         (0) root         (0)      207 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/redis-index.yaml
--rw-rw-rw-   0 root         (0) root         (0)      307 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/redis.yaml
--rw-rw-rw-   0 root         (0) root         (0)      601 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/remote.yaml
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/replicated.yaml
--rw-rw-rw-   0 root         (0) root         (0)      592 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/s3.yaml
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/sharded.yaml
--rw-rw-rw-   0 root         (0) root         (0)      530 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/sql-index.yaml
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/sql.yaml
--rw-rw-rw-   0 root         (0) root         (0)      281 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/with-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4776 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_enums.py
--rw-rw-rw-   0 root         (0) root         (0)     8802 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.646185 buildgrid-0.0.96/buildgrid/_protos/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.647186 buildgrid-0.0.96/buildgrid/_protos/build/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.647186 buildgrid-0.0.96/buildgrid/_protos/build/bazel/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.647186 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.647186 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.649186 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7795 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    27103 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    16783 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)    15404 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    16783 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)    15550 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.650185 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.652186 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30140 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)   136470 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    59894 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)    47588 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    59894 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)    47884 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.652186 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.654186 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2066 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3176 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    12298 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7788 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    12298 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7844 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.656185 buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1484 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     2068 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.657186 buildgrid-0.0.96/buildgrid/_protos/build/buildbox/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/buildbox/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1944 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4156 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.658186 buildgrid-0.0.96/buildgrid/_protos/buildgrid/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.662186 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3156 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    10940 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3824 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     9955 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2881 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2872 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2872 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.662186 buildgrid-0.0.96/buildgrid/_protos/google/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.668186 buildgrid-0.0.96/buildgrid/_protos/google/api/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1612 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1622 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3481 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1926 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     6343 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2291 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18246 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.670185 buildgrid-0.0.96/buildgrid/_protos/google/bytestream/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/bytestream/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3246 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     7478 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10732 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     8880 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10732 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     8996 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.670185 buildgrid-0.0.96/buildgrid/_protos/google/devtools/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.671186 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.675186 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5933 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18014 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2545 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     5408 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     6758 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    10427 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     8451 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     5461 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     8451 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     5547 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.675186 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.681186 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7859 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    23457 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    11879 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7140 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    11879 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7256 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     6133 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    21890 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     5337 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     9321 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     7651 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     4382 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     7651 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     4498 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2751 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    11299 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.683185 buildgrid-0.0.96/buildgrid/_protos/google/longrunning/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/longrunning/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5084 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     7984 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10950 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7133 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10950 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7279 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.688186 buildgrid-0.0.96/buildgrid/_protos/google/rpc/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1890 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    13407 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4774 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18695 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1573 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4889 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1358 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_types.py
--rw-rw-rw-   0 root         (0) root         (0)      604 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.689185 buildgrid-0.0.96/buildgrid/browser/
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/browser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4469 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/browser/app.py
--rw-rw-rw-   0 root         (0) root         (0)    34436 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/browser/rest_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2277 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/browser/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.690185 buildgrid-0.0.96/buildgrid/cleanup/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/cleanup/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10716 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/cleanup/cleanup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.691186 buildgrid-0.0.96/buildgrid/cleanup/janitor/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/cleanup/janitor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/cleanup/janitor/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3318 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/cleanup/janitor/index.py
--rw-rw-rw-   0 root         (0) root         (0)     5829 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/cleanup/janitor/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     1403 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/cleanup/janitor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.694186 buildgrid-0.0.96/buildgrid/client/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5099 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/actioncache.py
--rw-rw-rw-   0 root         (0) root         (0)     4457 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/asset.py
--rw-rw-rw-   0 root         (0) root         (0)     1631 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/auth_token_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     5113 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/authentication.py
--rwxrwxrwx   0 root         (0) root         (0)     1650 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/capabilities.py
--rw-rw-rw-   0 root         (0) root         (0)    41408 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/cas.py
--rw-rw-rw-   0 root         (0) root         (0)    13926 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/channel.py
--rw-rw-rw-   0 root         (0) root         (0)     4437 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/interceptors.py
--rw-rw-rw-   0 root         (0) root         (0)     2012 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/logstream.py
--rw-rw-rw-   0 root         (0) root         (0)     3410 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/client/retrier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.697185 buildgrid-0.0.96/buildgrid/server/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.697185 buildgrid-0.0.96/buildgrid/server/actioncache/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.700185 buildgrid-0.0.96/buildgrid/server/actioncache/caches/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8125 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/action_cache_abc.py
--rw-rw-rw-   0 root         (0) root         (0)     5605 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     4197 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/mirrored_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     6546 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/redis_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     6573 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/remote_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    11674 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/s3_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     4686 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/with_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3341 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/caches/write_once_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3703 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     4045 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/actioncache/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.701186 buildgrid-0.0.96/buildgrid/server/auth/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2363 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/auth/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1905 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/auth/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/auth/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    15244 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/auth/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.702185 buildgrid-0.0.96/buildgrid/server/bots/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/bots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11230 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/bots/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     7343 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/bots/job_assigner.py
--rw-rw-rw-   0 root         (0) root         (0)     5647 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/bots/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.702185 buildgrid-0.0.96/buildgrid/server/build_events/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/build_events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6045 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/build_events/service.py
--rw-rw-rw-   0 root         (0) root         (0)     7213 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/build_events/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.703185 buildgrid-0.0.96/buildgrid/server/capabilities/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/capabilities/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7113 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/capabilities/instance.py
--rwxrwxrwx   0 root         (0) root         (0)     3342 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/capabilities/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.704186 buildgrid-0.0.96/buildgrid/server/cas/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21156 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/instance.py
--rw-rw-rw-   0 root         (0) root         (0)    12330 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.707185 buildgrid-0.0.96/buildgrid/server/cas/storage/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3702 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.708186 buildgrid-0.0.96/buildgrid/server/cas/storage/index/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/index/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3335 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/index/index_abc.py
--rw-rw-rw-   0 root         (0) root         (0)    13464 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/index/redis.py
--rw-rw-rw-   0 root         (0) root         (0)    38579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/index/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.709185 buildgrid-0.0.96/buildgrid/server/cas/storage/index/sql_dialect_delegates/
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/index/sql_dialect_delegates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2136 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py
--rw-rw-rw-   0 root         (0) root         (0)     2120 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py
--rw-rw-rw-   0 root         (0) root         (0)     4436 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/lru_memory_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     5330 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/redis.py
--rw-rw-rw-   0 root         (0) root         (0)     8601 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/remote.py
--rw-rw-rw-   0 root         (0) root         (0)    11295 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/replicated.py
--rw-rw-rw-   0 root         (0) root         (0)    14426 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     6056 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/sharded.py
--rw-rw-rw-   0 root         (0) root         (0)     7039 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/size_differentiated.py
--rw-rw-rw-   0 root         (0) root         (0)     9519 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/sql.py
--rw-rw-rw-   0 root         (0) root         (0)     9510 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/storage_abc.py
--rw-rw-rw-   0 root         (0) root         (0)     7850 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/cas/storage/with_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3029 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/context.py
--rw-rw-rw-   0 root         (0) root         (0)     2194 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.709185 buildgrid-0.0.96/buildgrid/server/execution/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/execution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9678 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/execution/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     7517 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/execution/service.py
--rw-rw-rw-   0 root         (0) root         (0)     3813 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/job_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    18608 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/metrics_names.py
--rw-rw-rw-   0 root         (0) root         (0)    14482 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/metrics_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    19548 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.710185 buildgrid-0.0.96/buildgrid/server/operations/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.712185 buildgrid-0.0.96/buildgrid/server/operations/filtering/
--rw-rw-rw-   0 root         (0) root         (0)      813 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/filtering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/filtering/filter.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/filtering/filter_grammar.lark
--rw-rw-rw-   0 root         (0) root         (0)     5769 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/filtering/interpreter.py
--rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/filtering/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4594 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/filtering/sanitizer.py
--rw-rw-rw-   0 root         (0) root         (0)     4935 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     6034 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/operations/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.712185 buildgrid-0.0.96/buildgrid/server/persistence/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.713185 buildgrid-0.0.96/buildgrid/server/persistence/sql/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.714186 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/README
--rw-rw-rw-   0 root         (0) root         (0)     2919 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/env.py
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.719185 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/
--rw-rw-rw-   0 root         (0) root         (0)     1127 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)     1718 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py
--rw-rw-rw-   0 root         (0) root         (0)     1463 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py
--rw-rw-rw-   0 root         (0) root         (0)     2422 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py
--rw-rw-rw-   0 root         (0) root         (0)     1269 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py
--rw-rw-rw-   0 root         (0) root         (0)     1155 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py
--rw-rw-rw-   0 root         (0) root         (0)     1581 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py
--rw-rw-rw-   0 root         (0) root         (0)     1065 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1793 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py
--rw-rw-rw-   0 root         (0) root         (0)     2343 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1259 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1191 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     1418 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py
--rw-rw-rw-   0 root         (0) root         (0)     4625 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py
--rw-rw-rw-   0 root         (0) root         (0)     2072 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py
--rw-rw-rw-   0 root         (0) root         (0)    79760 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/impl.py
--rw-rw-rw-   0 root         (0) root         (0)     8915 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/models.py
--rw-rw-rw-   0 root         (0) root         (0)     6206 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/notifier.py
--rw-rw-rw-   0 root         (0) root         (0)    10298 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/persistence/sql/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.719185 buildgrid-0.0.96/buildgrid/server/redis/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/redis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6197 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/redis/provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4739 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/request_metadata_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.720185 buildgrid-0.0.96/buildgrid/server/s3/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18695 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/s3/s3utils.py
--rw-rw-rw-   0 root         (0) root         (0)    31657 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/server.py
--rw-rw-rw-   0 root         (0) root         (0)     6126 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/servicer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.720185 buildgrid-0.0.96/buildgrid/server/sql/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/sql/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22200 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/sql/provider.py
--rw-rw-rw-   0 root         (0) root         (0)     6225 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/sql/sqlutils.py
--rw-rw-rw-   0 root         (0) root         (0)     4806 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/threading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.721186 buildgrid-0.0.96/buildgrid/server/utils/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4484 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/utils/async_lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/utils/context.py
--rw-rw-rw-   0 root         (0) root         (0)    10885 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/server/utils/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     5450 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/settings.py
--rw-rw-rw-   0 root         (0) root         (0)    12244 2024-05-28 15:28:48.000000 buildgrid-0.0.96/buildgrid/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.735185 buildgrid-0.0.96/buildgrid.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7030 2024-05-28 15:29:20.000000 buildgrid-0.0.96/buildgrid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    21169 2024-05-28 15:29:20.000000 buildgrid-0.0.96/buildgrid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 15:29:20.000000 buildgrid-0.0.96/buildgrid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-28 15:29:20.000000 buildgrid-0.0.96/buildgrid.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1233 2024-05-28 15:29:20.000000 buildgrid-0.0.96/buildgrid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-28 15:29:20.000000 buildgrid-0.0.96/buildgrid.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.627186 buildgrid-0.0.96/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.726185 buildgrid-0.0.96/data/config/
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/all-in-one.yml
--rw-rw-rw-   0 root         (0) root         (0)      588 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/artifacts.yml
--rwxrwxrwx   0 root         (0) root         (0)     1351 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/basic-with-disk.yml
--rw-rw-rw-   0 root         (0) root         (0)     1159 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/bots-interface.yml
--rw-rw-rw-   0 root         (0) root         (0)      896 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/cache.yml
--rw-rw-rw-   0 root         (0) root         (0)     1302 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/controller.yml
--rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/default.yml
--rw-rw-rw-   0 root         (0) root         (0)      832 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/index-sqlite-no-execution.yml
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/index-sqlite.yml
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/logstream.yml
--rw-rw-rw-   0 root         (0) root         (0)     1239 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/monitoring-controller.yml
--rw-rw-rw-   0 root         (0) root         (0)     1143 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/multi-layer-storage.yml
--rw-rw-rw-   0 root         (0) root         (0)     1474 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/redis-cache.yml
--rw-rw-rw-   0 root         (0) root         (0)     1067 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/s3-indexed-cas.yml
--rw-rw-rw-   0 root         (0) root         (0)     1270 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/storage-redis.yml
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/storage-s3.yml
--rw-rw-rw-   0 root         (0) root         (0)      900 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/storage.yml
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/with-metering.yml
--rw-rw-rw-   0 root         (0) root         (0)     1478 2024-05-28 15:28:48.000000 buildgrid-0.0.96/data/config/with-pgbouncer.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.727185 buildgrid-0.0.96/docs/
--rw-rw-rw-   0 root         (0) root         (0)      610 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.727185 buildgrid-0.0.96/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.729185 buildgrid-0.0.96/docs/source/data/
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/source/data/basic-disk-cas.yml
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/source/data/bazel-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      490 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/source/data/buildstream-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      446 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/source/data/cas-and-ac.yml
--rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/source/data/cas-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/source/data/execution-and-bots.yml
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/source/data/sqlite-index-cas-only.yml
--rw-rw-rw-   0 root         (0) root         (0)     1425 2024-05-28 15:28:48.000000 buildgrid-0.0.96/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5463 2024-05-28 15:28:48.000000 buildgrid-0.0.96/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-28 15:29:20.744186 buildgrid-0.0.96/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      643 2024-05-28 15:28:48.000000 buildgrid-0.0.96/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.731186 buildgrid-0.0.96/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.628186 buildgrid-0.0.96/tests/auth/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 15:29:20.735185 buildgrid-0.0.96/tests/auth/data/
--rw-rw-rw-   0 root         (0) root         (0)      733 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/auth.yaml
--rw-rw-rw-   0 root         (0) root         (0)      417 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwks-valid.json
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-hs256-conflicting.secret
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-hs256-expired.token
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-hs256-matching.secret
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-hs256-unbounded.token
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-hs256-valid.token
--rw-rw-rw-   0 root         (0) root         (0)      272 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-rs256-conflicting.pub.key
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-rs256-expired.token
--rw-rw-rw-   0 root         (0) root         (0)      559 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-rs256-jwk-encrypted.token
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-rs256-matching.priv.key
--rw-rw-rw-   0 root         (0) root         (0)      272 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-rs256-matching.pub.key
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-rs256-unbounded.token
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/auth/data/jwt-rs256-valid.token
--rw-rw-rw-   0 root         (0) root         (0)     3829 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_async_lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    15407 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_execution_instance.py
--rw-rw-rw-   0 root         (0) root         (0)     2199 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_job_assigner.py
--rw-rw-rw-   0 root         (0) root         (0)    12358 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_metrics_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3447 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_mirrored_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     2098 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_multithreaded_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2777 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_request_metadata_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    32384 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)    10567 2024-05-28 15:28:48.000000 buildgrid-0.0.96/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.190367 buildgrid-0.0.97/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-05-31 13:14:34.000000 buildgrid-0.0.97/BuildGrid.doap
+-rw-rw-rw-   0 root         (0) root         (0)     9648 2024-05-31 13:14:34.000000 buildgrid-0.0.97/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11338 2024-05-31 13:14:34.000000 buildgrid-0.0.97/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      500 2024-05-31 13:14:34.000000 buildgrid-0.0.97/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7030 2024-05-31 13:15:02.190367 buildgrid-0.0.97/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2932 2024-05-31 13:14:34.000000 buildgrid-0.0.97/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.083367 buildgrid-0.0.97/buildgrid/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.085367 buildgrid-0.0.97/buildgrid/_app/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5675 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.088367 buildgrid-0.0.97/buildgrid/_app/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6755 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/commands/cmd_actioncache.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/commands/cmd_browser_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     3170 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/commands/cmd_capabilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    10608 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/commands/cmd_cas.py
+-rw-rw-rw-   0 root         (0) root         (0)     8817 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/commands/cmd_cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)    12570 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/commands/cmd_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2840 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/commands/cmd_janitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     4842 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/commands/cmd_logstream.py
+-rw-rw-rw-   0 root         (0) root         (0)    11215 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/commands/cmd_operation.py
+-rw-rw-rw-   0 root         (0) root         (0)     8166 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/commands/cmd_server.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/commands/rpc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.089367 buildgrid-0.0.97/buildgrid/_app/settings/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   111784 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     8691 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/reference.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.089367 buildgrid-0.0.97/buildgrid/_app/settings/schemas/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.090367 buildgrid-0.0.97/buildgrid/_app/settings/schemas/caches/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/caches/lru-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/caches/mirrored-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      676 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/caches/with-cache.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.090367 buildgrid-0.0.97/buildgrid/_app/settings/schemas/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/clients/asset-client.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.091367 buildgrid-0.0.97/buildgrid/_app/settings/schemas/connections/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/connections/redis.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/connections/sql.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.091367 buildgrid-0.0.97/buildgrid/_app/settings/schemas/misc/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/misc/channel.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.092367 buildgrid-0.0.97/buildgrid/_app/settings/schemas/scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/scheduler/memory.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3907 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/scheduler/sql.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.094367 buildgrid-0.0.97/buildgrid/_app/settings/schemas/services/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/services/action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/services/bots.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      343 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/services/bytestream.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      273 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/services/cas.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1640 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/services/execution.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/services/platform-queues.yml
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/services/s3-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/services/write-once-action-cache.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.097367 buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/disk.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/lru.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/operations_sql_storage.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      207 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/redis-index.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/redis.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      601 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/remote.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/replicated.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      592 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/s3.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/sharded.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      530 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/sql-index.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/sql.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      281 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/with-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4776 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     8802 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.097367 buildgrid-0.0.97/buildgrid/_protos/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.097367 buildgrid-0.0.97/buildgrid/_protos/build/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.098367 buildgrid-0.0.97/buildgrid/_protos/build/bazel/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.098367 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.098367 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/asset/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/asset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.100367 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/asset/v1/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/asset/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7795 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    27103 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    16783 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)    15404 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    16783 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)    15550 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.100367 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.102367 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/v2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30140 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)   136470 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    59894 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)    47588 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    59894 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)    47884 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.103367 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.104367 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/v1/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2066 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3176 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    12298 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7788 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    12298 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7844 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.106367 buildgrid-0.0.97/buildgrid/_protos/build/bazel/semver/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/semver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/semver/semver_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2068 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.108367 buildgrid-0.0.97/buildgrid/_protos/build/buildbox/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/buildbox/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1944 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/buildbox/execution_stats_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4156 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.108367 buildgrid-0.0.97/buildgrid/_protos/buildgrid/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.112367 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3156 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/messaging_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10940 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3824 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     9955 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2881 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2872 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2872 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.113367 buildgrid-0.0.97/buildgrid/_protos/google/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.119367 buildgrid-0.0.97/buildgrid/_protos/google/api/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/annotations_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/annotations_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/annotations_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/client_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/client_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/client_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/client_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/client_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/field_behavior_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     6343 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/field_behavior_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/field_behavior_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/http_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18246 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/http_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/http_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/http_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/http_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.120367 buildgrid-0.0.97/buildgrid/_protos/google/bytestream/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/bytestream/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3246 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/bytestream/bytestream_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     7478 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10732 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     8880 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10732 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     8996 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.121367 buildgrid-0.0.97/buildgrid/_protos/google/devtools/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.121367 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.125367 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5933 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18014 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5408 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     6758 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10427 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     8451 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5461 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     8451 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     5547 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.126367 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.132367 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7859 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    23457 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    11879 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7140 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    11879 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7256 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     6133 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    21890 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     5337 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     9321 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4382 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     4498 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    11299 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.133367 buildgrid-0.0.97/buildgrid/_protos/google/longrunning/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/longrunning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5084 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/longrunning/operations_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     7984 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/longrunning/operations_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10950 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7133 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10950 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7279 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.138367 buildgrid-0.0.97/buildgrid/_protos/google/rpc/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/code_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    13407 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/code_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/code_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4774 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/error_details_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18695 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/error_details_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/error_details_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1573 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/status_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4889 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/status_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      604 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.139367 buildgrid-0.0.97/buildgrid/browser/
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/browser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4469 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/browser/app.py
+-rw-rw-rw-   0 root         (0) root         (0)    34436 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/browser/rest_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/browser/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.139367 buildgrid-0.0.97/buildgrid/cleanup/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/cleanup/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10716 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/cleanup/cleanup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.140367 buildgrid-0.0.97/buildgrid/cleanup/janitor/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/cleanup/janitor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/cleanup/janitor/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3318 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/cleanup/janitor/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     5829 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/cleanup/janitor/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1403 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/cleanup/janitor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.143367 buildgrid-0.0.97/buildgrid/client/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5099 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/client/actioncache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4457 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/client/asset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/client/auth_token_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     5113 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/client/authentication.py
+-rwxrwxrwx   0 root         (0) root         (0)     1650 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/client/capabilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    41408 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/client/cas.py
+-rw-rw-rw-   0 root         (0) root         (0)    13926 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/client/channel.py
+-rw-rw-rw-   0 root         (0) root         (0)     4437 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/client/interceptors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2012 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/client/logstream.py
+-rw-rw-rw-   0 root         (0) root         (0)     3410 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/client/retrier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.146367 buildgrid-0.0.97/buildgrid/server/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.146367 buildgrid-0.0.97/buildgrid/server/actioncache/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/actioncache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.149367 buildgrid-0.0.97/buildgrid/server/actioncache/caches/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/actioncache/caches/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7571 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/actioncache/caches/action_cache_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5605 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/actioncache/caches/lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4197 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/actioncache/caches/mirrored_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     6546 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/actioncache/caches/redis_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     6573 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/actioncache/caches/remote_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    11674 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/actioncache/caches/s3_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4686 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/actioncache/caches/with_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/actioncache/caches/write_once_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3703 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/actioncache/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/actioncache/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.150367 buildgrid-0.0.97/buildgrid/server/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2363 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/auth/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/auth/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/auth/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15244 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/auth/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.151367 buildgrid-0.0.97/buildgrid/server/bots/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/bots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11380 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/bots/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     7876 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/bots/job_assigner.py
+-rw-rw-rw-   0 root         (0) root         (0)     5647 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/bots/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.152367 buildgrid-0.0.97/buildgrid/server/build_events/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/build_events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6045 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/build_events/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     7213 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/build_events/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.152367 buildgrid-0.0.97/buildgrid/server/capabilities/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/capabilities/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7113 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/capabilities/instance.py
+-rwxrwxrwx   0 root         (0) root         (0)     3342 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/capabilities/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.153367 buildgrid-0.0.97/buildgrid/server/cas/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21158 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)    12348 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.156367 buildgrid-0.0.97/buildgrid/server/cas/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3702 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.157367 buildgrid-0.0.97/buildgrid/server/cas/storage/index/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/index/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3335 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/index/index_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)    13469 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/index/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)    38847 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/index/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.158367 buildgrid-0.0.97/buildgrid/server/cas/storage/index/sql_dialect_delegates/
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/index/sql_dialect_delegates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2204 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2188 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4436 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/lru_memory_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     5330 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)     8601 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/remote.py
+-rw-rw-rw-   0 root         (0) root         (0)    11295 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/replicated.py
+-rw-rw-rw-   0 root         (0) root         (0)    14426 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     6056 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/sharded.py
+-rw-rw-rw-   0 root         (0) root         (0)     7039 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/size_differentiated.py
+-rw-rw-rw-   0 root         (0) root         (0)     9519 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     9510 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/storage_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7850 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/cas/storage/with_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3029 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     2371 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.158367 buildgrid-0.0.97/buildgrid/server/execution/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/execution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9678 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/execution/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     7517 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/execution/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     3813 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/job_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    18608 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/metrics_names.py
+-rw-rw-rw-   0 root         (0) root         (0)    14482 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/metrics_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    19548 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.159367 buildgrid-0.0.97/buildgrid/server/operations/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.161367 buildgrid-0.0.97/buildgrid/server/operations/filtering/
+-rw-rw-rw-   0 root         (0) root         (0)      813 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/operations/filtering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/operations/filtering/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/operations/filtering/filter_grammar.lark
+-rw-rw-rw-   0 root         (0) root         (0)     5769 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/operations/filtering/interpreter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/operations/filtering/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4594 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/operations/filtering/sanitizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4935 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/operations/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     6034 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/operations/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.161367 buildgrid-0.0.97/buildgrid/server/persistence/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.162367 buildgrid-0.0.97/buildgrid/server/persistence/sql/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.163367 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/README
+-rw-rw-rw-   0 root         (0) root         (0)     2919 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/env.py
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.167367 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2422 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1191 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py
+-rw-rw-rw-   0 root         (0) root         (0)     4625 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py
+-rw-rw-rw-   0 root         (0) root         (0)     2072 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py
+-rw-rw-rw-   0 root         (0) root         (0)    80435 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     8915 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6206 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/notifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    10298 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/persistence/sql/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.168367 buildgrid-0.0.97/buildgrid/server/redis/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/redis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6197 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/redis/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4739 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/request_metadata_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.168367 buildgrid-0.0.97/buildgrid/server/s3/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18695 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/s3/s3utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    31657 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/server.py
+-rw-rw-rw-   0 root         (0) root         (0)     6126 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/servicer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.169367 buildgrid-0.0.97/buildgrid/server/sql/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/sql/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22200 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/sql/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     6225 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/sql/sqlutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4806 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/threading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.170367 buildgrid-0.0.97/buildgrid/server/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4484 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/utils/async_lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/utils/context.py
+-rw-rw-rw-   0 root         (0) root         (0)    10885 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/server/utils/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5450 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    12244 2024-05-31 13:14:34.000000 buildgrid-0.0.97/buildgrid/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.183367 buildgrid-0.0.97/buildgrid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7030 2024-05-31 13:15:02.000000 buildgrid-0.0.97/buildgrid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21169 2024-05-31 13:15:02.000000 buildgrid-0.0.97/buildgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 13:15:02.000000 buildgrid-0.0.97/buildgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-31 13:15:02.000000 buildgrid-0.0.97/buildgrid.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1233 2024-05-31 13:15:02.000000 buildgrid-0.0.97/buildgrid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-31 13:15:02.000000 buildgrid-0.0.97/buildgrid.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.079367 buildgrid-0.0.97/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.175367 buildgrid-0.0.97/data/config/
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/all-in-one.yml
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/artifacts.yml
+-rwxrwxrwx   0 root         (0) root         (0)     1351 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/basic-with-disk.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/bots-interface.yml
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/cache.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/controller.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/default.yml
+-rw-rw-rw-   0 root         (0) root         (0)      832 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/index-sqlite-no-execution.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/index-sqlite.yml
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/logstream.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/monitoring-controller.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/multi-layer-storage.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/redis-cache.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/s3-indexed-cas.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/storage-redis.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/storage-s3.yml
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/storage.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/with-metering.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2024-05-31 13:14:34.000000 buildgrid-0.0.97/data/config/with-pgbouncer.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.175367 buildgrid-0.0.97/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      610 2024-05-31 13:14:34.000000 buildgrid-0.0.97/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.175367 buildgrid-0.0.97/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.177367 buildgrid-0.0.97/docs/source/data/
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-31 13:14:34.000000 buildgrid-0.0.97/docs/source/data/basic-disk-cas.yml
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-05-31 13:14:34.000000 buildgrid-0.0.97/docs/source/data/bazel-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      490 2024-05-31 13:14:34.000000 buildgrid-0.0.97/docs/source/data/buildstream-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      446 2024-05-31 13:14:34.000000 buildgrid-0.0.97/docs/source/data/cas-and-ac.yml
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-31 13:14:34.000000 buildgrid-0.0.97/docs/source/data/cas-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-05-31 13:14:34.000000 buildgrid-0.0.97/docs/source/data/execution-and-bots.yml
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-31 13:14:34.000000 buildgrid-0.0.97/docs/source/data/sqlite-index-cas-only.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2024-05-31 13:14:34.000000 buildgrid-0.0.97/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5463 2024-05-31 13:14:34.000000 buildgrid-0.0.97/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-31 13:15:02.190367 buildgrid-0.0.97/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      643 2024-05-31 13:14:34.000000 buildgrid-0.0.97/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.179367 buildgrid-0.0.97/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.080367 buildgrid-0.0.97/tests/auth/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 13:15:02.182367 buildgrid-0.0.97/tests/auth/data/
+-rw-rw-rw-   0 root         (0) root         (0)      733 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/auth/data/auth.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/auth/data/jwks-valid.json
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/auth/data/jwt-hs256-conflicting.secret
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/auth/data/jwt-hs256-expired.token
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/auth/data/jwt-hs256-matching.secret
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/auth/data/jwt-hs256-unbounded.token
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/auth/data/jwt-hs256-valid.token
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/auth/data/jwt-rs256-conflicting.pub.key
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/auth/data/jwt-rs256-expired.token
+-rw-rw-rw-   0 root         (0) root         (0)      559 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/auth/data/jwt-rs256-jwk-encrypted.token
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/auth/data/jwt-rs256-matching.priv.key
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/auth/data/jwt-rs256-matching.pub.key
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/auth/data/jwt-rs256-unbounded.token
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/auth/data/jwt-rs256-valid.token
+-rw-rw-rw-   0 root         (0) root         (0)     3829 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/test_async_lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    15407 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/test_execution_instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     2199 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/test_job_assigner.py
+-rw-rw-rw-   0 root         (0) root         (0)    12358 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/test_metrics_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3447 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/test_mirrored_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/test_multithreaded_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/test_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/test_request_metadata_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    32444 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/test_scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)    10567 2024-05-31 13:14:34.000000 buildgrid-0.0.97/tests/test_utils.py
```

### Comparing `buildgrid-0.0.96/BuildGrid.doap` & `buildgrid-0.0.97/BuildGrid.doap`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/CONTRIBUTING.rst` & `buildgrid-0.0.97/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/LICENSE` & `buildgrid-0.0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/PKG-INFO` & `buildgrid-0.0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildgrid
-Version: 0.0.96
+Version: 0.0.97
 Summary: A remote execution service
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://buildgrid.build
 Project-URL: Documentation, https://buildgrid.build
 Project-URL: Repository, https://gitlab.com/BuildGrid/buildgrid
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `buildgrid-0.0.96/README.rst` & `buildgrid-0.0.97/README.rst`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/__init__.py` & `buildgrid-0.0.97/buildgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/__init__.py` & `buildgrid-0.0.97/buildgrid/_app/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/cli.py` & `buildgrid-0.0.97/buildgrid/_app/cli.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/commands/__init__.py` & `buildgrid-0.0.97/buildgrid/_app/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/commands/cmd_actioncache.py` & `buildgrid-0.0.97/buildgrid/_app/commands/cmd_actioncache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/commands/cmd_browser_backend.py` & `buildgrid-0.0.97/buildgrid/_app/commands/cmd_browser_backend.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/commands/cmd_capabilities.py` & `buildgrid-0.0.97/buildgrid/_app/commands/cmd_capabilities.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/commands/cmd_cas.py` & `buildgrid-0.0.97/buildgrid/_app/commands/cmd_cas.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/commands/cmd_cleanup.py` & `buildgrid-0.0.97/buildgrid/_app/commands/cmd_cleanup.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/commands/cmd_execute.py` & `buildgrid-0.0.97/buildgrid/_app/commands/cmd_execute.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/commands/cmd_janitor.py` & `buildgrid-0.0.97/buildgrid/_app/commands/cmd_janitor.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/commands/cmd_logstream.py` & `buildgrid-0.0.97/buildgrid/_app/commands/cmd_logstream.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/commands/cmd_operation.py` & `buildgrid-0.0.97/buildgrid/_app/commands/cmd_operation.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/commands/cmd_server.py` & `buildgrid-0.0.97/buildgrid/_app/commands/cmd_server.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/commands/rpc_utils.py` & `buildgrid-0.0.97/buildgrid/_app/commands/rpc_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/settings/__init__.py` & `buildgrid-0.0.97/buildgrid/_app/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/settings/parser.py` & `buildgrid-0.0.97/buildgrid/_app/settings/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1438,14 +1438,18 @@
             stream of an `Execute` or `WaitExecution` request. Defaults to 600s
             (10 minutes).
         endpoints (list): List of service/endpoint types to enable. Possible services are
             ``execution``, ``operations``, and ``bots``. By default all three are enabled.
         max_list_operations_page_size (int): The maximum number of operations that can
             be returned in a ListOperations response. A page token will be returned
             with the response to allow the client to get the next page of results.
+        priority_assignment_percentage (int): A value between 0 and 100 (inclusive) representing
+            the percentage of workers to assign jobs to in priority order. The remainder will be
+            assigned work in oldest-first order. Defaults to 100, or all work assigned in priority
+            order. Only relevant when the ``bots`` endpoint is enabled.
 
         property_keys: Deprecated field. Set this in the scheduler.
         wildcard_property_keys: Deprecated field. Set this in the scheduler.
         storage: Deprecated field. All internal state is now managed by the provided scheduler.
         sql: Deprecated field. All internal state is now managed by the provided scheduler.
         discard_unwatched_jobs: Deprecated field. Unused.
         permissive_bot_session: Deprecated field. UpdateBotSession is always validated.
@@ -1461,14 +1465,15 @@
 
     def __new__(
         cls,
         _yaml_filename: str,
         operation_stream_keepalive_timeout=600,
         endpoints=ServiceName.default_services(),
         max_list_operations_page_size=DEFAULT_MAX_LIST_OPERATION_PAGE_SIZE,
+        priority_assignment_percentage: int = 100,
         # Deprecated options kept to support migrations.
         data_store=None,
         scheduler=None,
         property_keys=None,
         wildcard_property_keys=None,
         logstream=None,
         storage: Optional[StorageABC] = None,
@@ -1605,14 +1610,15 @@
                 scheduler.logstream_channel = logstream_channel
 
         return ExecutionController(
             scheduler,
             operation_stream_keepalive_timeout=operation_stream_keepalive_timeout,
             services=endpoints,
             max_list_operations_page_size=max_list_operations_page_size,
+            priority_assignment_percentage=priority_assignment_percentage,
         )
 
 
 class Bots(YamlFactory):
     """Generates :class:`buildgrid.server.bots.instance.BotsInterface`
     using the tag ``!bots``.
 
@@ -1624,14 +1630,18 @@
               action-cache: *remote-cache
               scheduler: *state-database
               bot-session-keepalive-timeout: 600
               permissive-bot-session: yes
 
     Args:
         scheduler(:class:`SQLDataStore`): Instance of data store to use for the scheduler's state.
+        priority_assignment_percentage (int): A value between 0 and 100 (inclusive) representing
+            the percentage of workers to assign jobs to in priority order. The remainder will be
+            assigned work in oldest-first order. Defaults to 100, or all work assigned in priority
+            order.
 
         storage: Deprecated field. All internal state is now managed by the provided scheduler.
         sql: Deprecated field. All internal state is now managed by the provided scheduler.
         action_cache: Deprecated field. Set this in the scheduler.
         bot_session_keepalive_timeout: Deprecated field. Set this in the scheduler.
         permissive_bot_session: Deprecated field. UpdateBotSession is always validated
         metering_service_client: Deprecated field. Set this in the scheduler.
@@ -1648,14 +1658,15 @@
         action_cache=None,
         bot_session_keepalive_timeout: Optional[int] = None,
         data_store=None,
         scheduler=None,
         permissive_bot_session: Optional[bool] = None,
         logstream=None,
         metering_service_client: Optional[metering.SyncMeteringServiceClient] = None,
+        priority_assignment_percentage: int = 100,
     ):
         scheduler = _validate_scheduler(cls, scheduler, data_store)
         if isinstance(action_cache, ActionCache):
             click.echo(
                 click.style(
                     "Warning: Passing an ActionCache instance (!action-cache) to an Execution "
                     "service is deprecated. Use a cache backend such as !lru-action-cache instead.",
@@ -1733,15 +1744,15 @@
                     client_key=logstream_credentials.get("tls-client-key"),
                     client_cert=logstream_credentials.get("tls-client-cert"),
                     server_cert=logstream_credentials.get("tls-server-cert"),
                 )
                 scheduler.logstream_instance = logstream_instance
                 scheduler.logstream_channel = logstream_channel
 
-        return BotsInterface(scheduler)
+        return BotsInterface(scheduler, priority_assignment_percentage=priority_assignment_percentage)
 
 
 class Action(YamlFactory):
     """Generates :class:`buildgrid.server.actioncache.service.ActionCacheService`
     using the tag ``!action-cache``.
 
     Usage
```

### Comparing `buildgrid-0.0.96/buildgrid/_app/settings/reference.yml` & `buildgrid-0.0.97/buildgrid/_app/settings/reference.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml` & `buildgrid-0.0.97/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml` & `buildgrid-0.0.97/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/settings/schemas/config.yaml` & `buildgrid-0.0.97/buildgrid/_app/settings/schemas/config.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/settings/schemas/connections/sql.yaml` & `buildgrid-0.0.97/buildgrid/_app/settings/schemas/connections/sql.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/settings/schemas/misc/channel.yaml` & `buildgrid-0.0.97/buildgrid/_app/settings/schemas/misc/channel.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/settings/schemas/scheduler/sql.yaml` & `buildgrid-0.0.97/buildgrid/_app/settings/schemas/scheduler/sql.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/action-cache.yaml` & `buildgrid-0.0.97/buildgrid/_app/settings/schemas/services/action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/bots.yaml` & `buildgrid-0.0.97/buildgrid/_app/settings/schemas/services/bots.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -41,7 +41,11 @@
           - tls-client-cert
           - tls-server-cert
     required:
       - url
       - instance-name
   metering-service-client:
     type: "!metering-service-client"
+  priority-assignment-percentage:
+    type: number
+    minimum: 0
+    maximum: 100
```

### Comparing `buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/execution.yaml` & `buildgrid-0.0.97/buildgrid/_app/settings/schemas/services/execution.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -72,7 +72,11 @@
           - tls-client-cert
           - tls-server-cert
     required:
       - url
       - instance-name
   metering-service-client:
     type: "!metering-service-client"
+  priority-assignment-percentage:
+    type: number
+    minimum: 0
+    maximum: 100
```

### Comparing `buildgrid-0.0.96/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml` & `buildgrid-0.0.97/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/remote.yaml` & `buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/remote.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/s3.yaml` & `buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/s3.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml` & `buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_app/settings/schemas/storage/sql-index.yaml` & `buildgrid-0.0.97/buildgrid/_app/settings/schemas/storage/sql-index.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_enums.py` & `buildgrid-0.0.97/buildgrid/_enums.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_exceptions.py` & `buildgrid-0.0.97/buildgrid/_exceptions.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/build/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/semver/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/semver/semver_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/build/buildbox/execution_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/buildgrid/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/buildgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/messaging_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py` & `buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py` & `buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/google/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/api/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/api/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/google/api/client_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/api/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/api/client_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/google/api/field_behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/api/field_behavior_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/api/http_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/bytestream/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/google/bytestream/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/google/bytestream/bytestream_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py` & `buildgrid-0.0.97/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py` & `buildgrid-0.0.97/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/longrunning/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/google/longrunning/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/google/longrunning/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/longrunning/operations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py` & `buildgrid-0.0.97/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py` & `buildgrid-0.0.97/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/rpc/__init__.py` & `buildgrid-0.0.97/buildgrid/_protos/google/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/google/rpc/code_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/rpc/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/google/rpc/error_details_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/rpc/error_details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2.py` & `buildgrid-0.0.97/buildgrid/_protos/google/rpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/rpc/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi` & `buildgrid-0.0.97/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_types.py` & `buildgrid-0.0.97/buildgrid/_types.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/_version.py` & `buildgrid-0.0.97/buildgrid/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "0.0.96"
+__version__ = "0.0.97"
```

### Comparing `buildgrid-0.0.96/buildgrid/browser/__init__.py` & `buildgrid-0.0.97/buildgrid/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/browser/app.py` & `buildgrid-0.0.97/buildgrid/browser/app.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/browser/rest_api.py` & `buildgrid-0.0.97/buildgrid/browser/rest_api.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/browser/utils.py` & `buildgrid-0.0.97/buildgrid/browser/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/cleanup/__init__.py` & `buildgrid-0.0.97/buildgrid/cleanup/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/cleanup/cleanup.py` & `buildgrid-0.0.97/buildgrid/cleanup/cleanup.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/cleanup/janitor/__init__.py` & `buildgrid-0.0.97/buildgrid/cleanup/janitor/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/cleanup/janitor/config.py` & `buildgrid-0.0.97/buildgrid/cleanup/janitor/config.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/cleanup/janitor/index.py` & `buildgrid-0.0.97/buildgrid/cleanup/janitor/index.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/cleanup/janitor/s3.py` & `buildgrid-0.0.97/buildgrid/cleanup/janitor/s3.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/cleanup/janitor/utils.py` & `buildgrid-0.0.97/buildgrid/cleanup/janitor/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/client/__init__.py` & `buildgrid-0.0.97/buildgrid/client/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/client/actioncache.py` & `buildgrid-0.0.97/buildgrid/client/actioncache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/client/asset.py` & `buildgrid-0.0.97/buildgrid/client/asset.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/client/auth_token_loader.py` & `buildgrid-0.0.97/buildgrid/client/auth_token_loader.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/client/authentication.py` & `buildgrid-0.0.97/buildgrid/client/authentication.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/client/capabilities.py` & `buildgrid-0.0.97/buildgrid/client/capabilities.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/client/cas.py` & `buildgrid-0.0.97/buildgrid/client/cas.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/client/channel.py` & `buildgrid-0.0.97/buildgrid/client/channel.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/client/interceptors.py` & `buildgrid-0.0.97/buildgrid/client/interceptors.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/client/logstream.py` & `buildgrid-0.0.97/buildgrid/client/logstream.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/client/retrier.py` & `buildgrid-0.0.97/buildgrid/client/retrier.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/__init__.py` & `buildgrid-0.0.97/buildgrid/server/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/actioncache/__init__.py` & `buildgrid-0.0.97/buildgrid/server/actioncache/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/actioncache/caches/__init__.py` & `buildgrid-0.0.97/buildgrid/server/actioncache/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/actioncache/caches/action_cache_abc.py` & `buildgrid-0.0.97/buildgrid/server/actioncache/caches/action_cache_abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,25 +156,14 @@
         # overhead.
         action = self._storage.get_message(action_digest, Action)
         action_blobs: Set[HashableDigest] = set()
         if action:
             action_blobs.add(HashableDigest(action_digest.hash, action_digest.size_bytes))
             action_blobs.add(HashableDigest(action.command_digest.hash, action.command_digest.size_bytes))
             action_blobs.add(HashableDigest(action.input_root_digest.hash, action.input_root_digest.size_bytes))
-            try:
-                for directory in self._storage.get_tree(action.input_root_digest, raise_on_missing_subdir=False):
-                    action_blobs.update(
-                        [
-                            HashableDigest(dir_node.digest.hash, dir_node.digest.size_bytes)
-                            for dir_node in directory.directories
-                        ]
-                    )
-            except NotFoundError:
-                # Checking blobs for the Action is best effort, it's okay if some are missing
-                pass
 
         blobs_to_check: Set[HashableDigest] = blobs_needed | action_blobs
         # No need to check the underlying storage for the empty blob as it is a special case blob which always exists
         # It is possible that the empty blob is not actually present in the underlying storage
         blobs_to_check.discard(HashableDigest(EMPTY_BLOB_DIGEST.hash, EMPTY_BLOB_DIGEST.size_bytes))
         missing = self._storage.missing_blobs([blob.to_digest() for blob in blobs_to_check])
         required_missing = [blob for blob in missing if HashableDigest(blob.hash, blob.size_bytes) in blobs_needed]
```

### Comparing `buildgrid-0.0.96/buildgrid/server/actioncache/caches/lru_cache.py` & `buildgrid-0.0.97/buildgrid/server/actioncache/caches/lru_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/actioncache/caches/mirrored_cache.py` & `buildgrid-0.0.97/buildgrid/server/actioncache/caches/mirrored_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/actioncache/caches/redis_cache.py` & `buildgrid-0.0.97/buildgrid/server/actioncache/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/actioncache/caches/remote_cache.py` & `buildgrid-0.0.97/buildgrid/server/actioncache/caches/remote_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/actioncache/caches/s3_cache.py` & `buildgrid-0.0.97/buildgrid/server/actioncache/caches/s3_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/actioncache/caches/with_cache.py` & `buildgrid-0.0.97/buildgrid/server/actioncache/caches/with_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/actioncache/caches/write_once_cache.py` & `buildgrid-0.0.97/buildgrid/server/actioncache/caches/write_once_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/actioncache/instance.py` & `buildgrid-0.0.97/buildgrid/server/actioncache/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/actioncache/service.py` & `buildgrid-0.0.97/buildgrid/server/actioncache/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/auth/__init__.py` & `buildgrid-0.0.97/buildgrid/server/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/auth/config.py` & `buildgrid-0.0.97/buildgrid/server/auth/config.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/auth/enums.py` & `buildgrid-0.0.97/buildgrid/server/auth/enums.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/auth/exceptions.py` & `buildgrid-0.0.97/buildgrid/server/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/auth/manager.py` & `buildgrid-0.0.97/buildgrid/server/auth/manager.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/bots/__init__.py` & `buildgrid-0.0.97/buildgrid/server/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/bots/instance.py` & `buildgrid-0.0.97/buildgrid/server/bots/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,23 @@
     SERVICE_NAME = BOTS_DESCRIPTOR.services_by_name["Bots"].full_name
 
     def __init__(
         self,
         scheduler: SQLDataStore,
         *,
         job_assignment_interval: float = 1.0,
+        priority_assignment_percentage: int = 100,
     ) -> None:
         self._stack = ExitStack()
 
-        self._job_assigner = JobAssigner(scheduler, job_assignment_interval=job_assignment_interval)
+        self._job_assigner = JobAssigner(
+            scheduler,
+            job_assignment_interval=job_assignment_interval,
+            priority_percentage=priority_assignment_percentage,
+        )
         self.scheduler = scheduler
 
         # Set the deadline event on worker stop to allow fast exit
         self.reaper = ContextWorker(self._reap_expired_sessions_loop, "BotReaper")
 
     def start(self) -> None:
         self._stack.enter_context(self.scheduler)
```

### Comparing `buildgrid-0.0.96/buildgrid/server/bots/job_assigner.py` & `buildgrid-0.0.97/buildgrid/server/bots/job_assigner.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import logging
+import random
 import threading
 import uuid
 from contextlib import contextmanager
 from itertools import chain, combinations
 from threading import Event, Lock
 from typing import Any, Dict, Iterable, Iterator, List, Set, TypeVar
 
@@ -29,25 +30,26 @@
 LOGGER = logging.getLogger(__name__)
 
 
 T = TypeVar("T", bound="JobAssigner")
 
 
 class JobAssigner:
-    def __init__(self, data_store: SQLDataStore, job_assignment_interval: float = 1.0):
+    def __init__(self, data_store: SQLDataStore, job_assignment_interval: float = 1.0, priority_percentage: int = 100):
         self._lock = Lock()
         # Dict[Hash, Dict[BotName, Dict[Key, Event]]]
         self._events: Dict[str, Dict[str, Dict[str, Event]]] = {}
         self._data_store = data_store
         # Here we allow immediately starting a new assignment if a bot is added to the lookup.
         self._new_bots_added = Event()
         self._job_assignment_worker = ContextWorker(
             target=self.begin, name="JobAssignment", on_shutdown_requested=self._new_bots_added.set
         )
         self._job_assignment_interval = job_assignment_interval
+        self._priority_percentage = priority_percentage
 
     def __enter__(self: T) -> T:
         self.start()
         return self
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         self.stop()
@@ -82,15 +84,15 @@
                 for worker_hash in worker_hashes:
                     del self._events[worker_hash][bot_session.name][key]
                     if len(self._events[worker_hash][bot_session.name]) == 0:
                         del self._events[worker_hash][bot_session.name]
                     if len(self._events[worker_hash]) == 0:
                         del self._events[worker_hash]
 
-    def assign_jobs(self, shutdown_requested: threading.Event) -> None:
+    def assign_jobs(self, shutdown_requested: threading.Event, oldest_first: bool = False) -> None:
         """Assign jobs to the currently connected workers
 
         This method iterates over the buckets of currently connected workers,
         and requests a number of job assignments from the data store to cover
         the number of workers in each bucket. Empty buckets are skipped.
         """
 
@@ -101,24 +103,32 @@
             if shutdown_requested.is_set():
                 return
 
             with self._lock:
                 bot_names = list(self._events.get(worker_hash, {}))
 
             if bot_names:
-                assigned_bot_names = self._data_store.assign_n_leases(capability_hash=worker_hash, bot_names=bot_names)
+                if oldest_first:
+                    assigned_bot_names = self._data_store.assign_n_leases_by_age(
+                        capability_hash=worker_hash, bot_names=bot_names
+                    )
+                else:
+                    assigned_bot_names = self._data_store.assign_n_leases_by_priority(
+                        capability_hash=worker_hash, bot_names=bot_names
+                    )
                 with self._lock:
                     for name in assigned_bot_names:
                         for event in self._events.get(worker_hash, {}).get(name, {}).values():
                             event.set()
 
     def begin(self, shutdown_requested: threading.Event) -> None:
         while not shutdown_requested.is_set():
             try:
-                self.assign_jobs(shutdown_requested)
+                oldest_first = random.randint(1, 100) > self._priority_percentage
+                self.assign_jobs(shutdown_requested, oldest_first=oldest_first)
             except Exception:
                 LOGGER.exception("Error in job assignment thread", exc_info=True)
             self._new_bots_added.wait(timeout=self._job_assignment_interval)
             self._new_bots_added.clear()
 
 
 def get_partial_capabilities(capabilities: Dict[str, List[str]]) -> Iterable[Dict[str, List[str]]]:
```

### Comparing `buildgrid-0.0.96/buildgrid/server/bots/service.py` & `buildgrid-0.0.97/buildgrid/server/bots/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/build_events/__init__.py` & `buildgrid-0.0.97/buildgrid/server/build_events/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/build_events/service.py` & `buildgrid-0.0.97/buildgrid/server/build_events/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/build_events/storage.py` & `buildgrid-0.0.97/buildgrid/server/build_events/storage.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/capabilities/__init__.py` & `buildgrid-0.0.97/buildgrid/server/capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/capabilities/instance.py` & `buildgrid-0.0.97/buildgrid/server/capabilities/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/capabilities/service.py` & `buildgrid-0.0.97/buildgrid/server/capabilities/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/__init__.py` & `buildgrid-0.0.97/buildgrid/server/cas/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/instance.py` & `buildgrid-0.0.97/buildgrid/server/cas/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,15 @@
             return
         tree = Tree(root=root, children=children)
         tree_digest = self._storage.put_message(tree)
         self._tree_cache[(root_digest.hash, root_digest.size_bytes)] = tree_digest
 
     get_tree_ignored_exceptions = (NotFoundError, RetriableError)
 
-    @DurationMetric(CAS_GET_TREE_TIME_METRIC_NAME, instanced=True)
+    @generator_method_duration_metric(CAS_GET_TREE_TIME_METRIC_NAME)
     @generator_method_exception_counter(
         CAS_GET_TREE_EXCEPTION_COUNT_METRIC_NAME,
         ignored_exceptions=get_tree_ignored_exceptions,
     )
     def get_tree(self, request: GetTreeRequest) -> Iterator[GetTreeResponse]:
         storage = self._storage
```

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/service.py` & `buildgrid-0.0.97/buildgrid/server/cas/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             status_code = code_pb2.OK
             response_proto.status.CopyFrom(status_pb2.Status(code=status_code))
 
         return response
 
     @authorize_unary_stream(lambda r: cast(str, r.instance_name))
     @track_request_id_generator
-    @DurationMetric(CAS_GET_TREE_TIME_METRIC_NAME)
+    @generator_method_duration_metric(CAS_GET_TREE_TIME_METRIC_NAME)
     @handle_errors_unary_stream(GetTreeResponse)
     def GetTree(self, request: GetTreeRequest, context: grpc.ServicerContext) -> Iterator[GetTreeResponse]:
         LOGGER.info(
             f"GetTree request from [{context.peer()}] "
             f"([{printable_request_metadata(context.invocation_metadata())}])"
         )
```

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/__init__.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/disk.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/disk.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/index/__init__.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/index/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/index/index_abc.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/index/index_abc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/index/redis.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/index/redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,16 +231,16 @@
             threshold_time = protect_blobs_after
         else:
             threshold_time = now
 
         # Used for metric publishing
         delete_start_time = time.time()
         metadata = {}
-        if self._instance_name:
-            metadata["instance-name"] = self._instance_name
+        if self.instance_name:
+            metadata["instance-name"] = self.instance_name
 
         seen: Set[str] = set()
         cursor = 0
         bytes_deleted = 0
 
         while n_bytes > 0:
             # Maybe count should be configurable or somehow self-tuning
@@ -259,29 +259,29 @@
                 return pipe.execute()
 
             raw_ttls = self._redis.execute_ro(get_ttls)
             ttls = [int(x) for x in raw_ttls]
 
             LOGGER.debug(f"scan returned {len(ttls)} keys")
             digests_to_delete: List[Digest] = []
+            failed_deletes: List[str] = []
             for key, ttl in zip(keys, ttls):
                 # Since FMB sets the ttl to self._ttl on every call we can
                 # use the time remaining to figure out when the last FMB
                 # call for that blob was.
                 blob_time = now - (self._ttl - timedelta(seconds=ttl))
                 if n_bytes <= 0:
                     break
 
                 digest = self._deconstruct_key(key)
                 if digest and (blob_time <= threshold_time) and (digest.hash not in seen):
                     n_bytes -= digest.size_bytes
                     digests_to_delete.append(digest)
 
             if digests_to_delete:
-                failed_deletes = []
                 if dry_run:
                     LOGGER.debug(f"Would delete {len(digests_to_delete)} digests")
                 else:
                     LOGGER.debug(f"Deleting {len(digests_to_delete)} digests")
                     failed_deletes = self.bulk_delete(digests_to_delete)
                     publish_counter_metric(
                         CLEANUP_STORAGE_DELETION_FAILURES_METRIC_NAME, len(failed_deletes), metadata
```

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/index/sql.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/index/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import itertools
 import logging
 import time
 from collections import deque
 from datetime import datetime, timedelta
 from typing import IO, Any, Deque, Dict, Iterator, List, Optional, Sequence, Tuple, cast
 
-from sqlalchemy import Column, and_, delete, func, select, text
+from sqlalchemy import Column, and_, delete, func, not_, select, text
 from sqlalchemy.exc import DBAPIError
 from sqlalchemy.orm import Session, load_only
 from sqlalchemy.orm.exc import StaleDataError
 from sqlalchemy.orm.query import Query
 from sqlalchemy.orm.session import Session as SessionType
 from sqlalchemy.sql.elements import BooleanClauseList
 
@@ -262,15 +262,17 @@
         """
         for part_start in range(0, len(digests), self._inclause_limit):
             part_end = min(len(digests), part_start + self._inclause_limit)
             part_digests = itertools.islice(digests, part_start, part_end)
             yield map(lambda digest: digest.hash, part_digests)
 
     @generator_method_duration_metric(CAS_INDEX_BULK_SELECT_DIGEST_TIME_METRIC_NAME)
-    def _bulk_select_digests(self, digests: Sequence[Digest], fetch_blobs: bool = False) -> Iterator[IndexEntry]:
+    def _bulk_select_digests(
+        self, digests: Sequence[Digest], fetch_blobs: bool = False, fetch_deleted: bool = True
+    ) -> Iterator[IndexEntry]:
         """Generator that selects all rows matching a digest list.
 
         SQLAlchemy Core is used for this because the ORM has problems with
         large numbers of bind variables for WHERE IN clauses.
 
         We only select on the digest hash (not hash and size) to allow for
         index-only queries on db backends that support them.
@@ -278,14 +280,16 @@
         index_table = IndexEntry.__table__
         with self._sql.scoped_session() as session:
             columns = [index_table.c.digest_hash]
             if fetch_blobs:
                 columns.append(index_table.c.inline_blob)
             for part in self._partitioned_hashes(digests):
                 stmt = select(columns).where(index_table.c.digest_hash.in_(part))
+                if not fetch_deleted:
+                    stmt = stmt.where(not_(index_table.c.deleted))
                 entries = session.execute(stmt)
                 yield from entries  # type: ignore
 
     @DurationMetric(CAS_INDEX_BULK_TIMESTAMP_UPDATE_TIME_METRIC_NAME, instanced=True)
     def _bulk_refresh_timestamps(
         self, digests: Sequence[Digest], session: SessionType, update_time: Optional[datetime] = None
     ) -> None:
@@ -327,15 +331,16 @@
                 )
                 .values(accessed_timestamp=timestamp)
             )
             session.execute(stmt)
             session.commit()
 
     def missing_blobs(self, digests: List[Digest]) -> List[Digest]:
-        entries = self._bulk_select_digests(digests)
+        # Blobs marked as deleted are considered as missing
+        entries = self._bulk_select_digests(digests, fetch_deleted=False)
 
         found_hashes = {entry.digest_hash for entry in entries}
 
         # Split the digests into two found/missing lists
         found_digests, missing_digests = [], []
         for digest in digests:
             if digest.hash in found_hashes:
@@ -379,14 +384,15 @@
         # Map digests to new entries
         entries_not_present = {
             digest.hash: {
                 "digest_hash": digest.hash,
                 "digest_size_bytes": digest.size_bytes,
                 "accessed_timestamp": update_time,
                 "inline_blob": (blob if digest.size_bytes <= self._max_inline_blob_size else None),
+                "deleted": False,
             }
             for (digest, blob) in digest_blob_pairs
         }
 
         entries_present = {}
         for entry in entries:
             entries_present[entry.digest_hash] = entries_not_present[entry.digest_hash]
```

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,22 +39,24 @@
         update_time = datetime.utcnow()
         new_rows = [
             {
                 "digest_hash": digest.hash,
                 "digest_size_bytes": digest.size_bytes,
                 "accessed_timestamp": update_time,
                 "inline_blob": (blob if digest.size_bytes <= max_inline_blob_size else None),
+                "deleted": False,
             }
             for (digest, blob) in digest_blob_pairs
         ]
 
         base_insert_stmt = insert(index_table).values(new_rows)
 
         update_stmt = base_insert_stmt.on_conflict_do_update(
             index_elements=["digest_hash"],
             set_={
                 "accessed_timestamp": update_time,
                 "inline_blob": coalesce(base_insert_stmt.excluded.inline_blob, index_table.c.inline_blob),
+                "deleted": False,
             },
         )
 
         session.execute(update_stmt)
```

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,22 +39,24 @@
         update_time = datetime.utcnow()
         new_rows = [
             {
                 "digest_hash": digest.hash,
                 "digest_size_bytes": digest.size_bytes,
                 "accessed_timestamp": update_time,
                 "inline_blob": (blob if digest.size_bytes <= max_inline_blob_size else None),
+                "deleted": False,
             }
             for (digest, blob) in digest_blob_pairs
         ]
 
         base_insert_stmt = insert(index_table).values(new_rows)
 
         update_stmt = base_insert_stmt.on_conflict_do_update(
             index_elements=["digest_hash"],
             set_={
                 "accessed_timestamp": update_time,
                 "inline_blob": coalesce(base_insert_stmt.excluded.inline_blob, index_table.c.inline_blob),
+                "deleted": False,
             },
         )
 
         session.execute(update_stmt)
```

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/lru_memory_cache.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/lru_memory_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/redis.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/redis.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/remote.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/remote.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/replicated.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/replicated.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/s3.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/s3.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/sharded.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/sharded.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/size_differentiated.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/size_differentiated.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/sql.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/sql.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/storage_abc.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/storage_abc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/cas/storage/with_cache.py` & `buildgrid-0.0.97/buildgrid/server/cas/storage/with_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/context.py` & `buildgrid-0.0.97/buildgrid/server/context.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/controller.py` & `buildgrid-0.0.97/buildgrid/server/controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,19 +39,24 @@
         self,
         scheduler: SQLDataStore,
         *,
         operation_stream_keepalive_timeout: Optional[int] = None,
         services: Iterable[str] = ServiceName.default_services(),
         max_list_operations_page_size: int = DEFAULT_MAX_LIST_OPERATION_PAGE_SIZE,
         job_assignment_interval: float = 1.0,
+        priority_assignment_percentage: int = 100,
     ) -> None:
         self.execution_instance: Optional[ExecutionInstance] = None
         if ServiceName.EXECUTION.value in services:
             self.execution_instance = ExecutionInstance(scheduler, operation_stream_keepalive_timeout)
 
         self.operations_instance: Optional[OperationsInstance] = None
         if ServiceName.OPERATIONS.value in services:
             self.operations_instance = OperationsInstance(scheduler, max_list_operations_page_size)
 
         self.bots_interface: Optional[BotsInterface] = None
         if ServiceName.BOTS.value in services:
-            self.bots_interface = BotsInterface(scheduler, job_assignment_interval=job_assignment_interval)
+            self.bots_interface = BotsInterface(
+                scheduler,
+                job_assignment_interval=job_assignment_interval,
+                priority_assignment_percentage=priority_assignment_percentage,
+            )
```

### Comparing `buildgrid-0.0.96/buildgrid/server/execution/__init__.py` & `buildgrid-0.0.97/buildgrid/server/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/execution/instance.py` & `buildgrid-0.0.97/buildgrid/server/execution/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/execution/service.py` & `buildgrid-0.0.97/buildgrid/server/execution/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/job_metrics.py` & `buildgrid-0.0.97/buildgrid/server/job_metrics.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/metrics_names.py` & `buildgrid-0.0.97/buildgrid/server/metrics_names.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/metrics_utils.py` & `buildgrid-0.0.97/buildgrid/server/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/monitoring.py` & `buildgrid-0.0.97/buildgrid/server/monitoring.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/operations/__init__.py` & `buildgrid-0.0.97/buildgrid/server/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/operations/filtering/__init__.py` & `buildgrid-0.0.97/buildgrid/server/operations/filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/operations/filtering/filter.py` & `buildgrid-0.0.97/buildgrid/server/operations/filtering/filter.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/operations/filtering/filter_grammar.lark` & `buildgrid-0.0.97/buildgrid/server/operations/filtering/filter_grammar.lark`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/operations/filtering/interpreter.py` & `buildgrid-0.0.97/buildgrid/server/operations/filtering/interpreter.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/operations/filtering/parser.py` & `buildgrid-0.0.97/buildgrid/server/operations/filtering/parser.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/operations/filtering/sanitizer.py` & `buildgrid-0.0.97/buildgrid/server/operations/filtering/sanitizer.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/operations/instance.py` & `buildgrid-0.0.97/buildgrid/server/operations/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/operations/service.py` & `buildgrid-0.0.97/buildgrid/server/operations/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/__init__.py` & `buildgrid-0.0.97/buildgrid/server/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/__init__.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/env.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/env.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/script.py.mako` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/impl.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -867,32 +867,48 @@
             return {}
 
         # This is only updated within the metrics asyncio loop; no race conditions
         self._last_scheduler_metrics_publish_time = datetime.utcnow()
 
         return metrics
 
-    @DurationMetric(BOTS_ASSIGN_JOB_LEASES_TIME_METRIC_NAME, instanced=True)
-    def assign_n_leases(
-        self,
-        *,
-        capability_hash: str,
-        bot_names: List[str],
-    ) -> List[str]:
-        job_statement = (
+    def _queued_jobs_by_capability(self, capability_hash: str) -> Select:
+        return (
             select(JobEntry)
             .with_for_update(skip_locked=True)
             .where(
                 JobEntry.assigned != True,  # noqa: E712
                 self._job_in_instance(),
                 JobEntry.platform_requirements == capability_hash,
                 JobEntry.stage == OperationStage.QUEUED.value,
             )
-            .order_by(JobEntry.priority, JobEntry.queued_timestamp)
         )
+
+    def assign_n_leases_by_priority(
+        self,
+        *,
+        capability_hash: str,
+        bot_names: List[str],
+    ) -> List[str]:
+        job_statement = self._queued_jobs_by_capability(capability_hash).order_by(
+            JobEntry.priority, JobEntry.queued_timestamp
+        )
+        return self._assign_n_leases(job_statement=job_statement, bot_names=bot_names)
+
+    def assign_n_leases_by_age(
+        self,
+        *,
+        capability_hash: str,
+        bot_names: List[str],
+    ) -> List[str]:
+        job_statement = self._queued_jobs_by_capability(capability_hash).order_by(JobEntry.queued_timestamp)
+        return self._assign_n_leases(job_statement=job_statement, bot_names=bot_names)
+
+    @DurationMetric(BOTS_ASSIGN_JOB_LEASES_TIME_METRIC_NAME, instanced=True)
+    def _assign_n_leases(self, *, job_statement: Select, bot_names: List[str]) -> List[str]:
         bot_statement = (
             select(BotEntry)
             .with_for_update(skip_locked=True)
             .where(
                 BotEntry.lease_id.is_(None),
                 self._bot_in_instance(),
                 BotEntry.name.in_(bot_names),
```

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/models.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/models.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/notifier.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/notifier.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/persistence/sql/utils.py` & `buildgrid-0.0.97/buildgrid/server/persistence/sql/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/redis/__init__.py` & `buildgrid-0.0.97/buildgrid/server/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/redis/provider.py` & `buildgrid-0.0.97/buildgrid/server/redis/provider.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/request_metadata_utils.py` & `buildgrid-0.0.97/buildgrid/server/request_metadata_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/s3/__init__.py` & `buildgrid-0.0.97/buildgrid/server/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/s3/s3utils.py` & `buildgrid-0.0.97/buildgrid/server/s3/s3utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/server.py` & `buildgrid-0.0.97/buildgrid/server/server.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/servicer.py` & `buildgrid-0.0.97/buildgrid/server/servicer.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/sql/__init__.py` & `buildgrid-0.0.97/buildgrid/server/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/sql/provider.py` & `buildgrid-0.0.97/buildgrid/server/sql/provider.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/sql/sqlutils.py` & `buildgrid-0.0.97/buildgrid/server/sql/sqlutils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/threading.py` & `buildgrid-0.0.97/buildgrid/server/threading.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/utils/__init__.py` & `buildgrid-0.0.97/buildgrid/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/utils/async_lru_cache.py` & `buildgrid-0.0.97/buildgrid/server/utils/async_lru_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/utils/context.py` & `buildgrid-0.0.97/buildgrid/server/utils/context.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/server/utils/decorators.py` & `buildgrid-0.0.97/buildgrid/server/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/settings.py` & `buildgrid-0.0.97/buildgrid/settings.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid/utils.py` & `buildgrid-0.0.97/buildgrid/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid.egg-info/PKG-INFO` & `buildgrid-0.0.97/buildgrid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildgrid
-Version: 0.0.96
+Version: 0.0.97
 Summary: A remote execution service
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://buildgrid.build
 Project-URL: Documentation, https://buildgrid.build
 Project-URL: Repository, https://gitlab.com/BuildGrid/buildgrid
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `buildgrid-0.0.96/buildgrid.egg-info/SOURCES.txt` & `buildgrid-0.0.97/buildgrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/buildgrid.egg-info/requires.txt` & `buildgrid-0.0.97/buildgrid.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/all-in-one.yml` & `buildgrid-0.0.97/data/config/all-in-one.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/artifacts.yml` & `buildgrid-0.0.97/data/config/artifacts.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/basic-with-disk.yml` & `buildgrid-0.0.97/data/config/basic-with-disk.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/bots-interface.yml` & `buildgrid-0.0.97/data/config/bots-interface.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/cache.yml` & `buildgrid-0.0.97/data/config/cache.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/controller.yml` & `buildgrid-0.0.97/data/config/controller.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/default.yml` & `buildgrid-0.0.97/data/config/default.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/index-sqlite-no-execution.yml` & `buildgrid-0.0.97/data/config/index-sqlite-no-execution.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/index-sqlite.yml` & `buildgrid-0.0.97/data/config/index-sqlite.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/monitoring-controller.yml` & `buildgrid-0.0.97/data/config/monitoring-controller.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/multi-layer-storage.yml` & `buildgrid-0.0.97/data/config/multi-layer-storage.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/redis-cache.yml` & `buildgrid-0.0.97/data/config/redis-cache.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/s3-indexed-cas.yml` & `buildgrid-0.0.97/data/config/s3-indexed-cas.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/storage-redis.yml` & `buildgrid-0.0.97/data/config/storage-redis.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/storage-s3.yml` & `buildgrid-0.0.97/data/config/storage-s3.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/storage.yml` & `buildgrid-0.0.97/data/config/storage.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/with-metering.yml` & `buildgrid-0.0.97/data/config/with-metering.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/data/config/with-pgbouncer.yml` & `buildgrid-0.0.97/data/config/with-pgbouncer.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/docs/Makefile` & `buildgrid-0.0.97/docs/Makefile`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/docs/source/data/execution-and-bots.yml` & `buildgrid-0.0.97/docs/source/data/execution-and-bots.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/docs/source/data/sqlite-index-cas-only.yml` & `buildgrid-0.0.97/docs/source/data/sqlite-index-cas-only.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/docs/source/index.rst` & `buildgrid-0.0.97/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/pyproject.toml` & `buildgrid-0.0.97/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "setuptools >= 44",
     "wheel >= 0.35",
 ]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "buildgrid"
-version = "0.0.96"
+version = "0.0.97"
 requires-python = ">=3.8"
 description = "A remote execution service"
 readme = "README.rst"
 license = {text = "Apache License, Version 2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
```

### Comparing `buildgrid-0.0.96/setup.cfg` & `buildgrid-0.0.97/setup.cfg`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/setup.py` & `buildgrid-0.0.97/setup.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/tests/auth/data/auth.yaml` & `buildgrid-0.0.97/tests/auth/data/auth.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/tests/auth/data/jwt-rs256-jwk-encrypted.token` & `buildgrid-0.0.97/tests/auth/data/jwt-rs256-jwk-encrypted.token`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/tests/auth/data/jwt-rs256-matching.priv.key` & `buildgrid-0.0.97/tests/auth/data/jwt-rs256-matching.priv.key`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/tests/test_async_lru_cache.py` & `buildgrid-0.0.97/tests/test_async_lru_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/tests/test_execution_instance.py` & `buildgrid-0.0.97/tests/test_execution_instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/tests/test_job_assigner.py` & `buildgrid-0.0.97/tests/test_job_assigner.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/tests/test_metrics_utils.py` & `buildgrid-0.0.97/tests/test_metrics_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/tests/test_mirrored_cache.py` & `buildgrid-0.0.97/tests/test_mirrored_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/tests/test_multithreaded_metrics.py` & `buildgrid-0.0.97/tests/test_multithreaded_metrics.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/tests/test_parser.py` & `buildgrid-0.0.97/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/tests/test_request_metadata_utils.py` & `buildgrid-0.0.97/tests/test_request_metadata_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.96/tests/test_scheduler.py` & `buildgrid-0.0.97/tests/test_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,15 @@
         action_digest=uncacheable_action_digest if do_not_cache else action_digest,
         command=command,
         platform_requirements={},
         priority=0,
         skip_cache_lookup=skip_cache_lookup,
         request_metadata=request_metadata,
     )
-    scheduler.assign_n_leases(capability_hash=hash_from_dict({}), bot_names=[bot_name])
+    scheduler.assign_n_leases_by_priority(capability_hash=hash_from_dict({}), bot_names=[bot_name])
     job_name = scheduler.get_operation_job_name(operation_name)
     return bot_name, bot_id, operation_name, job_name
 
 
 @pytest.mark.parametrize("monitoring", [True, False])
 def test_update_lease_state(controller, context, monitoring, push_service: MockAssetPushServicer):
     scheduler = controller.execution_instance.scheduler
@@ -287,15 +287,15 @@
     with scheduler._sql.session() as session:
         job = scheduler._get_job(job_name, session)
         assert job.n_tries == 1
         assert job.stage == OperationStage.QUEUED.value
 
     scheduler.close_bot_sessions(bot_name)
     bot_name = scheduler.add_bot_entry(bot_session_id=bot_id, bot_session_status=BotStatus.OK.value)
-    scheduler.assign_n_leases(capability_hash=hash_from_dict({}), bot_names=[bot_name])
+    scheduler.assign_n_leases_by_priority(capability_hash=hash_from_dict({}), bot_names=[bot_name])
 
     with scheduler._sql.session() as session:
         job = scheduler._get_job(job_name, session)
         assert job.n_tries == 2
         assert job.stage == OperationStage.QUEUED.value
 
     scheduler.close_bot_sessions(bot_name)
@@ -332,15 +332,15 @@
     bot_name = scheduler.add_bot_entry(bot_session_id=bot_id, bot_session_status=BotStatus.OK.value)
 
     with scheduler._sql.session() as session:
         job = scheduler._get_job(job_name, session)
         assert job.leases[0].worker_name is None
         assert job.stage == OperationStage.QUEUED.value
 
-    scheduler.assign_n_leases(capability_hash=hash_from_dict({}), bot_names=[bot_name])
+    scheduler.assign_n_leases_by_priority(capability_hash=hash_from_dict({}), bot_names=[bot_name])
 
     with scheduler._sql.session() as session:
         job = scheduler._get_job(job_name, session)
         assert job.leases[0].worker_name is not None
         assert job.stage == OperationStage.QUEUED.value
 
 
@@ -730,22 +730,22 @@
     with pytest.raises(InvalidArgumentError):
         scheduler_b.synchronize_bot_lease(bot_name, bot_id, BotStatus.OK.value, None)
 
     scheduler_a.close_bot_sessions(bot_name)
     bot_name = scheduler_a.add_bot_entry(bot_session_id=bot_id, bot_session_status=BotStatus.OK.value)
 
     # Attempt to assign leases from the instance which didn't get the job
-    scheduler_b.assign_n_leases(capability_hash=hash_from_dict({}), bot_names=[bot_name])
+    scheduler_b.assign_n_leases_by_priority(capability_hash=hash_from_dict({}), bot_names=[bot_name])
 
     # Check that the job is unaffected
     lease = scheduler_a.synchronize_bot_lease(bot_name, bot_id, BotStatus.OK.value, None)
     assert lease is None
 
     # Attempt to assign leases from the instance which did get the job
-    scheduler_a.assign_n_leases(capability_hash=hash_from_dict({}), bot_names=[bot_name])
+    scheduler_a.assign_n_leases_by_priority(capability_hash=hash_from_dict({}), bot_names=[bot_name])
 
     # This time the job should have a lease
     lease = scheduler_a.synchronize_bot_lease(bot_name, bot_id, BotStatus.OK.value, None)
     assert lease.state == LeaseState.PENDING.value
 
 
 def test_isolated_instances_list_operations(isolated_controllers):
```

### Comparing `buildgrid-0.0.96/tests/test_utils.py` & `buildgrid-0.0.97/tests/test_utils.py`

 * *Files identical despite different names*

