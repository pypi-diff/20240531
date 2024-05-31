# Comparing `tmp/hgitaly-1.6.0.tar.gz` & `tmp/hgitaly-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgitaly-1.6.0.tar", last modified: Wed May 22 11:16:33 2024, max compression
+gzip compressed data, was "hgitaly-1.7.0.tar", last modified: Fri May 31 16:20:54 2024, max compression
```

## Comparing `hgitaly-1.6.0.tar` & `hgitaly-1.7.0.tar`

### file list

```diff
@@ -1,178 +1,179 @@
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.834704 hgitaly-1.6.0/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18092 2022-09-23 11:31:54.000000 hgitaly-1.6.0/LICENSE
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       33 2022-09-23 11:31:54.000000 hgitaly-1.6.0/MANIFEST.in
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15668 2024-05-22 11:16:33.833704 hgitaly-1.6.0/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15287 2024-03-07 11:59:14.000000 hgitaly-1.6.0/README.md
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.771703 hgitaly-1.6.0/hgext3rd/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      157 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgext3rd/__init__.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.772703 hgitaly-1.6.0/hgext3rd/hgitaly/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4418 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgext3rd/hgitaly/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1551 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgext3rd/hgitaly/revset.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.772703 hgitaly-1.6.0/hgext3rd/hgitaly/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgext3rd/hgitaly/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2021 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgext3rd/hgitaly/tests/test_revset.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5392 2023-02-11 11:25:44.000000 hgitaly-1.6.0/hgext3rd/hgitaly/tests/test_serve.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.785703 hgitaly-1.6.0/hgitaly/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        6 2024-05-22 11:16:03.000000 hgitaly-1.6.0/hgitaly/VERSION
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      361 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    13506 2023-07-30 07:54:28.000000 hgitaly-1.6.0/hgitaly/branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      744 2023-11-18 14:23:07.000000 hgitaly-1.6.0/hgitaly/changelog.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    13280 2024-03-25 19:47:19.000000 hgitaly-1.6.0/hgitaly/diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4985 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/errors.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2749 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgitaly/feature.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5607 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/file_content.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      701 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/file_context.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4495 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/git.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7133 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/gitlab_ref.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.787703 hgitaly-1.6.0/hgitaly/license_detector/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4650 2023-12-12 12:58:20.000000 hgitaly-1.6.0/hgitaly/license_detector/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)   270608 2023-12-12 12:58:20.000000 hgitaly-1.6.0/hgitaly/license_detector/spdx-licenses.json
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.790703 hgitaly-1.6.0/hgitaly/linguist/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6420 2023-09-25 08:12:33.000000 hgitaly-1.6.0/hgitaly/linguist/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)   122122 2023-09-25 08:12:33.000000 hgitaly-1.6.0/hgitaly/linguist/languages.json
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1183 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgitaly/logging.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10350 2023-09-25 08:37:11.000000 hgitaly-1.6.0/hgitaly/manifest.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9596 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/message.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1506 2024-03-25 19:47:19.000000 hgitaly-1.6.0/hgitaly/oid.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      953 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/pagination.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1010 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/path.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3252 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/peer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      711 2023-05-03 12:26:53.000000 hgitaly-1.6.0/hgitaly/procutil.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7973 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7891 2024-01-05 19:34:28.000000 hgitaly-1.6.0/hgitaly/revision.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5689 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgitaly/revset.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.793703 hgitaly-1.6.0/hgitaly/server/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      417 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/server/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1683 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/server/address.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6288 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/server/mono.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7216 2023-05-03 12:26:53.000000 hgitaly-1.6.0/hgitaly/server/prefork.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.795704 hgitaly-1.6.0/hgitaly/server/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/server/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1256 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/server/tests/test_address.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3272 2023-05-03 12:26:53.000000 hgitaly-1.6.0/hgitaly/server/tests/test_mono.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6502 2023-02-11 11:25:44.000000 hgitaly-1.6.0/hgitaly/server/tests/test_prefork.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3704 2023-02-11 11:25:44.000000 hgitaly-1.6.0/hgitaly/server/tests/test_worker.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3748 2023-02-11 11:25:44.000000 hgitaly-1.6.0/hgitaly/server/worker.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.799703 hgitaly-1.6.0/hgitaly/service/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/service/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1787 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/service/analysis.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5013 2023-09-25 08:12:33.000000 hgitaly-1.6.0/hgitaly/service/blob.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    47634 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/service/commit.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    25147 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/service/diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2217 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgitaly/service/interceptors.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1954 2022-10-27 17:19:53.000000 hgitaly-1.6.0/hgitaly/service/mercurial_changeset.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    16868 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/service/mercurial_operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7480 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgitaly/service/mercurial_repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9852 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/service/operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    23474 2024-03-25 19:49:12.000000 hgitaly-1.6.0/hgitaly/service/ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    33242 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/service/repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      769 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgitaly/service/server.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.806704 hgitaly-1.6.0/hgitaly/service/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/service/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7380 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/service/tests/fixture.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3972 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/service/tests/test_analysis.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4628 2023-09-25 08:12:33.000000 hgitaly-1.6.0/hgitaly/service/tests/test_blob.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    53225 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/service/tests/test_commit.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2020 2023-12-12 12:58:20.000000 hgitaly-1.6.0/hgitaly/service/tests/test_default_branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    26417 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/service/tests/test_diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2973 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/service/tests/test_mercurial_changeset.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    22959 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/service/tests/test_mercurial_operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18968 2024-01-07 12:13:06.000000 hgitaly-1.6.0/hgitaly/service/tests/test_mercurial_repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10594 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/service/tests/test_operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    22409 2024-03-25 19:49:12.000000 hgitaly-1.6.0/hgitaly/service/tests/test_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    45598 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/service/tests/test_repository_service.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      721 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/service/tests/test_server.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17084 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/servicer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1331 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/ssh.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5895 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/stream.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.819704 hgitaly-1.6.0/hgitaly/stub/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/stub/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2812 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/stub/analysis_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3419 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/stub/analysis_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9342 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/stub/blob_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    12934 2024-01-05 19:34:28.000000 hgitaly-1.6.0/hgitaly/stub/blob_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32146 2024-03-25 19:47:19.000000 hgitaly-1.6.0/hgitaly/stub/commit_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    39150 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/commit_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18818 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/stub/diff_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17269 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/stub/diff_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6477 2024-03-25 19:47:19.000000 hgitaly-1.6.0/hgitaly/stub/errors_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2022-10-27 17:19:53.000000 hgitaly-1.6.0/hgitaly/stub/errors_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2922 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/lint_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/stub/lint_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4218 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/mercurial_changeset_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2901 2022-10-27 17:19:53.000000 hgitaly-1.6.0/hgitaly/stub/mercurial_changeset_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7531 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/mercurial_operations_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7995 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/mercurial_operations_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    11048 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/mercurial_repository_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17065 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/mercurial_repository_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29692 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/stub/operations_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32883 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/operations_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    20829 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/stub/ref_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29202 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/stub/ref_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    45594 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/stub/repository_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    76171 2024-05-22 11:15:45.000000 hgitaly-1.6.0/hgitaly/stub/repository_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5080 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/server_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7231 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/server_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5996 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/stub/shared_pb2.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/stub/shared_pb2_grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1653 2023-07-30 07:54:28.000000 hgitaly-1.6.0/hgitaly/tag.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.821704 hgitaly-1.6.0/hgitaly/testing/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      317 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/testing/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1278 2023-02-11 11:25:44.000000 hgitaly-1.6.0/hgitaly/testing/bundle.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2828 2024-01-05 19:34:28.000000 hgitaly-1.6.0/hgitaly/testing/context.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      901 2023-05-03 12:26:53.000000 hgitaly-1.6.0/hgitaly/testing/grpc.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1147 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/testing/ssh.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3920 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/testing/sshd.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.821704 hgitaly-1.6.0/hgitaly/testing/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/testing/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1191 2024-01-07 12:13:06.000000 hgitaly-1.6.0/hgitaly/testing/tests/test_sshd.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.827704 hgitaly-1.6.0/hgitaly/tests/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/tests/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4609 2024-01-05 19:34:28.000000 hgitaly-1.6.0/hgitaly/tests/common.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9403 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/tests/test_branch.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3605 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/tests/test_diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3778 2024-02-09 22:39:22.000000 hgitaly-1.6.0/hgitaly/tests/test_errors.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2406 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgitaly/tests/test_feature.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1439 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/tests/test_file_context.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4932 2024-05-20 13:45:10.000000 hgitaly-1.6.0/hgitaly/tests/test_gitlab_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1495 2023-12-12 12:58:20.000000 hgitaly-1.6.0/hgitaly/tests/test_license_detector.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1547 2023-12-12 12:58:20.000000 hgitaly-1.6.0/hgitaly/tests/test_linguist.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5582 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/tests/test_manifest.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3374 2023-02-11 11:25:44.000000 hgitaly-1.6.0/hgitaly/tests/test_messages.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1114 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/tests/test_oid.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1669 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/tests/test_peer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      582 2023-03-21 12:09:38.000000 hgitaly-1.6.0/hgitaly/tests/test_repository.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6392 2023-03-23 14:16:22.000000 hgitaly-1.6.0/hgitaly/tests/test_revision.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      679 2023-02-11 11:25:44.000000 hgitaly-1.6.0/hgitaly/tests/test_revset.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10160 2024-01-05 19:34:28.000000 hgitaly-1.6.0/hgitaly/tests/test_servicer.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1951 2024-03-07 11:59:14.000000 hgitaly-1.6.0/hgitaly/tests/test_stream.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1315 2022-09-23 11:31:54.000000 hgitaly-1.6.0/hgitaly/tests/test_tag.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    24221 2024-01-05 19:34:28.000000 hgitaly-1.6.0/hgitaly/tests/test_workdir.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2017 2023-09-25 08:12:33.000000 hgitaly-1.6.0/hgitaly/util.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    14533 2024-01-05 19:34:28.000000 hgitaly-1.6.0/hgitaly/workdir.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.786703 hgitaly-1.6.0/hgitaly.egg-info/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15668 2024-05-22 11:16:33.000000 hgitaly-1.6.0/hgitaly.egg-info/PKG-INFO
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4680 2024-05-22 11:16:33.000000 hgitaly-1.6.0/hgitaly.egg-info/SOURCES.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2024-05-22 11:16:33.000000 hgitaly-1.6.0/hgitaly.egg-info/dependency_links.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      151 2024-05-22 11:16:33.000000 hgitaly-1.6.0/hgitaly.egg-info/requires.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       35 2024-05-22 11:16:33.000000 hgitaly-1.6.0/hgitaly.egg-info/top_level.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      151 2024-02-09 22:39:22.000000 hgitaly-1.6.0/install-requirements.txt
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2024-05-22 11:16:33.834704 hgitaly-1.6.0/setup.cfg
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      968 2023-12-12 12:58:20.000000 hgitaly-1.6.0/setup.py
-drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-22 11:16:33.833704 hgitaly-1.6.0/tests_with_gitaly/
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2437 2023-07-05 15:04:47.000000 hgitaly-1.6.0/tests_with_gitaly/__init__.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    24858 2024-05-22 11:15:45.000000 hgitaly-1.6.0/tests_with_gitaly/comparison.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3545 2023-05-03 12:26:53.000000 hgitaly-1.6.0/tests_with_gitaly/conftest.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2455 2023-07-05 15:04:47.000000 hgitaly-1.6.0/tests_with_gitaly/gitaly.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1775 2023-05-03 12:26:53.000000 hgitaly-1.6.0/tests_with_gitaly/hgitaly_rhgitaly_comparison.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2509 2024-03-10 13:55:24.000000 hgitaly-1.6.0/tests_with_gitaly/rhgitaly.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    25541 2024-05-22 11:15:45.000000 hgitaly-1.6.0/tests_with_gitaly/test_blob_tree.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    34125 2024-05-20 13:45:11.000000 hgitaly-1.6.0/tests_with_gitaly/test_commit.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3284 2023-07-05 15:04:47.000000 hgitaly-1.6.0/tests_with_gitaly/test_comparison.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29596 2024-03-25 19:47:19.000000 hgitaly-1.6.0/tests_with_gitaly/test_diff.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1371 2022-10-27 17:19:53.000000 hgitaly-1.6.0/tests_with_gitaly/test_gitaly_server.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    11653 2024-02-09 22:39:22.000000 hgitaly-1.6.0/tests_with_gitaly/test_operations.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17745 2024-03-25 19:49:12.000000 hgitaly-1.6.0/tests_with_gitaly/test_ref.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29926 2024-05-22 11:15:45.000000 hgitaly-1.6.0/tests_with_gitaly/test_repository_service.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      941 2023-05-03 12:26:53.000000 hgitaly-1.6.0/tests_with_gitaly/test_rhgitaly_server.py
--rw-r--r--   0 gracinet  (1000) gracinet  (1000)      820 2023-05-03 12:26:53.000000 hgitaly-1.6.0/tests_with_gitaly/test_server.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-31 16:20:54.908607 hgitaly-1.7.0/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18092 2024-05-28 10:18:12.000000 hgitaly-1.7.0/LICENSE
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       33 2024-05-28 10:18:12.000000 hgitaly-1.7.0/MANIFEST.in
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15954 2024-05-31 16:20:54.908607 hgitaly-1.7.0/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15287 2024-05-28 10:18:12.000000 hgitaly-1.7.0/README.md
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-31 16:20:54.866608 hgitaly-1.7.0/hgext3rd/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      157 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgext3rd/__init__.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-31 16:20:54.866608 hgitaly-1.7.0/hgext3rd/hgitaly/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4418 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgext3rd/hgitaly/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1551 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgext3rd/hgitaly/revset.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-31 16:20:54.867608 hgitaly-1.7.0/hgext3rd/hgitaly/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgext3rd/hgitaly/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2021 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgext3rd/hgitaly/tests/test_revset.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5392 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgext3rd/hgitaly/tests/test_serve.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-31 16:20:54.872608 hgitaly-1.7.0/hgitaly/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        6 2024-05-31 12:58:27.000000 hgitaly-1.7.0/hgitaly/VERSION
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      361 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    13506 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      744 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/changelog.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    13280 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4985 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/errors.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2749 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/feature.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5607 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/file_content.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      701 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/file_context.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4495 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/git.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7133 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/gitlab_ref.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-31 16:20:54.874608 hgitaly-1.7.0/hgitaly/license_detector/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4650 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/license_detector/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)   270608 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/license_detector/spdx-licenses.json
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-31 16:20:54.876608 hgitaly-1.7.0/hgitaly/linguist/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6420 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/linguist/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)   122122 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/linguist/languages.json
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1183 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/logging.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10350 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/manifest.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9596 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/message.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1506 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/oid.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      953 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/pagination.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1010 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/path.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3252 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/peer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      711 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/procutil.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7973 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7891 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/revision.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5689 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/revset.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-31 16:20:54.878608 hgitaly-1.7.0/hgitaly/server/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      417 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/server/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1683 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/server/address.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6288 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/server/mono.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7216 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/server/prefork.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-31 16:20:54.879608 hgitaly-1.7.0/hgitaly/server/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/server/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1256 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/server/tests/test_address.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3272 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/server/tests/test_mono.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6502 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/server/tests/test_prefork.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3704 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/server/tests/test_worker.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3748 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/server/worker.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-31 16:20:54.883608 hgitaly-1.7.0/hgitaly/service/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1787 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/analysis.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5013 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/blob.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    47634 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/commit.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    25147 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2217 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/interceptors.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1954 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/mercurial_changeset.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    16868 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/mercurial_operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7480 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/mercurial_repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9852 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    23474 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    33242 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      769 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/server.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-31 16:20:54.887608 hgitaly-1.7.0/hgitaly/service/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       17 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7380 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/tests/fixture.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3972 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/tests/test_analysis.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4628 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/tests/test_blob.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    53225 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/tests/test_commit.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2020 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/tests/test_default_branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    26417 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/tests/test_diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2973 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/tests/test_mercurial_changeset.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    22959 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/tests/test_mercurial_operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18968 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/tests/test_mercurial_repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10594 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/tests/test_operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    22409 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/tests/test_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    45598 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/tests/test_repository_service.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      721 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/service/tests/test_server.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17084 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/servicer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1331 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/ssh.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5895 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/stream.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-31 16:20:54.897608 hgitaly-1.7.0/hgitaly/stub/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        0 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/stub/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2812 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/analysis_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3419 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/analysis_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9342 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/blob_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    12934 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/blob_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32146 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/commit_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    39150 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/commit_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    18818 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/diff_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17269 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/diff_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6477 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/errors_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/errors_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2922 2024-05-31 12:59:16.000000 hgitaly-1.7.0/hgitaly/stub/lint_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2024-05-31 12:59:16.000000 hgitaly-1.7.0/hgitaly/stub/lint_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4218 2024-05-31 12:59:18.000000 hgitaly-1.7.0/hgitaly/stub/mercurial_changeset_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2901 2024-05-31 12:59:18.000000 hgitaly-1.7.0/hgitaly/stub/mercurial_changeset_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7531 2024-05-31 12:59:18.000000 hgitaly-1.7.0/hgitaly/stub/mercurial_operations_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7995 2024-05-31 12:59:18.000000 hgitaly-1.7.0/hgitaly/stub/mercurial_operations_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    11149 2024-05-31 12:59:18.000000 hgitaly-1.7.0/hgitaly/stub/mercurial_repository_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17065 2024-05-31 12:59:18.000000 hgitaly-1.7.0/hgitaly/stub/mercurial_repository_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29692 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/operations_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    32883 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/operations_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    20829 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/ref_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29202 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/ref_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    45594 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/repository_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    76171 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/repository_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5080 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/server_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     7231 2024-05-31 12:59:17.000000 hgitaly-1.7.0/hgitaly/stub/server_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5996 2024-05-31 12:59:16.000000 hgitaly-1.7.0/hgitaly/stub/shared_pb2.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      159 2024-05-31 12:59:16.000000 hgitaly-1.7.0/hgitaly/stub/shared_pb2_grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1653 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tag.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-31 16:20:54.898608 hgitaly-1.7.0/hgitaly/testing/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      317 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/testing/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1278 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/testing/bundle.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2828 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/testing/context.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      901 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/testing/grpc.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1147 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/testing/ssh.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3920 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/testing/sshd.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-31 16:20:54.899608 hgitaly-1.7.0/hgitaly/testing/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/testing/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1191 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/testing/tests/test_sshd.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-31 16:20:54.903607 hgitaly-1.7.0/hgitaly/tests/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      246 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4609 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/common.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     9403 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_branch.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3605 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3778 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_errors.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2406 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_feature.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1439 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_file_context.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4932 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_gitlab_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1495 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_license_detector.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1547 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_linguist.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     5582 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_manifest.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3374 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_messages.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1114 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_oid.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1669 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_peer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      582 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     6392 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_revision.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      679 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_revset.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    10160 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_servicer.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1951 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_stream.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1315 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_tag.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    24221 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/tests/test_workdir.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2017 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/util.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    14533 2024-05-28 10:18:12.000000 hgitaly-1.7.0/hgitaly/workdir.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-31 16:20:54.908607 hgitaly-1.7.0/hgitaly.egg-info/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    15954 2024-05-31 16:20:54.000000 hgitaly-1.7.0/hgitaly.egg-info/PKG-INFO
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4727 2024-05-31 16:20:54.000000 hgitaly-1.7.0/hgitaly.egg-info/SOURCES.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)        1 2024-05-31 16:20:54.000000 hgitaly-1.7.0/hgitaly.egg-info/dependency_links.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      151 2024-05-31 16:20:54.000000 hgitaly-1.7.0/hgitaly.egg-info/requires.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       35 2024-05-31 16:20:54.000000 hgitaly-1.7.0/hgitaly.egg-info/top_level.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      151 2024-05-28 10:18:12.000000 hgitaly-1.7.0/install-requirements.txt
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)       38 2024-05-31 16:20:54.908607 hgitaly-1.7.0/setup.cfg
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      968 2024-05-28 10:18:12.000000 hgitaly-1.7.0/setup.py
+drwxr-xr-x   0 gracinet  (1000) gracinet  (1000)        0 2024-05-31 16:20:54.907607 hgitaly-1.7.0/tests_with_gitaly/
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2437 2024-05-28 10:18:12.000000 hgitaly-1.7.0/tests_with_gitaly/__init__.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    24858 2024-05-30 17:39:59.000000 hgitaly-1.7.0/tests_with_gitaly/comparison.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4493 2024-05-31 11:53:36.000000 hgitaly-1.7.0/tests_with_gitaly/conftest.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     2455 2024-05-28 10:18:12.000000 hgitaly-1.7.0/tests_with_gitaly/gitaly.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4000 2024-05-31 11:53:36.000000 hgitaly-1.7.0/tests_with_gitaly/hgitaly_rhgitaly_comparison.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3246 2024-05-31 11:55:31.000000 hgitaly-1.7.0/tests_with_gitaly/rhgitaly.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    25541 2024-05-28 10:18:12.000000 hgitaly-1.7.0/tests_with_gitaly/test_blob_tree.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    34125 2024-05-28 10:18:12.000000 hgitaly-1.7.0/tests_with_gitaly/test_commit.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     3284 2024-05-28 10:18:12.000000 hgitaly-1.7.0/tests_with_gitaly/test_comparison.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29596 2024-05-28 10:18:12.000000 hgitaly-1.7.0/tests_with_gitaly/test_diff.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     1371 2024-05-28 10:18:12.000000 hgitaly-1.7.0/tests_with_gitaly/test_gitaly_server.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)     4106 2024-05-31 12:07:03.000000 hgitaly-1.7.0/tests_with_gitaly/test_mercurial_repository.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    11653 2024-05-28 10:18:12.000000 hgitaly-1.7.0/tests_with_gitaly/test_operations.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    17745 2024-05-28 10:18:12.000000 hgitaly-1.7.0/tests_with_gitaly/test_ref.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)    29926 2024-05-31 12:05:41.000000 hgitaly-1.7.0/tests_with_gitaly/test_repository_service.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      941 2024-05-28 10:18:12.000000 hgitaly-1.7.0/tests_with_gitaly/test_rhgitaly_server.py
+-rw-r--r--   0 gracinet  (1000) gracinet  (1000)      836 2024-05-31 11:53:36.000000 hgitaly-1.7.0/tests_with_gitaly/test_server.py
```

### Comparing `hgitaly-1.6.0/LICENSE` & `hgitaly-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/PKG-INFO` & `hgitaly-1.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: hgitaly
-Version: 1.6.0
-Summary: Server-side implementation of Gitaly protocol for Mercurial
-Home-page: https://foss.heptapod.net/heptapod/hgitaly
-Author: Georges Racinet
-Author-email: georges.racinet@octobus.net
-License: GPLv2+
-Keywords: hg mercurial heptapod gitlab
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # HGitaly
 
 HGitaly is Gitaly server for Mercurial.
 
 It implements the subset of the Gitaly gRPC protocol that is relevant for
 Mercurial repositories, as well as its own HGitaly protocol, with methods
 that are specific to Mercurial.
```

### Comparing `hgitaly-1.6.0/README.md` & `hgitaly-1.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: hgitaly
+Version: 1.7.0
+Summary: Server-side implementation of Gitaly protocol for Mercurial
+Home-page: https://foss.heptapod.net/heptapod/hgitaly
+Author: Georges Racinet
+Author-email: georges.racinet@octobus.net
+License: GPLv2+
+Keywords: hg mercurial heptapod gitlab
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: heptapod>=4.4.1dev0
+Requires-Dist: protobuf~=4.21.0
+Requires-Dist: grpcio~=1.58.0
+Requires-Dist: grpcio-status~=1.58.0
+Requires-Dist: grpc-interceptor
+Requires-Dist: hg-loggingmod
+Requires-Dist: psutil
+Requires-Dist: importlib_resources~=2.0.0
+Requires-Dist: spdx-lookup
+
 # HGitaly
 
 HGitaly is Gitaly server for Mercurial.
 
 It implements the subset of the Gitaly gRPC protocol that is relevant for
 Mercurial repositories, as well as its own HGitaly protocol, with methods
 that are specific to Mercurial.
```

### Comparing `hgitaly-1.6.0/hgext3rd/hgitaly/__init__.py` & `hgitaly-1.7.0/hgext3rd/hgitaly/__init__.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgext3rd/hgitaly/revset.py` & `hgitaly-1.7.0/hgext3rd/hgitaly/revset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgext3rd/hgitaly/tests/test_revset.py` & `hgitaly-1.7.0/hgext3rd/hgitaly/tests/test_revset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgext3rd/hgitaly/tests/test_serve.py` & `hgitaly-1.7.0/hgext3rd/hgitaly/tests/test_serve.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/branch.py` & `hgitaly-1.7.0/hgitaly/branch.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/changelog.py` & `hgitaly-1.7.0/hgitaly/changelog.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/diff.py` & `hgitaly-1.7.0/hgitaly/diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/errors.py` & `hgitaly-1.7.0/hgitaly/errors.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/feature.py` & `hgitaly-1.7.0/hgitaly/feature.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/file_content.py` & `hgitaly-1.7.0/hgitaly/file_content.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/file_context.py` & `hgitaly-1.7.0/hgitaly/file_context.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/git.py` & `hgitaly-1.7.0/hgitaly/git.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/gitlab_ref.py` & `hgitaly-1.7.0/hgitaly/gitlab_ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/license_detector/__init__.py` & `hgitaly-1.7.0/hgitaly/license_detector/__init__.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/license_detector/spdx-licenses.json` & `hgitaly-1.7.0/hgitaly/license_detector/spdx-licenses.json`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/linguist/__init__.py` & `hgitaly-1.7.0/hgitaly/linguist/__init__.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/linguist/languages.json` & `hgitaly-1.7.0/hgitaly/linguist/languages.json`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/logging.py` & `hgitaly-1.7.0/hgitaly/logging.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/manifest.py` & `hgitaly-1.7.0/hgitaly/manifest.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/message.py` & `hgitaly-1.7.0/hgitaly/message.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/oid.py` & `hgitaly-1.7.0/hgitaly/oid.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/pagination.py` & `hgitaly-1.7.0/hgitaly/pagination.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/path.py` & `hgitaly-1.7.0/hgitaly/path.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/peer.py` & `hgitaly-1.7.0/hgitaly/peer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/procutil.py` & `hgitaly-1.7.0/hgitaly/procutil.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/repository.py` & `hgitaly-1.7.0/hgitaly/repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/revision.py` & `hgitaly-1.7.0/hgitaly/revision.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/revset.py` & `hgitaly-1.7.0/hgitaly/revset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/server/address.py` & `hgitaly-1.7.0/hgitaly/server/address.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/server/mono.py` & `hgitaly-1.7.0/hgitaly/server/mono.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/server/prefork.py` & `hgitaly-1.7.0/hgitaly/server/prefork.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/server/tests/test_address.py` & `hgitaly-1.7.0/hgitaly/server/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/server/tests/test_mono.py` & `hgitaly-1.7.0/hgitaly/server/tests/test_mono.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/server/tests/test_prefork.py` & `hgitaly-1.7.0/hgitaly/server/tests/test_prefork.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/server/tests/test_worker.py` & `hgitaly-1.7.0/hgitaly/server/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/server/worker.py` & `hgitaly-1.7.0/hgitaly/server/worker.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/analysis.py` & `hgitaly-1.7.0/hgitaly/service/analysis.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/blob.py` & `hgitaly-1.7.0/hgitaly/service/blob.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/commit.py` & `hgitaly-1.7.0/hgitaly/service/commit.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/diff.py` & `hgitaly-1.7.0/hgitaly/service/diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/interceptors.py` & `hgitaly-1.7.0/hgitaly/service/interceptors.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/mercurial_changeset.py` & `hgitaly-1.7.0/hgitaly/service/mercurial_changeset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/mercurial_operations.py` & `hgitaly-1.7.0/hgitaly/service/mercurial_operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/mercurial_repository.py` & `hgitaly-1.7.0/hgitaly/service/mercurial_repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/operations.py` & `hgitaly-1.7.0/hgitaly/service/operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/ref.py` & `hgitaly-1.7.0/hgitaly/service/ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/repository.py` & `hgitaly-1.7.0/hgitaly/service/repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/server.py` & `hgitaly-1.7.0/hgitaly/service/server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/tests/fixture.py` & `hgitaly-1.7.0/hgitaly/service/tests/fixture.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/tests/test_analysis.py` & `hgitaly-1.7.0/hgitaly/service/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/tests/test_blob.py` & `hgitaly-1.7.0/hgitaly/service/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/tests/test_commit.py` & `hgitaly-1.7.0/hgitaly/service/tests/test_commit.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/tests/test_default_branch.py` & `hgitaly-1.7.0/hgitaly/service/tests/test_default_branch.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/tests/test_diff.py` & `hgitaly-1.7.0/hgitaly/service/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/tests/test_mercurial_changeset.py` & `hgitaly-1.7.0/hgitaly/service/tests/test_mercurial_changeset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/tests/test_mercurial_operations.py` & `hgitaly-1.7.0/hgitaly/service/tests/test_mercurial_operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/tests/test_mercurial_repository.py` & `hgitaly-1.7.0/hgitaly/service/tests/test_mercurial_repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/tests/test_operations.py` & `hgitaly-1.7.0/hgitaly/service/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/tests/test_ref.py` & `hgitaly-1.7.0/hgitaly/service/tests/test_ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/tests/test_repository_service.py` & `hgitaly-1.7.0/hgitaly/service/tests/test_repository_service.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/service/tests/test_server.py` & `hgitaly-1.7.0/hgitaly/service/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/servicer.py` & `hgitaly-1.7.0/hgitaly/servicer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/ssh.py` & `hgitaly-1.7.0/hgitaly/ssh.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stream.py` & `hgitaly-1.7.0/hgitaly/stream.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/analysis_pb2.py` & `hgitaly-1.7.0/hgitaly/stub/analysis_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/analysis_pb2_grpc.py` & `hgitaly-1.7.0/hgitaly/stub/analysis_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/blob_pb2.py` & `hgitaly-1.7.0/hgitaly/stub/blob_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/blob_pb2_grpc.py` & `hgitaly-1.7.0/hgitaly/stub/blob_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/commit_pb2.py` & `hgitaly-1.7.0/hgitaly/stub/commit_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/commit_pb2_grpc.py` & `hgitaly-1.7.0/hgitaly/stub/commit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/diff_pb2.py` & `hgitaly-1.7.0/hgitaly/stub/diff_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/diff_pb2_grpc.py` & `hgitaly-1.7.0/hgitaly/stub/diff_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/errors_pb2.py` & `hgitaly-1.7.0/hgitaly/stub/errors_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/lint_pb2.py` & `hgitaly-1.7.0/hgitaly/stub/lint_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/mercurial_changeset_pb2.py` & `hgitaly-1.7.0/hgitaly/stub/mercurial_changeset_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/mercurial_changeset_pb2_grpc.py` & `hgitaly-1.7.0/hgitaly/stub/mercurial_changeset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/mercurial_operations_pb2.py` & `hgitaly-1.7.0/hgitaly/stub/mercurial_operations_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/mercurial_operations_pb2_grpc.py` & `hgitaly-1.7.0/hgitaly/stub/mercurial_operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/mercurial_repository_pb2.py` & `hgitaly-1.7.0/hgitaly/stub/mercurial_repository_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import lint_pb2 as lint__pb2
 from . import shared_pb2 as shared__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1amercurial-repository.proto\x12\x07hgitaly\x1a\nlint.proto\x1a\x0cshared.proto\"Y\n\x11InitConfigRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0enamespace_path\x18\x02 \x01(\t\"\x14\n\x12InitConfigResponse\"\x95\x02\n\x15HeptapodConfigSection\x12!\n\x14\x61llow_multiple_heads\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x1c\n\x0f\x61llow_bookmarks\x18\x03 \x01(\x08H\x01\x88\x01\x01\x12\x45\n\x0c\x61uto_publish\x18\x04 \x01(\x0e\x32*.hgitaly.HeptapodConfigSection.AutoPublishH\x02\x88\x01\x01\"6\n\x0b\x41utoPublish\x12\x11\n\rWITHOUT_TOPIC\x10\x00\x12\x0b\n\x07NOTHING\x10\x01\x12\x07\n\x03\x41LL\x10\x02\x42\x17\n\x15_allow_multiple_headsB\x12\n\x10_allow_bookmarksB\x0f\n\r_auto_publish\"V\n\x17GetManagedConfigRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\r\n\x05local\x18\x02 \x01(\x08\"]\n\x18GetManagedConfigResponse\x12\x0f\n\x07inherit\x18\x01 \x01(\x08\x12\x30\n\x08heptapod\x18\x02 \x01(\x0b\x32\x1e.hgitaly.HeptapodConfigSection\"\xc2\x01\n\x17SetManagedConfigRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x14\n\x07inherit\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x30\n\x08heptapod\x18\x03 \x01(\x0b\x32\x1e.hgitaly.HeptapodConfigSection\x12\x14\n\x0cremove_items\x18\x04 \x03(\t\x12\x0f\n\x07\x62y_line\x18\x05 \x01(\tB\n\n\x08_inherit\"\x1a\n\x18SetManagedConfigResponse\"\x8d\x01\n\x14GetConfigItemRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12(\n\x07\x61s_type\x18\x02 \x01(\x0e\x32\x17.hgitaly.ConfigItemType\x12\x0f\n\x07section\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\"H\n\x15GetConfigItemResponse\x12\x13\n\tas_string\x18\x01 \x01(\tH\x00\x12\x11\n\x07\x61s_bool\x18\x02 \x01(\x08H\x00\x42\x07\n\x05value\">\n\x0eRecoverRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"%\n\x0fRecoverResponse\x12\x12\n\nnot_needed\x18\x01 \x01(\x08\"?\n\x0fOptimizeRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x12\n\x10OptimizeResponse\"\x88\x01\n\x12ResetCachesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x31\n\x06\x63\x61\x63hes\x18\x02 \x03(\x0e\x32!.hgitaly.ResetCachesRequest.Cache\"\x11\n\x05\x43\x61\x63he\x12\x08\n\x04TAGS\x10\x00\"\x15\n\x13ResetCachesResponse\"b\n\rMercurialPeer\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0f\n\x07ssh_key\x18\x05 \x01(\t\x12\x17\n\x0fssh_known_hosts\x18\x06 \x01(\t\x12\x1a\n\x12ssh_remote_command\x18\x07 \x01(\x0c\"\xa7\x01\n\x0bPushRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12+\n\x0bremote_peer\x18\x02 \x01(\x0b\x32\x16.hgitaly.MercurialPeer\x12%\n\x1donly_gitlab_branches_matching\x18\x03 \x03(\x0c\x12\x16\n\x0einclude_drafts\x18\x04 \x01(\x08\"&\n\x0cPushResponse\x12\x16\n\x0enew_changesets\x18\x01 \x01(\x08\"\x81\x01\n\x0bPullRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12+\n\x0bremote_peer\x18\x02 \x01(\x0b\x32\x16.hgitaly.MercurialPeer\x12\x17\n\x0fgitlab_branches\x18\x03 \x03(\x0c\"&\n\x0cPullResponse\x12\x16\n\x0enew_changesets\x18\x01 \x01(\x08*&\n\x0e\x43onfigItemType\x12\n\n\x06STRING\x10\x00\x12\x08\n\x04\x42OOL\x10\x01\x32\xe0\x05\n\x1aMercurialRepositoryService\x12M\n\nInitConfig\x12\x1a.hgitaly.InitConfigRequest\x1a\x1b.hgitaly.InitConfigResponse\"\x06\xfa\x97(\x02\x08\x01\x12V\n\rGetConfigItem\x12\x1d.hgitaly.GetConfigItemRequest\x1a\x1e.hgitaly.GetConfigItemResponse\"\x06\xfa\x97(\x02\x08\x02\x12\x44\n\x07Recover\x12\x17.hgitaly.RecoverRequest\x1a\x18.hgitaly.RecoverResponse\"\x06\xfa\x97(\x02\x08\x02\x12G\n\x08Optimize\x12\x18.hgitaly.OptimizeRequest\x1a\x19.hgitaly.OptimizeResponse\"\x06\xfa\x97(\x02\x08\x01\x12P\n\x0bResetCaches\x12\x1b.hgitaly.ResetCachesRequest\x1a\x1c.hgitaly.ResetCachesResponse\"\x06\xfa\x97(\x02\x08\x01\x12_\n\x10GetManagedConfig\x12 .hgitaly.GetManagedConfigRequest\x1a!.hgitaly.GetManagedConfigResponse\"\x06\xfa\x97(\x02\x08\x02\x12_\n\x10SetManagedConfig\x12 .hgitaly.SetManagedConfigRequest\x1a!.hgitaly.SetManagedConfigResponse\"\x06\xfa\x97(\x02\x08\x01\x12;\n\x04Push\x12\x14.hgitaly.PushRequest\x1a\x15.hgitaly.PushResponse\"\x06\xfa\x97(\x02\x08\x01\x12;\n\x04Pull\x12\x14.hgitaly.PullRequest\x1a\x15.hgitaly.PullResponse\"\x06\xfa\x97(\x02\x08\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1amercurial-repository.proto\x12\x07hgitaly\x1a\nlint.proto\x1a\x0cshared.proto\"Y\n\x11InitConfigRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x16\n\x0enamespace_path\x18\x02 \x01(\t\"\x14\n\x12InitConfigResponse\"\x95\x02\n\x15HeptapodConfigSection\x12!\n\x14\x61llow_multiple_heads\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x1c\n\x0f\x61llow_bookmarks\x18\x03 \x01(\x08H\x01\x88\x01\x01\x12\x45\n\x0c\x61uto_publish\x18\x04 \x01(\x0e\x32*.hgitaly.HeptapodConfigSection.AutoPublishH\x02\x88\x01\x01\"6\n\x0b\x41utoPublish\x12\x11\n\rWITHOUT_TOPIC\x10\x00\x12\x0b\n\x07NOTHING\x10\x01\x12\x07\n\x03\x41LL\x10\x02\x42\x17\n\x15_allow_multiple_headsB\x12\n\x10_allow_bookmarksB\x0f\n\r_auto_publish\"V\n\x17GetManagedConfigRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\r\n\x05local\x18\x02 \x01(\x08\"]\n\x18GetManagedConfigResponse\x12\x0f\n\x07inherit\x18\x01 \x01(\x08\x12\x30\n\x08heptapod\x18\x02 \x01(\x0b\x32\x1e.hgitaly.HeptapodConfigSection\"\xc2\x01\n\x17SetManagedConfigRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x14\n\x07inherit\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x30\n\x08heptapod\x18\x03 \x01(\x0b\x32\x1e.hgitaly.HeptapodConfigSection\x12\x14\n\x0cremove_items\x18\x04 \x03(\t\x12\x0f\n\x07\x62y_line\x18\x05 \x01(\tB\n\n\x08_inherit\"\x1a\n\x18SetManagedConfigResponse\"\x8d\x01\n\x14GetConfigItemRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12(\n\x07\x61s_type\x18\x02 \x01(\x0e\x32\x17.hgitaly.ConfigItemType\x12\x0f\n\x07section\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\"H\n\x15GetConfigItemResponse\x12\x13\n\tas_string\x18\x01 \x01(\tH\x00\x12\x11\n\x07\x61s_bool\x18\x02 \x01(\x08H\x00\x42\x07\n\x05value\">\n\x0eRecoverRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"%\n\x0fRecoverResponse\x12\x12\n\nnot_needed\x18\x01 \x01(\x08\"?\n\x0fOptimizeRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\"\x12\n\x10OptimizeResponse\"\x88\x01\n\x12ResetCachesRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12\x31\n\x06\x63\x61\x63hes\x18\x02 \x03(\x0e\x32!.hgitaly.ResetCachesRequest.Cache\"\x11\n\x05\x43\x61\x63he\x12\x08\n\x04TAGS\x10\x00\"\x15\n\x13ResetCachesResponse\"b\n\rMercurialPeer\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x0f\n\x07ssh_key\x18\x05 \x01(\t\x12\x17\n\x0fssh_known_hosts\x18\x06 \x01(\t\x12\x1a\n\x12ssh_remote_command\x18\x07 \x01(\x0c\"\xa7\x01\n\x0bPushRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12+\n\x0bremote_peer\x18\x02 \x01(\x0b\x32\x16.hgitaly.MercurialPeer\x12%\n\x1donly_gitlab_branches_matching\x18\x03 \x03(\x0c\x12\x16\n\x0einclude_drafts\x18\x04 \x01(\x08\"&\n\x0cPushResponse\x12\x16\n\x0enew_changesets\x18\x01 \x01(\x08\"\xb8\x01\n\x0bPullRequest\x12,\n\nrepository\x18\x01 \x01(\x0b\x32\x12.gitaly.RepositoryB\x04\x98\xc6,\x01\x12+\n\x0bremote_peer\x18\x02 \x01(\x0b\x32\x16.hgitaly.MercurialPeer\x12\x1a\n\x04user\x18\x04 \x01(\x0b\x32\x0c.gitaly.User\x12\x1b\n\x13mercurial_revisions\x18\x05 \x03(\x0cJ\x04\x08\x03\x10\x04R\x0fgitlab_branches\"&\n\x0cPullResponse\x12\x16\n\x0enew_changesets\x18\x01 \x01(\x08*&\n\x0e\x43onfigItemType\x12\n\n\x06STRING\x10\x00\x12\x08\n\x04\x42OOL\x10\x01\x32\xe0\x05\n\x1aMercurialRepositoryService\x12M\n\nInitConfig\x12\x1a.hgitaly.InitConfigRequest\x1a\x1b.hgitaly.InitConfigResponse\"\x06\xfa\x97(\x02\x08\x01\x12V\n\rGetConfigItem\x12\x1d.hgitaly.GetConfigItemRequest\x1a\x1e.hgitaly.GetConfigItemResponse\"\x06\xfa\x97(\x02\x08\x02\x12\x44\n\x07Recover\x12\x17.hgitaly.RecoverRequest\x1a\x18.hgitaly.RecoverResponse\"\x06\xfa\x97(\x02\x08\x02\x12G\n\x08Optimize\x12\x18.hgitaly.OptimizeRequest\x1a\x19.hgitaly.OptimizeResponse\"\x06\xfa\x97(\x02\x08\x01\x12P\n\x0bResetCaches\x12\x1b.hgitaly.ResetCachesRequest\x1a\x1c.hgitaly.ResetCachesResponse\"\x06\xfa\x97(\x02\x08\x01\x12_\n\x10GetManagedConfig\x12 .hgitaly.GetManagedConfigRequest\x1a!.hgitaly.GetManagedConfigResponse\"\x06\xfa\x97(\x02\x08\x02\x12_\n\x10SetManagedConfig\x12 .hgitaly.SetManagedConfigRequest\x1a!.hgitaly.SetManagedConfigResponse\"\x06\xfa\x97(\x02\x08\x01\x12;\n\x04Push\x12\x14.hgitaly.PushRequest\x1a\x15.hgitaly.PushResponse\"\x06\xfa\x97(\x02\x08\x01\x12;\n\x04Pull\x12\x14.hgitaly.PullRequest\x1a\x15.hgitaly.PullResponse\"\x06\xfa\x97(\x02\x08\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'mercurial_repository_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -55,16 +55,16 @@
   _MERCURIALREPOSITORYSERVICE.methods_by_name['GetManagedConfig']._serialized_options = b'\372\227(\002\010\002'
   _MERCURIALREPOSITORYSERVICE.methods_by_name['SetManagedConfig']._options = None
   _MERCURIALREPOSITORYSERVICE.methods_by_name['SetManagedConfig']._serialized_options = b'\372\227(\002\010\001'
   _MERCURIALREPOSITORYSERVICE.methods_by_name['Push']._options = None
   _MERCURIALREPOSITORYSERVICE.methods_by_name['Push']._serialized_options = b'\372\227(\002\010\001'
   _MERCURIALREPOSITORYSERVICE.methods_by_name['Pull']._options = None
   _MERCURIALREPOSITORYSERVICE.methods_by_name['Pull']._serialized_options = b'\372\227(\002\010\001'
-  _globals['_CONFIGITEMTYPE']._serialized_start=1916
-  _globals['_CONFIGITEMTYPE']._serialized_end=1954
+  _globals['_CONFIGITEMTYPE']._serialized_start=1971
+  _globals['_CONFIGITEMTYPE']._serialized_end=2009
   _globals['_INITCONFIGREQUEST']._serialized_start=65
   _globals['_INITCONFIGREQUEST']._serialized_end=154
   _globals['_INITCONFIGRESPONSE']._serialized_start=156
   _globals['_INITCONFIGRESPONSE']._serialized_end=176
   _globals['_HEPTAPODCONFIGSECTION']._serialized_start=179
   _globals['_HEPTAPODCONFIGSECTION']._serialized_end=456
   _globals['_HEPTAPODCONFIGSECTION_AUTOPUBLISH']._serialized_start=340
@@ -98,13 +98,13 @@
   _globals['_MERCURIALPEER']._serialized_start=1434
   _globals['_MERCURIALPEER']._serialized_end=1532
   _globals['_PUSHREQUEST']._serialized_start=1535
   _globals['_PUSHREQUEST']._serialized_end=1702
   _globals['_PUSHRESPONSE']._serialized_start=1704
   _globals['_PUSHRESPONSE']._serialized_end=1742
   _globals['_PULLREQUEST']._serialized_start=1745
-  _globals['_PULLREQUEST']._serialized_end=1874
-  _globals['_PULLRESPONSE']._serialized_start=1876
-  _globals['_PULLRESPONSE']._serialized_end=1914
-  _globals['_MERCURIALREPOSITORYSERVICE']._serialized_start=1957
-  _globals['_MERCURIALREPOSITORYSERVICE']._serialized_end=2693
+  _globals['_PULLREQUEST']._serialized_end=1929
+  _globals['_PULLRESPONSE']._serialized_start=1931
+  _globals['_PULLRESPONSE']._serialized_end=1969
+  _globals['_MERCURIALREPOSITORYSERVICE']._serialized_start=2012
+  _globals['_MERCURIALREPOSITORYSERVICE']._serialized_end=2748
 # @@protoc_insertion_point(module_scope)
```

### Comparing `hgitaly-1.6.0/hgitaly/stub/mercurial_repository_pb2_grpc.py` & `hgitaly-1.7.0/hgitaly/stub/mercurial_repository_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/operations_pb2.py` & `hgitaly-1.7.0/hgitaly/stub/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/operations_pb2_grpc.py` & `hgitaly-1.7.0/hgitaly/stub/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/ref_pb2.py` & `hgitaly-1.7.0/hgitaly/stub/ref_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/ref_pb2_grpc.py` & `hgitaly-1.7.0/hgitaly/stub/ref_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/repository_pb2.py` & `hgitaly-1.7.0/hgitaly/stub/repository_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/repository_pb2_grpc.py` & `hgitaly-1.7.0/hgitaly/stub/repository_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/server_pb2.py` & `hgitaly-1.7.0/hgitaly/stub/server_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/server_pb2_grpc.py` & `hgitaly-1.7.0/hgitaly/stub/server_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/stub/shared_pb2.py` & `hgitaly-1.7.0/hgitaly/stub/shared_pb2.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tag.py` & `hgitaly-1.7.0/hgitaly/tag.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/testing/bundle.py` & `hgitaly-1.7.0/hgitaly/testing/bundle.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/testing/context.py` & `hgitaly-1.7.0/hgitaly/testing/context.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/testing/grpc.py` & `hgitaly-1.7.0/hgitaly/testing/grpc.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/testing/ssh.py` & `hgitaly-1.7.0/hgitaly/testing/ssh.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/testing/sshd.py` & `hgitaly-1.7.0/hgitaly/testing/sshd.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/testing/tests/test_sshd.py` & `hgitaly-1.7.0/hgitaly/testing/tests/test_sshd.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/common.py` & `hgitaly-1.7.0/hgitaly/tests/common.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_branch.py` & `hgitaly-1.7.0/hgitaly/tests/test_branch.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_diff.py` & `hgitaly-1.7.0/hgitaly/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_errors.py` & `hgitaly-1.7.0/hgitaly/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_feature.py` & `hgitaly-1.7.0/hgitaly/tests/test_feature.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_file_context.py` & `hgitaly-1.7.0/hgitaly/tests/test_file_context.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_gitlab_ref.py` & `hgitaly-1.7.0/hgitaly/tests/test_gitlab_ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_license_detector.py` & `hgitaly-1.7.0/hgitaly/tests/test_license_detector.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_linguist.py` & `hgitaly-1.7.0/hgitaly/tests/test_linguist.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_manifest.py` & `hgitaly-1.7.0/hgitaly/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_messages.py` & `hgitaly-1.7.0/hgitaly/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_oid.py` & `hgitaly-1.7.0/hgitaly/tests/test_oid.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_peer.py` & `hgitaly-1.7.0/hgitaly/tests/test_peer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_repository.py` & `hgitaly-1.7.0/hgitaly/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_revision.py` & `hgitaly-1.7.0/hgitaly/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_revset.py` & `hgitaly-1.7.0/hgitaly/tests/test_revset.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_servicer.py` & `hgitaly-1.7.0/hgitaly/tests/test_servicer.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_stream.py` & `hgitaly-1.7.0/hgitaly/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_tag.py` & `hgitaly-1.7.0/hgitaly/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/tests/test_workdir.py` & `hgitaly-1.7.0/hgitaly/tests/test_workdir.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/util.py` & `hgitaly-1.7.0/hgitaly/util.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly/workdir.py` & `hgitaly-1.7.0/hgitaly/workdir.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/hgitaly.egg-info/PKG-INFO` & `hgitaly-1.7.0/hgitaly.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 Metadata-Version: 2.1
 Name: hgitaly
-Version: 1.6.0
+Version: 1.7.0
 Summary: Server-side implementation of Gitaly protocol for Mercurial
 Home-page: https://foss.heptapod.net/heptapod/hgitaly
 Author: Georges Racinet
 Author-email: georges.racinet@octobus.net
 License: GPLv2+
 Keywords: hg mercurial heptapod gitlab
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: heptapod>=4.4.1dev0
+Requires-Dist: protobuf~=4.21.0
+Requires-Dist: grpcio~=1.58.0
+Requires-Dist: grpcio-status~=1.58.0
+Requires-Dist: grpc-interceptor
+Requires-Dist: hg-loggingmod
+Requires-Dist: psutil
+Requires-Dist: importlib_resources~=2.0.0
+Requires-Dist: spdx-lookup
 
 # HGitaly
 
 HGitaly is Gitaly server for Mercurial.
 
 It implements the subset of the Gitaly gRPC protocol that is relevant for
 Mercurial repositories, as well as its own HGitaly protocol, with methods
```

### Comparing `hgitaly-1.6.0/hgitaly.egg-info/SOURCES.txt` & `hgitaly-1.7.0/hgitaly.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -148,12 +148,13 @@
 tests_with_gitaly/hgitaly_rhgitaly_comparison.py
 tests_with_gitaly/rhgitaly.py
 tests_with_gitaly/test_blob_tree.py
 tests_with_gitaly/test_commit.py
 tests_with_gitaly/test_comparison.py
 tests_with_gitaly/test_diff.py
 tests_with_gitaly/test_gitaly_server.py
+tests_with_gitaly/test_mercurial_repository.py
 tests_with_gitaly/test_operations.py
 tests_with_gitaly/test_ref.py
 tests_with_gitaly/test_repository_service.py
 tests_with_gitaly/test_rhgitaly_server.py
 tests_with_gitaly/test_server.py
```

### Comparing `hgitaly-1.6.0/setup.py` & `hgitaly-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/tests_with_gitaly/__init__.py` & `hgitaly-1.7.0/tests_with_gitaly/__init__.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/tests_with_gitaly/comparison.py` & `hgitaly-1.7.0/tests_with_gitaly/comparison.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/tests_with_gitaly/conftest.py` & `hgitaly-1.7.0/tests_with_gitaly/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -74,18 +74,44 @@
                                    monkeypatch,
                                    rhgitaly_channel=rhgitaly_channel,
                                    ) as comparison:
         yield comparison
 
 
 @pytest.fixture()
+def rhgitaly(server_repos_root,  # module scope
+             rhgitaly_channel,  # module scope
+             ):
+    with hgitaly_rhgitaly_comparison_fixture(
+            server_repos_root=server_repos_root,
+            rhgitaly_channel=rhgitaly_channel
+    ) as fixture:
+        yield fixture
+
+
+@pytest.fixture()
 def hgitaly_rhgitaly_comparison(server_repos_root,  # module scope
                                 rhgitaly_channel,  # module scope
                                 grpc_channel,  # module scope
                                 monkeypatch,  # function scope
-                                ):
+                                ):  # pragma no cover, remove when used again
+    with hgitaly_rhgitaly_comparison_fixture(
+            server_repos_root,
+            hgitaly_channel=grpc_channel,
+            rhgitaly_channel=rhgitaly_channel,
+    ) as comparison:
+        yield comparison
+
+
+@pytest.fixture()
+def hgitaly_rhgitaly_comparison_no_repo(server_repos_root,  # module scope
+                                        rhgitaly_channel,  # module scope
+                                        grpc_channel,  # module scope
+                                        monkeypatch,  # function scope
+                                        ):
     with hgitaly_rhgitaly_comparison_fixture(
             server_repos_root,
             hgitaly_channel=grpc_channel,
             rhgitaly_channel=rhgitaly_channel,
+            skip_repo=True,
     ) as comparison:
         yield comparison
```

### Comparing `hgitaly-1.6.0/tests_with_gitaly/gitaly.py` & `hgitaly-1.7.0/tests_with_gitaly/gitaly.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/tests_with_gitaly/rhgitaly.py` & `hgitaly-1.7.0/tests_with_gitaly/rhgitaly.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,25 +16,44 @@
 
 HGITALY_SOURCE_ROOT = Path(__file__).parent.parent
 
 
 @attr.s
 class RHGitalyServer:
     home_dir = attr.ib()
+    env_overrides = attr.ib(default=None)
+    """Optional environment variables overrides.
+
+    If not ``None``, this :class:`dict` will be applied to the process
+    environment, after the several settings normally performed :meth:`running`.
+    To be used in special cases only.
+    """
+
+    termination_timeout = attr.ib(default=1)
+    """Time allowed for RHGitaly to shutdown after termination request
+
+    Useful to test that termination actually works. Normally it should be
+    very fast, even with the `debug` build.
+    """
+
+    socket_name = attr.ib(default='rhgitaly.socket')
 
     @contextmanager
     def running(self):
         env = dict(os.environ)
         env['GITALY_TESTING_NO_GIT_HOOKS'] = "1"  # will be eventually useful
         timeout = int(env.pop('RHGITALY_STARTUP_TIMEOUT', '30').strip())
 
         env['RHGITALY_REPOSITORIES_ROOT'] = str(self.home_dir / 'default')
-        socket_path = self.home_dir / 'rhgitaly.socket'
+        socket_path = self.home_dir / self.socket_name
         url = 'unix:%s' % socket_path.resolve()
         env['RHGITALY_LISTEN_URL'] = url
+
+        if self.env_overrides is not None:
+            env.update(self.env_overrides)
         rhgitaly_dir = HGITALY_SOURCE_ROOT / 'rust/rhgitaly'
 
         rhgitaly_exe = env.get('RHGITALY_EXECUTABLE')
         if rhgitaly_exe is None:  # pragma no cover
             subprocess.check_call(('cargo', 'build', '--locked'),
                                   cwd=rhgitaly_dir)
             run_cmd = ('cargo', 'run')
@@ -46,14 +65,15 @@
             rhgitaly = subprocess.Popen(
                 run_cmd,
                 stdout=logf, stderr=logf,
                 env=env,
                 cwd=rhgitaly_dir,
             )
 
+        self.pid = rhgitaly.pid
         # visible and useful only by putting a breakpoint right before it:
         print(f"Tests dir: {self.home_dir}")
 
         try:
             # tonic (actually H2) does not accept the default authority
             # set in the case of Unix Domain Sockets by gRPC 1.58.
             # See https://github.com/hyperium/tonic/issues/742 and for instance
@@ -63,8 +83,8 @@
                     url,
                     options=[('grpc.default_authority', 'localhost')]
             ) as channel:
                 wait_server_accepts_connection(channel, timeout=timeout)
                 yield channel
         finally:
             rhgitaly.terminate()
-            rhgitaly.wait()
+            rhgitaly.wait(timeout=self.termination_timeout)
```

### Comparing `hgitaly-1.6.0/tests_with_gitaly/test_blob_tree.py` & `hgitaly-1.7.0/tests_with_gitaly/test_blob_tree.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/tests_with_gitaly/test_commit.py` & `hgitaly-1.7.0/tests_with_gitaly/test_commit.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/tests_with_gitaly/test_comparison.py` & `hgitaly-1.7.0/tests_with_gitaly/test_comparison.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/tests_with_gitaly/test_diff.py` & `hgitaly-1.7.0/tests_with_gitaly/test_diff.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/tests_with_gitaly/test_gitaly_server.py` & `hgitaly-1.7.0/tests_with_gitaly/test_gitaly_server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/tests_with_gitaly/test_operations.py` & `hgitaly-1.7.0/tests_with_gitaly/test_operations.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/tests_with_gitaly/test_ref.py` & `hgitaly-1.7.0/tests_with_gitaly/test_ref.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/tests_with_gitaly/test_repository_service.py` & `hgitaly-1.7.0/tests_with_gitaly/test_repository_service.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/tests_with_gitaly/test_rhgitaly_server.py` & `hgitaly-1.7.0/tests_with_gitaly/test_rhgitaly_server.py`

 * *Files identical despite different names*

### Comparing `hgitaly-1.6.0/tests_with_gitaly/test_server.py` & `hgitaly-1.7.0/tests_with_gitaly/test_server.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 from . import skip_comparison_tests
 
 if skip_comparison_tests():  # pragma no cover
     pytestmark = pytest.mark.skip
 
 
-def test_compare_server_info(hgitaly_rhgitaly_comparison):
-    fixture = hgitaly_rhgitaly_comparison
+def test_compare_server_info(hgitaly_rhgitaly_comparison_no_repo):
+    fixture = hgitaly_rhgitaly_comparison_no_repo
     rpc_helper = fixture.rpc_helper(
         stub_cls=ServerServiceStub,
         method_name='ServerInfo',
         request_cls=ServerInfoRequest,
         repository_arg=False,
     )
```

