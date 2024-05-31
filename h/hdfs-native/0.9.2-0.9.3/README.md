# Comparing `tmp/hdfs_native-0.9.2.tar.gz` & `tmp/hdfs_native-0.9.3.tar.gz`

## Comparing `hdfs_native-0.9.2.tar` & `hdfs_native-0.9.3.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0     1001      127     1874 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/Cargo.toml
--rw-r--r--   0     1001      127     2127 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/benches/ec.rs
--rw-r--r--   0     1001      127     5698 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/benches/io.rs
--rw-r--r--   0     1001      127     1069 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/benches/rpc.rs
--rw-r--r--   0     1001      127     1052 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/build.rs
--rw-r--r--   0     1001      127     1918 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/examples/simple.rs
--rw-r--r--   0     1001      127     1754 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/minidfs/pom.xml
--rw-r--r--   0     1001      127    10183 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/minidfs/src/main/java/main/Main.java
--rw-r--r--   0     1001      127      334 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/minidfs/src/main/resources/log4j.properties
--rw-r--r--   0     1001      127    24644 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/client.rs
--rw-r--r--   0     1001      127     6384 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/common/config.rs
--rw-r--r--   0     1001      127       16 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/common/mod.rs
--rw-r--r--   0     1001      127     6685 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/ec/gf256.rs
--rw-r--r--   0     1001      127     7576 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/ec/matrix.rs
--rw-r--r--   0     1001      127     4952 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/ec/mod.rs
--rw-r--r--   0     1001      127     1711 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/error.rs
--rw-r--r--   0     1001      127    10044 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/file.rs
--rw-r--r--   0     1001      127    16387 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/hdfs/block_reader.rs
--rw-r--r--   0     1001      127    19697 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/hdfs/block_writer.rs
--rw-r--r--   0     1001      127    24269 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/hdfs/connection.rs
--rw-r--r--   0     1001      127      132 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/hdfs/mod.rs
--rw-r--r--   0     1001      127    14975 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/hdfs/protocol.rs
--rw-r--r--   0     1001      127     5913 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/hdfs/proxy.rs
--rw-r--r--   0     1001      127     1257 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/lib.rs
--rw-r--r--   0     1001      127     4855 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/minidfs.rs
--rw-r--r--   0     1001      127     2863 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/FSProtos.proto
--rw-r--r--   0     1001      127     2090 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/GenericRefreshProtocol.proto
--rw-r--r--   0     1001      127     1760 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/GetUserMappingsProtocol.proto
--rw-r--r--   0     1001      127     3715 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/HAServiceProtocol.proto
--rw-r--r--   0     1001      127     1922 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/IpcConnectionContext.proto
--rw-r--r--   0     1001      127     2924 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/ProtobufRpcEngine.proto
--rw-r--r--   0     1001      127     2915 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/ProtobufRpcEngine2.proto
--rw-r--r--   0     1001      127     2725 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/ProtocolInfo.proto
--rw-r--r--   0     1001      127     1767 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/RefreshAuthorizationPolicyProtocol.proto
--rw-r--r--   0     1001      127     1673 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/RefreshCallQueueProtocol.proto
--rw-r--r--   0     1001      127     2160 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/RefreshUserMappingsProtocol.proto
--rw-r--r--   0     1001      127     7706 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/RpcHeader.proto
--rw-r--r--   0     1001      127     2236 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/Security.proto
--rw-r--r--   0     1001      127     2193 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/TraceAdmin.proto
--rw-r--r--   0     1001      127     1867 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/ZKFCProtocol.proto
--rw-r--r--   0     1001      127    27673 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/hadoop.common.rs
--rw-r--r--   0     1001      127   168627 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/hadoop.hdfs.rs
--rw-r--r--   0     1001      127     8411 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/ClientDatanodeProtocol.proto
--rw-r--r--   0     1001      127    31840 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/ClientNamenodeProtocol.proto
--rw-r--r--   0     1001      127     2523 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/ReconfigurationProtocol.proto
--rw-r--r--   0     1001      127     2794 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/acl.proto
--rw-r--r--   0     1001      127     9922 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/datatransfer.proto
--rw-r--r--   0     1001      127     3028 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/encryption.proto
--rw-r--r--   0     1001      127     3281 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/erasurecoding.proto
--rw-r--r--   0     1001      127    21153 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/hdfs.proto
--rw-r--r--   0     1001      127     3607 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/inotify.proto
--rw-r--r--   0     1001      127     1996 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/xattr.proto
--rw-r--r--   0     1001      127      463 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/proto/mod.rs
--rw-r--r--   0     1001      127    22064 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/security/digest.rs
--rw-r--r--   0     1001      127     5289 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/security/gssapi.rs
--rw-r--r--   0     1001      127       81 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/security/mod.rs
--rw-r--r--   0     1001      127    27171 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/security/sasl.rs
--rw-r--r--   0     1001      127    14514 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/security/user.rs
--rw-r--r--   0     1001      127      171 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/src/test.rs
--rw-r--r--   0     1001      127     1498 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/tests/common/mod.rs
--rw-r--r--   0     1001      127     8808 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/tests/test_ec.rs
--rw-r--r--   0     1001      127     9145 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/tests/test_integration.rs
--rw-r--r--   0     1001      127     2203 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/tests/test_read.rs
--rw-r--r--   0     1001      127     3512 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/tests/test_viewfs.rs
--rw-r--r--   0     1001      127     4512 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/tests/test_write.rs
--rw-r--r--   0     1001      127     1629 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/crates/hdfs-native/tests/test_write_resiliency.rs
--rw-r--r--   0     1001      127     4247 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/README.md
--rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 hdfs_native-0.9.2/python/Cargo.toml
--rw-r--r--   0     1001      127      550 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/python/README.md
--rw-r--r--   0     1001      127     3802 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/python/python/hdfs_native/__init__.py
--rw-r--r--   0     1001      127     1596 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/python/python/hdfs_native/_internal.pyi
--rw-r--r--   0     1001      127       25 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/python/requirements-dev.txt
--rw-r--r--   0     1001      127      741 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/python/src/error.rs
--rw-r--r--   0     1001      127     6563 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/python/src/lib.rs
--rw-r--r--   0     1001      127      682 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/python/tests/conftest.py
--rw-r--r--   0     1001      127     1538 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/python/tests/test_integration.py
--rw-r--r--   0     1001      127    64519 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/Cargo.lock
--rw-r--r--   0        0        0      199 1970-01-01 00:00:00.000000 hdfs_native-0.9.2/Cargo.toml
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 hdfs_native-0.9.2/pyproject.toml
--rw-r--r--   0     1001      127     3802 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/python/hdfs_native/__init__.py
--rw-r--r--   0     1001      127     1596 2024-05-16 23:35:41.000000 hdfs_native-0.9.2/python/hdfs_native/_internal.pyi
--rw-r--r--   0        0        0     1217 1970-01-01 00:00:00.000000 hdfs_native-0.9.2/PKG-INFO
+-rw-r--r--   0     1001      127     1756 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/Cargo.toml
+-rw-r--r--   0     1001      127     2127 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/benches/ec.rs
+-rw-r--r--   0     1001      127     5450 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/benches/io.rs
+-rw-r--r--   0     1001      127     1069 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/benches/rpc.rs
+-rw-r--r--   0     1001      127     1052 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/build.rs
+-rw-r--r--   0     1001      127     1918 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/examples/simple.rs
+-rw-r--r--   0     1001      127     2081 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/minidfs/pom.xml
+-rw-r--r--   0     1001      127    10183 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/minidfs/src/main/java/main/Main.java
+-rw-r--r--   0     1001      127      334 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/minidfs/src/main/resources/log4j.properties
+-rw-r--r--   0     1001      127    24644 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/client.rs
+-rw-r--r--   0     1001      127     6384 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/common/config.rs
+-rw-r--r--   0     1001      127       16 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/common/mod.rs
+-rw-r--r--   0     1001      127     6685 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/ec/gf256.rs
+-rw-r--r--   0     1001      127     7576 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/ec/matrix.rs
+-rw-r--r--   0     1001      127     4952 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/ec/mod.rs
+-rw-r--r--   0     1001      127     1711 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/error.rs
+-rw-r--r--   0     1001      127    10044 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/file.rs
+-rw-r--r--   0     1001      127    19574 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/hdfs/block_reader.rs
+-rw-r--r--   0     1001      127    19850 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/hdfs/block_writer.rs
+-rw-r--r--   0     1001      127    24269 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/hdfs/connection.rs
+-rw-r--r--   0     1001      127      132 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/hdfs/mod.rs
+-rw-r--r--   0     1001      127    14975 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/hdfs/protocol.rs
+-rw-r--r--   0     1001      127     6053 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/hdfs/proxy.rs
+-rw-r--r--   0     1001      127     1257 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/lib.rs
+-rw-r--r--   0     1001      127     4855 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/minidfs.rs
+-rw-r--r--   0     1001      127     2863 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/common/FSProtos.proto
+-rw-r--r--   0     1001      127     2090 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/common/GenericRefreshProtocol.proto
+-rw-r--r--   0     1001      127     1760 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/common/GetUserMappingsProtocol.proto
+-rw-r--r--   0     1001      127     3715 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/common/HAServiceProtocol.proto
+-rw-r--r--   0     1001      127     1922 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/common/IpcConnectionContext.proto
+-rw-r--r--   0     1001      127     2924 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/common/ProtobufRpcEngine.proto
+-rw-r--r--   0     1001      127     2915 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/common/ProtobufRpcEngine2.proto
+-rw-r--r--   0     1001      127     2725 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/common/ProtocolInfo.proto
+-rw-r--r--   0     1001      127     1767 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/common/RefreshAuthorizationPolicyProtocol.proto
+-rw-r--r--   0     1001      127     1673 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/common/RefreshCallQueueProtocol.proto
+-rw-r--r--   0     1001      127     2160 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/common/RefreshUserMappingsProtocol.proto
+-rw-r--r--   0     1001      127     7706 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/common/RpcHeader.proto
+-rw-r--r--   0     1001      127     2236 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/common/Security.proto
+-rw-r--r--   0     1001      127     2193 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/common/TraceAdmin.proto
+-rw-r--r--   0     1001      127     1867 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/common/ZKFCProtocol.proto
+-rw-r--r--   0     1001      127    27673 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/hadoop.common.rs
+-rw-r--r--   0     1001      127   168627 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/hadoop.hdfs.rs
+-rw-r--r--   0     1001      127     8411 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/hdfs/ClientDatanodeProtocol.proto
+-rw-r--r--   0     1001      127    31840 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/hdfs/ClientNamenodeProtocol.proto
+-rw-r--r--   0     1001      127     2523 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/hdfs/ReconfigurationProtocol.proto
+-rw-r--r--   0     1001      127     2794 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/hdfs/acl.proto
+-rw-r--r--   0     1001      127     9922 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/hdfs/datatransfer.proto
+-rw-r--r--   0     1001      127     3028 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/hdfs/encryption.proto
+-rw-r--r--   0     1001      127     3281 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/hdfs/erasurecoding.proto
+-rw-r--r--   0     1001      127    21153 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/hdfs/hdfs.proto
+-rw-r--r--   0     1001      127     3607 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/hdfs/inotify.proto
+-rw-r--r--   0     1001      127     1996 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/hdfs/xattr.proto
+-rw-r--r--   0     1001      127      463 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/proto/mod.rs
+-rw-r--r--   0     1001      127    22064 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/security/digest.rs
+-rw-r--r--   0     1001      127     5289 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/security/gssapi.rs
+-rw-r--r--   0     1001      127       81 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/security/mod.rs
+-rw-r--r--   0     1001      127    27171 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/security/sasl.rs
+-rw-r--r--   0     1001      127    14514 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/security/user.rs
+-rw-r--r--   0     1001      127      171 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/src/test.rs
+-rw-r--r--   0     1001      127     1498 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/tests/common/mod.rs
+-rw-r--r--   0     1001      127     8894 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/tests/test_ec.rs
+-rw-r--r--   0     1001      127     9310 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/tests/test_integration.rs
+-rw-r--r--   0     1001      127     2203 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/tests/test_read.rs
+-rw-r--r--   0     1001      127     3512 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/tests/test_viewfs.rs
+-rw-r--r--   0     1001      127     4512 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/tests/test_write.rs
+-rw-r--r--   0     1001      127     1611 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/rust/tests/test_write_resiliency.rs
+-rw-r--r--   0     1001      127     4233 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/README.md
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 hdfs_native-0.9.3/python/Cargo.toml
+-rw-r--r--   0     1001      127      550 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/python/README.md
+-rw-r--r--   0     1001      127     3802 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/python/python/hdfs_native/__init__.py
+-rw-r--r--   0     1001      127     1596 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/python/python/hdfs_native/_internal.pyi
+-rw-r--r--   0     1001      127       25 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/python/requirements-dev.txt
+-rw-r--r--   0     1001      127      741 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/python/src/error.rs
+-rw-r--r--   0     1001      127     6563 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/python/src/lib.rs
+-rw-r--r--   0     1001      127      668 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/python/tests/conftest.py
+-rw-r--r--   0     1001      127     1538 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/python/tests/test_integration.py
+-rw-r--r--   0     1001      127    51987 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/Cargo.lock
+-rw-r--r--   0        0        0      156 1970-01-01 00:00:00.000000 hdfs_native-0.9.3/Cargo.toml
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 hdfs_native-0.9.3/pyproject.toml
+-rw-r--r--   0     1001      127     3802 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/python/hdfs_native/__init__.py
+-rw-r--r--   0     1001      127     1596 2024-05-31 12:03:02.000000 hdfs_native-0.9.3/python/hdfs_native/_internal.pyi
+-rw-r--r--   0        0        0     1217 1970-01-01 00:00:00.000000 hdfs_native-0.9.3/PKG-INFO
```

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/Cargo.toml` & `hdfs_native-0.9.3/rust/Cargo.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [package]
 name = "hdfs-native"
-version = "0.9.2"
+version = "0.9.3"
 edition = "2021"
 authors = ["Adam Binford <adamq43@gmail.com>"]
 homepage = "https://github.com/Kimahriman/hdfs-native"
 repository = "https://github.com/Kimahriman/hdfs-native"
 keywords = ["hadoop", "hdfs"]
 description = "Native HDFS client implementation in Rust"
-readme = "../../README.md"
+readme = "../README.md"
 license = "Apache-2.0"
 
 [dependencies]
 aes = "0.8"
 base64 = "0.21"
 bytes = { workspace = true }
 cbc = "0.1"
-chrono = { workspace = true }
+chrono = "0.4"
 cipher = "0.4"
 crc = "3.2"
 ctr = "0.9"
 des = "0.8"
 # Just used for benchmarks
 fs-hdfs3 = { version = "0.1.12", optional = true }
-futures = { workspace = true }
+futures = "0.3"
 g2p = "1"
 hex = "0.4"
 hmac = "0.12"
 libc = "0.2"
-libgssapi = { version = "0.7", default-features = false, optional = true, git = "https://github.com/Kimahriman/libgssapi.git", branch = "raw-slice-panic" }
+libgssapi = { version = "0.7", default-features = false, optional = true }
 log = { workspace = true }
 md-5 = "0.10"
 num-traits = "0.2"
 once_cell = "1"
 prost = "0.12"
 prost-types = "0.12"
 rand = "0.8"
@@ -48,15 +48,15 @@
 [build-dependencies]
 prost-build = { version = "0.12", optional = true }
 protobuf-src = { version = "1.1", optional = true }
 
 [dev-dependencies]
 criterion = { version = "0.5", features = ["async_tokio", "async_futures"] }
 env_logger = "0.10"
-serial_test = "2.0.0"
+serial_test = "2"
 tempfile = "3"
 which = "4"
 
 [features]
 kerberos = ["libgssapi"]
 
 generate-protobuf = ["prost-build", "protobuf-src"]
```

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/benches/ec.rs` & `hdfs_native-0.9.3/rust/benches/ec.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/benches/io.rs` & `hdfs_native-0.9.3/rust/benches/io.rs`

 * *Files 3% similar despite different names*

```diff
@@ -31,30 +31,29 @@
     let ints_to_write: usize = 32 * 1024 * 1024; // 128 MiB file
 
     let rt = tokio::runtime::Builder::new_multi_thread()
         .enable_all()
         .build()
         .unwrap();
 
+    rt.block_on(async { write_file(&client, "/bench", ints_to_write).await });
+
     let mut group = c.benchmark_group("read");
     group.throughput(Throughput::Bytes((ints_to_write * 4) as u64));
-    group.sample_size(10);
+    group.sample_size(50);
 
     group.bench_function("read-native", |b| {
-        rt.block_on(async { write_file(&client, "/bench", ints_to_write).await });
-        let reader = rt.block_on(client.read("/bench")).unwrap();
         b.to_async(&rt).iter(|| async {
-            // let reader = client.read("/bench").await.unwrap();
+            let reader = client.read("/bench").await.unwrap();
 
             reader.read_range(0, reader.file_length()).await.unwrap()
         })
     });
-    group.sample_size(10);
+    group.sample_size(50);
     group.bench_function("read-libhdfs", |b| {
-        rt.block_on(async { write_file(&client, "/bench", ints_to_write).await });
         let fs = get_hdfs().unwrap();
         b.iter(|| {
             let mut buf = BytesMut::zeroed(ints_to_write * 4);
             let mut bytes_read = 0;
             let reader = fs.open("/bench").unwrap();
 
             while bytes_read < ints_to_write * 4 {
@@ -65,26 +64,26 @@
             reader.close().unwrap();
             buf
         })
     });
 
     drop(group);
 
+    rt.block_on(async { write_file(&client, "/ec-3-2/bench", ints_to_write).await });
+
     let mut group = c.benchmark_group("read-ec");
     group.throughput(Throughput::Bytes((ints_to_write * 4) as u64));
-    group.sample_size(10);
+    group.sample_size(50);
     group.bench_function("read-native", |b| {
-        rt.block_on(async { write_file(&client, "/ec-3-2/bench", ints_to_write).await });
         let reader = rt.block_on(client.read("/ec-3-2/bench")).unwrap();
         b.to_async(&rt)
             .iter(|| async { reader.read_range(0, reader.file_length()).await.unwrap() })
     });
-    group.sample_size(10);
+    group.sample_size(50);
     group.bench_function("read-libhdfs", |b| {
-        rt.block_on(async { write_file(&client, "/ec-3-2/bench", ints_to_write).await });
         let fs = get_hdfs().unwrap();
         b.iter(|| {
             let mut buf = BytesMut::zeroed(ints_to_write * 4);
             let mut bytes_read = 0;
             let reader = fs.open("/ec-3-2/bench").unwrap();
 
             while bytes_read < ints_to_write * 4 {
```

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/benches/rpc.rs` & `hdfs_native-0.9.3/rust/benches/rpc.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/build.rs` & `hdfs_native-0.9.3/rust/build.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/examples/simple.rs` & `hdfs_native-0.9.3/rust/examples/simple.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/minidfs/pom.xml` & `hdfs_native-0.9.3/rust/minidfs/pom.xml`

 * *Files 7% similar despite different names*

#### Comparing `hdfs_native-0.9.2/crates/hdfs-native/minidfs/pom.xml` & `hdfs_native-0.9.3/rust/minidfs/pom.xml`

```diff
@@ -4,33 +4,44 @@
   <groupId>hdfs.native</groupId>
   <artifactId>minidfs</artifactId>
   <version>1.0-SNAPSHOT</version>
   <dependencies>
     <dependency>
       <groupId>org.apache.hadoop</groupId>
       <artifactId>hadoop-minicluster</artifactId>
-      <version>3.3.6</version>
+      <version>3.4.0</version>
+      <exclusions>
+        <exclusion>
+          <groupId>ch.qos.logback</groupId>
+          <artifactId>*</artifactId>
+        </exclusion>
+      </exclusions>
     </dependency>
     <dependency>
       <groupId>org.apache.hadoop</groupId>
       <artifactId>hadoop-minikdc</artifactId>
-      <version>3.3.6</version>
+      <version>3.4.0</version>
     </dependency>
     <dependency>
       <groupId>org.apache.hadoop</groupId>
       <artifactId>hadoop-hdfs-rbf</artifactId>
-      <version>3.3.6</version>
+      <version>3.4.0</version>
     </dependency>
     <dependency>
       <groupId>org.apache.hadoop</groupId>
       <artifactId>hadoop-hdfs-rbf</artifactId>
-      <version>3.3.6</version>
+      <version>3.4.0</version>
       <type>test-jar</type>
     </dependency>
     <dependency>
+      <groupId>org.apache.hadoop</groupId>
+      <artifactId>hadoop-federation-balance</artifactId>
+      <version>3.4.0</version>
+    </dependency>
+    <dependency>
       <groupId>junit</groupId>
       <artifactId>junit</artifactId>
       <version>4.13.2</version>
     </dependency>
     <dependency>
       <groupId>org.mockito</groupId>
       <artifactId>mockito-core</artifactId>
```

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/minidfs/src/main/java/main/Main.java` & `hdfs_native-0.9.3/rust/minidfs/src/main/java/main/Main.java`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/client.rs` & `hdfs_native-0.9.3/rust/src/client.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/common/config.rs` & `hdfs_native-0.9.3/rust/src/common/config.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/ec/gf256.rs` & `hdfs_native-0.9.3/rust/src/ec/gf256.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/ec/matrix.rs` & `hdfs_native-0.9.3/rust/src/ec/matrix.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/ec/mod.rs` & `hdfs_native-0.9.3/rust/src/ec/mod.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/error.rs` & `hdfs_native-0.9.3/rust/src/error.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/file.rs` & `hdfs_native-0.9.3/rust/src/file.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/hdfs/block_reader.rs` & `hdfs_native-0.9.3/rust/src/hdfs/block_reader.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,41 @@
-use std::{collections::HashMap, sync::Arc};
+use std::{
+    collections::{HashMap, VecDeque},
+    sync::Arc,
+};
 
 use bytes::{Buf, BufMut, Bytes, BytesMut};
 use futures::{
-    future::join_all,
     stream::{self, BoxStream},
     Stream, StreamExt,
 };
 use log::{debug, warn};
+use tokio::{
+    sync::mpsc::{self, Receiver, Sender},
+    task::JoinHandle,
+};
 
 use crate::{
     ec::EcSchema,
     hdfs::connection::{DatanodeConnection, Op, DATANODE_CACHE},
     proto::{
         common,
-        hdfs::{self, BlockOpResponseProto},
+        hdfs::{
+            self, BlockOpResponseProto, LocatedBlockProto, PacketHeaderProto,
+            ReadOpChecksumInfoProto,
+        },
     },
     HdfsError, Result,
 };
 
 use super::protocol::NamenodeProtocol;
 
+// The number of packets to queue up on reads
+const READ_PACKET_BUFFER_LEN: usize = 100;
+
 pub(crate) fn get_block_stream(
     protocol: Arc<NamenodeProtocol>,
     block: hdfs::LocatedBlockProto,
     offset: usize,
     len: usize,
     ec_schema: Option<EcSchema>,
 ) -> BoxStream<'static, Result<Bytes>> {
@@ -95,376 +107,454 @@
 
 struct ReplicatedBlockStream {
     protocol: Arc<NamenodeProtocol>,
     block: hdfs::LocatedBlockProto,
     offset: usize,
     len: usize,
 
-    connection: Option<DatanodeConnection>,
-    checksum_info: Option<hdfs::ReadOpChecksumInfoProto>,
+    listener: Option<JoinHandle<Result<DatanodeConnection>>>,
+    sender: Sender<Result<(PacketHeaderProto, Bytes)>>,
+    receiver: Receiver<Result<(PacketHeaderProto, Bytes)>>,
     current_replica: usize,
 }
 
 impl ReplicatedBlockStream {
     fn new(
         protocol: Arc<NamenodeProtocol>,
         block: hdfs::LocatedBlockProto,
         offset: usize,
         len: usize,
     ) -> Self {
+        let (sender, receiver) = mpsc::channel(READ_PACKET_BUFFER_LEN);
+
         Self {
             protocol,
             block,
             offset,
             len,
-            connection: None,
-            checksum_info: None,
+            listener: None,
+            sender,
+            receiver,
             current_replica: 0,
         }
     }
 
-    async fn select_next_datanode(&mut self) -> Result<()> {
-        if self.connection.is_some() {
-            self.current_replica += 1;
-            if self.current_replica >= self.block.locs.len() {
-                return Err(HdfsError::DataTransferError(
-                    "All DataNodes failed".to_string(),
-                ));
-            }
+    async fn select_next_datanode(
+        &mut self,
+    ) -> Result<(DatanodeConnection, Option<ReadOpChecksumInfoProto>)> {
+        if self.current_replica >= self.block.locs.len() {
+            return Err(HdfsError::DataTransferError(
+                "All DataNodes failed".to_string(),
+            ));
         }
 
         let datanode = &self.block.locs[self.current_replica].id;
 
+        self.current_replica += 1;
+
         let (connection, response) = connect_and_send(
             &self.protocol,
             datanode,
             &self.block.b,
             self.block.block_token.clone(),
             self.offset as u64,
             self.len as u64,
         )
         .await?;
 
         if response.status() != hdfs::Status::Success {
             return Err(HdfsError::DataTransferError(response.message().to_string()));
         }
 
-        self.connection = Some(connection);
-        self.checksum_info = response.read_op_checksum_info;
-
-        Ok(())
+        Ok((connection, response.read_op_checksum_info))
     }
 
     async fn next_packet(&mut self) -> Result<Option<Bytes>> {
-        if self.connection.is_none() {
-            self.select_next_datanode().await?;
-        }
-
-        if self.len == 0 {
-            let mut conn = self.connection.take().unwrap();
+        let (header, data) = loop {
+            if self.listener.is_none() {
+                let (connection, checksum_info) = self.select_next_datanode().await?;
+                self.listener = Some(Self::start_packet_listener(
+                    connection,
+                    checksum_info,
+                    self.sender.clone(),
+                ));
+            }
 
-            // Read the final empty packet
-            conn.read_packet().await?;
+            match self.receiver.recv().await {
+                Some(Ok(data)) => break data,
+                Some(Err(e)) => {
+                    // Some error communicating with datanode, log a warning and then retry on a different Datanode
+                    warn!("Error occured while reading from DataNode: {:?}", e);
+                    self.listener = None;
+                }
+                None => {
+                    // This means there's a disconnect between the data we are getting back and what we asked for,
+                    // so just raise an error
+                    return Err(HdfsError::DataTransferError(
+                        "Not enough data returned from DataNode".to_string(),
+                    ));
+                }
+            }
+        };
 
-            conn.send_read_success().await?;
+        if self.len == 0 {
+            let conn = self.listener.take().unwrap().await.unwrap()?;
             DATANODE_CACHE.release(conn);
             return Ok(None);
         }
 
-        let conn = self.connection.as_mut().unwrap();
-
-        let packet = conn.read_packet().await?;
-
-        let packet_offset = if self.offset > packet.header.offset_in_block as usize {
-            self.offset - packet.header.offset_in_block as usize
+        let packet_offset = if self.offset > header.offset_in_block as usize {
+            self.offset - header.offset_in_block as usize
         } else {
             0
         };
-        let packet_len = usize::min(packet.header.data_len as usize - packet_offset, self.len);
-        let packet_data = packet.get_data(&self.checksum_info)?;
+        let packet_len = usize::min(header.data_len as usize - packet_offset, self.len);
 
         self.offset += packet_len;
         self.len -= packet_len;
 
         Ok(Some(
-            packet_data.slice(packet_offset..(packet_offset + packet_len)),
+            data.slice(packet_offset..(packet_offset + packet_len)),
         ))
     }
 
+    fn start_packet_listener(
+        mut connection: DatanodeConnection,
+        checksum_info: Option<ReadOpChecksumInfoProto>,
+        sender: Sender<Result<(PacketHeaderProto, Bytes)>>,
+    ) -> JoinHandle<Result<DatanodeConnection>> {
+        tokio::spawn(async move {
+            loop {
+                let packet = connection.read_packet().await?;
+                let header = packet.header.clone();
+                let data = packet.get_data(&checksum_info)?;
+                let empty_packet = data.is_empty();
+                sender.send(Ok((header, data))).await.unwrap();
+
+                if empty_packet {
+                    connection.send_read_success().await?;
+                    break;
+                }
+            }
+            Ok(connection)
+        })
+    }
+
     fn into_stream(self) -> impl Stream<Item = Result<Bytes>> {
         stream::unfold(self, |mut state| async move {
             let next = state.next_packet().await.transpose();
             next.map(|n| (n, state))
         })
     }
 }
 
+// Reads cells of data from a DataNode connection
+struct CellReader {
+    cell_size: usize,
+    cell_buffer: BytesMut,
+    current_packet: Bytes,
+    block_stream: Option<ReplicatedBlockStream>,
+}
+
+impl CellReader {
+    fn new(cell_size: usize, block_stream: Option<ReplicatedBlockStream>) -> Self {
+        Self {
+            cell_size,
+            cell_buffer: BytesMut::with_capacity(cell_size),
+            current_packet: Bytes::new(),
+            block_stream,
+        }
+    }
+
+    async fn next_cell(&mut self) -> Result<Bytes> {
+        // We always should be reading a full cell, no current optimizations for a partial cell
+        // Only exception is the final cell may be partial
+        while self.cell_buffer.len() < self.cell_size {
+            if !self.current_packet.has_remaining() {
+                if let Some(block_stream) = self.block_stream.as_mut() {
+                    match block_stream.next_packet().await? {
+                        Some(next_packet) => self.current_packet = next_packet,
+                        None => {
+                            break;
+                        }
+                    }
+                } else {
+                    // At the end of a block, just return all 0s
+                    break;
+                }
+            }
+
+            let bytes_to_copy = usize::min(
+                self.cell_size - self.cell_buffer.len(),
+                self.current_packet.remaining(),
+            );
+
+            self.cell_buffer
+                .put(self.current_packet.split_to(bytes_to_copy));
+        }
+
+        // Pad a partial final cell with zeros
+        self.cell_buffer.resize(self.cell_size, 0);
+
+        Ok(std::mem::replace(
+            &mut self.cell_buffer,
+            BytesMut::with_capacity(self.cell_size),
+        )
+        .freeze())
+    }
+}
+
+/// Erasure coded data is stored in "cells" that are striped across Data Nodes.
+/// An example of what 3-2-1024k cells would look like:
+/// ----------------------------------------------
+/// | blk_0  | blk_1  | blk_2  | blk_3  | blk_4  |
+/// |--------|--------|--------|--------|--------|
+/// | cell_0 | cell_1 | cell_2 | parity | parity |
+/// | cell_3 | cell_4 | cell_5 | parity | parity |
+/// ----------------------------------------------
+///
+/// Where cell_0 contains the first 1024k bytes, cell_1 contains the next 1024k bytes, and so on.
+///
+/// For an initial, simple implementation, determine the cells containing the start and end
+/// of the range being requested, and request all "rows" or horizontal stripes of data containing
+/// and between the start and end cell. So if the read range starts in cell_1 and ends in cell_4,
+/// simply read all data blocks for cell_0 through cell_5.
+///
+/// We then convert these logical horizontal stripes into vertical stripes to read from each block/DataNode.
+/// In this case, we will have one read for cell_0 and cell_3 from blk_0, one for cell_1 and cell_4 from blk_1,
+/// and one for cell_2 and cell_5 from blk_2. We read each block a cell at a time, and return the horizontal
+/// stripe of cells when we have all cells in a row. So first the first call to read_slice returns cells
+/// cell_0, cell_1, and cell_2, and the second returns cell_3, cell_4, and cell_5. If any cell fails to read
+/// we construct a read of a parity block for the remaining horizontal slices we still need to process. If
+/// more reads fail than we have parity rows, the entire read fails.
+///
+/// In the future we can look at making this more efficient by not reading as many extra cells that aren't
+/// part of the range being requested at all. Currently the overhead of not doing this would be up to
+/// `data_units * cell_size * 2` of extra data being read from disk (basically two extra "rows" of data).
 struct StripedBlockStream {
     protocol: Arc<NamenodeProtocol>,
-    block: hdfs::LocatedBlockProto,
-    offset: usize,
-    len: usize,
+    block: LocatedBlockProto,
+    block_map: HashMap<usize, (hdfs::DatanodeInfoProto, common::TokenProto)>,
+    remaining: usize,
+    bytes_to_skip: usize,
     ec_schema: EcSchema,
+    // Position of the start of the current cell in a single block
+    current_block_start: usize,
+    // End location in a single block we need to read
+    block_end: usize,
+    cell_readers: Vec<Option<CellReader>>,
 }
 
 impl StripedBlockStream {
     fn new(
         protocol: Arc<NamenodeProtocol>,
         block: hdfs::LocatedBlockProto,
         offset: usize,
         len: usize,
         ec_schema: EcSchema,
     ) -> Self {
-        Self {
-            protocol,
-            block,
-            offset,
-            len,
-            ec_schema,
-        }
-    }
-
-    /// Hacky "stream" of a single value to match replicated behavior
-    /// TODO: Stream the results based on rows of cells?
-    fn into_stream(self) -> impl Stream<Item = Result<Bytes>> {
-        stream::once(async move { self.read_striped().await })
-    }
-
-    /// Erasure coded data is stored in "cells" that are striped across Data Nodes.
-    /// An example of what 3-2-1024k cells would look like:
-    /// ----------------------------------------------
-    /// | blk_0  | blk_1  | blk_2  | blk_3  | blk_4  |
-    /// |--------|--------|--------|--------|--------|
-    /// | cell_0 | cell_1 | cell_2 | parity | parity |
-    /// | cell_3 | cell_4 | cell_5 | parity | parity |
-    /// ----------------------------------------------
-    ///
-    /// Where cell_0 contains the first 1024k bytes, cell_1 contains the next 1024k bytes, and so on.
-    ///
-    /// For an initial, simple implementation, determine the cells containing the start and end
-    /// of the range being requested, and request all "rows" or horizontal stripes of data containing
-    /// and between the start and end cell. So if the read range starts in cell_1 and ends in cell_4,
-    /// simply read all data blocks for cell_0 through cell_5.
-    ///
-    /// We then convert these logical horizontal stripes into vertical stripes to read from each block/DataNode.
-    /// In this case, we will have one read for cell_0 and cell_3 from blk_0, one for cell_1 and cell_4 from blk_1,
-    /// and one for cell_2 and cell_5 from blk_2. If all of these reads succeed, we know we have everything we need
-    /// to reconstruct the data being requested. If any read fails, we will then request the parity cells for the same
-    /// vertical range of cells. If more data block reads fail then parity blocks exist, the read will fail.
-    ///
-    /// Once we have enough of the vertical stripes, we can then convert those back into horizontal stripes to
-    /// re-create each "row" of data. Then we simply need to take the range being requested out of the range
-    /// we reconstructed.
-    ///
-    /// In the future we can look at making this more efficient by not reading as many extra cells that aren't
-    /// part of the range being requested at all. Currently the overhead of not doing this would be up to
-    /// `data_units * cell_size * 2` of extra data being read from disk (basically two extra "rows" of data).
-    async fn read_striped(&self) -> Result<Bytes> {
-        let mut buf = BytesMut::with_capacity(self.len);
+        assert_eq!(block.block_indices().len(), block.locs.len());
 
         // Cell IDs for the range we are reading, inclusive
-        let starting_cell = self.ec_schema.cell_for_offset(self.offset);
-        let ending_cell = self.ec_schema.cell_for_offset(self.offset + self.len - 1);
+        let starting_cell = ec_schema.cell_for_offset(offset);
+        let ending_cell = ec_schema.cell_for_offset(offset + len - 1);
 
         // Logical rows or horizontal stripes we need to read, tail-exclusive
-        let starting_row = self.ec_schema.row_for_cell(starting_cell);
-        let ending_row = self.ec_schema.row_for_cell(ending_cell) + 1;
+        let starting_row = ec_schema.row_for_cell(starting_cell);
+        let ending_row = ec_schema.row_for_cell(ending_cell) + 1;
+        let block_end = ec_schema.offset_for_row(ending_row);
+
+        let current_block_start = ec_schema.offset_for_row(starting_row);
 
-        // Block start/end within each vertical stripe, tail-exclusive
-        let block_start = self.ec_schema.offset_for_row(starting_row);
-        let block_end = self.ec_schema.offset_for_row(ending_row);
-        let block_read_len = block_end - block_start;
-
-        assert_eq!(self.block.block_indices().len(), self.block.locs.len());
-        let datanode_infos: Vec<(&hdfs::DatanodeInfoProto, &common::TokenProto)> = self
-            .block
+        let bytes_to_skip = offset - starting_row * ec_schema.data_units * ec_schema.cell_size;
+
+        let datanode_infos: Vec<(hdfs::DatanodeInfoProto, common::TokenProto)> = block
             .locs
             .iter()
-            .zip(self.block.block_tokens.iter())
+            .cloned()
+            .zip(block.block_tokens.iter().cloned())
             .collect();
 
-        let block_map: HashMap<u8, (&hdfs::DatanodeInfoProto, &common::TokenProto)> = self
-            .block
+        let block_map: HashMap<usize, (hdfs::DatanodeInfoProto, common::TokenProto)> = block
             .block_indices()
             .iter()
             .copied()
-            .zip(datanode_infos.into_iter())
+            .map(|i| i as usize)
+            .zip(datanode_infos)
             .collect();
 
-        let mut stripe_results: Vec<Option<Bytes>> =
-            vec![None; self.ec_schema.data_units + self.ec_schema.parity_units];
-
-        let mut futures = Vec::new();
+        Self {
+            protocol,
+            block,
+            block_map,
+            remaining: len,
+            bytes_to_skip,
+            ec_schema,
+            current_block_start,
+            block_end,
+            cell_readers: vec![],
+        }
+    }
 
-        for index in 0..self.ec_schema.data_units as u8 {
-            let datanode_info = block_map.get(&index);
-            futures.push(self.read_vertical_stripe(
-                &self.ec_schema,
-                index,
-                datanode_info.map(|(datanode, _)| datanode),
-                datanode_info.map(|(_, token)| token),
-                block_start,
-                block_read_len,
-            ));
+    // Reads the next slice of cells and decodes if necessary
+    async fn read_slice(&mut self) -> Result<Option<VecDeque<Bytes>>> {
+        if self.remaining == 0 {
+            return Ok(None);
         }
 
-        // Do the actual reads and count how many data blocks failed
-        let mut failed_data_blocks = 0usize;
-        for (index, result) in join_all(futures).await.into_iter().enumerate() {
-            if let Ok(bytes) = result {
-                stripe_results[index] = Some(bytes);
-            } else {
-                failed_data_blocks += 1;
+        // Check if we need to start any new reads
+        let mut good_blocks = self.cell_readers.iter().filter(|r| r.is_some()).count();
+        while good_blocks < self.ec_schema.data_units {
+            if self.start_next_reader().await? {
+                good_blocks += 1;
             }
         }
 
-        let mut blocks_needed = failed_data_blocks;
-        let mut parity_unit = 0usize;
-        while blocks_needed > 0 && parity_unit < self.ec_schema.parity_units {
-            let block_index = (self.ec_schema.data_units + parity_unit) as u8;
-            let datanode_info = block_map.get(&block_index);
-            let result = self
-                .read_vertical_stripe(
-                    &self.ec_schema,
-                    block_index,
-                    datanode_info.map(|(datanode, _)| datanode),
-                    datanode_info.map(|(_, token)| token),
-                    block_start,
-                    block_read_len,
-                )
-                .await;
-
-            if let Ok(bytes) = result {
-                stripe_results[block_index as usize] = Some(bytes);
-                blocks_needed -= 1;
-            }
-            parity_unit += 1;
-        }
-
-        let decoded_bufs = self.ec_schema.ec_decode(stripe_results)?;
-        let mut bytes_to_skip =
-            self.offset - starting_row * self.ec_schema.data_units * self.ec_schema.cell_size;
-        let mut bytes_to_write = self.len;
-        for mut cell in decoded_bufs.into_iter() {
-            if bytes_to_skip > 0 {
-                if bytes_to_skip >= cell.len() {
-                    bytes_to_skip -= cell.len();
+        let mut slice = vec![None; self.ec_schema.data_units + self.ec_schema.parity_units];
+        let mut good_cells = 0;
+        let mut block_index = 0;
+        while good_cells < self.ec_schema.data_units {
+            if block_index >= self.cell_readers.len() {
+                // Need to start reading from the next parity
+                if !self.start_next_reader().await? {
+                    block_index += 1;
                     continue;
-                } else {
-                    cell.advance(bytes_to_skip);
-                    bytes_to_skip = 0;
                 }
             }
+            if let Some(reader) = self.cell_readers[block_index].as_mut() {
+                match reader.next_cell().await {
+                    Ok(bytes) => {
+                        slice[block_index] = Some(bytes);
+                        good_cells += 1;
+                    }
+                    Err(e) => {
+                        warn!(
+                            "Error reading erasure coded block, trying next replica: {:?}",
+                            e
+                        );
+                        self.cell_readers[block_index] = None;
+                    }
+                }
+            }
+            block_index += 1;
+        }
+
+        let mut decoded = VecDeque::from(self.ec_schema.ec_decode(slice)?);
 
-            if cell.len() >= bytes_to_write {
-                buf.put(cell.split_to(bytes_to_write));
-                break;
+        // Skip any bytes at the beginning
+        while self.bytes_to_skip > 0 {
+            if decoded[0].len() < self.bytes_to_skip {
+                self.bytes_to_skip -= decoded.pop_front().unwrap().len();
             } else {
-                bytes_to_write -= cell.len();
-                buf.put(cell);
+                let _ = decoded[0].split_to(self.bytes_to_skip);
+                self.bytes_to_skip = 0;
+            }
+        }
+
+        let total_size: usize = decoded.iter().map(|bytes| bytes.len()).sum();
+        if total_size > self.remaining {
+            let mut bytes_to_trim = total_size - self.remaining;
+            while bytes_to_trim > 0 {
+                if decoded.back().unwrap().len() <= bytes_to_trim {
+                    bytes_to_trim -= decoded.pop_back().unwrap().len();
+                } else {
+                    let last_cell = decoded.back_mut().unwrap();
+                    let _ = last_cell.split_off(last_cell.len() - bytes_to_trim);
+                    bytes_to_trim = 0;
+                }
             }
+            self.remaining = 0;
+        } else {
+            self.remaining -= total_size;
         }
 
-        Ok(buf.freeze())
+        self.current_block_start += self.ec_schema.cell_size;
+
+        Ok(Some(decoded))
     }
 
-    async fn read_vertical_stripe(
-        &self,
-        ec_schema: &EcSchema,
-        index: u8,
-        datanode: Option<&&hdfs::DatanodeInfoProto>,
-        token: Option<&&common::TokenProto>,
-        offset: usize,
-        len: usize,
-    ) -> Result<Bytes> {
+    async fn start_next_reader(&mut self) -> Result<bool> {
+        if self.cell_readers.len() >= self.ec_schema.data_units + self.ec_schema.parity_units {
+            return Err(HdfsError::ErasureCodingError(
+                "Not enough valid shards".to_string(),
+            ));
+        }
+
+        let index = self.cell_readers.len();
+
         #[cfg(feature = "integration-test")]
         if let Some(fault_injection) = crate::test::EC_FAULT_INJECTOR.lock().unwrap().as_ref() {
-            if fault_injection.fail_blocks.contains(&(index as usize)) {
+            if fault_injection.fail_blocks.contains(&index) {
                 debug!("Failing block read for {}", index);
-                return Err(HdfsError::InternalError("Testing error".to_string()));
+                self.cell_readers.push(None);
+                return Ok(false);
             }
         }
-        let max_block_offset =
-            ec_schema.max_offset(index as usize, self.block.b.num_bytes() as usize);
-
-        let read_len = usize::min(len, max_block_offset - offset);
 
-        if read_len == 0 {
-            // We're past the end of the file so there's nothign to read, just return a zeroed buffer
-            Ok(BytesMut::zeroed(len).freeze())
-        } else if let Some((datanode_info, token)) = datanode.zip(token) {
-            let mut buf = BytesMut::zeroed(len);
+        let max_block_offset = self
+            .ec_schema
+            .max_offset(index, self.block.b.num_bytes() as usize);
+
+        let end = usize::min(self.block_end, max_block_offset);
+        let len = end - self.current_block_start;
+
+        // Three cases we need to worry about
+        // 1. The length to read is 0, which means we are reading the last slice and this index
+        //    is past the end of the data. Just create a reader that returns all 0s, regardless
+        //    if the block exists or not.
+        // 2. We have the DataNode info, so start reading from it
+        // 3. We don't have the DataNode info, so this shard isn't valid
+        if len == 0 {
+            self.cell_readers
+                .push(Some(CellReader::new(self.ec_schema.cell_size, None)));
+            Ok(true)
+        } else if let Some((datanode_info, token)) = self.block_map.get(&index) {
+            let mut block = self.block.clone();
 
             // Each vertical stripe has a block ID of the original located block ID + block index
             // That was fun to figure out
-            let mut block = self.block.b.clone();
-            block.block_id += index as u64;
+            block.b.block_id += index as u64;
+            block.locs = vec![datanode_info.clone()];
+            block.block_token = token.clone();
+
+            let block_stream = ReplicatedBlockStream::new(
+                Arc::clone(&self.protocol),
+                block,
+                self.current_block_start,
+                len,
+            );
 
-            self.read_from_datanode(&datanode_info.id, &block, token, offset, read_len, &mut buf)
-                .await?;
+            self.cell_readers.push(Some(CellReader::new(
+                self.ec_schema.cell_size,
+                Some(block_stream),
+            )));
 
-            Ok(buf.freeze())
+            Ok(true)
         } else {
-            // There should be data to read but we didn't get block info for this index, so this shard is missing
-            Err(HdfsError::ErasureCodingError(
-                "Shard is missing".to_string(),
-            ))
+            self.cell_readers.push(None);
+            Ok(false)
         }
     }
 
-    async fn read_from_datanode(
-        &self,
-        datanode: &hdfs::DatanodeIdProto,
-        block: &hdfs::ExtendedBlockProto,
-        token: &common::TokenProto,
-        offset: usize,
-        len: usize,
-        mut buf: &mut [u8],
-    ) -> Result<()> {
-        if len == 0 {
-            return Ok(());
-        }
+    fn into_stream(self) -> impl Stream<Item = Result<Bytes>> {
+        stream::unfold(
+            (self, VecDeque::new()),
+            |(mut stream, mut buffers)| async move {
+                if buffers.is_empty() {
+                    match stream.read_slice().await {
+                        Ok(Some(next_buffers)) => {
+                            buffers = next_buffers;
+                        }
+                        Ok(None) => {
+                            return None;
+                        }
+                        Err(e) => {
+                            return Some((Err(e), (stream, buffers)));
+                        }
+                    }
+                }
 
-        let (mut connection, response) = connect_and_send(
-            &self.protocol,
-            datanode,
-            block,
-            token.clone(),
-            offset as u64,
-            len as u64,
+                buffers.pop_front().map(|b| (Ok(b), (stream, buffers)))
+            },
         )
-        .await?;
-
-        if response.status() != hdfs::Status::Success {
-            return Err(HdfsError::DataTransferError(response.message().to_string()));
-        }
-
-        // First handle the offset into the first packet
-        let mut packet = connection.read_packet().await?;
-        let packet_offset = offset - packet.header.offset_in_block as usize;
-        let data_len = packet.header.data_len as usize - packet_offset;
-        let data_to_read = usize::min(data_len, len);
-        let mut data_left = len - data_to_read;
-
-        let packet_data = packet.get_data(&response.read_op_checksum_info)?;
-        buf.put(packet_data.slice(packet_offset..(packet_offset + data_to_read)));
-
-        while data_left > 0 {
-            packet = connection.read_packet().await?;
-            // TODO: Error checking
-            let data_to_read = usize::min(data_left, packet.header.data_len as usize);
-            buf.put(
-                packet
-                    .get_data(&response.read_op_checksum_info)?
-                    .slice(0..data_to_read),
-            );
-            data_left -= data_to_read;
-        }
-
-        // There should be one last empty packet after we are done
-        connection.read_packet().await?;
-        connection.send_read_success().await?;
-        DATANODE_CACHE.release(connection);
-
-        Ok(())
     }
 }
```

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/hdfs/block_writer.rs` & `hdfs_native-0.9.3/rust/src/hdfs/block_writer.rs`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 use super::protocol::NamenodeProtocol;
 
 const HEART_BEAT_SEQNO: i64 = -1;
 const UNKNOWN_SEQNO: i64 = -2;
 
 const HEARTBEAT_INTERVAL_SECONDS: u64 = 30;
 
+// The number of packets and acks to queue up on writes
+const WRITE_PACKET_BUFFER_LEN: usize = 100;
+
 /// Wrapper around both types of block writers. This was simpler than trying to
 /// do dynamic dispatch with a BlockWriter trait.
 pub(crate) enum BlockWriter {
     Replicated(ReplicatedBlockWriter),
     Striped(StripedBlockWriter),
 }
 
@@ -146,16 +149,17 @@
         debug!("Block write request: {:?}", &message);
         let response = connection.send(Op::WriteBlock, &message).await?;
         debug!("Block write response: {:?}", response);
 
         let (reader, writer) = connection.split();
 
         // Channel for tracking packets that need to be acked
-        let (ack_queue_sender, ack_queue_receiever) = mpsc::channel::<(i64, bool)>(100);
-        let (packet_sender, packet_receiver) = mpsc::channel::<Packet>(100);
+        let (ack_queue_sender, ack_queue_receiever) =
+            mpsc::channel::<(i64, bool)>(WRITE_PACKET_BUFFER_LEN);
+        let (packet_sender, packet_receiver) = mpsc::channel::<Packet>(WRITE_PACKET_BUFFER_LEN);
 
         let ack_listener_handle = Self::listen_for_acks(reader, ack_queue_receiever);
         let packet_sender_handle = Self::start_packet_sender(writer, packet_receiver);
         let heartbeat_handle = Self::start_heartbeat_sender(packet_sender.clone());
 
         let bytes_per_checksum = server_defaults.bytes_per_checksum;
         let write_packet_size = server_defaults.write_packet_size;
```

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/hdfs/connection.rs` & `hdfs_native-0.9.3/rust/src/hdfs/connection.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/hdfs/protocol.rs` & `hdfs_native-0.9.3/rust/src/hdfs/protocol.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/hdfs/proxy.rs` & `hdfs_native-0.9.3/rust/src/hdfs/proxy.rs`

 * *Files 2% similar despite different names*

```diff
@@ -167,11 +167,14 @@
             attempts += 1;
         }
     }
 
     fn convert_rpc_error(exception: String, msg: String) -> HdfsError {
         match exception.as_ref() {
             "org.apache.hadoop.fs.FileAlreadyExistsException" => HdfsError::AlreadyExists(msg),
+            "org.apache.hadoop.hdfs.protocol.AlreadyBeingCreatedException" => {
+                HdfsError::AlreadyExists(msg)
+            }
             _ => HdfsError::RPCError(exception, msg),
         }
     }
 }
```

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/lib.rs` & `hdfs_native-0.9.3/rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/minidfs.rs` & `hdfs_native-0.9.3/rust/src/minidfs.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/FSProtos.proto` & `hdfs_native-0.9.3/rust/src/proto/common/FSProtos.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/GenericRefreshProtocol.proto` & `hdfs_native-0.9.3/rust/src/proto/common/GenericRefreshProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/GetUserMappingsProtocol.proto` & `hdfs_native-0.9.3/rust/src/proto/common/GetUserMappingsProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/HAServiceProtocol.proto` & `hdfs_native-0.9.3/rust/src/proto/common/HAServiceProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/IpcConnectionContext.proto` & `hdfs_native-0.9.3/rust/src/proto/common/IpcConnectionContext.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/ProtobufRpcEngine.proto` & `hdfs_native-0.9.3/rust/src/proto/common/ProtobufRpcEngine.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/ProtobufRpcEngine2.proto` & `hdfs_native-0.9.3/rust/src/proto/common/ProtobufRpcEngine2.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/ProtocolInfo.proto` & `hdfs_native-0.9.3/rust/src/proto/common/ProtocolInfo.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/RefreshAuthorizationPolicyProtocol.proto` & `hdfs_native-0.9.3/rust/src/proto/common/RefreshAuthorizationPolicyProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/RefreshCallQueueProtocol.proto` & `hdfs_native-0.9.3/rust/src/proto/common/RefreshCallQueueProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/RefreshUserMappingsProtocol.proto` & `hdfs_native-0.9.3/rust/src/proto/common/RefreshUserMappingsProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/RpcHeader.proto` & `hdfs_native-0.9.3/rust/src/proto/common/RpcHeader.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/Security.proto` & `hdfs_native-0.9.3/rust/src/proto/common/Security.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/TraceAdmin.proto` & `hdfs_native-0.9.3/rust/src/proto/common/TraceAdmin.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/common/ZKFCProtocol.proto` & `hdfs_native-0.9.3/rust/src/proto/common/ZKFCProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/hadoop.common.rs` & `hdfs_native-0.9.3/rust/src/proto/hadoop.common.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/hadoop.hdfs.rs` & `hdfs_native-0.9.3/rust/src/proto/hadoop.hdfs.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/ClientDatanodeProtocol.proto` & `hdfs_native-0.9.3/rust/src/proto/hdfs/ClientDatanodeProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/ClientNamenodeProtocol.proto` & `hdfs_native-0.9.3/rust/src/proto/hdfs/ClientNamenodeProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/ReconfigurationProtocol.proto` & `hdfs_native-0.9.3/rust/src/proto/hdfs/ReconfigurationProtocol.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/acl.proto` & `hdfs_native-0.9.3/rust/src/proto/hdfs/acl.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/datatransfer.proto` & `hdfs_native-0.9.3/rust/src/proto/hdfs/datatransfer.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/encryption.proto` & `hdfs_native-0.9.3/rust/src/proto/hdfs/encryption.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/erasurecoding.proto` & `hdfs_native-0.9.3/rust/src/proto/hdfs/erasurecoding.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/hdfs.proto` & `hdfs_native-0.9.3/rust/src/proto/hdfs/hdfs.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/inotify.proto` & `hdfs_native-0.9.3/rust/src/proto/hdfs/inotify.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/proto/hdfs/xattr.proto` & `hdfs_native-0.9.3/rust/src/proto/hdfs/xattr.proto`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/security/digest.rs` & `hdfs_native-0.9.3/rust/src/security/digest.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/security/gssapi.rs` & `hdfs_native-0.9.3/rust/src/security/gssapi.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/security/sasl.rs` & `hdfs_native-0.9.3/rust/src/security/sasl.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/src/security/user.rs` & `hdfs_native-0.9.3/rust/src/security/user.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/tests/common/mod.rs` & `hdfs_native-0.9.3/rust/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/tests/test_ec.rs` & `hdfs_native-0.9.3/rust/tests/test_ec.rs`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,16 @@
             .unwrap();
         assert!(cmd.wait().unwrap().success());
 
         Ok(())
     }
 
     fn verify_read(mut data: Bytes, size: usize) {
-        assert!(size % 4 == 0);
+        assert_eq!(size % 4, 0);
+        assert_eq!(data.len(), size);
         let num_ints = size / 4;
 
         for i in 0..num_ints as u32 {
             assert_eq!(data.get_u32(), i, "Different values at integer {}", i);
         }
     }
 
@@ -93,14 +94,15 @@
         ]
     }
     #[tokio::test]
     #[serial]
     async fn test_erasure_coded_read() -> Result<()> {
         let _ = env_logger::builder().is_test(true).try_init();
 
+        #[allow(unused_mut)]
         let mut dfs_features = HashSet::from([DfsFeatures::EC]);
         #[cfg(feature = "kerberos")]
         dfs_features.insert(DfsFeatures::Security);
 
         let dfs = MiniDfs::with_features(&dfs_features);
         let client = Client::default();
 
@@ -114,15 +116,15 @@
                 let reader = client.read(&file).await?;
                 assert_eq!(reader.file_length(), file_size);
 
                 for faults in 0..parity {
                     let _ = EC_FAULT_INJECTOR.lock().unwrap().insert(EcFaultInjection {
                         fail_blocks: (0..faults).collect(),
                     });
-                    let data = reader.read_range(0, reader.file_length()).await?;
+                    let data = reader.read_range(0, file_size).await?;
                     verify_read(data, file_size);
                 }
 
                 // Fail more than the number of parity shards, read should fail
                 let _ = EC_FAULT_INJECTOR.lock().unwrap().insert(EcFaultInjection {
                     fail_blocks: (0..=parity).collect(),
                 });
@@ -167,14 +169,15 @@
     }
 
     #[tokio::test]
     #[serial]
     async fn test_erasure_coded_write() -> Result<()> {
         let _ = env_logger::builder().is_test(true).try_init();
 
+        #[allow(unused_mut)]
         let mut dfs_features = HashSet::from([DfsFeatures::EC]);
         #[cfg(feature = "kerberos")]
         dfs_features.insert(DfsFeatures::Security);
 
         let _dfs = MiniDfs::with_features(&dfs_features);
         let client = Client::default();
```

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/tests/test_integration.rs` & `hdfs_native-0.9.3/rust/tests/test_integration.rs`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         test_with_features(&HashSet::from([DfsFeatures::Security, DfsFeatures::Token]))
             .await
             .unwrap();
     }
 
     #[tokio::test]
     #[serial]
+    #[cfg(feature = "kerberos")]
     async fn test_integrity_kerberos() {
         test_with_features(&HashSet::from([
             DfsFeatures::Security,
             DfsFeatures::Integrity,
         ]))
         .await
         .unwrap();
@@ -77,50 +78,54 @@
         ]))
         .await
         .unwrap();
     }
 
     #[tokio::test]
     #[serial]
+    #[cfg(feature = "kerberos")]
     async fn test_aes() {
         test_with_features(&HashSet::from([
             DfsFeatures::Security,
             DfsFeatures::Privacy,
             DfsFeatures::AES,
         ]))
         .await
         .unwrap();
     }
 
     #[tokio::test]
     #[serial]
+    #[cfg(feature = "kerberos")]
     async fn test_forced_data_transfer_encryption() {
         // DataTransferEncryption enabled but privacy isn't, still force encryption
         test_with_features(&HashSet::from([
             DfsFeatures::Security,
             DfsFeatures::DataTransferEncryption,
         ]))
         .await
         .unwrap();
     }
 
     #[tokio::test]
     #[serial]
+    #[cfg(feature = "kerberos")]
     async fn test_data_transfer_encryption() {
         test_with_features(&HashSet::from([
             DfsFeatures::Security,
             DfsFeatures::Privacy,
             DfsFeatures::DataTransferEncryption,
         ]))
         .await
         .unwrap();
     }
 
     #[tokio::test]
     #[serial]
+    #[cfg(feature = "kerberos")]
     async fn test_data_transfer_encryption_aes() {
         test_with_features(&HashSet::from([
             DfsFeatures::Security,
             DfsFeatures::Privacy,
             DfsFeatures::DataTransferEncryption,
             DfsFeatures::AES,
         ]))
```

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/tests/test_read.rs` & `hdfs_native-0.9.3/rust/tests/test_read.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/tests/test_viewfs.rs` & `hdfs_native-0.9.3/rust/tests/test_viewfs.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/tests/test_write.rs` & `hdfs_native-0.9.3/rust/tests/test_write.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/crates/hdfs-native/tests/test_write_resiliency.rs` & `hdfs_native-0.9.3/rust/tests/test_write_resiliency.rs`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     #[serial]
     async fn test_write_resiliency() -> Result<()> {
         let _ = env_logger::builder().is_test(true).try_init();
 
         #[cfg(feature = "kerberos")]
         let _dfs = MiniDfs::with_features(&HashSet::from([DfsFeatures::HA, DfsFeatures::Security]));
         #[cfg(not(feature = "kerberos"))]
-        let _dfs = MiniDfs::with_features(&HashSet::from([DfsFeatures::HA, DfsFeatures::RBF]));
+        let _dfs = MiniDfs::with_features(&HashSet::from([DfsFeatures::HA]));
         let client = Client::default();
 
         // Second client for checking lease
         let client2 = Client::default();
 
         let file = "/testfile";
```

### Comparing `hdfs_native-0.9.2/README.md` & `hdfs_native-0.9.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 ### Python tests
 See the [Python README](./python/README.md)
 
 ## Running benchmarks
 Some of the benchmarks compare performance to the JVM based client through libhdfs via the fs-hdfs3 crate. Because of that, some extra setup is required to run the benchmarks:
 
 ```bash
-export HADOOP_CONF_DIR=$(pwd)/crates/hdfs-native/target/test
+export HADOOP_CONF_DIR=$(pwd)/rust/target/test
 export CLASSPATH=$(hadoop classpath)
 ```
 
 then you can run the benchmarks with
 ```bash
 cargo bench -p hdfs-native --features benchmark
 ```
```

### Comparing `hdfs_native-0.9.2/python/Cargo.toml` & `hdfs_native-0.9.3/python/Cargo.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "hdfs-native-python"
-version = "0.9.2"
+version = "0.9.3"
 edition = "2021"
 authors = ["Adam Binford <adamq43@gmail.com>"]
 homepage = "https://github.com/Kimahriman/hdfs-native"
 repository = "https://github.com/Kimahriman/hdfs-native"
 keywords = ["hadoop", "hdfs"]
 description = "Python bindings for native HDFS client implementation in Rust"
 license = "Apache-2.0"
@@ -23,15 +23,15 @@
 
 [package.metadata.maturin]
 name = "hdfs_native._internal"
 
 [dependencies]
 bytes = { workspace = true } 
 env_logger = "0.10"
-hdfs-native = { path = "../crates/hdfs-native" }
-log = "0.4"
+hdfs-native = { path = "../rust" }
+log = { workspace = true }
 pyo3 = { version = "0.20", features = ["extension-module", "abi3", "abi3-py38"] }
 thiserror = { workspace = true }
 tokio = { workspace = true, features = ["rt-multi-thread"] }
 
 [features]
 kerberos = ["hdfs-native/kerberos"]
```

### Comparing `hdfs_native-0.9.2/python/README.md` & `hdfs_native-0.9.3/python/README.md`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/python/python/hdfs_native/__init__.py` & `hdfs_native-0.9.3/python/python/hdfs_native/__init__.py`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/python/python/hdfs_native/_internal.pyi` & `hdfs_native-0.9.3/python/python/hdfs_native/_internal.pyi`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/python/src/error.rs` & `hdfs_native-0.9.3/python/src/error.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/python/src/lib.rs` & `hdfs_native-0.9.3/python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/python/tests/test_integration.py` & `hdfs_native-0.9.3/python/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/Cargo.lock` & `hdfs_native-0.9.3/Cargo.lock`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "addr2line"
-version = "0.21.0"
+version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a30b2e23b9e17a9f90641c7ab1549cd9b44f296d3ccbf309d2863cfe398a0cb"
+checksum = "6e4503c46a5c0c7844e948c9a4d6acd9f50cccb4de1c48eb9e291ea17470c678"
 dependencies = [
  "gimli",
 ]
 
 [[package]]
 name = "adler"
 version = "1.0.2"
@@ -26,17 +26,17 @@
  "cfg-if",
  "cipher",
  "cpufeatures",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "android-tzdata"
 version = "0.1.1"
@@ -56,55 +56,44 @@
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "anstyle"
-version = "1.0.6"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
+checksum = "038dfcf04a5feb68e9c60b21c9625a54c2c0616e79b72b0fd87075a056ae1d1b"
 
 [[package]]
 name = "anyhow"
-version = "1.0.80"
+version = "1.0.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ad32ce52e4161730f7098c077cd2ed6229b5804ccf99e5366be1ab72a98b4e1"
-
-[[package]]
-name = "async-trait"
-version = "0.1.77"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c980ee35e870bd1a4d2c8294d4c04d0499e67bca1e4b5cefcc693c2fa00caea9"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.50",
-]
+checksum = "b3d1d046238990b9cf5bcde22a3fb3584ee5cf65fb2765f454ed428c7a0063da"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "autotools"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aef8da1805e028a172334c3b680f93e71126f2327622faef2ec3d893c0a4ad77"
+checksum = "ef941527c41b0fc0dd48511a8154cd5fc7e29200a0ff8b7203c5d777dbc795cf"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "17c6a35df3749d2e8bb1b7b21a976d82b15548788d2735b9d82f329268f71a11"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -141,42 +130,42 @@
 
 [[package]]
 name = "bindgen"
 version = "0.69.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a00dc851838a2120612785d195287475a3ac45514741da670b735818822129a0"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "cexpr",
  "clang-sys",
  "itertools 0.12.1",
  "lazy_static",
  "lazycell",
  "log",
  "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "syn 2.0.50",
+ "syn 2.0.66",
  "which",
 ]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
@@ -190,23 +179,23 @@
 checksum = "a8894febbff9f758034a5b8e12d87918f56dfc64a8e1fe757d65e29041538d93"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.0"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d32a994c2b3ca201d9b263612a374263f05e7adde37c4707f693dcd375076d1f"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
@@ -217,20 +206,17 @@
 checksum = "26b52a9543ae338f279b96b0b9fed9c8093744685043739079ce85cd58f289a6"
 dependencies = [
  "cipher",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
-dependencies = [
- "libc",
-]
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 
 [[package]]
 name = "cexpr"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
 dependencies = [
@@ -241,25 +227,24 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.34"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bc015644b92d5890fab7489e49d21f879d5c990186827d42ec511919404f38b"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
- "serde",
  "wasm-bindgen",
- "windows-targets 0.52.0",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "ciborium"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42e69ffd6f0917f5c029256a24d0161db17cea3997d185db0d35926308770f0e"
@@ -293,59 +278,49 @@
 dependencies = [
  "crypto-common",
  "inout",
 ]
 
 [[package]]
 name = "clang-sys"
-version = "1.7.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67523a3b4be3ce1989d607a828d036249522dd9c1c8de7f4dd2dae43a37369d1"
+checksum = "0b023947811758c97c59bf9d1c188fd619ad4718dcaa767947df1cadb14f39f4"
 dependencies = [
  "glob",
  "libc",
  "libloading",
 ]
 
 [[package]]
 name = "clap"
-version = "4.5.1"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c918d541ef2913577a0f9566e9ce27cb35b6df072075769e0b26cb5a554520da"
+checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
 dependencies = [
  "clap_builder",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.5.1"
+version = "4.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f3e7391dad68afb0c2ede1bf619f579a3dc9c2ec67f089baa397123a2f3d1eb"
+checksum = "ae129e2e766ae0ec03484e609954119f123cc1fe650337e155d03b022f24f7b4"
 dependencies = [
  "anstyle",
  "clap_lex",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
 
 [[package]]
-name = "core-foundation"
-version = "0.9.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "91e195e091a93c46f7102ec7818a2aa394e1e1771c3ab4825963fa03e45afb8f"
-dependencies = [
- "core-foundation-sys",
- "libc",
-]
-
-[[package]]
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "cpufeatures"
@@ -354,17 +329,17 @@
 checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc"
-version = "3.2.0"
+version = "3.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2b432c56615136f8dba245fed7ec3d5518c500a31108661067e61e72fe7e6bc"
+checksum = "69e6e4d7b33a94f0991c26729976b10ebde1d34c3ee82408fb536164fa10d636"
 dependencies = [
  "crc-catalog",
 ]
 
 [[package]]
 name = "crc-catalog"
 version = "2.4.0"
@@ -426,17 +401,17 @@
 checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.19"
+version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+checksum = "22ec99545bb0ed0ea7bb9b8e1e9122ea386ff8a48c0922e43f36d45ab09e0e80"
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
@@ -489,33 +464,18 @@
 dependencies = [
  "block-buffer",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
-name = "doc-comment"
-version = "0.3.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
-
-[[package]]
 name = "either"
-version = "1.10.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
-
-[[package]]
-name = "encoding_rs"
-version = "0.8.33"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
-dependencies = [
- "cfg-if",
-]
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
 name = "env_logger"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4cd405aab171cb85d6735e5c8d9db038c17d3ca007a4d2c25f337935c3d90580"
 dependencies = [
@@ -530,41 +490,35 @@
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
-version = "0.3.8"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
+checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.1"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
-name = "fnv"
-version = "1.0.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
-
-[[package]]
 name = "form_urlencoded"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
@@ -635,15 +589,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -708,73 +662,54 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.28.1"
+version = "0.29.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
+checksum = "40ecd4077b5ae9fd2e9e169b102c6c330d0605168eb0e8bf79952b256dbefffd"
 
 [[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
-name = "h2"
-version = "0.3.24"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb2c4422095b67ee78da96fbb51a4cc413b3b25883c7717ff7ca1ab31022c9c9"
-dependencies = [
- "bytes",
- "fnv",
- "futures-core",
- "futures-sink",
- "futures-util",
- "http",
- "indexmap",
- "slab",
- "tokio",
- "tokio-util",
- "tracing",
-]
-
-[[package]]
 name = "half"
-version = "2.3.1"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc52e53916c08643f1b56ec082790d1e86a32e58dc5268f897f313fbae7b4872"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
 dependencies = [
  "cfg-if",
  "crunchy",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "hdfs-native"
-version = "0.9.2"
+version = "0.9.3"
 dependencies = [
  "aes",
  "base64",
  "bytes",
  "cbc",
  "chrono",
  "cipher",
@@ -809,35 +744,16 @@
  "url",
  "users",
  "uuid",
  "which",
 ]
 
 [[package]]
-name = "hdfs-native-object-store"
-version = "0.9.2"
-dependencies = [
- "async-trait",
- "bytes",
- "chrono",
- "criterion",
- "env_logger",
- "futures",
- "hdfs-native",
- "object_store",
- "serial_test",
- "tempfile",
- "thiserror",
- "tokio",
- "which",
-]
-
-[[package]]
 name = "hdfs-native-python"
-version = "0.9.2"
+version = "0.9.3"
 dependencies = [
  "bytes",
  "env_logger",
  "hdfs-native",
  "log",
  "pyo3",
  "thiserror",
@@ -847,18 +763,24 @@
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
+name = "heck"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
+
+[[package]]
 name = "hermit-abi"
-version = "0.3.6"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd5256b483761cd23699d0da46cc6fd2ee3be420bbe6d020ae4a091e70b7e9fd"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
@@ -877,92 +799,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3d1354bf6b7235cb4a0576c2619fd4ed18183f689b12b006a0ee7329eeff9a5"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
-name = "http"
-version = "0.2.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8947b1a6fad4393052c7ba1f4cd97bed3e953a95c79c92ad9b051a04611d9fbb"
-dependencies = [
- "bytes",
- "fnv",
- "itoa",
-]
-
-[[package]]
-name = "http-body"
-version = "0.4.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ceab25649e9960c0311ea418d17bee82c0dcec1bd053b5f9a66e265a693bed2"
-dependencies = [
- "bytes",
- "http",
- "pin-project-lite",
-]
-
-[[package]]
-name = "httparse"
-version = "1.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
-
-[[package]]
-name = "httpdate"
-version = "1.0.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df3b46402a9d5adb4c86a0cf463f42e19994e3ee891101b1841f30a545cb49a9"
-
-[[package]]
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
-name = "hyper"
-version = "0.14.28"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
-dependencies = [
- "bytes",
- "futures-channel",
- "futures-core",
- "futures-util",
- "h2",
- "http",
- "http-body",
- "httparse",
- "httpdate",
- "itoa",
- "pin-project-lite",
- "socket2",
- "tokio",
- "tower-service",
- "tracing",
- "want",
-]
-
-[[package]]
-name = "hyper-rustls"
-version = "0.24.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec3efd23720e2049821a693cbc7e65ea87c72f1c58ff2f9522ff332b1491e590"
-dependencies = [
- "futures-util",
- "http",
- "hyper",
- "rustls",
- "tokio",
- "tokio-rustls",
-]
-
-[[package]]
 name = "iana-time-zone"
 version = "0.1.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
@@ -989,45 +839,39 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.2.3"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "233cf39063f058ea2caae4091bf4a3ef70a653afbc026f5c4a4135d114e3c177"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "inout"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0c10553d664a4d0bcff9f4215d0aac67a639cc68ef660840afe309b807bc9f5"
 dependencies = [
  "block-padding",
  "generic-array",
 ]
 
 [[package]]
-name = "ipnet"
-version = "2.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f518f335dce6725a761382244631d86cf0ccb2863413590b31338feb467f9c3"
-
-[[package]]
 name = "is-terminal"
 version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
 dependencies = [
  "hermit-abi",
  "libc",
@@ -1041,41 +885,32 @@
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itertools"
-version = "0.11.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
-dependencies = [
- "either",
-]
-
-[[package]]
-name = "itertools"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "js-sys"
-version = "0.3.68"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "406cda4b368d531c842222cf9d2600a9a4acce8d29423695379c6868a143a9ee"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
@@ -1086,148 +921,144 @@
 name = "lazycell"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libgssapi"
-version = "0.7.0"
-source = "git+https://github.com/Kimahriman/libgssapi.git?branch=raw-slice-panic#9e235de9b00776a8fb21b574e32dcbe2a673cf34"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c502363cc9845707a9b9fa938b732111fa7d7a4e518ebda8e46c5a1471192a15"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "bytes",
  "lazy_static",
  "libgssapi-sys",
 ]
 
 [[package]]
 name = "libgssapi-sys"
 version = "0.3.1"
-source = "git+https://github.com/Kimahriman/libgssapi.git?branch=raw-slice-panic#9e235de9b00776a8fb21b574e32dcbe2a673cf34"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b57d9a71c774ec53b1b9119dbbcc589b5209831f0ddc0ff4210640051f545372"
 dependencies = [
  "bindgen 0.69.4",
  "pkg-config",
 ]
 
 [[package]]
 name = "libloading"
-version = "0.8.1"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c571b676ddfc9a8c12f1f3d3085a7b163966a8fd8098a90640953ce5f6170161"
+checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
- "windows-sys 0.48.0",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.13"
+version = "0.4.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
+checksum = "78b3ae25bc7c8c38cec158d1f2757ee79e9b3740fbc7ccf0e59e4b08d793fa89"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "md-5"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d89e7ee0cfbedfc4da3340218492196241d89eefb6dab27de5df917a6d2e78cf"
 dependencies = [
  "cfg-if",
  "digest",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
-name = "mime"
-version = "0.3.17"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
-
-[[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.2"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
+checksum = "87dfd01fe195c66b572b37921ad8803d010623c0aca821bea2302239d155cdae"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.10"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f3d0b296e374a4e6f3c7b0a1f5a51d748a0d34c85e7dc48fc3fa9a87657fe09"
+checksum = "a4a650543ca06a924e8b371db273b2756685faae30f8487da1b56505a8f78b0c"
 dependencies = [
  "libc",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "multimap"
-version = "0.8.3"
+version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5ce46fe64a9d73be07dcbe690a38ce1b293be448fd8ce1e6c1b8062c9f72c6a"
+checksum = "defc4c55412d89136f966bbb339008b474350e5e6e78d2714439c386b3137a03"
 
 [[package]]
 name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
@@ -1236,89 +1067,54 @@
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "object"
-version = "0.32.2"
+version = "0.35.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
+checksum = "b8ec7ab813848ba4522158d5517a6093db1ded27575b070f4177b8d12b41db5e"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
-name = "object_store"
-version = "0.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d139f545f64630e2e3688fd9f81c470888ab01edeb72d13b4e86c566f1130000"
-dependencies = [
- "async-trait",
- "base64",
- "bytes",
- "chrono",
- "futures",
- "humantime",
- "hyper",
- "itertools 0.12.1",
- "parking_lot",
- "percent-encoding",
- "quick-xml",
- "rand",
- "reqwest",
- "ring",
- "serde",
- "serde_json",
- "snafu",
- "tokio",
- "tracing",
- "url",
- "walkdir",
-]
-
-[[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
-name = "openssl-probe"
-version = "0.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
-
-[[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "peeking_take_while"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
@@ -1327,27 +1123,27 @@
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "petgraph"
-version = "0.6.4"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1d3afd2628e69da2be385eb6f2fd57c8ac7977ceeff6dc166ff1657b0e386a9"
+checksum = "b4c5cc86750666a3ed20bdaf5ca2a0344f9c67674cae0515bec2da16fbaa47db"
 dependencies = [
  "fixedbitset",
  "indexmap",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
@@ -1355,115 +1151,120 @@
 name = "pkg-config"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
 name = "plotters"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
+checksum = "a15b6eccb8484002195a3e44fe65a4ce8e93a625797a063735536fd59cb01cf3"
 dependencies = [
  "num-traits",
  "plotters-backend",
  "plotters-svg",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "plotters-backend"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e76628b4d3a7581389a35d5b6e2139607ad7c75b17aed325f210aa91f4a9609"
+checksum = "414cec62c6634ae900ea1c56128dfe87cf63e7caece0852ec76aba307cebadb7"
 
 [[package]]
 name = "plotters-svg"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38f6d39893cca0701371e3c27294f09797214b86f1fb951b89ade8ec04e2abab"
+checksum = "81b30686a7d9c3e010b84284bdd26a29f2138574f52f5eb6f794fc0ad924e705"
 dependencies = [
  "plotters-backend",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "prettyplease"
-version = "0.2.16"
+version = "0.2.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a41cf62165e97c7f814d2221421dbb9afcbcdb0a88068e5ea206e19951c2cbb5"
+checksum = "5f12335488a2f3b0a83b14edad48dca9879ce89b2edd10e80237e4e852dd645e"
 dependencies = [
  "proc-macro2",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prost"
-version = "0.12.3"
+version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "146c289cda302b98a28d40c8b3b90498d6e526dd24ac2ecea73e4e491685b94a"
+checksum = "deb1435c188b76130da55f17a466d252ff7b1418b2ad3e037d127b94e3411f29"
 dependencies = [
  "bytes",
  "prost-derive",
 ]
 
 [[package]]
 name = "prost-build"
-version = "0.12.3"
+version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c55e02e35260070b6f716a2423c2ff1c3bb1642ddca6f99e1f26d06268a0e2d2"
+checksum = "22505a5c94da8e3b7c2996394d1c933236c4d743e81a410bcca4e6989fc066a4"
 dependencies = [
  "bytes",
- "heck",
- "itertools 0.11.0",
+ "heck 0.5.0",
+ "itertools 0.12.1",
  "log",
  "multimap",
  "once_cell",
  "petgraph",
  "prettyplease",
  "prost",
  "prost-types",
  "regex",
- "syn 2.0.50",
+ "syn 2.0.66",
  "tempfile",
- "which",
 ]
 
 [[package]]
 name = "prost-derive"
-version = "0.12.3"
+version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "efb6c9a1dd1def8e2124d17e83a20af56f1570d6c2d2bd9e266ccb768df3840e"
+checksum = "81bddcdb20abf9501610992b6759a4c888aef7d1a7247ef75e2404275ac24af1"
 dependencies = [
  "anyhow",
- "itertools 0.11.0",
+ "itertools 0.12.1",
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "prost-types"
-version = "0.12.3"
+version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "193898f59edcf43c26227dcd4c8427f00d99d61e95dcde58dabd49fa291d470e"
+checksum = "9091c90b0a32608e984ff2fa4091273cbdd755d54935c51d520887f4a1dbd5b0"
 dependencies = [
  "prost",
 ]
 
 [[package]]
 name = "protobuf-src"
 version = "1.1.0+21.5"
@@ -1471,88 +1272,80 @@
 checksum = "c7ac8852baeb3cc6fb83b93646fb93c0ffe5d14bf138c945ceb4b9948ee0e3c1"
 dependencies = [
  "autotools",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a89dc7a5850d0e983be1ec2a463a171d20990487c3cfcd68b5363f1ee3d6fe0"
+checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07426f0d8fe5a601f26293f300afd1a7b1ed5e78b2a705870c5f30893c5163be"
+checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb7dec17e17766b46bca4f1a4215a85006b4c2ecde122076c562dd058da6cf1"
+checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05f738b4e40d50b5711957f142878cfa0f28e054aa0ebdfc3fd137a843f74ed3"
+checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fc910d4851847827daf9d6cdd4a823fbdaab5b8818325c5e97a86da79e8881f"
+checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
- "heck",
+ "heck 0.4.1",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 2.0.50",
-]
-
-[[package]]
-name = "quick-xml"
-version = "0.31.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1004a344b30a54e2ee58d66a71b32d2db2feb0a31f9a2d302bf0536f15de2a33"
-dependencies = [
- "memchr",
- "serde",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1581,17 +1374,17 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.8.1"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa7237101a77a10773db45d62004a272517633fbcc3df19d96455ede1122e051"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -1601,286 +1394,131 @@
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bb987efffd3c6d0d8f5f89510bb458559eab11e4f869acb20bf845e016259cd"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
-
-[[package]]
-name = "reqwest"
-version = "0.11.24"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c6920094eb85afde5e4a138be3f2de8bbdf28000f0029e72c45025a56b042251"
-dependencies = [
- "base64",
- "bytes",
- "encoding_rs",
- "futures-core",
- "futures-util",
- "h2",
- "http",
- "http-body",
- "hyper",
- "hyper-rustls",
- "ipnet",
- "js-sys",
- "log",
- "mime",
- "once_cell",
- "percent-encoding",
- "pin-project-lite",
- "rustls",
- "rustls-native-certs",
- "rustls-pemfile",
- "serde",
- "serde_json",
- "serde_urlencoded",
- "sync_wrapper",
- "system-configuration",
- "tokio",
- "tokio-rustls",
- "tokio-util",
- "tower-service",
- "url",
- "wasm-bindgen",
- "wasm-bindgen-futures",
- "wasm-streams",
- "web-sys",
- "winreg",
-]
-
-[[package]]
-name = "ring"
-version = "0.17.8"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c17fa4cb658e3583423e915b9f3acc01cceaee1860e33d59ebae66adc3a2dc0d"
-dependencies = [
- "cc",
- "cfg-if",
- "getrandom",
- "libc",
- "spin",
- "untrusted",
- "windows-sys 0.52.0",
-]
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "roxmltree"
 version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "862340e351ce1b271a378ec53f304a5558f7db87f3769dc655a8f6ecbb68b302"
 dependencies = [
  "xmlparser",
 ]
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.38.31"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
-name = "rustls"
-version = "0.21.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
-dependencies = [
- "log",
- "ring",
- "rustls-webpki",
- "sct",
-]
-
-[[package]]
-name = "rustls-native-certs"
-version = "0.6.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9aace74cb666635c918e9c12bc0d348266037aa8eb599b5cba565709a8dff00"
-dependencies = [
- "openssl-probe",
- "rustls-pemfile",
- "schannel",
- "security-framework",
-]
-
-[[package]]
-name = "rustls-pemfile"
-version = "1.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
-dependencies = [
- "base64",
-]
-
-[[package]]
-name = "rustls-webpki"
-version = "0.101.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
-dependencies = [
- "ring",
- "untrusted",
-]
-
-[[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
-name = "schannel"
-version = "0.1.23"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbc91545643bcf3a0bbb6569265615222618bdf33ce4ffbbd13c4bbd4c093534"
-dependencies = [
- "windows-sys 0.52.0",
-]
-
-[[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
-name = "sct"
-version = "0.7.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da046153aa2352493d6cb7da4b6e5c0c057d8a1d0a9aa8560baffdd945acd414"
-dependencies = [
- "ring",
- "untrusted",
-]
-
-[[package]]
-name = "security-framework"
-version = "2.9.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05b64fb303737d99b81884b2c63433e9ae28abebe5eb5045dcdd175dc2ecf4de"
-dependencies = [
- "bitflags 1.3.2",
- "core-foundation",
- "core-foundation-sys",
- "libc",
- "security-framework-sys",
-]
-
-[[package]]
-name = "security-framework-sys"
-version = "2.9.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e932934257d3b408ed8f30db49d85ea163bfe74961f017f405b025af298f0c7a"
-dependencies = [
- "core-foundation-sys",
- "libc",
-]
-
-[[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "7253ab4de971e72fb7be983802300c30b5a7f0c2e56fab8abfc6a214307c0094"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "500cbc0ebeb6f46627f50f3f5811ccf6bf00643be300b4c3eabc0ef55dc5b5ba"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
-dependencies = [
- "itoa",
- "ryu",
- "serde",
-]
-
-[[package]]
-name = "serde_urlencoded"
-version = "0.7.1"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
- "form_urlencoded",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serial_test"
@@ -1900,15 +1538,15 @@
 name = "serial_test_derive"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91d129178576168c589c9ec973feedf7d3126c01ac2bf08795109aa35b69fb8f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "shlex"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fda2ff0d084019ba4d7c6f371c95d8fd75ce3524c3cb8fb653a3023f6323e64"
@@ -1920,57 +1558,29 @@
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
-
-[[package]]
-name = "snafu"
-version = "0.7.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4de37ad025c587a29e8f3f5605c00f70b98715ef90b9061a815b9e59e9042d6"
-dependencies = [
- "doc-comment",
- "snafu-derive",
-]
-
-[[package]]
-name = "snafu-derive"
-version = "0.7.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "990079665f075b699031e9c08fd3ab99be5029b96f3b78dc0709e8f77e4efebf"
-dependencies = [
- "heck",
- "proc-macro2",
- "quote",
- "syn 1.0.109",
-]
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.5.5"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
-name = "spin"
-version = "0.9.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
-
-[[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "syn"
@@ -1981,61 +1591,34 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.50"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74f1bdc9872430ce9b75da68329d1c1746faf50ffac5f19e02b71e37ff881ffb"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "sync_wrapper"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
-
-[[package]]
-name = "system-configuration"
-version = "0.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba3a3adc5c275d719af8cb4272ea1c4a6d668a777f37e115f6d11ddbc1c8e0e7"
-dependencies = [
- "bitflags 1.3.2",
- "core-foundation",
- "system-configuration-sys",
-]
-
-[[package]]
-name = "system-configuration-sys"
-version = "0.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75fb188eb626b924683e3b95e3a48e63551fcfb51949de2f06a9d91dbee93c9"
-dependencies = [
- "core-foundation-sys",
- "libc",
-]
-
-[[package]]
 name = "target-lexicon"
-version = "0.12.13"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tempfile"
-version = "3.10.0"
+version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a365e8cd18e44762ef95d87f284f4b5cd04107fec2ff3052bd6a3e6069669e67"
+checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
  "cfg-if",
  "fastrand",
  "rustix",
  "windows-sys 0.52.0",
 ]
 
@@ -2046,30 +1629,30 @@
 checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.57"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e45bcbe8ed29775f228095caf2cd67af7a4ccf756ebff23a306bf3e8b47b24b"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.57"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a953cb265bef375dae3de6663da4d3804eee9682ea80d8e2542529b73c531c81"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "tinytemplate"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4d6b5f19ff7664e8c98d03e2139cb510db9b0a60b55f8e8709b689d939b6bc"
@@ -2091,108 +1674,41 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.36.0"
+version = "1.38.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61285f6515fa018fb2d1e46eb21223fff441ee8db5d0f1435e8ab4f5cdb80931"
+checksum = "ba4f4a02a7a80d6f274636f0aa95c7e383b912d41fe721a31f29e29698585a4a"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
  "socket2",
  "tokio-macros",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
+checksum = "5f5ae998a069d4b5aba8ee9dad856af7d520c3699e6159b185c2acd48155d39a"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
-]
-
-[[package]]
-name = "tokio-rustls"
-version = "0.24.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
-dependencies = [
- "rustls",
- "tokio",
-]
-
-[[package]]
-name = "tokio-util"
-version = "0.7.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
-dependencies = [
- "bytes",
- "futures-core",
- "futures-sink",
- "pin-project-lite",
- "tokio",
- "tracing",
+ "syn 2.0.66",
 ]
 
 [[package]]
-name = "tower-service"
-version = "0.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
-
-[[package]]
-name = "tracing"
-version = "0.1.40"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
-dependencies = [
- "pin-project-lite",
- "tracing-attributes",
- "tracing-core",
-]
-
-[[package]]
-name = "tracing-attributes"
-version = "0.1.27"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.50",
-]
-
-[[package]]
-name = "tracing-core"
-version = "0.1.32"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
-dependencies = [
- "once_cell",
-]
-
-[[package]]
-name = "try-lock"
-version = "0.2.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e421abadd41a4225275504ea4d6566923418b7f05506fbc9c0fe86ba7396114b"
-
-[[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
 name = "unicode-bidi"
@@ -2204,34 +1720,28 @@
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
-name = "untrusted"
-version = "0.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
-
-[[package]]
 name = "url"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31e6302e3bb753d46e83516cae55ae196fc0c309407cf11ab35cc51a4c2a4633"
 dependencies = [
  "form_urlencoded",
  "idna",
@@ -2245,136 +1755,102 @@
 checksum = "24cc0f6d6f267b73e5a2cadf007ba8f9bc39c6a6f9666f8cf25ea809a153b032"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.7.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f00cc9702ca12d3c81455259621e676d0f7251cec66a21e98fe2e9a37db93b2a"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d71d857dc86794ca4c280d616f7da00d2dbfd8cd788846559a6813e6aa4b54ee"
+checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
-name = "want"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
-dependencies = [
- "try-lock",
-]
-
-[[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1e124130aee3fb58c5bdd6b639a0509486b0338acaaae0c84a5124b0f588b7f"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c9e7e1900c352b609c8488ad12639a311045f40a35491fb69ba8c12f758af70b"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
-name = "wasm-bindgen-futures"
-version = "0.4.41"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "877b9c3f61ceea0e56331985743b13f3d25c406a7098d45180fb5f09bc19ed97"
-dependencies = [
- "cfg-if",
- "js-sys",
- "wasm-bindgen",
- "web-sys",
-]
-
-[[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b30af9e2d358182b5c7449424f017eba305ed32a7010509ede96cdc4696c46ed"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "642f325be6301eb8107a83d12a8ac6c1e1c54345a7ef1a9261962dfefda09e66"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.50",
+ "syn 2.0.66",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f186bd2dcf04330886ce82d6f33dd75a7bfcf69ecf5763b89fcde53b6ac9838"
-
-[[package]]
-name = "wasm-streams"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b65dc4c90b63b118468cf747d8bf3566c1913ef60be765b5730ead9e0a3ba129"
-dependencies = [
- "futures-util",
- "js-sys",
- "wasm-bindgen",
- "wasm-bindgen-futures",
- "web-sys",
-]
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "web-sys"
-version = "0.3.68"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96565907687f7aceb35bc5fc03770a8a0471d82e479f25832f54a0e3f4b28446"
+checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "which"
@@ -2385,51 +1861,29 @@
  "either",
  "home",
  "once_cell",
  "rustix",
 ]
 
 [[package]]
-name = "winapi"
-version = "0.3.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
-dependencies = [
- "winapi-i686-pc-windows-gnu",
- "winapi-x86_64-pc-windows-gnu",
-]
-
-[[package]]
-name = "winapi-i686-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
-
-[[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
-name = "winapi-x86_64-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
-
-[[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
@@ -2439,15 +1893,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -2459,119 +1913,116 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.0",
- "windows_aarch64_msvc 0.52.0",
- "windows_i686_gnu 0.52.0",
- "windows_i686_msvc 0.52.0",
- "windows_x86_64_gnu 0.52.0",
- "windows_x86_64_gnullvm 0.52.0",
- "windows_x86_64_msvc 0.52.0",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
-
-[[package]]
-name = "winreg"
-version = "0.50.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
-dependencies = [
- "cfg-if",
- "windows-sys 0.48.0",
-]
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "xmlparser"
 version = "0.13.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "66fee0b777b0f5ac1c69bb06d361268faafa61cd4682ae064a171c16c433e9e4"
```

### Comparing `hdfs_native-0.9.2/pyproject.toml` & `hdfs_native-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/python/hdfs_native/__init__.py` & `hdfs_native-0.9.3/python/hdfs_native/__init__.py`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/python/hdfs_native/_internal.pyi` & `hdfs_native-0.9.3/python/hdfs_native/_internal.pyi`

 * *Files identical despite different names*

### Comparing `hdfs_native-0.9.2/PKG-INFO` & `hdfs_native-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hdfs-native
-Version: 0.9.2
+Version: 0.9.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: typing-extensions
 Summary: Python bindings for hdfs-native Rust library
 Keywords: hadoop,hdfs
 Home-Page: https://github.com/Kimahriman/hdfs-native
```
