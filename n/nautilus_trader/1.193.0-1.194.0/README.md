# Comparing `tmp/nautilus_trader-1.193.0.tar.gz` & `tmp/nautilus_trader-1.194.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautilus_trader-1.193.0.tar", max compression
+gzip compressed data, was "nautilus_trader-1.194.0.tar", max compression
```

## Comparing `nautilus_trader-1.193.0.tar` & `nautilus_trader-1.194.0.tar`

### file list

```diff
@@ -1,1129 +1,1132 @@
--rw-r--r--   0        0        0     7651 2024-05-24 12:14:01.313010 nautilus_trader-1.193.0/LICENSE
--rw-r--r--   0        0        0    25213 2024-05-24 12:14:01.313010 nautilus_trader-1.193.0/README.md
--rw-r--r--   0        0        0    12823 2024-05-24 12:14:01.313010 nautilus_trader-1.193.0/build.py
--rw-r--r--   0        0        0      663 2024-05-24 12:14:01.325010 nautilus_trader-1.193.0/nautilus_core/.cargo/config.toml
--rw-r--r--   0        0        0   135456 2024-05-24 12:14:01.325010 nautilus_trader-1.193.0/nautilus_core/Cargo.lock
--rw-r--r--   0        0        0     2305 2024-05-24 12:14:01.325010 nautilus_trader-1.193.0/nautilus_core/Cargo.toml
--rw-r--r--   0        0        0     7652 2024-05-24 12:14:01.325010 nautilus_trader-1.193.0/nautilus_core/LICENSE
--rw-r--r--   0        0        0     1248 2024-05-24 12:14:01.325010 nautilus_trader-1.193.0/nautilus_core/README.md
--rw-r--r--   0        0        0      967 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/Cargo.toml
--rw-r--r--   0        0        0     9225 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/account/base.rs
--rw-r--r--   0        0        0    20368 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/account/cash.rs
--rw-r--r--   0        0        0    22074 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/account/margin.rs
--rw-r--r--   0        0        0     1015 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/account/mod.rs
--rw-r--r--   0        0        0     2376 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/account/stubs.rs
--rw-r--r--   0        0        0     1673 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/lib.rs
--rw-r--r--   0        0        0     6160 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/python/cash.rs
--rw-r--r--   0        0        0     8441 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/python/margin.rs
--rw-r--r--   0        0        0     1557 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/python/mod.rs
--rw-r--r--   0        0        0     2609 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/python/transformer.rs
--rw-r--r--   0        0        0     2598 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/accounting/src/stubs.rs
--rw-r--r--   0        0        0     1669 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/Cargo.toml
--rw-r--r--   0        0        0     1217 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/bin/sandbox.rs
--rw-r--r--   0        0        0     2250 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/common.rs
--rw-r--r--   0        0        0    44341 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/decode.rs
--rw-r--r--   0        0        0     3482 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/enums.rs
--rw-r--r--   0        0        0    15981 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/live.rs
--rw-r--r--   0        0        0    11923 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/loader.rs
--rw-r--r--   0        0        0     1113 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/mod.rs
--rw-r--r--   0        0        0    10104 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/publishers.json
--rw-r--r--   0        0        0     5323 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/enums.rs
--rw-r--r--   0        0        0    19510 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/historical.rs
--rw-r--r--   0        0        0     8154 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/live.rs
--rw-r--r--   0        0        0    13415 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/loader.rs
--rw-r--r--   0        0        0     1702 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/mod.rs
--rw-r--r--   0        0        0     7715 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/types.rs
--rw-r--r--   0        0        0     6477 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/symbology.rs
--rw-r--r--   0        0        0       81 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.cbbo.dbn.zst
--rw-r--r--   0        0        0      693 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.definition.dbn.zst
--rw-r--r--   0        0        0      673 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.definition.v1.dbn.zst
--rw-r--r--   0        0        0      661 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.imbalance.dbn.zst
--rw-r--r--   0        0        0      465 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.mbo.dbn
--rw-r--r--   0        0        0      174 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.mbo.dbn.zst
--rw-r--r--   0        0        0      192 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.mbp-1.dbn.zst
--rw-r--r--   0        0        0      374 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.mbp-10.dbn.zst
--rw-r--r--   0        0        0      103 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.ohlcv-1d.dbn.zst
--rw-r--r--   0        0        0      186 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.ohlcv-1h.dbn.zst
--rw-r--r--   0        0        0      165 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.ohlcv-1m.dbn.zst
--rw-r--r--   0        0        0      157 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.ohlcv-1s.dbn.zst
--rw-r--r--   0        0        0      139 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.statistics.dbn.zst
--rw-r--r--   0        0        0      197 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.tbbo.dbn.zst
--rw-r--r--   0        0        0      173 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.trades.dbn.zst
--rw-r--r--   0        0        0     6857 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/types.rs
--rw-r--r--   0        0        0     1771 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/adapters/src/lib.rs
--rw-r--r--   0        0        0     1234 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/backtest/Cargo.toml
--rw-r--r--   0        0        0     2046 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/backtest/build.rs
--rw-r--r--   0        0        0      484 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/backtest/cbindgen.toml
--rw-r--r--   0        0        0      807 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/backtest/cbindgen_cython.toml
--rw-r--r--   0        0        0     6213 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/backtest/src/engine.rs
--rw-r--r--   0        0        0     1701 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/backtest/src/lib.rs
--rw-r--r--   0        0        0     8782 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/backtest/src/matching_engine.rs
--rw-r--r--   0        0        0      669 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/cli/Cargo.toml
--rw-r--r--   0        0        0     1289 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/cli/src/bin/cli.rs
--rw-r--r--   0        0        0      902 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/cli/src/database/mod.rs
--rw-r--r--   0        0        0     2258 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/cli/src/database/postgres.rs
--rw-r--r--   0        0        0     1198 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/cli/src/lib.rs
--rw-r--r--   0        0        0     2230 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/cli/src/opt.rs
--rw-r--r--   0        0        0       65 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/clippy.toml
--rw-r--r--   0        0        0     1611 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/common/Cargo.toml
--rw-r--r--   0        0        0     2759 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/common/build.rs
--rw-r--r--   0        0        0      548 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/common/cbindgen.toml
--rw-r--r--   0        0        0      823 2024-05-24 12:14:01.329010 nautilus_trader-1.193.0/nautilus_core/common/cbindgen_cython.toml
--rw-r--r--   0        0        0    96074 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/cache/core.rs
--rw-r--r--   0        0        0     8710 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/cache/database.rs
--rw-r--r--   0        0        0     1086 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/cache/mod.rs
--rw-r--r--   0        0        0    11713 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/clock.rs
--rw-r--r--   0        0        0     9339 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/enums.rs
--rw-r--r--   0        0        0     8014 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/factories.rs
--rw-r--r--   0        0        0    12261 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/ffi/clock.rs
--rw-r--r--   0        0        0     3086 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/ffi/enums.rs
--rw-r--r--   0        0        0     5911 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/ffi/logging.rs
--rw-r--r--   0        0        0     1014 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/ffi/mod.rs
--rw-r--r--   0        0        0     1771 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/ffi/timer.rs
--rw-r--r--   0        0        0     5028 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/generators/client_order_id.rs
--rw-r--r--   0        0        0     1380 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/generators/mod.rs
--rw-r--r--   0        0        0     4982 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/generators/order_list_id.rs
--rw-r--r--   0        0        0     5582 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/generators/position_id.rs
--rw-r--r--   0        0        0     3412 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/handlers.rs
--rw-r--r--   0        0        0     2956 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/interface/account.rs
--rw-r--r--   0        0        0      977 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/interface/mod.rs
--rw-r--r--   0        0        0     2065 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/lib.rs
--rw-r--r--   0        0        0     7640 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/logging/headers.rs
--rw-r--r--   0        0        0    23893 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/logging/logger.rs
--rw-r--r--   0        0        0     5414 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/logging/mod.rs
--rw-r--r--   0        0        0     7744 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/logging/writer.rs
--rw-r--r--   0        0        0    20886 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/msgbus/core.rs
--rw-r--r--   0        0        0     1664 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/msgbus/database.rs
--rw-r--r--   0        0        0     1046 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/msgbus/mod.rs
--rw-r--r--   0        0        0     5841 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/python/clock.rs
--rw-r--r--   0        0        0     4513 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/python/enums.rs
--rw-r--r--   0        0        0     4896 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/python/logging.rs
--rw-r--r--   0        0        0     1999 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/python/mod.rs
--rw-r--r--   0        0        0     3479 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/python/timer.rs
--rw-r--r--   0        0        0     2848 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/python/versioning.rs
--rw-r--r--   0        0        0     1717 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/runtime.rs
--rw-r--r--   0        0        0     1374 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/stubs.rs
--rw-r--r--   0        0        0     2496 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/testing.rs
--rw-r--r--   0        0        0    17675 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/timer.rs
--rw-r--r--   0        0        0     5943 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/common/src/xrate.rs
--rw-r--r--   0        0        0      850 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/Cargo.toml
--rw-r--r--   0        0        0     2755 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/build.rs
--rw-r--r--   0        0        0      717 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/cbindgen.toml
--rw-r--r--   0        0        0      824 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/cbindgen_cython.toml
--rw-r--r--   0        0        0    18382 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/correctness.rs
--rw-r--r--   0        0        0     9172 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/datetime.rs
--rw-r--r--   0        0        0     2799 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/deserialization.rs
--rw-r--r--   0        0        0     1156 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/equality.rs
--rw-r--r--   0        0        0     5695 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/ffi/cvec.rs
--rw-r--r--   0        0        0     1248 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/ffi/datetime.rs
--rw-r--r--   0        0        0     1031 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/ffi/mod.rs
--rw-r--r--   0        0        0     8229 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/ffi/parsing.rs
--rw-r--r--   0        0        0     6642 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/ffi/string.rs
--rw-r--r--   0        0        0     3986 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/ffi/uuid.rs
--rw-r--r--   0        0        0     1924 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/lib.rs
--rw-r--r--   0        0        0     1409 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/message.rs
--rw-r--r--   0        0        0     8197 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/nanos.rs
--rw-r--r--   0        0        0     3425 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/parsing.rs
--rw-r--r--   0        0        0     1067 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/python/casing.rs
--rw-r--r--   0        0        0     2691 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/python/datetime.rs
--rw-r--r--   0        0        0     2894 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/python/mod.rs
--rw-r--r--   0        0        0     1407 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/python/serialization.rs
--rw-r--r--   0        0        0     3120 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/python/uuid.rs
--rw-r--r--   0        0        0     1814 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/serialization.rs
--rw-r--r--   0        0        0     8831 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/time.rs
--rw-r--r--   0        0        0     6040 2024-05-24 12:14:01.333010 nautilus_trader-1.193.0/nautilus_core/core/src/uuid.rs
--rw-r--r--   0        0        0     1371 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/Cargo.toml
--rw-r--r--   0        0        0     6813 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/client.rs
--rw-r--r--   0        0        0     8306 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/engine.rs
--rw-r--r--   0        0        0     1733 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/lib.rs
--rw-r--r--   0        0        0    18827 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/matching_core.rs
--rw-r--r--   0        0        0     2761 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/messages/cancel.rs
--rw-r--r--   0        0        0     2581 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/messages/cancel_all.rs
--rw-r--r--   0        0        0     2561 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/messages/cancel_batch.rs
--rw-r--r--   0        0        0     2809 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/messages/mod.rs
--rw-r--r--   0        0        0     3416 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/messages/modify.rs
--rw-r--r--   0        0        0     2757 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/messages/query.rs
--rw-r--r--   0        0        0     3171 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/messages/submit.rs
--rw-r--r--   0        0        0     3214 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/execution/src/messages/submit_list.rs
--rw-r--r--   0        0        0      746 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/Cargo.toml
--rw-r--r--   0        0        0     8897 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/ama.rs
--rw-r--r--   0        0        0     6979 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/dema.rs
--rw-r--r--   0        0        0     6902 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/ema.rs
--rw-r--r--   0        0        0     8322 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/hma.rs
--rw-r--r--   0        0        0     2875 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/mod.rs
--rw-r--r--   0        0        0     6925 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/rma.rs
--rw-r--r--   0        0        0     6142 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/sma.rs
--rw-r--r--   0        0        0     7476 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/vidya.rs
--rw-r--r--   0        0        0     7727 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/average/wma.rs
--rw-r--r--   0        0        0     6332 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/book/imbalance.rs
--rw-r--r--   0        0        0      940 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/book/mod.rs
--rw-r--r--   0        0        0     3206 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/indicator.rs
--rw-r--r--   0        0        0     1773 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/lib.rs
--rw-r--r--   0        0        0     7660 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/aroon.rs
--rw-r--r--   0        0        0     5019 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/bias.rs
--rw-r--r--   0        0        0     7008 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/cmo.rs
--rw-r--r--   0        0        0      970 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/mod.rs
--rw-r--r--   0        0        0     7876 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/rsi.rs
--rw-r--r--   0        0        0     2922 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/ama.rs
--rw-r--r--   0        0        0     2799 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/dema.rs
--rw-r--r--   0        0        0     2880 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/ema.rs
--rw-r--r--   0        0        0     2759 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/hma.rs
--rw-r--r--   0        0        0      976 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/mod.rs
--rw-r--r--   0        0        0     2865 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/rma.rs
--rw-r--r--   0        0        0     2765 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/sma.rs
--rw-r--r--   0        0        0     3101 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/vidya.rs
--rw-r--r--   0        0        0     2755 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/wma.rs
--rw-r--r--   0        0        0     2221 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/book/imbalance.rs
--rw-r--r--   0        0        0      903 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/book/mod.rs
--rw-r--r--   0        0        0     2217 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/mod.rs
--rw-r--r--   0        0        0     2901 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/aroon.rs
--rw-r--r--   0        0        0     2682 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/bias.rs
--rw-r--r--   0        0        0     2748 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/cmo.rs
--rw-r--r--   0        0        0      939 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/mod.rs
--rw-r--r--   0        0        0     2583 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/rsi.rs
--rw-r--r--   0        0        0     2005 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/ratio/efficiency_ratio.rs
--rw-r--r--   0        0        0      910 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/ratio/mod.rs
--rw-r--r--   0        0        0     3005 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/volatility/atr.rs
--rw-r--r--   0        0        0      897 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/python/volatility/mod.rs
--rw-r--r--   0        0        0     8102 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/ratio/efficiency_ratio.rs
--rw-r--r--   0        0        0      938 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/ratio/mod.rs
--rw-r--r--   0        0        0     5818 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/stubs.rs
--rw-r--r--   0        0        0     1509 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/testing.rs
--rw-r--r--   0        0        0     9258 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/volatility/atr.rs
--rw-r--r--   0        0        0      930 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/indicators/src/volatility/mod.rs
--rw-r--r--   0        0        0     1527 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/Cargo.toml
--rw-r--r--   0        0        0     1855 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/lib.rs
--rw-r--r--   0        0        0     1430 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/mod.rs
--rw-r--r--   0        0        0     3422 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/redis/cache.rs
--rw-r--r--   0        0        0     1065 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/redis/mod.rs
--rw-r--r--   0        0        0     1960 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/redis/msgbus.rs
--rw-r--r--   0        0        0     6622 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/sql/cache_database.rs
--rw-r--r--   0        0        0      908 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/sql/mod.rs
--rw-r--r--   0        0        0    21364 2024-05-24 12:14:01.337010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/redis/cache.rs
--rw-r--r--   0        0        0    10578 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/redis/mod.rs
--rw-r--r--   0        0        0     7063 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/redis/msgbus.rs
--rw-r--r--   0        0        0    11599 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/cache_database.rs
--rw-r--r--   0        0        0     1137 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/mod.rs
--rw-r--r--   0        0        0      987 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/general.rs
--rw-r--r--   0        0        0    26965 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/instruments.rs
--rw-r--r--   0        0        0      953 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/mod.rs
--rw-r--r--   0        0        0    19284 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/orders.rs
--rw-r--r--   0        0        0     1805 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/types.rs
--rw-r--r--   0        0        0    10685 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/pg.rs
--rw-r--r--   0        0        0    18517 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/queries.rs
--rw-r--r--   0        0        0    13104 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/infrastructure/tests/test_cache_database_postgres.rs
--rw-r--r--   0        0        0     1430 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/Cargo.toml
--rw-r--r--   0        0        0      400 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/benches/criterion_fixed_precision_benchmark.rs
--rw-r--r--   0        0        0      225 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/benches/iai_fixed_precision_benchmark.rs
--rw-r--r--   0        0        0     2757 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/build.rs
--rw-r--r--   0        0        0     1617 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/cbindgen.toml
--rw-r--r--   0        0        0     1839 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/cbindgen_cython.toml
--rw-r--r--   0        0        0    33910 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/currencies.rs
--rw-r--r--   0        0        0    16919 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/bar.rs
--rw-r--r--   0        0        0     8316 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/delta.rs
--rw-r--r--   0        0        0     8465 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/deltas.rs
--rw-r--r--   0        0        0    11159 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/depth.rs
--rw-r--r--   0        0        0     3040 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/mod.rs
--rw-r--r--   0        0        0     6445 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/order.rs
--rw-r--r--   0        0        0     8044 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/quote.rs
--rw-r--r--   0        0        0     9402 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/stubs.rs
--rw-r--r--   0        0        0     6693 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/data/trade.rs
--rw-r--r--   0        0        0    30931 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/enums.rs
--rw-r--r--   0        0        0      940 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/account/mod.rs
--rw-r--r--   0        0        0     4946 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/account/state.rs
--rw-r--r--   0        0        0     4078 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/account/stubs.rs
--rw-r--r--   0        0        0     1012 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/mod.rs
--rw-r--r--   0        0        0     7811 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/accepted.rs
--rw-r--r--   0        0        0     8419 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/cancel_rejected.rs
--rw-r--r--   0        0        0     7695 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/canceled.rs
--rw-r--r--   0        0        0     7190 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/denied.rs
--rw-r--r--   0        0        0     7034 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/emulated.rs
--rw-r--r--   0        0        0     5516 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/event.rs
--rw-r--r--   0        0        0     8131 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/expired.rs
--rw-r--r--   0        0        0    11711 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/filled.rs
--rw-r--r--   0        0        0    18687 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/initialized.rs
--rw-r--r--   0        0        0     3888 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/mod.rs
--rw-r--r--   0        0        0     8402 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/modify_rejected.rs
--rw-r--r--   0        0        0     8063 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/pending_cancel.rs
--rw-r--r--   0        0        0     8081 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/pending_update.rs
--rw-r--r--   0        0        0     7761 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/rejected.rs
--rw-r--r--   0        0        0     7291 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/released.rs
--rw-r--r--   0        0        0    11494 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/stubs.rs
--rw-r--r--   0        0        0     7334 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/submitted.rs
--rw-r--r--   0        0        0     8180 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/triggered.rs
--rw-r--r--   0        0        0     9016 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/order/updated.rs
--rw-r--r--   0        0        0     1987 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/position/changed.rs
--rw-r--r--   0        0        0     2106 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/position/closed.rs
--rw-r--r--   0        0        0     1200 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/position/mod.rs
--rw-r--r--   0        0        0     1791 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/position/opened.rs
--rw-r--r--   0        0        0     1985 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/events/position/state.rs
--rw-r--r--   0        0        0     6050 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/bar.rs
--rw-r--r--   0        0        0     1845 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/delta.rs
--rw-r--r--   0        0        0     3549 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/deltas.rs
--rw-r--r--   0        0        0     3787 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/depth.rs
--rw-r--r--   0        0        0      988 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/mod.rs
--rw-r--r--   0        0        0     2417 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/order.rs
--rw-r--r--   0        0        0     2745 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/quote.rs
--rw-r--r--   0        0        0     2203 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/trade.rs
--rw-r--r--   0        0        0    15015 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/enums.rs
--rw-r--r--   0        0        0      899 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/events/mod.rs
--rw-r--r--   0        0        0     4681 2024-05-24 12:14:01.341010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/events/order.rs
--rw-r--r--   0        0        0     3279 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/account_id.rs
--rw-r--r--   0        0        0     2234 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/client_id.rs
--rw-r--r--   0        0        0     1398 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/client_order_id.rs
--rw-r--r--   0        0        0     1381 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/component_id.rs
--rw-r--r--   0        0        0     1412 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/exec_algorithm_id.rs
--rw-r--r--   0        0        0     4223 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/instrument_id.rs
--rw-r--r--   0        0        0     1177 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/mod.rs
--rw-r--r--   0        0        0     1384 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/order_list_id.rs
--rw-r--r--   0        0        0     1374 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/position_id.rs
--rw-r--r--   0        0        0     1374 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/strategy_id.rs
--rw-r--r--   0        0        0     1343 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/symbol.rs
--rw-r--r--   0        0        0     1603 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/trade_id.rs
--rw-r--r--   0        0        0     1360 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/trader_id.rs
--rw-r--r--   0        0        0     2003 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/venue.rs
--rw-r--r--   0        0        0     1391 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/venue_order_id.rs
--rw-r--r--   0        0        0      903 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/instruments/mod.rs
--rw-r--r--   0        0        0     5668 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/instruments/synthetic.rs
--rw-r--r--   0        0        0     1073 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/mod.rs
--rw-r--r--   0        0        0     8567 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/orderbook/book.rs
--rw-r--r--   0        0        0     3621 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/orderbook/level.rs
--rw-r--r--   0        0        0      913 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/orderbook/mod.rs
--rw-r--r--   0        0        0     5719 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/currency.rs
--rw-r--r--   0        0        0      950 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/mod.rs
--rw-r--r--   0        0        0     1596 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/money.rs
--rw-r--r--   0        0        0     1589 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/price.rs
--rw-r--r--   0        0        0     1845 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/quantity.rs
--rw-r--r--   0        0        0     4561 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/account_id.rs
--rw-r--r--   0        0        0     2846 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/client_id.rs
--rw-r--r--   0        0        0     4794 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/client_order_id.rs
--rw-r--r--   0        0        0     2897 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/component_id.rs
--rw-r--r--   0        0        0     2899 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/exec_algorithm_id.rs
--rw-r--r--   0        0        0     4866 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/instrument_id.rs
--rw-r--r--   0        0        0     1909 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/macros.rs
--rw-r--r--   0        0        0     3032 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/mod.rs
--rw-r--r--   0        0        0     2899 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/order_list_id.rs
--rw-r--r--   0        0        0     2874 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/position_id.rs
--rw-r--r--   0        0        0     4369 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/strategy_id.rs
--rw-r--r--   0        0        0     4518 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/stubs.rs
--rw-r--r--   0        0        0     3053 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/symbol.rs
--rw-r--r--   0        0        0     4233 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/trade_id.rs
--rw-r--r--   0        0        0     3598 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/trader_id.rs
--rw-r--r--   0        0        0     3604 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/venue.rs
--rw-r--r--   0        0        0     2905 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/venue_order_id.rs
--rw-r--r--   0        0        0    11059 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/any.rs
--rw-r--r--   0        0        0     7700 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/crypto_future.rs
--rw-r--r--   0        0        0     7750 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/crypto_perpetual.rs
--rw-r--r--   0        0        0     7499 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/currency_pair.rs
--rw-r--r--   0        0        0     6626 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/equity.rs
--rw-r--r--   0        0        0     7324 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/futures_contract.rs
--rw-r--r--   0        0        0     7448 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/futures_spread.rs
--rw-r--r--   0        0        0     5480 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/mod.rs
--rw-r--r--   0        0        0     7574 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/options_contract.rs
--rw-r--r--   0        0        0     7439 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/options_spread.rs
--rw-r--r--   0        0        0    13302 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/stubs.rs
--rw-r--r--   0        0        0     6493 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/instruments/synthetic.rs
--rw-r--r--   0        0        0     2074 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/lib.rs
--rw-r--r--   0        0        0     1595 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/macros.rs
--rw-r--r--   0        0        0     3536 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/aggregation.rs
--rw-r--r--   0        0        0     4309 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/analysis.rs
--rw-r--r--   0        0        0    23019 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/book.rs
--rw-r--r--   0        0        0     2836 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/display.rs
--rw-r--r--   0        0        0     1988 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/error.rs
--rw-r--r--   0        0        0    22495 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/ladder.rs
--rw-r--r--   0        0        0    13057 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/level.rs
--rw-r--r--   0        0        0     1067 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/mod.rs
--rw-r--r--   0        0        0    24817 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/any.rs
--rw-r--r--   0        0        0    31687 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/base.rs
--rw-r--r--   0        0        0     9307 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/default.rs
--rw-r--r--   0        0        0    14285 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/limit.rs
--rw-r--r--   0        0        0    11226 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/limit_if_touched.rs
--rw-r--r--   0        0        0     4555 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/list.rs
--rw-r--r--   0        0        0    11942 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/market.rs
--rw-r--r--   0        0        0    10843 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/market_if_touched.rs
--rw-r--r--   0        0        0    10035 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/market_to_limit.rs
--rw-r--r--   0        0        0     1270 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/mod.rs
--rw-r--r--   0        0        0    12288 2024-05-24 12:14:01.345010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/stop_limit.rs
--rw-r--r--   0        0        0    10817 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/stop_market.rs
--rw-r--r--   0        0        0     8366 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/stubs.rs
--rw-r--r--   0        0        0    11871 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/trailing_stop_limit.rs
--rw-r--r--   0        0        0    11317 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/orders/trailing_stop_market.rs
--rw-r--r--   0        0        0     3061 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/polymorphism.rs
--rw-r--r--   0        0        0    72892 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/position.rs
--rw-r--r--   0        0        0     7166 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/common.rs
--rw-r--r--   0        0        0    12321 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/data/bar.rs
--rw-r--r--   0        0        0    10587 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/data/delta.rs
--rw-r--r--   0        0        0     4435 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/data/deltas.rs
--rw-r--r--   0        0        0     8920 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/data/depth.rs
--rw-r--r--   0        0        0     3425 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/data/mod.rs
--rw-r--r--   0        0        0     5608 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/data/order.rs
--rw-r--r--   0        0        0    14445 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/data/quote.rs
--rw-r--r--   0        0        0    12629 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/data/trade.rs
--rw-r--r--   0        0        0    44501 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/enums.rs
--rw-r--r--   0        0        0      899 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/account/mod.rs
--rw-r--r--   0        0        0     6244 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/account/state.rs
--rw-r--r--   0        0        0      966 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/mod.rs
--rw-r--r--   0        0        0     3547 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/accepted.rs
--rw-r--r--   0        0        0     4036 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/cancel_rejected.rs
--rw-r--r--   0        0        0     3819 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/canceled.rs
--rw-r--r--   0        0        0     3297 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/denied.rs
--rw-r--r--   0        0        0     3110 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/emulated.rs
--rw-r--r--   0        0        0     3815 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/expired.rs
--rw-r--r--   0        0        0     7663 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/filled.rs
--rw-r--r--   0        0        0    11003 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/initialized.rs
--rw-r--r--   0        0        0     5587 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/mod.rs
--rw-r--r--   0        0        0     4047 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/modify_rejected.rs
--rw-r--r--   0        0        0     3710 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/pending_cancel.rs
--rw-r--r--   0        0        0     3710 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/pending_update.rs
--rw-r--r--   0        0        0     3570 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/rejected.rs
--rw-r--r--   0        0        0     3269 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/released.rs
--rw-r--r--   0        0        0     3259 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/submitted.rs
--rw-r--r--   0        0        0     3817 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/triggered.rs
--rw-r--r--   0        0        0     4457 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/updated.rs
--rw-r--r--   0        0        0     3628 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/identifiers/instrument_id.rs
--rw-r--r--   0        0        0     1993 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/identifiers/mod.rs
--rw-r--r--   0        0        0     3411 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/identifiers/trade_id.rs
--rw-r--r--   0        0        0     9563 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/crypto_future.rs
--rw-r--r--   0        0        0     9055 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/crypto_perpetual.rs
--rw-r--r--   0        0        0     8593 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/currency_pair.rs
--rw-r--r--   0        0        0     7022 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/equity.rs
--rw-r--r--   0        0        0     8544 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/futures_contract.rs
--rw-r--r--   0        0        0     8806 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/futures_spread.rs
--rw-r--r--   0        0        0     3614 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/mod.rs
--rw-r--r--   0        0        0     9059 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/options_contract.rs
--rw-r--r--   0        0        0     8804 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/options_spread.rs
--rw-r--r--   0        0        0     3531 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/macros.rs
--rw-r--r--   0        0        0     7351 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/mod.rs
--rw-r--r--   0        0        0     6786 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orderbook/book.rs
--rw-r--r--   0        0        0     2104 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orderbook/level.rs
--rw-r--r--   0        0        0      983 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orderbook/mod.rs
--rw-r--r--   0        0        0    22070 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/limit.rs
--rw-r--r--   0        0        0     4518 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/limit_if_touched.rs
--rw-r--r--   0        0        0    18609 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/market.rs
--rw-r--r--   0        0        0     4433 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/market_if_touched.rs
--rw-r--r--   0        0        0     4159 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/market_to_limit.rs
--rw-r--r--   0        0        0     4422 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/mod.rs
--rw-r--r--   0        0        0    22168 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/stop_limit.rs
--rw-r--r--   0        0        0     4412 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/stop_market.rs
--rw-r--r--   0        0        0     4750 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/trailing_stop_limit.rs
--rw-r--r--   0        0        0     4610 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/trailing_stop_market.rs
--rw-r--r--   0        0        0    12642 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/position.rs
--rw-r--r--   0        0        0     6219 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/types/balance.rs
--rw-r--r--   0        0        0     5123 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/types/currency.rs
--rw-r--r--   0        0        0     1062 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/types/mod.rs
--rw-r--r--   0        0        0    14239 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/types/money.rs
--rw-r--r--   0        0        0    14708 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/types/price.rs
--rw-r--r--   0        0        0    14615 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/python/types/quantity.rs
--rw-r--r--   0        0        0     5470 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/stubs.rs
--rw-r--r--   0        0        0     5786 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/types/balance.rs
--rw-r--r--   0        0        0     7530 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/types/currency.rs
--rw-r--r--   0        0        0     6622 2024-05-24 12:14:01.349010 nautilus_trader-1.193.0/nautilus_core/model/src/types/fixed.rs
--rw-r--r--   0        0        0     1118 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/model/src/types/mod.rs
--rw-r--r--   0        0        0    11756 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/model/src/types/money.rs
--rw-r--r--   0        0        0    14431 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/model/src/types/price.rs
--rw-r--r--   0        0        0    14504 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/model/src/types/quantity.rs
--rw-r--r--   0        0        0     1475 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/model/src/types/stubs.rs
--rw-r--r--   0        0        0     3064 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/model/src/venues.rs
--rw-r--r--   0        0        0     1036 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/Cargo.toml
--rw-r--r--   0        0        0     1655 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/benches/test_client.rs
--rw-r--r--   0        0        0     1374 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/benches/test_server.rs
--rw-r--r--   0        0        0    12459 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/http.rs
--rw-r--r--   0        0        0     1802 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/lib.rs
--rw-r--r--   0        0        0     1475 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/python/mod.rs
--rw-r--r--   0        0        0     6239 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/clock.rs
--rw-r--r--   0        0        0     5417 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/gcra.rs
--rw-r--r--   0        0        0     8865 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/mod.rs
--rw-r--r--   0        0        0     4079 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/nanos.rs
--rw-r--r--   0        0        0     9739 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/quota.rs
--rw-r--r--   0        0        0    23594 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/socket.rs
--rw-r--r--   0        0        0    28915 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/src/websocket.rs
--rw-r--r--   0        0        0       18 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/.gitignore
--rw-r--r--   0        0        0     2862 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/CHANGELOG.md
--rw-r--r--   0        0        0     2061 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/Cargo.toml
--rw-r--r--   0        0        0     1093 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/LICENSE
--rw-r--r--   0        0        0     2861 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/README.md
--rw-r--r--   0        0        0      268 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/rustfmt.toml
--rw-r--r--   0        0        0     6900 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/compat.rs
--rw-r--r--   0        0        0     2747 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/connect.rs
--rw-r--r--   0        0        0     5469 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/handshake.rs
--rw-r--r--   0        0        0    14303 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/lib.rs
--rw-r--r--   0        0        0     2854 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/stream.rs
--rw-r--r--   0        0        0     8647 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/tls.rs
--rw-r--r--   0        0        0     1300 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/Cargo.toml
--rw-r--r--   0        0        0     3658 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/benches/bench_persistence.rs
--rw-r--r--   0        0        0    12962 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/bar.rs
--rw-r--r--   0        0        0    15825 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/delta.rs
--rw-r--r--   0        0        0    41488 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/depth.rs
--rw-r--r--   0        0        0     4662 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/mod.rs
--rw-r--r--   0        0        0    12628 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/quote.rs
--rw-r--r--   0        0        0    12946 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/trade.rs
--rw-r--r--   0        0        0    10343 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/backend/kmerge_batch.rs
--rw-r--r--   0        0        0     1025 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/backend/mod.rs
--rw-r--r--   0        0        0     8065 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/backend/session.rs
--rw-r--r--   0        0        0     1736 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/lib.rs
--rw-r--r--   0        0        0      922 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/backend/mod.rs
--rw-r--r--   0        0        0     4265 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/backend/session.rs
--rw-r--r--   0        0        0    12804 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/backend/transformer.rs
--rw-r--r--   0        0        0     1696 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/mod.rs
--rw-r--r--   0        0        0     2824 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/bar.rs
--rw-r--r--   0        0        0     3031 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/delta.rs
--rw-r--r--   0        0        0      942 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/mod.rs
--rw-r--r--   0        0        0     2955 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/quote.rs
--rw-r--r--   0        0        0     2952 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/trade.rs
--rw-r--r--   0        0        0    10633 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/tests/test_catalog.rs
--rw-r--r--   0        0        0     2159 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/persistence/tests/test_util.rs
--rw-r--r--   0        0        0     1469 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/pyo3/Cargo.toml
--rw-r--r--   0        0        0     4929 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/pyo3/src/lib.rs
--rw-r--r--   0        0        0       50 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/rust-toolchain.toml
--rw-r--r--   0        0        0      225 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_core/rustfmt.toml
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_trader/__init__.pxd
--rw-r--r--   0        0        0     2270 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_trader/__init__.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.353010 nautilus_trader-1.193.0/nautilus_trader/accounting/__init__.pxd
--rw-r--r--   0        0        0     1414 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/__init__.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/__init__.pxd
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/__init__.py
--rw-r--r--   0        0        0     4195 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/base.pxd
--rw-r--r--   0        0        0    14679 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/base.pyx
--rw-r--r--   0        0        0     1740 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/betting.pxd
--rw-r--r--   0        0        0     4117 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/betting.pyx
--rw-r--r--   0        0        0     2013 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/cash.pxd
--rw-r--r--   0        0        0    13601 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/cash.pyx
--rw-r--r--   0        0        0     3309 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/margin.pxd
--rw-r--r--   0        0        0    22719 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/margin.pyx
--rw-r--r--   0        0        0     1489 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/calculators.pxd
--rw-r--r--   0        0        0    10740 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/calculators.pyx
--rw-r--r--   0        0        0     2111 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/error.py
--rw-r--r--   0        0        0     1089 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/factory.pxd
--rw-r--r--   0        0        0     4065 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/factory.pyx
--rw-r--r--   0        0        0     2653 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/manager.pxd
--rw-r--r--   0        0        0    22688 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/accounting/manager.pyx
--rw-r--r--   0        0        0     1153 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/__init__.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/_template/__init__.py
--rw-r--r--   0        0        0     1013 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/_template/core.py
--rw-r--r--   0        0        0    14665 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/_template/data.py
--rw-r--r--   0        0        0     7371 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/_template/execution.py
--rw-r--r--   0        0        0     2601 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/_template/providers.py
--rw-r--r--   0        0        0      945 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/__init__.py
--rw-r--r--   0        0        0    12517 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/client.py
--rw-r--r--   0        0        0     3924 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/common.py
--rw-r--r--   0        0        0     2529 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/config.py
--rw-r--r--   0        0        0     2038 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/constants.py
--rw-r--r--   0        0        0    12440 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/data.py
--rw-r--r--   0        0        0    10941 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/data_types.py
--rw-r--r--   0        0        0    42389 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/execution.py
--rw-r--r--   0        0        0     7519 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/factories.py
--rw-r--r--   0        0        0     1257 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/orderbook.pxd
--rw-r--r--   0        0        0     1770 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/orderbook.pyx
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/__init__.py
--rw-r--r--   0        0        0     3234 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/common.py
--rw-r--r--   0        0        0     4607 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/core.py
--rw-r--r--   0        0        0    19955 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/requests.py
--rw-r--r--   0        0        0    19805 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/streaming.py
--rw-r--r--   0        0        0    12917 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/providers.py
--rw-r--r--   0        0        0     9450 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/sockets.py
--rw-r--r--   0        0        0      938 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/__init__.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/__init__.py
--rw-r--r--   0        0        0      997 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/constants.py
--rw-r--r--   0        0        0     1871 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/credentials.py
--rw-r--r--   0        0        0    39673 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/data.py
--rw-r--r--   0        0        0    19212 2024-05-24 12:14:01.357010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/enums.py
--rw-r--r--   0        0        0    41882 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/execution.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/schemas/__init__.py
--rw-r--r--   0        0        0    10932 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/schemas/account.py
--rw-r--r--   0        0        0    22048 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/schemas/market.py
--rw-r--r--   0        0        0     1209 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/schemas/user.py
--rw-r--r--   0        0        0     2570 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/symbol.py
--rw-r--r--   0        0        0    15632 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/types.py
--rw-r--r--   0        0        0     3476 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/urls.py
--rw-r--r--   0        0        0     5353 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/config.py
--rw-r--r--   0        0        0    13709 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/factories.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/__init__.py
--rw-r--r--   0        0        0     6564 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/data.py
--rw-r--r--   0        0        0     6637 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/enums.py
--rw-r--r--   0        0        0    13348 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/execution.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/__init__.py
--rw-r--r--   0        0        0    16026 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/account.py
--rw-r--r--   0        0        0     3629 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/market.py
--rw-r--r--   0        0        0     1962 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/user.py
--rw-r--r--   0        0        0     4834 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/wallet.py
--rw-r--r--   0        0        0    17736 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/providers.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/__init__.py
--rw-r--r--   0        0        0     7352 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/account.py
--rw-r--r--   0        0        0     7646 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/market.py
--rw-r--r--   0        0        0    15368 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/user.py
--rw-r--r--   0        0        0     1281 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/wallet.py
--rw-r--r--   0        0        0     5070 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/types.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/__init__.py
--rw-r--r--   0        0        0    27258 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/account.py
--rw-r--r--   0        0        0     5511 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/client.py
--rw-r--r--   0        0        0     3295 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/endpoint.py
--rw-r--r--   0        0        0     1588 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/error.py
--rw-r--r--   0        0        0    32496 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/market.py
--rw-r--r--   0        0        0     7723 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/user.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/__init__.py
--rw-r--r--   0        0        0     5582 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/data.py
--rw-r--r--   0        0        0     5563 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/enums.py
--rw-r--r--   0        0        0    10055 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/execution.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/__init__.py
--rw-r--r--   0        0        0    26141 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/account.py
--rw-r--r--   0        0        0     6645 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/market.py
--rw-r--r--   0        0        0     1968 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/user.py
--rw-r--r--   0        0        0     4590 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/wallet.py
--rw-r--r--   0        0        0    13691 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/providers.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/__init__.py
--rw-r--r--   0        0        0     3270 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/account.py
--rw-r--r--   0        0        0     6832 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/market.py
--rw-r--r--   0        0        0    11717 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/user.py
--rw-r--r--   0        0        0     1262 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/wallet.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/websocket/__init__.py
--rw-r--r--   0        0        0    16321 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/binance/websocket/client.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/__init__.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/__init__.py
--rw-r--r--   0        0        0     1572 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/constants.py
--rw-r--r--   0        0        0     1825 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/credentials.py
--rw-r--r--   0        0        0    10724 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/enums.py
--rw-r--r--   0        0        0     1502 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/error.py
--rw-r--r--   0        0        0     4018 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/parsing.py
--rw-r--r--   0        0        0     4250 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/symbol.py
--rw-r--r--   0        0        0     2623 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/urls.py
--rw-r--r--   0        0        0     3425 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/config.py
--rw-r--r--   0        0        0    28863 2024-05-24 12:14:01.361010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/data.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/__init__.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/account/__init__.py
--rw-r--r--   0        0        0     2369 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/account/fee_rate.py
--rw-r--r--   0        0        0     2381 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/account/position_info.py
--rw-r--r--   0        0        0     2293 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/account/wallet_balance.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/asset/__init__.py
--rw-r--r--   0        0        0     2225 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/asset/coin_info.py
--rw-r--r--   0        0        0     2594 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/endpoint.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/__init__.py
--rw-r--r--   0        0        0     3608 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/instruments_info.py
--rw-r--r--   0        0        0     2222 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/klines.py
--rw-r--r--   0        0        0     2060 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/server_time.py
--rw-r--r--   0        0        0     3322 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/tickers.py
--rw-r--r--   0        0        0     2132 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/trades.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/__init__.py
--rw-r--r--   0        0        0     2866 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/amend_order.py
--rw-r--r--   0        0        0     2879 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_amend_order.py
--rw-r--r--   0        0        0     2525 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_cancel_order.py
--rw-r--r--   0        0        0     3228 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_place_order.py
--rw-r--r--   0        0        0     2433 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/cancel_all_orders.py
--rw-r--r--   0        0        0     2439 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/cancel_order.py
--rw-r--r--   0        0        0     2466 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/open_orders.py
--rw-r--r--   0        0        0     2756 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/order_history.py
--rw-r--r--   0        0        0     2987 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/place_order.py
--rw-r--r--   0        0        0     2679 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/trade_history.py
--rw-r--r--   0        0        0    35884 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/execution.py
--rw-r--r--   0        0        0     9039 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/factories.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/__init__.py
--rw-r--r--   0        0        0    13207 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/account.py
--rw-r--r--   0        0        0     1963 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/asset.py
--rw-r--r--   0        0        0     6629 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/client.py
--rw-r--r--   0        0        0     1083 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/errors.py
--rw-r--r--   0        0        0     7979 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/market.py
--rw-r--r--   0        0        0     1180 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/user.py
--rw-r--r--   0        0        0    11303 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/providers.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/__init__.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/account/__init__.py
--rw-r--r--   0        0        0     3413 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/account/balance.py
--rw-r--r--   0        0        0     1204 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/account/fee_rate.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/asset/__init__.py
--rw-r--r--   0        0        0     1947 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/asset/coin_info.py
--rw-r--r--   0        0        0     2114 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/common.py
--rw-r--r--   0        0        0    15794 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/instrument.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/__init__.py
--rw-r--r--   0        0        0     2184 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/kline.py
--rw-r--r--   0        0        0     4540 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/orderbook.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/risk_limit.py
--rw-r--r--   0        0        0     1088 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/server_time.py
--rw-r--r--   0        0        0     4461 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/ticker.py
--rw-r--r--   0        0        0     2476 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/trades.py
--rw-r--r--   0        0        0     9705 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/order.py
--rw-r--r--   0        0        0     2665 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/position.py
--rw-r--r--   0        0        0     4044 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/trade.py
--rw-r--r--   0        0        0    21528 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/ws.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/websocket/__init__.py
--rw-r--r--   0        0        0    11105 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/websocket/client.py
--rw-r--r--   0        0        0     1689 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/__init__.py
--rw-r--r--   0        0        0     2749 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/common.py
--rw-r--r--   0        0        0     2727 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/config.py
--rw-r--r--   0        0        0     1210 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/constants.py
--rw-r--r--   0        0        0    39036 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/data.py
--rw-r--r--   0        0        0     1315 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/enums.py
--rw-r--r--   0        0        0     6043 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/factories.py
--rw-r--r--   0        0        0    10712 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/loaders.py
--rw-r--r--   0        0        0    10149 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/providers.py
--rw-r--r--   0        0        0    10104 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/publishers.json
--rw-r--r--   0        0        0     1141 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/databento/types.py
--rw-r--r--   0        0        0     1193 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/env.py
--rw-r--r--   0        0        0      930 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/__init__.py
--rw-r--r--   0        0        0     1014 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/__init__.py
--rw-r--r--   0        0        0     6415 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/account.py
--rw-r--r--   0        0        0    26860 2024-05-24 12:14:01.365010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/client.py
--rw-r--r--   0        0        0    15878 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/common.py
--rw-r--r--   0        0        0     8356 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/connection.py
--rw-r--r--   0        0        0     7167 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/contract.py
--rw-r--r--   0        0        0     8724 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/error.py
--rw-r--r--   0        0        0    32019 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/market_data.py
--rw-r--r--   0        0        0    10341 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/order.py
--rw-r--r--   0        0        0    43317 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/wrapper.py
--rw-r--r--   0        0        0     6988 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/common.py
--rw-r--r--   0        0        0     8127 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/config.py
--rw-r--r--   0        0        0    17152 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/data.py
--rw-r--r--   0        0        0    39055 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/execution.py
--rw-r--r--   0        0        0     9005 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/factories.py
--rw-r--r--   0        0        0     7876 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/gateway.py
--rw-r--r--   0        0        0     1054 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/historic/__init__.py
--rw-r--r--   0        0        0    21095 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/historic/client.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/parsing/__init__.py
--rw-r--r--   0        0        0     3579 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/parsing/data.py
--rw-r--r--   0        0        0     4007 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/parsing/execution.py
--rw-r--r--   0        0        0    24117 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/parsing/instruments.py
--rw-r--r--   0        0        0    12263 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/providers.py
--rw-r--r--   0        0        0     4904 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/web.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/sandbox/__init__.py
--rw-r--r--   0        0        0     2360 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/sandbox/config.py
--rw-r--r--   0        0        0     8365 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/sandbox/execution.py
--rw-r--r--   0        0        0     2676 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/sandbox/factory.py
--rw-r--r--   0        0        0      937 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/tardis/__init__.py
--rw-r--r--   0        0        0     2909 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/adapters/tardis/loaders.py
--rw-r--r--   0        0        0      978 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/__init__.py
--rw-r--r--   0        0        0    15183 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/analyzer.py
--rw-r--r--   0        0        0     5714 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/reporter.py
--rw-r--r--   0        0        0     3940 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistic.py
--rw-r--r--   0        0        0     2255 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/__init__.py
--rw-r--r--   0        0        0     1997 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/expectancy.py
--rw-r--r--   0        0        0     1705 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/long_ratio.py
--rw-r--r--   0        0        0     1468 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/loser_avg.py
--rw-r--r--   0        0        0     1514 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/loser_max.py
--rw-r--r--   0        0        0     1512 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/loser_min.py
--rw-r--r--   0        0        0     1563 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/profit_factor.py
--rw-r--r--   0        0        0     1399 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/returns_avg.py
--rw-r--r--   0        0        0     1414 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/returns_avg_loss.py
--rw-r--r--   0        0        0     1413 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/returns_avg_win.py
--rw-r--r--   0        0        0     1716 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/returns_volatility.py
--rw-r--r--   0        0        0     1323 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/risk_return_ratio.py
--rw-r--r--   0        0        0     1776 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/sharpe_ratio.py
--rw-r--r--   0        0        0     1883 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/sortino_ratio.py
--rw-r--r--   0        0        0     1498 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/win_rate.py
--rw-r--r--   0        0        0     1489 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/winner_avg.py
--rw-r--r--   0        0        0     1347 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/winner_max.py
--rw-r--r--   0        0        0     1494 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/winner_min.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/__init__.pxd
--rw-r--r--   0        0        0      946 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/__init__.py
--rw-r--r--   0        0        0     1868 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/__main__.py
--rw-r--r--   0        0        0     3840 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/auction.py
--rw-r--r--   0        0        0     9257 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/config.py
--rw-r--r--   0        0        0     1100 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/data_client.pxd
--rw-r--r--   0        0        0    13931 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/data_client.pyx
--rw-r--r--   0        0        0     2162 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/engine.pxd
--rw-r--r--   0        0        0    51527 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/engine.pyx
--rw-r--r--   0        0        0     7614 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/exchange.pxd
--rw-r--r--   0        0        0    31318 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/exchange.pyx
--rw-r--r--   0        0        0     1084 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/execution_client.pxd
--rw-r--r--   0        0        0     5264 2024-05-24 12:14:01.369010 nautilus_trader-1.193.0/nautilus_trader/backtest/execution_client.pyx
--rw-r--r--   0        0        0    12270 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/backtest/matching_engine.pxd
--rw-r--r--   0        0        0    98825 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/backtest/matching_engine.pyx
--rw-r--r--   0        0        0     2658 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/backtest/models.pxd
--rw-r--r--   0        0        0     8785 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/backtest/models.pyx
--rw-r--r--   0        0        0     1893 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/backtest/modules.pxd
--rw-r--r--   0        0        0     8483 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/backtest/modules.pyx
--rw-r--r--   0        0        0    15294 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/backtest/node.py
--rw-r--r--   0        0        0     3072 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/backtest/results.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/__init__.pxd
--rw-r--r--   0        0        0     1220 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/__init__.py
--rw-r--r--   0        0        0    10536 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/base.pxd
--rw-r--r--   0        0        0    25831 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/base.pyx
--rw-r--r--   0        0        0     8701 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/cache.pxd
--rw-r--r--   0        0        0   135124 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/cache.pyx
--rw-r--r--   0        0        0     2884 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/config.py
--rw-r--r--   0        0        0     1104 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/database.pxd
--rw-r--r--   0        0        0    36283 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/database.pyx
--rw-r--r--   0        0        0     5051 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/facade.pxd
--rw-r--r--   0        0        0    11952 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/facade.pyx
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/postgres/__init__.py
--rw-r--r--   0        0        0     4228 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/postgres/adapter.py
--rw-r--r--   0        0        0    12833 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/cache/postgres/transformers.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/__init__.pxd
--rw-r--r--   0        0        0     1571 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/__init__.py
--rw-r--r--   0        0        0    11890 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/actor.pxd
--rw-r--r--   0        0        0    92278 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/actor.pyx
--rw-r--r--   0        0        0    11128 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/component.pxd
--rw-r--r--   0        0        0    88235 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/component.pyx
--rw-r--r--   0        0        0    16788 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/config.py
--rw-r--r--   0        0        0     1849 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/enums.py
--rw-r--r--   0        0        0    10785 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/executor.py
--rw-r--r--   0        0        0     9517 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/factories.pxd
--rw-r--r--   0        0        0    58923 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/factories.pyx
--rw-r--r--   0        0        0     1320 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/functions.py
--rw-r--r--   0        0        0     2143 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/generators.pxd
--rw-r--r--   0        0        0     7841 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/generators.pyx
--rw-r--r--   0        0        0     2723 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/messages.pxd
--rw-r--r--   0        0        0    11741 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/messages.pyx
--rw-r--r--   0        0        0    10413 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/common/providers.py
--rw-r--r--   0        0        0     5512 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/config/__init__.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/core/__init__.pxd
--rw-r--r--   0        0        0     1339 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/core/__init__.py
--rw-r--r--   0        0        0     1230 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/core/asynchronous.py
--rw-r--r--   0        0        0     3683 2024-05-24 12:14:01.373010 nautilus_trader-1.193.0/nautilus_trader/core/correctness.pxd
--rw-r--r--   0        0        0    37316 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/correctness.pyx
--rw-r--r--   0        0        0      897 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/data.pxd
--rw-r--r--   0        0        0     1954 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/data.pyx
--rw-r--r--   0        0        0     1363 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/datetime.pxd
--rw-r--r--   0        0        0     7616 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/datetime.pyx
--rw-r--r--   0        0        0     1230 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/fsm.pxd
--rw-r--r--   0        0        0     4364 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/fsm.pyx
--rw-r--r--   0        0        0     2511 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/includes/algorithms.h
--rw-r--r--   0        0        0      907 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/includes/backtest.h
--rw-r--r--   0        0        0    15890 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/includes/common.h
--rw-r--r--   0        0        0     3055 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/includes/core.h
--rw-r--r--   0        0        0    65849 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/includes/model.h
--rw-r--r--   0        0        0     2529 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/inspect.py
--rw-r--r--   0        0        0     2137 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/message.pxd
--rw-r--r--   0        0        0     6509 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/message.pyx
--rw-r--r--   0        0        0    87295 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/nautilus_pyo3.pyi
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/rust/__init__.pxd
--rw-r--r--   0        0        0     2685 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/rust/algorithms.pxd
--rw-r--r--   0        0        0     1050 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/rust/backtest.pxd
--rw-r--r--   0        0        0    15615 2024-05-24 12:19:06.972391 nautilus_trader-1.193.0/nautilus_trader/core/rust/common.pxd
--rw-r--r--   0        0        0     1222 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/rust/common.pyx
--rw-r--r--   0        0        0     3107 2024-05-24 12:16:20.244731 nautilus_trader-1.193.0/nautilus_trader/core/rust/core.pxd
--rw-r--r--   0        0        0    61890 2024-05-24 12:17:40.812571 nautilus_trader-1.193.0/nautilus_trader/core/rust/model.pxd
--rw-r--r--   0        0        0     2702 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/rust/model.pyx
--rw-r--r--   0        0        0     1359 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/stats.pxd
--rw-r--r--   0        0        0     5710 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/stats.pyx
--rw-r--r--   0        0        0     3870 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/string.pxd
--rw-r--r--   0        0        0     1049 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/uuid.pxd
--rw-r--r--   0        0        0     2755 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/core/uuid.pyx
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/__init__.pxd
--rw-r--r--   0        0        0     1360 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/__init__.py
--rw-r--r--   0        0        0     4191 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/aggregation.pxd
--rw-r--r--   0        0        0    24575 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/aggregation.pyx
--rw-r--r--   0        0        0     8072 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/client.pxd
--rw-r--r--   0        0        0    39952 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/client.pyx
--rw-r--r--   0        0        0     2142 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/config.py
--rw-r--r--   0        0        0    10088 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/engine.pxd
--rw-r--r--   0        0        0    65384 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/engine.pyx
--rw-r--r--   0        0        0     2391 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/messages.pxd
--rw-r--r--   0        0        0     8362 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/data/messages.pyx
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/__init__.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/algorithms/__init__.py
--rw-r--r--   0        0        0     4226 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/algorithms/blank.py
--rw-r--r--   0        0        0    11242 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/algorithms/twap.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/__init__.pxd
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/__init__.py
--rw-r--r--   0        0        0     5269 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/blank.py
--rw-r--r--   0        0        0    11736 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross.py
--rw-r--r--   0        0        0    11534 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_bracket.py
--rw-r--r--   0        0        0    14158 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_bracket_algo.py
--rw-r--r--   0        0        0    10284 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_cython.pyx
--rw-r--r--   0        0        0    11178 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_long_only.py
--rw-r--r--   0        0        0    15993 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_stop_entry.py
--rw-r--r--   0        0        0    14118 2024-05-24 12:14:01.377010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_trailing_stop.py
--rw-r--r--   0        0        0    12012 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_twap.py
--rw-r--r--   0        0        0     5286 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/market_maker.py
--rw-r--r--   0        0        0     8954 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/orderbook_imbalance.py
--rw-r--r--   0        0        0     9291 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/orderbook_imbalance_rust.py
--rw-r--r--   0        0        0     2839 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/signal_strategy.py
--rw-r--r--   0        0        0     4718 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/subscribe.py
--rw-r--r--   0        0        0     7283 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/talib_strategy.py
--rw-r--r--   0        0        0    14071 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/examples/strategies/volatility_market_maker.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/__init__.pxd
--rw-r--r--   0        0        0     1353 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/__init__.py
--rw-r--r--   0        0        0     8527 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/algorithm.pxd
--rw-r--r--   0        0        0    52607 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/algorithm.pyx
--rw-r--r--   0        0        0     7359 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/client.pxd
--rw-r--r--   0        0        0    29170 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/client.pyx
--rw-r--r--   0        0        0     3587 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/config.py
--rw-r--r--   0        0        0     4001 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/emulator.pxd
--rw-r--r--   0        0        0    35586 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/emulator.pyx
--rw-r--r--   0        0        0     6956 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/engine.pxd
--rw-r--r--   0        0        0    46472 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/engine.pyx
--rw-r--r--   0        0        0     4593 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/manager.pxd
--rw-r--r--   0        0        0    24284 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/manager.pyx
--rw-r--r--   0        0        0     3590 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/matching_core.pxd
--rw-r--r--   0        0        0    16178 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/matching_core.pyx
--rw-r--r--   0        0        0     5598 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/messages.pxd
--rw-r--r--   0        0        0    34648 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/messages.pyx
--rw-r--r--   0        0        0    22236 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/reports.py
--rw-r--r--   0        0        0     1726 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/trailing.pxd
--rw-r--r--   0        0        0    17089 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/execution/trailing.pyx
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/__init__.pxd
--rw-r--r--   0        0        0     1188 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/__init__.py
--rw-r--r--   0        0        0     1722 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/amat.pxd
--rw-r--r--   0        0        0     4832 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/amat.pyx
--rw-r--r--   0        0        0     1482 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/aroon.pxd
--rw-r--r--   0        0        0     3470 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/aroon.pyx
--rw-r--r--   0        0        0     1474 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/atr.pxd
--rw-r--r--   0        0        0     4320 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/atr.pyx
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/__init__.pxd
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/__init__.py
--rw-r--r--   0        0        0     1770 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/ama.pxd
--rw-r--r--   0        0        0     5185 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/ama.pyx
--rw-r--r--   0        0        0     1063 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/dema.pxd
--rw-r--r--   0        0        0     3840 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/dema.pyx
--rw-r--r--   0        0        0     1096 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/ema.pxd
--rw-r--r--   0        0        0     3454 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/ema.pyx
--rw-r--r--   0        0        0     1247 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/hma.pxd
--rw-r--r--   0        0        0     4323 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/hma.pyx
--rw-r--r--   0        0        0     3114 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/ma_factory.pyx
--rw-r--r--   0        0        0     1568 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/moving_average.pxd
--rw-r--r--   0        0        0     2960 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/moving_average.pyx
--rw-r--r--   0        0        0     1080 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/rma.pxd
--rw-r--r--   0        0        0     3466 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/rma.pyx
--rw-r--r--   0        0        0     1020 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/sma.pxd
--rw-r--r--   0        0        0     3530 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/sma.pyx
--rw-r--r--   0        0        0     1283 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/vidya.pxd
--rw-r--r--   0        0        0     4592 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/vidya.pyx
--rw-r--r--   0        0        0     1174 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/wma.pxd
--rw-r--r--   0        0        0     4700 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/average/wma.pyx
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/base/__init__.pxd
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/base/__init__.py
--rw-r--r--   0        0        0     1701 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/base/indicator.pxd
--rw-r--r--   0        0        0     3029 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/base/indicator.pyx
--rw-r--r--   0        0        0     1315 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/bias.pxd
--rw-r--r--   0        0        0     2868 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/bias.pyx
--rw-r--r--   0        0        0     1579 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/bollinger_bands.pxd
--rw-r--r--   0        0        0     5219 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/bollinger_bands.pyx
--rw-r--r--   0        0        0     1635 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/cci.pxd
--rw-r--r--   0        0        0     4056 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/cci.pyx
--rw-r--r--   0        0        0     1375 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/cmo.pxd
--rw-r--r--   0        0        0     3766 2024-05-24 12:14:01.381010 nautilus_trader-1.193.0/nautilus_trader/indicators/cmo.pyx
--rw-r--r--   0        0        0     1658 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/dm.pxd
--rw-r--r--   0        0        0     3732 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/dm.pyx
--rw-r--r--   0        0        0     1490 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/donchian_channel.pxd
--rw-r--r--   0        0        0     4374 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/donchian_channel.pyx
--rw-r--r--   0        0        0     1231 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/efficiency_ratio.pxd
--rw-r--r--   0        0        0     3119 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/efficiency_ratio.pyx
--rw-r--r--   0        0        0     3168 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_candlesticks.pxd
--rw-r--r--   0        0        0    12540 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_candlesticks.pyx
--rw-r--r--   0        0        0     1347 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enum.pyx
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/__init__.pxd
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/__init__.py
--rw-r--r--   0        0        0      976 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pxd
--rw-r--r--   0        0        0      980 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pyx
--rw-r--r--   0        0        0      947 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pxd
--rw-r--r--   0        0        0      987 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pyx
--rw-r--r--   0        0        0     1020 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pxd
--rw-r--r--   0        0        0      972 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pyx
--rw-r--r--   0        0        0      972 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pxd
--rw-r--r--   0        0        0      980 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pyx
--rw-r--r--   0        0        0     1805 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/keltner_channel.pxd
--rw-r--r--   0        0        0     4675 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/keltner_channel.pyx
--rw-r--r--   0        0        0     1395 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/keltner_position.pxd
--rw-r--r--   0        0        0     4280 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/keltner_position.pyx
--rw-r--r--   0        0        0     1713 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/kvo.pxd
--rw-r--r--   0        0        0     4727 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/kvo.pyx
--rw-r--r--   0        0        0     1636 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/linear_regression.pxd
--rw-r--r--   0        0        0     3839 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/linear_regression.pyx
--rw-r--r--   0        0        0     1664 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/macd.pxd
--rw-r--r--   0        0        0     4809 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/macd.pyx
--rw-r--r--   0        0        0     1232 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/obv.pxd
--rw-r--r--   0        0        0     2958 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/obv.pyx
--rw-r--r--   0        0        0     1514 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/pressure.pxd
--rw-r--r--   0        0        0     4383 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/pressure.pyx
--rw-r--r--   0        0        0     1476 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/psl.pxd
--rw-r--r--   0        0        0     3311 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/psl.pyx
--rw-r--r--   0        0        0     1227 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/roc.pxd
--rw-r--r--   0        0        0     2726 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/roc.pyx
--rw-r--r--   0        0        0     1393 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/rsi.pxd
--rw-r--r--   0        0        0     3767 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/rsi.pyx
--rw-r--r--   0        0        0     1763 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/rvi.pxd
--rw-r--r--   0        0        0     4539 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/rvi.pyx
--rw-r--r--   0        0        0     1444 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/spread_analyzer.pxd
--rw-r--r--   0        0        0     3391 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/spread_analyzer.pyx
--rw-r--r--   0        0        0     1485 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/stochastics.pxd
--rw-r--r--   0        0        0     3884 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/stochastics.pyx
--rw-r--r--   0        0        0     2271 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/swings.pxd
--rw-r--r--   0        0        0     4678 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/swings.pyx
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/ta_lib/__init__.py
--rw-r--r--   0        0        0     1993 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/ta_lib/common.py
--rw-r--r--   0        0        0    29656 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/ta_lib/manager.py
--rw-r--r--   0        0        0     1458 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/vhf.pxd
--rw-r--r--   0        0        0     3513 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/vhf.pyx
--rw-r--r--   0        0        0     1485 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/volatility_ratio.pxd
--rw-r--r--   0        0        0     4482 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/volatility_ratio.pyx
--rw-r--r--   0        0        0     1270 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/vwap.pxd
--rw-r--r--   0        0        0     2938 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/indicators/vwap.pyx
--rw-r--r--   0        0        0     1155 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/__init__.py
--rw-r--r--   0        0        0     1861 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/__main__.py
--rw-r--r--   0        0        0     8314 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/config.py
--rw-r--r--   0        0        0    34312 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/data_client.py
--rw-r--r--   0        0        0    16375 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/data_engine.py
--rw-r--r--   0        0        0    18927 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/execution_client.py
--rw-r--r--   0        0        0    41082 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/execution_engine.py
--rw-r--r--   0        0        0     3395 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/factories.py
--rw-r--r--   0        0        0    16754 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/node.py
--rw-r--r--   0        0        0     9369 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/node_builder.py
--rw-r--r--   0        0        0     9696 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/live/risk_engine.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/model/__init__.pxd
--rw-r--r--   0        0        0     1652 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/model/__init__.py
--rw-r--r--   0        0        0     3380 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/model/book.pxd
--rw-r--r--   0        0        0    24325 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/model/book.pyx
--rw-r--r--   0        0        0     5067 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/model/currencies.py
--rw-r--r--   0        0        0    13066 2024-05-24 12:14:01.385010 nautilus_trader-1.193.0/nautilus_trader/model/data.pxd
--rw-r--r--   0        0        0   126566 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/data.pyx
--rw-r--r--   0        0        0     7811 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/enums.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/events/__init__.pxd
--rw-r--r--   0        0        0     2829 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/events/__init__.py
--rw-r--r--   0        0        0     2220 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/events/account.pxd
--rw-r--r--   0        0        0     6660 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/events/account.pyx
--rw-r--r--   0        0        0    12302 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/events/order.pxd
--rw-r--r--   0        0        0   136228 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/events/order.pyx
--rw-r--r--   0        0        0     5628 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/events/position.pxd
--rw-r--r--   0        0        0    35393 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/events/position.pyx
--rw-r--r--   0        0        0     5142 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/functions.pxd
--rw-r--r--   0        0        0    10333 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/functions.pyx
--rw-r--r--   0        0        0     4039 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/identifiers.pxd
--rw-r--r--   0        0        0    27544 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/identifiers.pyx
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/__init__.pxd
--rw-r--r--   0        0        0     2302 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/__init__.py
--rw-r--r--   0        0        0     5519 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/base.pxd
--rw-r--r--   0        0        0    21031 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/base.pyx
--rw-r--r--   0        0        0     1778 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/betting.pxd
--rw-r--r--   0        0        0     8622 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/betting.pyx
--rw-r--r--   0        0        0     1449 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/cfd.pxd
--rw-r--r--   0        0        0    13625 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/cfd.pyx
--rw-r--r--   0        0        0     1296 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/commodity.pxd
--rw-r--r--   0        0        0    13011 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/commodity.pyx
--rw-r--r--   0        0        0     1756 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/crypto_future.pxd
--rw-r--r--   0        0        0    14480 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/crypto_future.pyx
--rw-r--r--   0        0        0     1563 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/crypto_perpetual.pxd
--rw-r--r--   0        0        0    13388 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/crypto_perpetual.pyx
--rw-r--r--   0        0        0     1334 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/currency_pair.pxd
--rw-r--r--   0        0        0    13495 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/currency_pair.pyx
--rw-r--r--   0        0        0     1284 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/equity.pxd
--rw-r--r--   0        0        0     9201 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/equity.pyx
--rw-r--r--   0        0        0     1736 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/futures_contract.pxd
--rw-r--r--   0        0        0    11356 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/futures_contract.pyx
--rw-r--r--   0        0        0     1824 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/futures_spread.pxd
--rw-r--r--   0        0        0    11963 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/futures_spread.pyx
--rw-r--r--   0        0        0     2068 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/options_contract.pxd
--rw-r--r--   0        0        0    12508 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/options_contract.pyx
--rw-r--r--   0        0        0     1930 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/options_spread.pxd
--rw-r--r--   0        0        0    12096 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/options_spread.pyx
--rw-r--r--   0        0        0     1555 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/synthetic.pxd
--rw-r--r--   0        0        0    12487 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/instruments/synthetic.pyx
--rw-r--r--   0        0        0     5934 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/objects.pxd
--rw-r--r--   0        0        0    52381 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/objects.pyx
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/__init__.pxd
--rw-r--r--   0        0        0     2094 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/__init__.py
--rw-r--r--   0        0        0     9471 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/base.pxd
--rw-r--r--   0        0        0    37731 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/base.pyx
--rw-r--r--   0        0        0     1770 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/limit.pxd
--rw-r--r--   0        0        0    21400 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/limit.pyx
--rw-r--r--   0        0        0     2175 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/limit_if_touched.pxd
--rw-r--r--   0        0        0    17609 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/limit_if_touched.pyx
--rw-r--r--   0        0        0     1842 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/list.pxd
--rw-r--r--   0        0        0     2365 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/list.pyx
--rw-r--r--   0        0        0     1272 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/market.pxd
--rw-r--r--   0        0        0    15939 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/market.pyx
--rw-r--r--   0        0        0     1612 2024-05-24 12:14:01.389010 nautilus_trader-1.193.0/nautilus_trader/model/orders/market_if_touched.pxd
--rw-r--r--   0        0        0    15818 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/market_if_touched.pyx
--rw-r--r--   0        0        0     1646 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/market_to_limit.pxd
--rw-r--r--   0        0        0    14283 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/market_to_limit.pyx
--rw-r--r--   0        0        0     2232 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/stop_limit.pxd
--rw-r--r--   0        0        0    20646 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/stop_limit.pyx
--rw-r--r--   0        0        0     1602 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/stop_market.pxd
--rw-r--r--   0        0        0    16030 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/stop_market.pyx
--rw-r--r--   0        0        0     2647 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/trailing_stop_limit.pxd
--rw-r--r--   0        0        0    19580 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/trailing_stop_limit.pyx
--rw-r--r--   0        0        0     1953 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/trailing_stop_market.pxd
--rw-r--r--   0        0        0    17208 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/trailing_stop_market.pyx
--rw-r--r--   0        0        0     1141 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/unpacker.pxd
--rw-r--r--   0        0        0     3926 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/orders/unpacker.pyx
--rw-r--r--   0        0        0     6940 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/position.pxd
--rw-r--r--   0        0        0    23901 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/position.pyx
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/__init__.pxd
--rw-r--r--   0        0        0     1443 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/__init__.py
--rw-r--r--   0        0        0     1581 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/base.pxd
--rw-r--r--   0        0        0     3709 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/base.pyx
--rw-r--r--   0        0        0     1147 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/__init__.py
--rw-r--r--   0        0        0     1371 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/fixed.pxd
--rw-r--r--   0        0        0     3921 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/fixed.pyx
--rw-r--r--   0        0        0     1388 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/tiered.pxd
--rw-r--r--   0        0        0     5436 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/tiered.pyx
--rw-r--r--   0        0        0     1333 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/model/venues.py
--rw-r--r--   0        0        0      973 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/__init__.py
--rw-r--r--   0        0        0     1079 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/__init__.py
--rw-r--r--   0        0        0     6321 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/base.py
--rw-r--r--   0        0        0    28127 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/parquet.py
--rw-r--r--   0        0        0     2073 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/singleton.py
--rw-r--r--   0        0        0     1327 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/types.py
--rw-r--r--   0        0        0     2886 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/config.py
--rw-r--r--   0        0        0     3561 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/funcs.py
--rw-r--r--   0        0        0     7025 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/loaders.py
--rw-r--r--   0        0        0     3392 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/wranglers.pxd
--rw-r--r--   0        0        0    30305 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/wranglers.pyx
--rw-r--r--   0        0        0    16480 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/wranglers_v2.py
--rw-r--r--   0        0        0    12974 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/persistence/writer.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/portfolio/__init__.pxd
--rw-r--r--   0        0        0     1123 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/portfolio/__init__.py
--rw-r--r--   0        0        0     2132 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/portfolio/base.pxd
--rw-r--r--   0        0        0     4233 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/portfolio/base.pyx
--rw-r--r--   0        0        0     3111 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/portfolio/portfolio.pxd
--rw-r--r--   0        0        0    38292 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/portfolio/portfolio.pyx
--rw-r--r--   0        0        0        0 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/py.typed
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/risk/__init__.pxd
--rw-r--r--   0        0        0     1084 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/risk/__init__.py
--rw-r--r--   0        0        0     1974 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/risk/config.py
--rw-r--r--   0        0        0     5474 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/risk/engine.pxd
--rw-r--r--   0        0        0    38261 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/risk/engine.pyx
--rw-r--r--   0        0        0     1747 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/risk/sizing.pxd
--rw-r--r--   0        0        0     7059 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/risk/sizing.pyx
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/__init__.pxd
--rw-r--r--   0        0        0     1106 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/__init__.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/__init__.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/__init__.py
--rw-r--r--   0        0        0     5360 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/account_state.py
--rw-r--r--   0        0        0     1689 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/component_events.py
--rw-r--r--   0        0        0    14111 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/instruments.py
--rw-r--r--   0        0        0     2191 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/order_events.py
--rw-r--r--   0        0        0     5923 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/position_events.py
--rw-r--r--   0        0        0    15753 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/schema.py
--rw-r--r--   0        0        0    13886 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/serializer.py
--rw-r--r--   0        0        0     1096 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/base.pxd
--rw-r--r--   0        0        0    12000 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/base.pyx
--rw-r--r--   0        0        0     1303 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/serializer.pxd
--rw-r--r--   0        0        0     5404 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/serialization/serializer.pyx
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/system/__init__.py
--rw-r--r--   0        0        0     6506 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/system/config.py
--rw-r--r--   0        0        0    40208 2024-05-24 12:14:01.393010 nautilus_trader-1.193.0/nautilus_trader/system/kernel.py
--rw-r--r--   0        0        0     1034 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/__init__.py
--rw-r--r--   0        0        0     2316 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/functions.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/__init__.py
--rw-r--r--   0        0        0     6382 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/actors.py
--rw-r--r--   0        0        0     5793 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/cache_database.py
--rw-r--r--   0        0        0     1550 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/controller.py
--rw-r--r--   0        0        0     3177 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/data.py
--rw-r--r--   0        0        0     2976 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/engines.py
--rw-r--r--   0        0        0    12678 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/exec_clients.py
--rw-r--r--   0        0        0     7299 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/strategies.py
--rw-r--r--   0        0        0    29811 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/providers.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/__init__.py
--rw-r--r--   0        0        0     3697 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/accounting_pyo3.py
--rw-r--r--   0        0        0     6642 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/data_pyo3.py
--rw-r--r--   0        0        0    19951 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/events_pyo3.py
--rw-r--r--   0        0        0     3912 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/identifiers_pyo3.py
--rw-r--r--   0        0        0    15113 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/instruments_pyo3.py
--rw-r--r--   0        0        0     5508 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/orders_pyo3.py
--rw-r--r--   0        0        0     2451 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/types_pyo3.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/__init__.py
--rw-r--r--   0        0        0     4828 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/commands.py
--rw-r--r--   0        0        0     5842 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/component.py
--rw-r--r--   0        0        0     6234 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/config.py
--rw-r--r--   0        0        0    22352 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/data.py
--rw-r--r--   0        0        0    14777 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/events.py
--rw-r--r--   0        0        0     9471 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/execution.py
--rw-r--r--   0        0        0     3991 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/identifiers.py
--rw-r--r--   0        0        0     3415 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/persistence.py
--rw-r--r--   0        0        0      869 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/trading/__init__.pxd
--rw-r--r--   0        0        0     1372 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/trading/__init__.py
--rw-r--r--   0        0        0     4730 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/trading/config.py
--rw-r--r--   0        0        0     5493 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/trading/controller.py
--rw-r--r--   0        0        0    18226 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/trading/filters.py
--rw-r--r--   0        0        0     8699 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/trading/strategy.pxd
--rw-r--r--   0        0        0    59399 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/trading/strategy.pyx
--rw-r--r--   0        0        0    25167 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/nautilus_trader/trading/trader.py
--rw-r--r--   0        0        0     8001 2024-05-24 12:14:01.397010 nautilus_trader-1.193.0/pyproject.toml
--rw-r--r--   0        0        0    27266 1970-01-01 00:00:00.000000 nautilus_trader-1.193.0/PKG-INFO
+-rw-r--r--   0        0        0     7651 2024-05-31 11:33:44.226135 nautilus_trader-1.194.0/LICENSE
+-rw-r--r--   0        0        0    25383 2024-05-31 11:33:44.226135 nautilus_trader-1.194.0/README.md
+-rw-r--r--   0        0        0    12823 2024-05-31 11:33:44.226135 nautilus_trader-1.194.0/build.py
+-rw-r--r--   0        0        0      663 2024-05-31 11:33:44.238135 nautilus_trader-1.194.0/nautilus_core/.cargo/config.toml
+-rw-r--r--   0        0        0   135452 2024-05-31 11:33:44.238135 nautilus_trader-1.194.0/nautilus_core/Cargo.lock
+-rw-r--r--   0        0        0     2305 2024-05-31 11:33:44.238135 nautilus_trader-1.194.0/nautilus_core/Cargo.toml
+-rw-r--r--   0        0        0     7652 2024-05-31 11:33:44.238135 nautilus_trader-1.194.0/nautilus_core/LICENSE
+-rw-r--r--   0        0        0     1248 2024-05-31 11:33:44.238135 nautilus_trader-1.194.0/nautilus_core/README.md
+-rw-r--r--   0        0        0      967 2024-05-31 11:33:44.238135 nautilus_trader-1.194.0/nautilus_core/accounting/Cargo.toml
+-rw-r--r--   0        0        0     9273 2024-05-31 11:33:44.238135 nautilus_trader-1.194.0/nautilus_core/accounting/src/account/base.rs
+-rw-r--r--   0        0        0    20416 2024-05-31 11:33:44.238135 nautilus_trader-1.194.0/nautilus_core/accounting/src/account/cash.rs
+-rw-r--r--   0        0        0    22124 2024-05-31 11:33:44.238135 nautilus_trader-1.194.0/nautilus_core/accounting/src/account/margin.rs
+-rw-r--r--   0        0        0     1016 2024-05-31 11:33:44.238135 nautilus_trader-1.194.0/nautilus_core/accounting/src/account/mod.rs
+-rw-r--r--   0        0        0     2376 2024-05-31 11:33:44.238135 nautilus_trader-1.194.0/nautilus_core/accounting/src/account/stubs.rs
+-rw-r--r--   0        0        0     1673 2024-05-31 11:33:44.238135 nautilus_trader-1.194.0/nautilus_core/accounting/src/lib.rs
+-rw-r--r--   0        0        0     6160 2024-05-31 11:33:44.238135 nautilus_trader-1.194.0/nautilus_core/accounting/src/python/cash.rs
+-rw-r--r--   0        0        0     8441 2024-05-31 11:33:44.238135 nautilus_trader-1.194.0/nautilus_core/accounting/src/python/margin.rs
+-rw-r--r--   0        0        0     1557 2024-05-31 11:33:44.238135 nautilus_trader-1.194.0/nautilus_core/accounting/src/python/mod.rs
+-rw-r--r--   0        0        0     2609 2024-05-31 11:33:44.238135 nautilus_trader-1.194.0/nautilus_core/accounting/src/python/transformer.rs
+-rw-r--r--   0        0        0     2598 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/accounting/src/stubs.rs
+-rw-r--r--   0        0        0     1669 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/Cargo.toml
+-rw-r--r--   0        0        0     1217 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/bin/sandbox.rs
+-rw-r--r--   0        0        0     2250 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/common.rs
+-rw-r--r--   0        0        0    44341 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/decode.rs
+-rw-r--r--   0        0        0     3474 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/enums.rs
+-rw-r--r--   0        0        0    15975 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/live.rs
+-rw-r--r--   0        0        0    11970 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/loader.rs
+-rw-r--r--   0        0        0     1104 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/mod.rs
+-rw-r--r--   0        0        0    10104 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/publishers.json
+-rw-r--r--   0        0        0     5323 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/python/enums.rs
+-rw-r--r--   0        0        0    19510 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/python/historical.rs
+-rw-r--r--   0        0        0     8154 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/python/live.rs
+-rw-r--r--   0        0        0    13415 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/python/loader.rs
+-rw-r--r--   0        0        0     1702 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/python/mod.rs
+-rw-r--r--   0        0        0     7715 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/python/types.rs
+-rw-r--r--   0        0        0     6477 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/symbology.rs
+-rw-r--r--   0        0        0       81 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.cbbo.dbn.zst
+-rw-r--r--   0        0        0      693 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.definition.dbn.zst
+-rw-r--r--   0        0        0      673 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.definition.v1.dbn.zst
+-rw-r--r--   0        0        0      661 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.imbalance.dbn.zst
+-rw-r--r--   0        0        0      465 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.mbo.dbn
+-rw-r--r--   0        0        0      174 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.mbo.dbn.zst
+-rw-r--r--   0        0        0      192 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.mbp-1.dbn.zst
+-rw-r--r--   0        0        0      374 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.mbp-10.dbn.zst
+-rw-r--r--   0        0        0      103 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.ohlcv-1d.dbn.zst
+-rw-r--r--   0        0        0      186 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.ohlcv-1h.dbn.zst
+-rw-r--r--   0        0        0      165 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.ohlcv-1m.dbn.zst
+-rw-r--r--   0        0        0      157 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.ohlcv-1s.dbn.zst
+-rw-r--r--   0        0        0      139 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.statistics.dbn.zst
+-rw-r--r--   0        0        0      197 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.tbbo.dbn.zst
+-rw-r--r--   0        0        0      173 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.trades.dbn.zst
+-rw-r--r--   0        0        0     6968 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/types.rs
+-rw-r--r--   0        0        0     1771 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/adapters/src/lib.rs
+-rw-r--r--   0        0        0     1234 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/backtest/Cargo.toml
+-rw-r--r--   0        0        0     2046 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/backtest/build.rs
+-rw-r--r--   0        0        0      484 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/backtest/cbindgen.toml
+-rw-r--r--   0        0        0      807 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/backtest/cbindgen_cython.toml
+-rw-r--r--   0        0        0     6280 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/backtest/src/engine.rs
+-rw-r--r--   0        0        0     1701 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/backtest/src/lib.rs
+-rw-r--r--   0        0        0     8820 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/backtest/src/matching_engine.rs
+-rw-r--r--   0        0        0      669 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/cli/Cargo.toml
+-rw-r--r--   0        0        0     1289 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/cli/src/bin/cli.rs
+-rw-r--r--   0        0        0      902 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/cli/src/database/mod.rs
+-rw-r--r--   0        0        0     2258 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/cli/src/database/postgres.rs
+-rw-r--r--   0        0        0     1198 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/cli/src/lib.rs
+-rw-r--r--   0        0        0     2230 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/cli/src/opt.rs
+-rw-r--r--   0        0        0       65 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/clippy.toml
+-rw-r--r--   0        0        0     1611 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/common/Cargo.toml
+-rw-r--r--   0        0        0     2759 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/common/build.rs
+-rw-r--r--   0        0        0      548 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/common/cbindgen.toml
+-rw-r--r--   0        0        0      823 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/common/cbindgen_cython.toml
+-rw-r--r--   0        0        0   102842 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/common/src/cache/core.rs
+-rw-r--r--   0        0        0     4922 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/common/src/cache/database.rs
+-rw-r--r--   0        0        0     1086 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/common/src/cache/mod.rs
+-rw-r--r--   0        0        0    12123 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/common/src/clock.rs
+-rw-r--r--   0        0        0     9346 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/common/src/enums.rs
+-rw-r--r--   0        0        0     8054 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/common/src/factories.rs
+-rw-r--r--   0        0        0    12239 2024-05-31 11:33:44.242135 nautilus_trader-1.194.0/nautilus_core/common/src/ffi/clock.rs
+-rw-r--r--   0        0        0     3086 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/ffi/enums.rs
+-rw-r--r--   0        0        0     5900 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/ffi/logging.rs
+-rw-r--r--   0        0        0     1003 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/ffi/mod.rs
+-rw-r--r--   0        0        0     1771 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/ffi/timer.rs
+-rw-r--r--   0        0        0     5087 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/generators/client_order_id.rs
+-rw-r--r--   0        0        0     1380 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/generators/mod.rs
+-rw-r--r--   0        0        0     5039 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/generators/order_list_id.rs
+-rw-r--r--   0        0        0     5638 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/generators/position_id.rs
+-rw-r--r--   0        0        0     3403 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/handlers.rs
+-rw-r--r--   0        0        0     2956 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/interface/account.rs
+-rw-r--r--   0        0        0      977 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/interface/mod.rs
+-rw-r--r--   0        0        0     2065 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/lib.rs
+-rw-r--r--   0        0        0     7640 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/logging/headers.rs
+-rw-r--r--   0        0        0    24139 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/logging/logger.rs
+-rw-r--r--   0        0        0     5414 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/logging/mod.rs
+-rw-r--r--   0        0        0     7942 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/logging/writer.rs
+-rw-r--r--   0        0        0    20928 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/msgbus/core.rs
+-rw-r--r--   0        0        0     1655 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/msgbus/database.rs
+-rw-r--r--   0        0        0     1046 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/msgbus/mod.rs
+-rw-r--r--   0        0        0     5841 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/python/clock.rs
+-rw-r--r--   0        0        0     4513 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/python/enums.rs
+-rw-r--r--   0        0        0     4896 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/python/logging.rs
+-rw-r--r--   0        0        0     1999 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/python/mod.rs
+-rw-r--r--   0        0        0     3479 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/python/timer.rs
+-rw-r--r--   0        0        0     2848 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/python/versioning.rs
+-rw-r--r--   0        0        0     1717 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/runtime.rs
+-rw-r--r--   0        0        0     1374 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/stubs.rs
+-rw-r--r--   0        0        0     2496 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/testing.rs
+-rw-r--r--   0        0        0    17733 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/timer.rs
+-rw-r--r--   0        0        0     5934 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/common/src/xrate.rs
+-rw-r--r--   0        0        0      850 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/Cargo.toml
+-rw-r--r--   0        0        0     2755 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/build.rs
+-rw-r--r--   0        0        0      717 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/cbindgen.toml
+-rw-r--r--   0        0        0      824 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/cbindgen_cython.toml
+-rw-r--r--   0        0        0    19226 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/correctness.rs
+-rw-r--r--   0        0        0     9163 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/datetime.rs
+-rw-r--r--   0        0        0     1362 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/equality.rs
+-rw-r--r--   0        0        0     5695 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/ffi/cvec.rs
+-rw-r--r--   0        0        0     1248 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/ffi/datetime.rs
+-rw-r--r--   0        0        0     1020 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/ffi/mod.rs
+-rw-r--r--   0        0        0     8229 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/ffi/parsing.rs
+-rw-r--r--   0        0        0     6642 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/ffi/string.rs
+-rw-r--r--   0        0        0     3986 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/ffi/uuid.rs
+-rw-r--r--   0        0        0     1899 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/lib.rs
+-rw-r--r--   0        0        0     1401 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/message.rs
+-rw-r--r--   0        0        0     8191 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/nanos.rs
+-rw-r--r--   0        0        0     3416 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/parsing.rs
+-rw-r--r--   0        0        0     1067 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/python/casing.rs
+-rw-r--r--   0        0        0     2691 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/python/datetime.rs
+-rw-r--r--   0        0        0     2894 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/python/mod.rs
+-rw-r--r--   0        0        0     1407 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/python/serialization.rs
+-rw-r--r--   0        0        0     3120 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/python/uuid.rs
+-rw-r--r--   0        0        0     3743 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/serialization.rs
+-rw-r--r--   0        0        0     9003 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/time.rs
+-rw-r--r--   0        0        0     6096 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/core/src/uuid.rs
+-rw-r--r--   0        0        0     1371 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/execution/Cargo.toml
+-rw-r--r--   0        0        0     6804 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/execution/src/client.rs
+-rw-r--r--   0        0        0     8306 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/execution/src/engine.rs
+-rw-r--r--   0        0        0     1733 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/execution/src/lib.rs
+-rw-r--r--   0        0        0    18871 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/execution/src/matching_core.rs
+-rw-r--r--   0        0        0     2809 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/execution/src/messages/cancel.rs
+-rw-r--r--   0        0        0     2633 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/execution/src/messages/cancel_all.rs
+-rw-r--r--   0        0        0     2615 2024-05-31 11:33:44.246135 nautilus_trader-1.194.0/nautilus_core/execution/src/messages/cancel_batch.rs
+-rw-r--r--   0        0        0     2801 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/execution/src/messages/mod.rs
+-rw-r--r--   0        0        0     3464 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/execution/src/messages/modify.rs
+-rw-r--r--   0        0        0     2804 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/execution/src/messages/query.rs
+-rw-r--r--   0        0        0     3219 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/execution/src/messages/submit.rs
+-rw-r--r--   0        0        0     3266 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/execution/src/messages/submit_list.rs
+-rw-r--r--   0        0        0      746 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/Cargo.toml
+-rw-r--r--   0        0        0     8955 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/average/ama.rs
+-rw-r--r--   0        0        0     7046 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/average/dema.rs
+-rw-r--r--   0        0        0     6963 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/average/ema.rs
+-rw-r--r--   0        0        0     8376 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/average/hma.rs
+-rw-r--r--   0        0        0     2889 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/average/mod.rs
+-rw-r--r--   0        0        0     6981 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/average/rma.rs
+-rw-r--r--   0        0        0     6198 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/average/sma.rs
+-rw-r--r--   0        0        0     7544 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/average/vidya.rs
+-rw-r--r--   0        0        0     6129 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/average/vwap.rs
+-rw-r--r--   0        0        0     7785 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/average/wma.rs
+-rw-r--r--   0        0        0     6387 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/book/imbalance.rs
+-rw-r--r--   0        0        0      940 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/book/mod.rs
+-rw-r--r--   0        0        0     3198 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/indicator.rs
+-rw-r--r--   0        0        0     1773 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/lib.rs
+-rw-r--r--   0        0        0     7712 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/momentum/aroon.rs
+-rw-r--r--   0        0        0     5079 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/momentum/bias.rs
+-rw-r--r--   0        0        0     7069 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/momentum/cmo.rs
+-rw-r--r--   0        0        0      983 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/momentum/mod.rs
+-rw-r--r--   0        0        0     7934 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/momentum/rsi.rs
+-rw-r--r--   0        0        0     6307 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/momentum/vhf.rs
+-rw-r--r--   0        0        0     2922 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/ama.rs
+-rw-r--r--   0        0        0     2799 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/dema.rs
+-rw-r--r--   0        0        0     2880 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/ema.rs
+-rw-r--r--   0        0        0     2759 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/hma.rs
+-rw-r--r--   0        0        0     1005 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/mod.rs
+-rw-r--r--   0        0        0     2865 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/rma.rs
+-rw-r--r--   0        0        0     2765 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/sma.rs
+-rw-r--r--   0        0        0     3164 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/vidya.rs
+-rw-r--r--   0        0        0     2322 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/vwap.rs
+-rw-r--r--   0        0        0     2755 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/wma.rs
+-rw-r--r--   0        0        0     2221 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/book/imbalance.rs
+-rw-r--r--   0        0        0      903 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/book/mod.rs
+-rw-r--r--   0        0        0     2359 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/mod.rs
+-rw-r--r--   0        0        0     2901 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/momentum/aroon.rs
+-rw-r--r--   0        0        0     2682 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/momentum/bias.rs
+-rw-r--r--   0        0        0     2748 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/momentum/cmo.rs
+-rw-r--r--   0        0        0      952 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/momentum/mod.rs
+-rw-r--r--   0        0        0     2583 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/momentum/rsi.rs
+-rw-r--r--   0        0        0     2646 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/momentum/vhf.rs
+-rw-r--r--   0        0        0     2005 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/ratio/efficiency_ratio.rs
+-rw-r--r--   0        0        0      910 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/ratio/mod.rs
+-rw-r--r--   0        0        0     3005 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/volatility/atr.rs
+-rw-r--r--   0        0        0      897 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/python/volatility/mod.rs
+-rw-r--r--   0        0        0     8154 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/ratio/efficiency_ratio.rs
+-rw-r--r--   0        0        0      938 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/ratio/mod.rs
+-rw-r--r--   0        0        0     6163 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/stubs.rs
+-rw-r--r--   0        0        0     1509 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/testing.rs
+-rw-r--r--   0        0        0     9311 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/volatility/atr.rs
+-rw-r--r--   0        0        0      930 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/indicators/src/volatility/mod.rs
+-rw-r--r--   0        0        0     1527 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/infrastructure/Cargo.toml
+-rw-r--r--   0        0        0     1855 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/lib.rs
+-rw-r--r--   0        0        0     1430 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/python/mod.rs
+-rw-r--r--   0        0        0     3369 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/python/redis/cache.rs
+-rw-r--r--   0        0        0     1065 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/python/redis/mod.rs
+-rw-r--r--   0        0        0     1960 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/python/redis/msgbus.rs
+-rw-r--r--   0        0        0     6622 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/python/sql/cache_database.rs
+-rw-r--r--   0        0        0      908 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/python/sql/mod.rs
+-rw-r--r--   0        0        0    28088 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/redis/cache.rs
+-rw-r--r--   0        0        0    10578 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/redis/mod.rs
+-rw-r--r--   0        0        0     7063 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/redis/msgbus.rs
+-rw-r--r--   0        0        0    11599 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/cache_database.rs
+-rw-r--r--   0        0        0     1137 2024-05-31 11:33:44.250135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/mod.rs
+-rw-r--r--   0        0        0      987 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/models/general.rs
+-rw-r--r--   0        0        0    26965 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/models/instruments.rs
+-rw-r--r--   0        0        0      953 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/models/mod.rs
+-rw-r--r--   0        0        0    19284 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/models/orders.rs
+-rw-r--r--   0        0        0     1805 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/models/types.rs
+-rw-r--r--   0        0        0    10744 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/pg.rs
+-rw-r--r--   0        0        0    18517 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/queries.rs
+-rw-r--r--   0        0        0    13104 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/infrastructure/tests/test_cache_database_postgres.rs
+-rw-r--r--   0        0        0     1430 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/Cargo.toml
+-rw-r--r--   0        0        0      400 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/benches/criterion_fixed_precision_benchmark.rs
+-rw-r--r--   0        0        0      225 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/benches/iai_fixed_precision_benchmark.rs
+-rw-r--r--   0        0        0     2757 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/build.rs
+-rw-r--r--   0        0        0     1617 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/cbindgen.toml
+-rw-r--r--   0        0        0     1839 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/cbindgen_cython.toml
+-rw-r--r--   0        0        0    33901 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/currencies.rs
+-rw-r--r--   0        0        0    17056 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/data/bar.rs
+-rw-r--r--   0        0        0     8367 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/data/delta.rs
+-rw-r--r--   0        0        0     8506 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/data/deltas.rs
+-rw-r--r--   0        0        0    11212 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/data/depth.rs
+-rw-r--r--   0        0        0     3030 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/data/mod.rs
+-rw-r--r--   0        0        0     6538 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/data/order.rs
+-rw-r--r--   0        0        0     8090 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/data/quote.rs
+-rw-r--r--   0        0        0     9594 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/data/stubs.rs
+-rw-r--r--   0        0        0     6739 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/data/trade.rs
+-rw-r--r--   0        0        0    30937 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/enums.rs
+-rw-r--r--   0        0        0      940 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/account/mod.rs
+-rw-r--r--   0        0        0     4995 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/account/state.rs
+-rw-r--r--   0        0        0     4078 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/account/stubs.rs
+-rw-r--r--   0        0        0      976 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/mod.rs
+-rw-r--r--   0        0        0     7859 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/accepted.rs
+-rw-r--r--   0        0        0     8473 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/cancel_rejected.rs
+-rw-r--r--   0        0        0     7743 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/canceled.rs
+-rw-r--r--   0        0        0     7238 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/denied.rs
+-rw-r--r--   0        0        0     7084 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/emulated.rs
+-rw-r--r--   0        0        0     5516 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/event.rs
+-rw-r--r--   0        0        0     8178 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/expired.rs
+-rw-r--r--   0        0        0    11827 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/filled.rs
+-rw-r--r--   0        0        0    18813 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/initialized.rs
+-rw-r--r--   0        0        0     3888 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/mod.rs
+-rw-r--r--   0        0        0     8456 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/modify_rejected.rs
+-rw-r--r--   0        0        0     8116 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/pending_cancel.rs
+-rw-r--r--   0        0        0     8134 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/pending_update.rs
+-rw-r--r--   0        0        0     7809 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/rejected.rs
+-rw-r--r--   0        0        0     7341 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/released.rs
+-rw-r--r--   0        0        0    11494 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/stubs.rs
+-rw-r--r--   0        0        0     7385 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/submitted.rs
+-rw-r--r--   0        0        0     8229 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/triggered.rs
+-rw-r--r--   0        0        0     9063 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/order/updated.rs
+-rw-r--r--   0        0        0     1987 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/position/changed.rs
+-rw-r--r--   0        0        0     2106 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/position/closed.rs
+-rw-r--r--   0        0        0     1200 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/position/mod.rs
+-rw-r--r--   0        0        0     1791 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/position/opened.rs
+-rw-r--r--   0        0        0     1985 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/events/position/state.rs
+-rw-r--r--   0        0        0     6050 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/data/bar.rs
+-rw-r--r--   0        0        0     1845 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/data/delta.rs
+-rw-r--r--   0        0        0     3549 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/data/deltas.rs
+-rw-r--r--   0        0        0     3787 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/data/depth.rs
+-rw-r--r--   0        0        0      988 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/data/mod.rs
+-rw-r--r--   0        0        0     2417 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/data/order.rs
+-rw-r--r--   0        0        0     2745 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/data/quote.rs
+-rw-r--r--   0        0        0     2203 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/data/trade.rs
+-rw-r--r--   0        0        0    15015 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/enums.rs
+-rw-r--r--   0        0        0      899 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/events/mod.rs
+-rw-r--r--   0        0        0     4681 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/events/order.rs
+-rw-r--r--   0        0        0     3279 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/account_id.rs
+-rw-r--r--   0        0        0     2234 2024-05-31 11:33:44.254135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/client_id.rs
+-rw-r--r--   0        0        0     1398 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/client_order_id.rs
+-rw-r--r--   0        0        0     1381 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/component_id.rs
+-rw-r--r--   0        0        0     1412 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/exec_algorithm_id.rs
+-rw-r--r--   0        0        0     4223 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/instrument_id.rs
+-rw-r--r--   0        0        0     1177 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/mod.rs
+-rw-r--r--   0        0        0     1384 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/order_list_id.rs
+-rw-r--r--   0        0        0     1374 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/position_id.rs
+-rw-r--r--   0        0        0     1374 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/strategy_id.rs
+-rw-r--r--   0        0        0     1343 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/symbol.rs
+-rw-r--r--   0        0        0     1603 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/trade_id.rs
+-rw-r--r--   0        0        0     1360 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/trader_id.rs
+-rw-r--r--   0        0        0     2003 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/venue.rs
+-rw-r--r--   0        0        0     1391 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/venue_order_id.rs
+-rw-r--r--   0        0        0      903 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/instruments/mod.rs
+-rw-r--r--   0        0        0     5657 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/instruments/synthetic.rs
+-rw-r--r--   0        0        0     1062 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/mod.rs
+-rw-r--r--   0        0        0     8556 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/orderbook/book.rs
+-rw-r--r--   0        0        0     3610 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/orderbook/level.rs
+-rw-r--r--   0        0        0      913 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/orderbook/mod.rs
+-rw-r--r--   0        0        0     5719 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/types/currency.rs
+-rw-r--r--   0        0        0      950 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/types/mod.rs
+-rw-r--r--   0        0        0     1596 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/types/money.rs
+-rw-r--r--   0        0        0     1589 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/types/price.rs
+-rw-r--r--   0        0        0     1845 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/ffi/types/quantity.rs
+-rw-r--r--   0        0        0     4581 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/account_id.rs
+-rw-r--r--   0        0        0     2850 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/client_id.rs
+-rw-r--r--   0        0        0     4837 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/client_order_id.rs
+-rw-r--r--   0        0        0     2903 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/component_id.rs
+-rw-r--r--   0        0        0     2915 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/exec_algorithm_id.rs
+-rw-r--r--   0        0        0     4871 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/instrument_id.rs
+-rw-r--r--   0        0        0     1971 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/macros.rs
+-rw-r--r--   0        0        0     3023 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/mod.rs
+-rw-r--r--   0        0        0     2940 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/order_list_id.rs
+-rw-r--r--   0        0        0     2879 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/position_id.rs
+-rw-r--r--   0        0        0     4410 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/strategy_id.rs
+-rw-r--r--   0        0        0     5268 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/stubs.rs
+-rw-r--r--   0        0        0     3089 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/symbol.rs
+-rw-r--r--   0        0        0     4291 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/trade_id.rs
+-rw-r--r--   0        0        0     3640 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/trader_id.rs
+-rw-r--r--   0        0        0     3614 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/venue.rs
+-rw-r--r--   0        0        0     2943 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/venue_order_id.rs
+-rw-r--r--   0        0        0    11059 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/instruments/any.rs
+-rw-r--r--   0        0        0     7749 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/instruments/crypto_future.rs
+-rw-r--r--   0        0        0     7802 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/instruments/crypto_perpetual.rs
+-rw-r--r--   0        0        0     7548 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/instruments/currency_pair.rs
+-rw-r--r--   0        0        0     6669 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/instruments/equity.rs
+-rw-r--r--   0        0        0     7376 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/instruments/futures_contract.rs
+-rw-r--r--   0        0        0     7498 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/instruments/futures_spread.rs
+-rw-r--r--   0        0        0     5471 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/instruments/mod.rs
+-rw-r--r--   0        0        0     7626 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/instruments/options_contract.rs
+-rw-r--r--   0        0        0     7489 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/instruments/options_spread.rs
+-rw-r--r--   0        0        0    13378 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/instruments/stubs.rs
+-rw-r--r--   0        0        0     6549 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/instruments/synthetic.rs
+-rw-r--r--   0        0        0     2074 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/lib.rs
+-rw-r--r--   0        0        0     1595 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/macros.rs
+-rw-r--r--   0        0        0     3609 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orderbook/aggregation.rs
+-rw-r--r--   0        0        0     4356 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orderbook/analysis.rs
+-rw-r--r--   0        0        0    23153 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orderbook/book.rs
+-rw-r--r--   0        0        0     2882 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orderbook/display.rs
+-rw-r--r--   0        0        0     2053 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orderbook/error.rs
+-rw-r--r--   0        0        0    22568 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orderbook/ladder.rs
+-rw-r--r--   0        0        0    13114 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orderbook/level.rs
+-rw-r--r--   0        0        0     1059 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orderbook/mod.rs
+-rw-r--r--   0        0        0    25461 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orders/any.rs
+-rw-r--r--   0        0        0    31865 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orders/base.rs
+-rw-r--r--   0        0        0     9406 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orders/default.rs
+-rw-r--r--   0        0        0    14332 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orders/limit.rs
+-rw-r--r--   0        0        0    11282 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orders/limit_if_touched.rs
+-rw-r--r--   0        0        0     4601 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orders/list.rs
+-rw-r--r--   0        0        0    11990 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orders/market.rs
+-rw-r--r--   0        0        0    10900 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orders/market_if_touched.rs
+-rw-r--r--   0        0        0    10090 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orders/market_to_limit.rs
+-rw-r--r--   0        0        0     1262 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orders/mod.rs
+-rw-r--r--   0        0        0    12339 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orders/stop_limit.rs
+-rw-r--r--   0        0        0    10869 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orders/stop_market.rs
+-rw-r--r--   0        0        0     8366 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orders/stubs.rs
+-rw-r--r--   0        0        0    11930 2024-05-31 11:33:44.258135 nautilus_trader-1.194.0/nautilus_core/model/src/orders/trailing_stop_limit.rs
+-rw-r--r--   0        0        0    11377 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/orders/trailing_stop_market.rs
+-rw-r--r--   0        0        0     3133 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/polymorphism.rs
+-rw-r--r--   0        0        0    72884 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/position.rs
+-rw-r--r--   0        0        0     7166 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/common.rs
+-rw-r--r--   0        0        0    12321 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/data/bar.rs
+-rw-r--r--   0        0        0    10587 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/data/delta.rs
+-rw-r--r--   0        0        0     4435 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/data/deltas.rs
+-rw-r--r--   0        0        0     8920 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/data/depth.rs
+-rw-r--r--   0        0        0     3417 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/data/mod.rs
+-rw-r--r--   0        0        0     5608 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/data/order.rs
+-rw-r--r--   0        0        0    14445 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/data/quote.rs
+-rw-r--r--   0        0        0    12629 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/data/trade.rs
+-rw-r--r--   0        0        0    44493 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/enums.rs
+-rw-r--r--   0        0        0      899 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/account/mod.rs
+-rw-r--r--   0        0        0     6244 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/account/state.rs
+-rw-r--r--   0        0        0      958 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/mod.rs
+-rw-r--r--   0        0        0     3547 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/accepted.rs
+-rw-r--r--   0        0        0     4036 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/cancel_rejected.rs
+-rw-r--r--   0        0        0     3819 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/canceled.rs
+-rw-r--r--   0        0        0     3297 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/denied.rs
+-rw-r--r--   0        0        0     3110 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/emulated.rs
+-rw-r--r--   0        0        0     3815 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/expired.rs
+-rw-r--r--   0        0        0     7663 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/filled.rs
+-rw-r--r--   0        0        0    11003 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/initialized.rs
+-rw-r--r--   0        0        0     5587 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/mod.rs
+-rw-r--r--   0        0        0     4047 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/modify_rejected.rs
+-rw-r--r--   0        0        0     3710 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/pending_cancel.rs
+-rw-r--r--   0        0        0     3710 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/pending_update.rs
+-rw-r--r--   0        0        0     3570 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/rejected.rs
+-rw-r--r--   0        0        0     3269 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/released.rs
+-rw-r--r--   0        0        0     3259 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/submitted.rs
+-rw-r--r--   0        0        0     3817 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/triggered.rs
+-rw-r--r--   0        0        0     4457 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/updated.rs
+-rw-r--r--   0        0        0     3628 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/identifiers/instrument_id.rs
+-rw-r--r--   0        0        0     1989 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/identifiers/mod.rs
+-rw-r--r--   0        0        0     3411 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/identifiers/trade_id.rs
+-rw-r--r--   0        0        0     9563 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/crypto_future.rs
+-rw-r--r--   0        0        0     9055 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/crypto_perpetual.rs
+-rw-r--r--   0        0        0     8593 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/currency_pair.rs
+-rw-r--r--   0        0        0     7022 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/equity.rs
+-rw-r--r--   0        0        0     8544 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/futures_contract.rs
+-rw-r--r--   0        0        0     8806 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/futures_spread.rs
+-rw-r--r--   0        0        0     3606 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/mod.rs
+-rw-r--r--   0        0        0     9059 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/options_contract.rs
+-rw-r--r--   0        0        0     8804 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/options_spread.rs
+-rw-r--r--   0        0        0     3531 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/macros.rs
+-rw-r--r--   0        0        0     7351 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/mod.rs
+-rw-r--r--   0        0        0     6786 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/orderbook/book.rs
+-rw-r--r--   0        0        0     2104 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/orderbook/level.rs
+-rw-r--r--   0        0        0      983 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/orderbook/mod.rs
+-rw-r--r--   0        0        0    22070 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/limit.rs
+-rw-r--r--   0        0        0     4518 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/limit_if_touched.rs
+-rw-r--r--   0        0        0    18609 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/market.rs
+-rw-r--r--   0        0        0     4433 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/market_if_touched.rs
+-rw-r--r--   0        0        0     4159 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/market_to_limit.rs
+-rw-r--r--   0        0        0     4422 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/mod.rs
+-rw-r--r--   0        0        0    22168 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/stop_limit.rs
+-rw-r--r--   0        0        0     4412 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/stop_market.rs
+-rw-r--r--   0        0        0     4750 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/trailing_stop_limit.rs
+-rw-r--r--   0        0        0     4610 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/trailing_stop_market.rs
+-rw-r--r--   0        0        0    12642 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/position.rs
+-rw-r--r--   0        0        0     6219 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/types/balance.rs
+-rw-r--r--   0        0        0     5123 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/types/currency.rs
+-rw-r--r--   0        0        0     1054 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/types/mod.rs
+-rw-r--r--   0        0        0    14239 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/types/money.rs
+-rw-r--r--   0        0        0    14708 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/types/price.rs
+-rw-r--r--   0        0        0    14615 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/python/types/quantity.rs
+-rw-r--r--   0        0        0     5470 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/stubs.rs
+-rw-r--r--   0        0        0     5786 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/types/balance.rs
+-rw-r--r--   0        0        0     7575 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/types/currency.rs
+-rw-r--r--   0        0        0     6622 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/types/fixed.rs
+-rw-r--r--   0        0        0     1110 2024-05-31 11:33:44.262135 nautilus_trader-1.194.0/nautilus_core/model/src/types/mod.rs
+-rw-r--r--   0        0        0    11798 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/model/src/types/money.rs
+-rw-r--r--   0        0        0    14431 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/model/src/types/price.rs
+-rw-r--r--   0        0        0    14549 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/model/src/types/quantity.rs
+-rw-r--r--   0        0        0     1475 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/model/src/types/stubs.rs
+-rw-r--r--   0        0        0     3064 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/model/src/venues.rs
+-rw-r--r--   0        0        0     1036 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/Cargo.toml
+-rw-r--r--   0        0        0     1655 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/benches/test_client.rs
+-rw-r--r--   0        0        0     1374 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/benches/test_server.rs
+-rw-r--r--   0        0        0    12501 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/src/http.rs
+-rw-r--r--   0        0        0     1802 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/src/lib.rs
+-rw-r--r--   0        0        0     1475 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/src/python/mod.rs
+-rw-r--r--   0        0        0     6239 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/src/ratelimiter/clock.rs
+-rw-r--r--   0        0        0     5467 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/src/ratelimiter/gcra.rs
+-rw-r--r--   0        0        0     8865 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/src/ratelimiter/mod.rs
+-rw-r--r--   0        0        0     4079 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/src/ratelimiter/nanos.rs
+-rw-r--r--   0        0        0     9739 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/src/ratelimiter/quota.rs
+-rw-r--r--   0        0        0    23585 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/src/socket.rs
+-rw-r--r--   0        0        0    28906 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/src/websocket.rs
+-rw-r--r--   0        0        0       18 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/.gitignore
+-rw-r--r--   0        0        0     2862 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/CHANGELOG.md
+-rw-r--r--   0        0        0     2061 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/Cargo.toml
+-rw-r--r--   0        0        0     1093 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/LICENSE
+-rw-r--r--   0        0        0     2861 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/README.md
+-rw-r--r--   0        0        0      268 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/rustfmt.toml
+-rw-r--r--   0        0        0     6900 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/src/compat.rs
+-rw-r--r--   0        0        0     2747 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/src/connect.rs
+-rw-r--r--   0        0        0     5469 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/src/handshake.rs
+-rw-r--r--   0        0        0    14303 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/src/lib.rs
+-rw-r--r--   0        0        0     2854 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/src/stream.rs
+-rw-r--r--   0        0        0     8647 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/src/tls.rs
+-rw-r--r--   0        0        0     1300 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/Cargo.toml
+-rw-r--r--   0        0        0     3658 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/benches/bench_persistence.rs
+-rw-r--r--   0        0        0    12962 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/arrow/bar.rs
+-rw-r--r--   0        0        0    15825 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/arrow/delta.rs
+-rw-r--r--   0        0        0    41488 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/arrow/depth.rs
+-rw-r--r--   0        0        0     4662 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/arrow/mod.rs
+-rw-r--r--   0        0        0    12628 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/arrow/quote.rs
+-rw-r--r--   0        0        0    12946 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/arrow/trade.rs
+-rw-r--r--   0        0        0    10386 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/backend/kmerge_batch.rs
+-rw-r--r--   0        0        0     1025 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/backend/mod.rs
+-rw-r--r--   0        0        0     8172 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/backend/session.rs
+-rw-r--r--   0        0        0     1736 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/lib.rs
+-rw-r--r--   0        0        0      922 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/python/backend/mod.rs
+-rw-r--r--   0        0        0     4265 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/python/backend/session.rs
+-rw-r--r--   0        0        0    12804 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/python/backend/transformer.rs
+-rw-r--r--   0        0        0     1696 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/python/mod.rs
+-rw-r--r--   0        0        0     2824 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/python/wranglers/bar.rs
+-rw-r--r--   0        0        0     3031 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/python/wranglers/delta.rs
+-rw-r--r--   0        0        0      942 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/python/wranglers/mod.rs
+-rw-r--r--   0        0        0     2955 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/python/wranglers/quote.rs
+-rw-r--r--   0        0        0     2952 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/src/python/wranglers/trade.rs
+-rw-r--r--   0        0        0    10633 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/tests/test_catalog.rs
+-rw-r--r--   0        0        0     2159 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/persistence/tests/test_util.rs
+-rw-r--r--   0        0        0     1469 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/pyo3/Cargo.toml
+-rw-r--r--   0        0        0     4929 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/pyo3/src/lib.rs
+-rw-r--r--   0        0        0       50 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/rust-toolchain.toml
+-rw-r--r--   0        0        0      225 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_core/rustfmt.toml
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_trader/__init__.pxd
+-rw-r--r--   0        0        0     2270 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_trader/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_trader/accounting/__init__.pxd
+-rw-r--r--   0        0        0     1414 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_trader/accounting/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/__init__.pxd
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.266136 nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/__init__.py
+-rw-r--r--   0        0        0     4195 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/base.pxd
+-rw-r--r--   0        0        0    14679 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/base.pyx
+-rw-r--r--   0        0        0     1740 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/betting.pxd
+-rw-r--r--   0        0        0     4117 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/betting.pyx
+-rw-r--r--   0        0        0     2013 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/cash.pxd
+-rw-r--r--   0        0        0    13601 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/cash.pyx
+-rw-r--r--   0        0        0     3309 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/margin.pxd
+-rw-r--r--   0        0        0    22719 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/margin.pyx
+-rw-r--r--   0        0        0     1489 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/accounting/calculators.pxd
+-rw-r--r--   0        0        0    10740 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/accounting/calculators.pyx
+-rw-r--r--   0        0        0     2111 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/accounting/error.py
+-rw-r--r--   0        0        0     1089 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/accounting/factory.pxd
+-rw-r--r--   0        0        0     4065 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/accounting/factory.pyx
+-rw-r--r--   0        0        0     2653 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/accounting/manager.pxd
+-rw-r--r--   0        0        0    22688 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/accounting/manager.pyx
+-rw-r--r--   0        0        0     1153 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/_template/__init__.py
+-rw-r--r--   0        0        0     1013 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/_template/core.py
+-rw-r--r--   0        0        0    14665 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/_template/data.py
+-rw-r--r--   0        0        0     7371 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/_template/execution.py
+-rw-r--r--   0        0        0     2601 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/_template/providers.py
+-rw-r--r--   0        0        0      945 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/__init__.py
+-rw-r--r--   0        0        0    12517 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/client.py
+-rw-r--r--   0        0        0     3924 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/common.py
+-rw-r--r--   0        0        0     2529 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/config.py
+-rw-r--r--   0        0        0     2038 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/constants.py
+-rw-r--r--   0        0        0    12440 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/data.py
+-rw-r--r--   0        0        0    10941 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/data_types.py
+-rw-r--r--   0        0        0    42389 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/execution.py
+-rw-r--r--   0        0        0     7519 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/factories.py
+-rw-r--r--   0        0        0     1257 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/orderbook.pxd
+-rw-r--r--   0        0        0     1770 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/orderbook.pyx
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/parsing/__init__.py
+-rw-r--r--   0        0        0     3234 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/parsing/common.py
+-rw-r--r--   0        0        0     4607 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/parsing/core.py
+-rw-r--r--   0        0        0    19955 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/parsing/requests.py
+-rw-r--r--   0        0        0    19805 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/parsing/streaming.py
+-rw-r--r--   0        0        0    12917 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/providers.py
+-rw-r--r--   0        0        0     9450 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/sockets.py
+-rw-r--r--   0        0        0      938 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/__init__.py
+-rw-r--r--   0        0        0      997 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/constants.py
+-rw-r--r--   0        0        0     1871 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/credentials.py
+-rw-r--r--   0        0        0    39673 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/data.py
+-rw-r--r--   0        0        0    19212 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/enums.py
+-rw-r--r--   0        0        0    41882 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/execution.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/schemas/__init__.py
+-rw-r--r--   0        0        0    10932 2024-05-31 11:33:44.270135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/schemas/account.py
+-rw-r--r--   0        0        0    22048 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/schemas/market.py
+-rw-r--r--   0        0        0     1209 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/schemas/user.py
+-rw-r--r--   0        0        0     2570 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/symbol.py
+-rw-r--r--   0        0        0    15632 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/types.py
+-rw-r--r--   0        0        0     3476 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/urls.py
+-rw-r--r--   0        0        0     5353 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/config.py
+-rw-r--r--   0        0        0    13709 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/factories.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/__init__.py
+-rw-r--r--   0        0        0     6564 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/data.py
+-rw-r--r--   0        0        0     6637 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/enums.py
+-rw-r--r--   0        0        0    13348 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/execution.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/http/__init__.py
+-rw-r--r--   0        0        0    16026 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/http/account.py
+-rw-r--r--   0        0        0     3629 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/http/market.py
+-rw-r--r--   0        0        0     1962 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/http/user.py
+-rw-r--r--   0        0        0     4834 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/http/wallet.py
+-rw-r--r--   0        0        0    17712 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/providers.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/schemas/__init__.py
+-rw-r--r--   0        0        0     7352 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/schemas/account.py
+-rw-r--r--   0        0        0     7646 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/schemas/market.py
+-rw-r--r--   0        0        0    15368 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/schemas/user.py
+-rw-r--r--   0        0        0     1281 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/schemas/wallet.py
+-rw-r--r--   0        0        0     5070 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/types.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/http/__init__.py
+-rw-r--r--   0        0        0    27258 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/http/account.py
+-rw-r--r--   0        0        0     5511 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/http/client.py
+-rw-r--r--   0        0        0     3295 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/http/endpoint.py
+-rw-r--r--   0        0        0     1588 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/http/error.py
+-rw-r--r--   0        0        0    32496 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/http/market.py
+-rw-r--r--   0        0        0     7723 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/http/user.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/__init__.py
+-rw-r--r--   0        0        0     5582 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/data.py
+-rw-r--r--   0        0        0     5563 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/enums.py
+-rw-r--r--   0        0        0    10055 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/execution.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/http/__init__.py
+-rw-r--r--   0        0        0    26141 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/http/account.py
+-rw-r--r--   0        0        0     6645 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/http/market.py
+-rw-r--r--   0        0        0     1968 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/http/user.py
+-rw-r--r--   0        0        0     4590 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/http/wallet.py
+-rw-r--r--   0        0        0    13667 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/providers.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/schemas/__init__.py
+-rw-r--r--   0        0        0     3270 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/schemas/account.py
+-rw-r--r--   0        0        0     6832 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/schemas/market.py
+-rw-r--r--   0        0        0    11717 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/schemas/user.py
+-rw-r--r--   0        0        0     1262 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/schemas/wallet.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/websocket/__init__.py
+-rw-r--r--   0        0        0    16319 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/binance/websocket/client.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/common/__init__.py
+-rw-r--r--   0        0        0     1572 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/common/constants.py
+-rw-r--r--   0        0        0     1825 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/common/credentials.py
+-rw-r--r--   0        0        0    10724 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/common/enums.py
+-rw-r--r--   0        0        0     1502 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/common/error.py
+-rw-r--r--   0        0        0     4024 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/common/parsing.py
+-rw-r--r--   0        0        0     4250 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/common/symbol.py
+-rw-r--r--   0        0        0     2623 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/common/urls.py
+-rw-r--r--   0        0        0     3425 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/config.py
+-rw-r--r--   0        0        0    28960 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/data.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/account/__init__.py
+-rw-r--r--   0        0        0     2369 2024-05-31 11:33:44.274135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/account/fee_rate.py
+-rw-r--r--   0        0        0     2381 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/account/position_info.py
+-rw-r--r--   0        0        0     2293 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/account/wallet_balance.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/asset/__init__.py
+-rw-r--r--   0        0        0     2225 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/asset/coin_info.py
+-rw-r--r--   0        0        0     2594 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/endpoint.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/market/__init__.py
+-rw-r--r--   0        0        0     3608 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/market/instruments_info.py
+-rw-r--r--   0        0        0     2222 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/market/klines.py
+-rw-r--r--   0        0        0     2060 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/market/server_time.py
+-rw-r--r--   0        0        0     3322 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/market/tickers.py
+-rw-r--r--   0        0        0     2132 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/market/trades.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/__init__.py
+-rw-r--r--   0        0        0     2866 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/amend_order.py
+-rw-r--r--   0        0        0     2879 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_amend_order.py
+-rw-r--r--   0        0        0     2525 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_cancel_order.py
+-rw-r--r--   0        0        0     3228 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_place_order.py
+-rw-r--r--   0        0        0     2433 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/cancel_all_orders.py
+-rw-r--r--   0        0        0     2439 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/cancel_order.py
+-rw-r--r--   0        0        0     2466 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/open_orders.py
+-rw-r--r--   0        0        0     2756 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/order_history.py
+-rw-r--r--   0        0        0     2987 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/place_order.py
+-rw-r--r--   0        0        0     2679 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/trade_history.py
+-rw-r--r--   0        0        0    35884 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/execution.py
+-rw-r--r--   0        0        0     9039 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/factories.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/http/__init__.py
+-rw-r--r--   0        0        0    13207 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/http/account.py
+-rw-r--r--   0        0        0     1963 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/http/asset.py
+-rw-r--r--   0        0        0     6629 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/http/client.py
+-rw-r--r--   0        0        0     1083 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/http/errors.py
+-rw-r--r--   0        0        0     7979 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/http/market.py
+-rw-r--r--   0        0        0     1180 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/http/user.py
+-rw-r--r--   0        0        0    11303 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/providers.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/account/__init__.py
+-rw-r--r--   0        0        0     3413 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/account/balance.py
+-rw-r--r--   0        0        0     1204 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/account/fee_rate.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/asset/__init__.py
+-rw-r--r--   0        0        0     1947 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/asset/coin_info.py
+-rw-r--r--   0        0        0     2114 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/common.py
+-rw-r--r--   0        0        0    15794 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/instrument.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/market/__init__.py
+-rw-r--r--   0        0        0     2184 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/market/kline.py
+-rw-r--r--   0        0        0     4540 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/market/orderbook.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/market/risk_limit.py
+-rw-r--r--   0        0        0     1088 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/market/server_time.py
+-rw-r--r--   0        0        0     4461 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/market/ticker.py
+-rw-r--r--   0        0        0     2476 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/market/trades.py
+-rw-r--r--   0        0        0     9705 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/order.py
+-rw-r--r--   0        0        0     2665 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/position.py
+-rw-r--r--   0        0        0     4044 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/trade.py
+-rw-r--r--   0        0        0    22850 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/ws.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/websocket/__init__.py
+-rw-r--r--   0        0        0    11105 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/websocket/client.py
+-rw-r--r--   0        0        0     1689 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/databento/__init__.py
+-rw-r--r--   0        0        0     2749 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/databento/common.py
+-rw-r--r--   0        0        0     2727 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/databento/config.py
+-rw-r--r--   0        0        0     1210 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/databento/constants.py
+-rw-r--r--   0        0        0    39036 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/databento/data.py
+-rw-r--r--   0        0        0     1315 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/databento/enums.py
+-rw-r--r--   0        0        0     6043 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/databento/factories.py
+-rw-r--r--   0        0        0    10712 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/databento/loaders.py
+-rw-r--r--   0        0        0    10149 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/databento/providers.py
+-rw-r--r--   0        0        0    10104 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/databento/publishers.json
+-rw-r--r--   0        0        0     1141 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/databento/types.py
+-rw-r--r--   0        0        0     1193 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/env.py
+-rw-r--r--   0        0        0      930 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/__init__.py
+-rw-r--r--   0        0        0     1014 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/__init__.py
+-rw-r--r--   0        0        0     6415 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/account.py
+-rw-r--r--   0        0        0    26860 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/client.py
+-rw-r--r--   0        0        0    15878 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/common.py
+-rw-r--r--   0        0        0     8356 2024-05-31 11:33:44.278135 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/connection.py
+-rw-r--r--   0        0        0     7167 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/contract.py
+-rw-r--r--   0        0        0     8724 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/error.py
+-rw-r--r--   0        0        0    32019 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/market_data.py
+-rw-r--r--   0        0        0    10341 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/order.py
+-rw-r--r--   0        0        0    43317 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/wrapper.py
+-rw-r--r--   0        0        0     6988 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/common.py
+-rw-r--r--   0        0        0     8127 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/config.py
+-rw-r--r--   0        0        0    17152 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/data.py
+-rw-r--r--   0        0        0    39055 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/execution.py
+-rw-r--r--   0        0        0     9005 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/factories.py
+-rw-r--r--   0        0        0     7876 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/gateway.py
+-rw-r--r--   0        0        0     1054 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/historic/__init__.py
+-rw-r--r--   0        0        0    21095 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/historic/client.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/parsing/__init__.py
+-rw-r--r--   0        0        0     3579 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/parsing/data.py
+-rw-r--r--   0        0        0     4007 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/parsing/execution.py
+-rw-r--r--   0        0        0    24117 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/parsing/instruments.py
+-rw-r--r--   0        0        0    12263 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/providers.py
+-rw-r--r--   0        0        0     4904 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/web.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/sandbox/__init__.py
+-rw-r--r--   0        0        0     2360 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/sandbox/config.py
+-rw-r--r--   0        0        0     8450 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/sandbox/execution.py
+-rw-r--r--   0        0        0     2676 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/sandbox/factory.py
+-rw-r--r--   0        0        0      937 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/tardis/__init__.py
+-rw-r--r--   0        0        0     2909 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/adapters/tardis/loaders.py
+-rw-r--r--   0        0        0      978 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/__init__.py
+-rw-r--r--   0        0        0    15183 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/analyzer.py
+-rw-r--r--   0        0        0     5714 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/reporter.py
+-rw-r--r--   0        0        0     3940 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistic.py
+-rw-r--r--   0        0        0     2255 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/__init__.py
+-rw-r--r--   0        0        0     1997 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/expectancy.py
+-rw-r--r--   0        0        0     1705 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/long_ratio.py
+-rw-r--r--   0        0        0     1468 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/loser_avg.py
+-rw-r--r--   0        0        0     1514 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/loser_max.py
+-rw-r--r--   0        0        0     1512 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/loser_min.py
+-rw-r--r--   0        0        0     1563 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/profit_factor.py
+-rw-r--r--   0        0        0     1399 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/returns_avg.py
+-rw-r--r--   0        0        0     1414 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/returns_avg_loss.py
+-rw-r--r--   0        0        0     1413 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/returns_avg_win.py
+-rw-r--r--   0        0        0     1716 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/returns_volatility.py
+-rw-r--r--   0        0        0     1323 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/risk_return_ratio.py
+-rw-r--r--   0        0        0     1776 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/sharpe_ratio.py
+-rw-r--r--   0        0        0     1883 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/sortino_ratio.py
+-rw-r--r--   0        0        0     1498 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/win_rate.py
+-rw-r--r--   0        0        0     1489 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/winner_avg.py
+-rw-r--r--   0        0        0     1347 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/winner_max.py
+-rw-r--r--   0        0        0     1494 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/winner_min.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/backtest/__init__.pxd
+-rw-r--r--   0        0        0      946 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/backtest/__init__.py
+-rw-r--r--   0        0        0     1868 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/backtest/__main__.py
+-rw-r--r--   0        0        0     3840 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/backtest/auction.py
+-rw-r--r--   0        0        0     9257 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/backtest/config.py
+-rw-r--r--   0        0        0     1100 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/backtest/data_client.pxd
+-rw-r--r--   0        0        0    13931 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/backtest/data_client.pyx
+-rw-r--r--   0        0        0     2162 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/backtest/engine.pxd
+-rw-r--r--   0        0        0    51499 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/backtest/engine.pyx
+-rw-r--r--   0        0        0     7849 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/backtest/exchange.pxd
+-rw-r--r--   0        0        0    33198 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/backtest/exchange.pyx
+-rw-r--r--   0        0        0     1084 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/backtest/execution_client.pxd
+-rw-r--r--   0        0        0     5264 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/backtest/execution_client.pyx
+-rw-r--r--   0        0        0    12270 2024-05-31 11:33:44.282136 nautilus_trader-1.194.0/nautilus_trader/backtest/matching_engine.pxd
+-rw-r--r--   0        0        0    98825 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/backtest/matching_engine.pyx
+-rw-r--r--   0        0        0     2658 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/backtest/models.pxd
+-rw-r--r--   0        0        0     8785 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/backtest/models.pyx
+-rw-r--r--   0        0        0     1893 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/backtest/modules.pxd
+-rw-r--r--   0        0        0     8483 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/backtest/modules.pyx
+-rw-r--r--   0        0        0    15294 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/backtest/node.py
+-rw-r--r--   0        0        0     3072 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/backtest/results.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/cache/__init__.pxd
+-rw-r--r--   0        0        0     1220 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/cache/__init__.py
+-rw-r--r--   0        0        0    10536 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/cache/base.pxd
+-rw-r--r--   0        0        0    25831 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/cache/base.pyx
+-rw-r--r--   0        0        0     8701 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/cache/cache.pxd
+-rw-r--r--   0        0        0   135124 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/cache/cache.pyx
+-rw-r--r--   0        0        0     2884 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/cache/config.py
+-rw-r--r--   0        0        0     1104 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/cache/database.pxd
+-rw-r--r--   0        0        0    36283 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/cache/database.pyx
+-rw-r--r--   0        0        0     5051 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/cache/facade.pxd
+-rw-r--r--   0        0        0    11952 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/cache/facade.pyx
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/cache/postgres/__init__.py
+-rw-r--r--   0        0        0     4228 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/cache/postgres/adapter.py
+-rw-r--r--   0        0        0    12833 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/cache/postgres/transformers.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/common/__init__.pxd
+-rw-r--r--   0        0        0     1571 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/common/__init__.py
+-rw-r--r--   0        0        0    11890 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/common/actor.pxd
+-rw-r--r--   0        0        0    92278 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/common/actor.pyx
+-rw-r--r--   0        0        0    11128 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/common/component.pxd
+-rw-r--r--   0        0        0    88235 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/common/component.pyx
+-rw-r--r--   0        0        0    16790 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/common/config.py
+-rw-r--r--   0        0        0     1849 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/common/enums.py
+-rw-r--r--   0        0        0    10785 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/common/executor.py
+-rw-r--r--   0        0        0     9517 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/common/factories.pxd
+-rw-r--r--   0        0        0    58923 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/common/factories.pyx
+-rw-r--r--   0        0        0     1320 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/common/functions.py
+-rw-r--r--   0        0        0     2143 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/common/generators.pxd
+-rw-r--r--   0        0        0     7841 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/common/generators.pyx
+-rw-r--r--   0        0        0     2723 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/common/messages.pxd
+-rw-r--r--   0        0        0    11741 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/common/messages.pyx
+-rw-r--r--   0        0        0    10413 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/common/providers.py
+-rw-r--r--   0        0        0     5512 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/config/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/core/__init__.pxd
+-rw-r--r--   0        0        0     1339 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/core/__init__.py
+-rw-r--r--   0        0        0     1230 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/core/asynchronous.py
+-rw-r--r--   0        0        0     3683 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/core/correctness.pxd
+-rw-r--r--   0        0        0    37557 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/core/correctness.pyx
+-rw-r--r--   0        0        0      897 2024-05-31 11:33:44.286136 nautilus_trader-1.194.0/nautilus_trader/core/data.pxd
+-rw-r--r--   0        0        0     1954 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/data.pyx
+-rw-r--r--   0        0        0     1363 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/datetime.pxd
+-rw-r--r--   0        0        0     7616 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/datetime.pyx
+-rw-r--r--   0        0        0     1230 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/fsm.pxd
+-rw-r--r--   0        0        0     4364 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/fsm.pyx
+-rw-r--r--   0        0        0     2511 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/includes/algorithms.h
+-rw-r--r--   0        0        0      907 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/includes/backtest.h
+-rw-r--r--   0        0        0    16091 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/includes/common.h
+-rw-r--r--   0        0        0     3055 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/includes/core.h
+-rw-r--r--   0        0        0    64690 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/includes/model.h
+-rw-r--r--   0        0        0     2529 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/inspect.py
+-rw-r--r--   0        0        0     2137 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/message.pxd
+-rw-r--r--   0        0        0     6509 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/message.pyx
+-rw-r--r--   0        0        0    88270 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/nautilus_pyo3.pyi
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/rust/__init__.pxd
+-rw-r--r--   0        0        0     2685 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/rust/algorithms.pxd
+-rw-r--r--   0        0        0     1050 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/rust/backtest.pxd
+-rw-r--r--   0        0        0    15818 2024-05-31 11:38:34.087206 nautilus_trader-1.194.0/nautilus_trader/core/rust/common.pxd
+-rw-r--r--   0        0        0     1222 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/rust/common.pyx
+-rw-r--r--   0        0        0     3107 2024-05-31 11:35:53.258719 nautilus_trader-1.194.0/nautilus_trader/core/rust/core.pxd
+-rw-r--r--   0        0        0    60647 2024-05-31 11:37:11.079095 nautilus_trader-1.194.0/nautilus_trader/core/rust/model.pxd
+-rw-r--r--   0        0        0     2702 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/rust/model.pyx
+-rw-r--r--   0        0        0     1359 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/stats.pxd
+-rw-r--r--   0        0        0     5710 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/stats.pyx
+-rw-r--r--   0        0        0     3870 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/string.pxd
+-rw-r--r--   0        0        0     1049 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/uuid.pxd
+-rw-r--r--   0        0        0     2755 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/core/uuid.pyx
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/data/__init__.pxd
+-rw-r--r--   0        0        0     1360 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/data/__init__.py
+-rw-r--r--   0        0        0     4191 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/data/aggregation.pxd
+-rw-r--r--   0        0        0    24575 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/data/aggregation.pyx
+-rw-r--r--   0        0        0     8072 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/data/client.pxd
+-rw-r--r--   0        0        0    39952 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/data/client.pyx
+-rw-r--r--   0        0        0     2304 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/data/config.py
+-rw-r--r--   0        0        0    10206 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/data/engine.pxd
+-rw-r--r--   0        0        0    68259 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/data/engine.pyx
+-rw-r--r--   0        0        0     2391 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/data/messages.pxd
+-rw-r--r--   0        0        0     8362 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/data/messages.pyx
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/algorithms/__init__.py
+-rw-r--r--   0        0        0     4226 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/algorithms/blank.py
+-rw-r--r--   0        0        0    11242 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/algorithms/twap.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/__init__.pxd
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/__init__.py
+-rw-r--r--   0        0        0     5269 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/blank.py
+-rw-r--r--   0        0        0    11736 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/ema_cross.py
+-rw-r--r--   0        0        0    11534 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/ema_cross_bracket.py
+-rw-r--r--   0        0        0    14158 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/ema_cross_bracket_algo.py
+-rw-r--r--   0        0        0    10284 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/ema_cross_cython.pyx
+-rw-r--r--   0        0        0    11178 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/ema_cross_long_only.py
+-rw-r--r--   0        0        0    15993 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/ema_cross_stop_entry.py
+-rw-r--r--   0        0        0    14118 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/ema_cross_trailing_stop.py
+-rw-r--r--   0        0        0    12012 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/ema_cross_twap.py
+-rw-r--r--   0        0        0     5286 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/market_maker.py
+-rw-r--r--   0        0        0     8954 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/orderbook_imbalance.py
+-rw-r--r--   0        0        0     9291 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/orderbook_imbalance_rust.py
+-rw-r--r--   0        0        0     2839 2024-05-31 11:33:44.290135 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/signal_strategy.py
+-rw-r--r--   0        0        0     4718 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/subscribe.py
+-rw-r--r--   0        0        0     7283 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/talib_strategy.py
+-rw-r--r--   0        0        0    14071 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/examples/strategies/volatility_market_maker.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/__init__.pxd
+-rw-r--r--   0        0        0     1353 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/__init__.py
+-rw-r--r--   0        0        0     8527 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/algorithm.pxd
+-rw-r--r--   0        0        0    52607 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/algorithm.pyx
+-rw-r--r--   0        0        0     7359 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/client.pxd
+-rw-r--r--   0        0        0    29170 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/client.pyx
+-rw-r--r--   0        0        0     3587 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/config.py
+-rw-r--r--   0        0        0     4001 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/emulator.pxd
+-rw-r--r--   0        0        0    35586 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/emulator.pyx
+-rw-r--r--   0        0        0     6956 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/engine.pxd
+-rw-r--r--   0        0        0    46472 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/engine.pyx
+-rw-r--r--   0        0        0     4593 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/manager.pxd
+-rw-r--r--   0        0        0    24284 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/manager.pyx
+-rw-r--r--   0        0        0     3590 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/matching_core.pxd
+-rw-r--r--   0        0        0    16178 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/matching_core.pyx
+-rw-r--r--   0        0        0     5598 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/messages.pxd
+-rw-r--r--   0        0        0    34648 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/messages.pyx
+-rw-r--r--   0        0        0    22236 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/reports.py
+-rw-r--r--   0        0        0     1726 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/trailing.pxd
+-rw-r--r--   0        0        0    17089 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/execution/trailing.pyx
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/__init__.pxd
+-rw-r--r--   0        0        0     1188 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/__init__.py
+-rw-r--r--   0        0        0     1722 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/amat.pxd
+-rw-r--r--   0        0        0     4832 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/amat.pyx
+-rw-r--r--   0        0        0     1482 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/aroon.pxd
+-rw-r--r--   0        0        0     3470 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/aroon.pyx
+-rw-r--r--   0        0        0     1474 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/atr.pxd
+-rw-r--r--   0        0        0     4320 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/atr.pyx
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/__init__.pxd
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/__init__.py
+-rw-r--r--   0        0        0     1770 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/ama.pxd
+-rw-r--r--   0        0        0     5185 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/ama.pyx
+-rw-r--r--   0        0        0     1063 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/dema.pxd
+-rw-r--r--   0        0        0     3840 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/dema.pyx
+-rw-r--r--   0        0        0     1096 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/ema.pxd
+-rw-r--r--   0        0        0     3454 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/ema.pyx
+-rw-r--r--   0        0        0     1247 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/hma.pxd
+-rw-r--r--   0        0        0     4323 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/hma.pyx
+-rw-r--r--   0        0        0     3114 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/ma_factory.pyx
+-rw-r--r--   0        0        0     1568 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/moving_average.pxd
+-rw-r--r--   0        0        0     2960 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/moving_average.pyx
+-rw-r--r--   0        0        0     1080 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/rma.pxd
+-rw-r--r--   0        0        0     3466 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/rma.pyx
+-rw-r--r--   0        0        0     1020 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/sma.pxd
+-rw-r--r--   0        0        0     3530 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/sma.pyx
+-rw-r--r--   0        0        0     1283 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/vidya.pxd
+-rw-r--r--   0        0        0     4592 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/vidya.pyx
+-rw-r--r--   0        0        0     1174 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/wma.pxd
+-rw-r--r--   0        0        0     4700 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/average/wma.pyx
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/base/__init__.pxd
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/base/__init__.py
+-rw-r--r--   0        0        0     1701 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/base/indicator.pxd
+-rw-r--r--   0        0        0     3029 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/base/indicator.pyx
+-rw-r--r--   0        0        0     1315 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/bias.pxd
+-rw-r--r--   0        0        0     2868 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/bias.pyx
+-rw-r--r--   0        0        0     1579 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/bollinger_bands.pxd
+-rw-r--r--   0        0        0     5219 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/bollinger_bands.pyx
+-rw-r--r--   0        0        0     1635 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/cci.pxd
+-rw-r--r--   0        0        0     4056 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/cci.pyx
+-rw-r--r--   0        0        0     1375 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/cmo.pxd
+-rw-r--r--   0        0        0     3766 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/cmo.pyx
+-rw-r--r--   0        0        0     1658 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/dm.pxd
+-rw-r--r--   0        0        0     3732 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/dm.pyx
+-rw-r--r--   0        0        0     1490 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/donchian_channel.pxd
+-rw-r--r--   0        0        0     4374 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/donchian_channel.pyx
+-rw-r--r--   0        0        0     1231 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/efficiency_ratio.pxd
+-rw-r--r--   0        0        0     3119 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/efficiency_ratio.pyx
+-rw-r--r--   0        0        0     3168 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_candlesticks.pxd
+-rw-r--r--   0        0        0    12540 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_candlesticks.pyx
+-rw-r--r--   0        0        0     1347 2024-05-31 11:33:44.294136 nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enum.pyx
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/__init__.pxd
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/__init__.py
+-rw-r--r--   0        0        0      976 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pxd
+-rw-r--r--   0        0        0      980 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pyx
+-rw-r--r--   0        0        0      947 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pxd
+-rw-r--r--   0        0        0      987 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pyx
+-rw-r--r--   0        0        0     1020 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pxd
+-rw-r--r--   0        0        0      972 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pyx
+-rw-r--r--   0        0        0      972 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pxd
+-rw-r--r--   0        0        0      980 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pyx
+-rw-r--r--   0        0        0     1805 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/keltner_channel.pxd
+-rw-r--r--   0        0        0     4675 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/keltner_channel.pyx
+-rw-r--r--   0        0        0     1395 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/keltner_position.pxd
+-rw-r--r--   0        0        0     4280 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/keltner_position.pyx
+-rw-r--r--   0        0        0     1713 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/kvo.pxd
+-rw-r--r--   0        0        0     4727 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/kvo.pyx
+-rw-r--r--   0        0        0     1636 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/linear_regression.pxd
+-rw-r--r--   0        0        0     3839 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/linear_regression.pyx
+-rw-r--r--   0        0        0     1664 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/macd.pxd
+-rw-r--r--   0        0        0     4809 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/macd.pyx
+-rw-r--r--   0        0        0     1232 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/obv.pxd
+-rw-r--r--   0        0        0     2958 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/obv.pyx
+-rw-r--r--   0        0        0     1514 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/pressure.pxd
+-rw-r--r--   0        0        0     4383 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/pressure.pyx
+-rw-r--r--   0        0        0     1476 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/psl.pxd
+-rw-r--r--   0        0        0     3311 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/psl.pyx
+-rw-r--r--   0        0        0     1227 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/roc.pxd
+-rw-r--r--   0        0        0     2726 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/roc.pyx
+-rw-r--r--   0        0        0     1393 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/rsi.pxd
+-rw-r--r--   0        0        0     3767 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/rsi.pyx
+-rw-r--r--   0        0        0     1763 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/rvi.pxd
+-rw-r--r--   0        0        0     4539 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/rvi.pyx
+-rw-r--r--   0        0        0     1444 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/spread_analyzer.pxd
+-rw-r--r--   0        0        0     3391 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/spread_analyzer.pyx
+-rw-r--r--   0        0        0     1485 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/stochastics.pxd
+-rw-r--r--   0        0        0     3884 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/stochastics.pyx
+-rw-r--r--   0        0        0     2271 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/swings.pxd
+-rw-r--r--   0        0        0     4678 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/swings.pyx
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/ta_lib/__init__.py
+-rw-r--r--   0        0        0     1993 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/ta_lib/common.py
+-rw-r--r--   0        0        0    29656 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/ta_lib/manager.py
+-rw-r--r--   0        0        0     1458 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/vhf.pxd
+-rw-r--r--   0        0        0     3513 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/vhf.pyx
+-rw-r--r--   0        0        0     1485 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/volatility_ratio.pxd
+-rw-r--r--   0        0        0     4482 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/volatility_ratio.pyx
+-rw-r--r--   0        0        0     1270 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/vwap.pxd
+-rw-r--r--   0        0        0     2938 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/indicators/vwap.pyx
+-rw-r--r--   0        0        0     1155 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/live/__init__.py
+-rw-r--r--   0        0        0     1861 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/live/__main__.py
+-rw-r--r--   0        0        0     8314 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/live/config.py
+-rw-r--r--   0        0        0    34312 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/live/data_client.py
+-rw-r--r--   0        0        0    16375 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/live/data_engine.py
+-rw-r--r--   0        0        0    18927 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/live/execution_client.py
+-rw-r--r--   0        0        0    41082 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/live/execution_engine.py
+-rw-r--r--   0        0        0     3395 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/live/factories.py
+-rw-r--r--   0        0        0    16754 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/live/node.py
+-rw-r--r--   0        0        0     9369 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/live/node_builder.py
+-rw-r--r--   0        0        0     9696 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/live/risk_engine.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/model/__init__.pxd
+-rw-r--r--   0        0        0     1652 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/model/__init__.py
+-rw-r--r--   0        0        0     3380 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/model/book.pxd
+-rw-r--r--   0        0        0    24325 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/model/book.pyx
+-rw-r--r--   0        0        0     5067 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/model/currencies.py
+-rw-r--r--   0        0        0    13066 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/model/data.pxd
+-rw-r--r--   0        0        0   126566 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/model/data.pyx
+-rw-r--r--   0        0        0     7811 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/model/enums.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/model/events/__init__.pxd
+-rw-r--r--   0        0        0     2829 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/model/events/__init__.py
+-rw-r--r--   0        0        0     2220 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/model/events/account.pxd
+-rw-r--r--   0        0        0     6660 2024-05-31 11:33:44.298136 nautilus_trader-1.194.0/nautilus_trader/model/events/account.pyx
+-rw-r--r--   0        0        0    12302 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/events/order.pxd
+-rw-r--r--   0        0        0   136228 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/events/order.pyx
+-rw-r--r--   0        0        0     5628 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/events/position.pxd
+-rw-r--r--   0        0        0    35393 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/events/position.pyx
+-rw-r--r--   0        0        0     5142 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/functions.pxd
+-rw-r--r--   0        0        0    10333 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/functions.pyx
+-rw-r--r--   0        0        0     4039 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/identifiers.pxd
+-rw-r--r--   0        0        0    27544 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/identifiers.pyx
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/__init__.pxd
+-rw-r--r--   0        0        0     2302 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/__init__.py
+-rw-r--r--   0        0        0     5519 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/base.pxd
+-rw-r--r--   0        0        0    21405 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/base.pyx
+-rw-r--r--   0        0        0     1778 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/betting.pxd
+-rw-r--r--   0        0        0     8622 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/betting.pyx
+-rw-r--r--   0        0        0     1449 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/cfd.pxd
+-rw-r--r--   0        0        0    13625 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/cfd.pyx
+-rw-r--r--   0        0        0     1296 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/commodity.pxd
+-rw-r--r--   0        0        0    13011 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/commodity.pyx
+-rw-r--r--   0        0        0     1756 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/crypto_future.pxd
+-rw-r--r--   0        0        0    14480 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/crypto_future.pyx
+-rw-r--r--   0        0        0     1563 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/crypto_perpetual.pxd
+-rw-r--r--   0        0        0    13388 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/crypto_perpetual.pyx
+-rw-r--r--   0        0        0     1334 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/currency_pair.pxd
+-rw-r--r--   0        0        0    13495 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/currency_pair.pyx
+-rw-r--r--   0        0        0     1284 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/equity.pxd
+-rw-r--r--   0        0        0     9201 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/equity.pyx
+-rw-r--r--   0        0        0     1736 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/futures_contract.pxd
+-rw-r--r--   0        0        0    11356 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/futures_contract.pyx
+-rw-r--r--   0        0        0     1824 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/futures_spread.pxd
+-rw-r--r--   0        0        0    11963 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/futures_spread.pyx
+-rw-r--r--   0        0        0     2068 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/options_contract.pxd
+-rw-r--r--   0        0        0    12508 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/options_contract.pyx
+-rw-r--r--   0        0        0     1930 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/options_spread.pxd
+-rw-r--r--   0        0        0    12096 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/options_spread.pyx
+-rw-r--r--   0        0        0     1555 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/synthetic.pxd
+-rw-r--r--   0        0        0    12487 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/instruments/synthetic.pyx
+-rw-r--r--   0        0        0     5934 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/objects.pxd
+-rw-r--r--   0        0        0    52381 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/objects.pyx
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/__init__.pxd
+-rw-r--r--   0        0        0     2094 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/__init__.py
+-rw-r--r--   0        0        0     9471 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/base.pxd
+-rw-r--r--   0        0        0    37731 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/base.pyx
+-rw-r--r--   0        0        0     1770 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/limit.pxd
+-rw-r--r--   0        0        0    21400 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/limit.pyx
+-rw-r--r--   0        0        0     2175 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/limit_if_touched.pxd
+-rw-r--r--   0        0        0    17609 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/limit_if_touched.pyx
+-rw-r--r--   0        0        0     1842 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/list.pxd
+-rw-r--r--   0        0        0     2365 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/list.pyx
+-rw-r--r--   0        0        0     1272 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/market.pxd
+-rw-r--r--   0        0        0    15939 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/market.pyx
+-rw-r--r--   0        0        0     1612 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/market_if_touched.pxd
+-rw-r--r--   0        0        0    15818 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/market_if_touched.pyx
+-rw-r--r--   0        0        0     1646 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/market_to_limit.pxd
+-rw-r--r--   0        0        0    14283 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/market_to_limit.pyx
+-rw-r--r--   0        0        0     2232 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/stop_limit.pxd
+-rw-r--r--   0        0        0    20646 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/stop_limit.pyx
+-rw-r--r--   0        0        0     1602 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/stop_market.pxd
+-rw-r--r--   0        0        0    16030 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/stop_market.pyx
+-rw-r--r--   0        0        0     2647 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/trailing_stop_limit.pxd
+-rw-r--r--   0        0        0    19580 2024-05-31 11:33:44.302136 nautilus_trader-1.194.0/nautilus_trader/model/orders/trailing_stop_limit.pyx
+-rw-r--r--   0        0        0     1953 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/model/orders/trailing_stop_market.pxd
+-rw-r--r--   0        0        0    17208 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/model/orders/trailing_stop_market.pyx
+-rw-r--r--   0        0        0     1141 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/model/orders/unpacker.pxd
+-rw-r--r--   0        0        0     3926 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/model/orders/unpacker.pyx
+-rw-r--r--   0        0        0     6940 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/model/position.pxd
+-rw-r--r--   0        0        0    23901 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/model/position.pyx
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/__init__.pxd
+-rw-r--r--   0        0        0     1443 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/__init__.py
+-rw-r--r--   0        0        0     1581 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/base.pxd
+-rw-r--r--   0        0        0     3709 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/base.pyx
+-rw-r--r--   0        0        0     1147 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/implementations/__init__.py
+-rw-r--r--   0        0        0     1371 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/implementations/fixed.pxd
+-rw-r--r--   0        0        0     3921 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/implementations/fixed.pyx
+-rw-r--r--   0        0        0     1388 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/implementations/tiered.pxd
+-rw-r--r--   0        0        0     5436 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/implementations/tiered.pyx
+-rw-r--r--   0        0        0     1333 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/model/venues.py
+-rw-r--r--   0        0        0      973 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/persistence/__init__.py
+-rw-r--r--   0        0        0     1079 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/persistence/catalog/__init__.py
+-rw-r--r--   0        0        0     6321 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/persistence/catalog/base.py
+-rw-r--r--   0        0        0    28127 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/persistence/catalog/parquet.py
+-rw-r--r--   0        0        0     2073 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/persistence/catalog/singleton.py
+-rw-r--r--   0        0        0     1327 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/persistence/catalog/types.py
+-rw-r--r--   0        0        0     2888 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/persistence/config.py
+-rw-r--r--   0        0        0     3561 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/persistence/funcs.py
+-rw-r--r--   0        0        0     7025 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/persistence/loaders.py
+-rw-r--r--   0        0        0     3392 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/persistence/wranglers.pxd
+-rw-r--r--   0        0        0    30305 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/persistence/wranglers.pyx
+-rw-r--r--   0        0        0    16480 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/persistence/wranglers_v2.py
+-rw-r--r--   0        0        0    13185 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/persistence/writer.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/portfolio/__init__.pxd
+-rw-r--r--   0        0        0     1123 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/portfolio/__init__.py
+-rw-r--r--   0        0        0     2132 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/portfolio/base.pxd
+-rw-r--r--   0        0        0     4233 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/portfolio/base.pyx
+-rw-r--r--   0        0        0     3111 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/portfolio/portfolio.pxd
+-rw-r--r--   0        0        0    38292 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/portfolio/portfolio.pyx
+-rw-r--r--   0        0        0        0 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/py.typed
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/risk/__init__.pxd
+-rw-r--r--   0        0        0     1084 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/risk/__init__.py
+-rw-r--r--   0        0        0     1974 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/risk/config.py
+-rw-r--r--   0        0        0     5474 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/risk/engine.pxd
+-rw-r--r--   0        0        0    38261 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/risk/engine.pyx
+-rw-r--r--   0        0        0     1747 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/risk/sizing.pxd
+-rw-r--r--   0        0        0     7059 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/risk/sizing.pyx
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/serialization/__init__.pxd
+-rw-r--r--   0        0        0     1106 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/serialization/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/implementations/__init__.py
+-rw-r--r--   0        0        0     5360 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/implementations/account_state.py
+-rw-r--r--   0        0        0     1689 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/implementations/component_events.py
+-rw-r--r--   0        0        0    14111 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/implementations/instruments.py
+-rw-r--r--   0        0        0     2191 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/implementations/order_events.py
+-rw-r--r--   0        0        0     5923 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/implementations/position_events.py
+-rw-r--r--   0        0        0    15753 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/schema.py
+-rw-r--r--   0        0        0    13937 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/serializer.py
+-rw-r--r--   0        0        0     1096 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/serialization/base.pxd
+-rw-r--r--   0        0        0    12000 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/serialization/base.pyx
+-rw-r--r--   0        0        0     1303 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/serialization/serializer.pxd
+-rw-r--r--   0        0        0     5404 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/serialization/serializer.pyx
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/system/__init__.py
+-rw-r--r--   0        0        0     6506 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/system/config.py
+-rw-r--r--   0        0        0    40208 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/system/kernel.py
+-rw-r--r--   0        0        0     1034 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/test_kit/__init__.py
+-rw-r--r--   0        0        0     2316 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/test_kit/functions.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/test_kit/mocks/__init__.py
+-rw-r--r--   0        0        0     6382 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/test_kit/mocks/actors.py
+-rw-r--r--   0        0        0     5793 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/test_kit/mocks/cache_database.py
+-rw-r--r--   0        0        0     1550 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/test_kit/mocks/controller.py
+-rw-r--r--   0        0        0     3177 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/test_kit/mocks/data.py
+-rw-r--r--   0        0        0     2976 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/test_kit/mocks/engines.py
+-rw-r--r--   0        0        0    12678 2024-05-31 11:33:44.306136 nautilus_trader-1.194.0/nautilus_trader/test_kit/mocks/exec_clients.py
+-rw-r--r--   0        0        0     7299 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/mocks/strategies.py
+-rw-r--r--   0        0        0    29839 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/providers.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/rust/__init__.py
+-rw-r--r--   0        0        0     3697 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/rust/accounting_pyo3.py
+-rw-r--r--   0        0        0     6642 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/rust/data_pyo3.py
+-rw-r--r--   0        0        0    19951 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/rust/events_pyo3.py
+-rw-r--r--   0        0        0     3912 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/rust/identifiers_pyo3.py
+-rw-r--r--   0        0        0    15113 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/rust/instruments_pyo3.py
+-rw-r--r--   0        0        0     5508 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/rust/orders_pyo3.py
+-rw-r--r--   0        0        0     2451 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/rust/types_pyo3.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/__init__.py
+-rw-r--r--   0        0        0     4828 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/commands.py
+-rw-r--r--   0        0        0     5842 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/component.py
+-rw-r--r--   0        0        0     6234 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/config.py
+-rw-r--r--   0        0        0    22387 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/data.py
+-rw-r--r--   0        0        0    14777 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/events.py
+-rw-r--r--   0        0        0     9471 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/execution.py
+-rw-r--r--   0        0        0     3991 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/identifiers.py
+-rw-r--r--   0        0        0     3415 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/persistence.py
+-rw-r--r--   0        0        0      869 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/trading/__init__.pxd
+-rw-r--r--   0        0        0     1372 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/trading/__init__.py
+-rw-r--r--   0        0        0     4730 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/trading/config.py
+-rw-r--r--   0        0        0     5493 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/trading/controller.py
+-rw-r--r--   0        0        0    18226 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/trading/filters.py
+-rw-r--r--   0        0        0     8699 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/trading/strategy.pxd
+-rw-r--r--   0        0        0    59399 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/trading/strategy.pyx
+-rw-r--r--   0        0        0    25167 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/nautilus_trader/trading/trader.py
+-rw-r--r--   0        0        0     8001 2024-05-31 11:33:44.310136 nautilus_trader-1.194.0/pyproject.toml
+-rw-r--r--   0        0        0    27436 1970-01-01 00:00:00.000000 nautilus_trader-1.194.0/PKG-INFO
```

### Comparing `nautilus_trader-1.193.0/LICENSE` & `nautilus_trader-1.194.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/README.md` & `nautilus_trader-1.194.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,38 +39,38 @@
 
 The platform is also universal and asset class agnostic - with any REST, WebSocket or FIX API able to be integrated via modular
 adapters. Thus, it can handle high-frequency trading operations for any asset classes
 including FX, Equities, Futures, Options, CFDs, Crypto and Betting - across multiple venues simultaneously.
 
 ## Features
 
-- **Fast** - Core written in Rust with asynchronous networking using [tokio](https://crates.io/crates/tokio)
-- **Reliable** - Type safety and thread safety through Rust. Redis backed performant state persistence
-- **Portable** - OS independent, runs on Linux, macOS, Windows. Deploy using Docker
-- **Flexible** - Modular adapters mean any REST, WebSocket, or FIX API can be integrated
-- **Advanced** - Time in force `IOC`, `FOK`, `GTD`, `AT_THE_OPEN`, `AT_THE_CLOSE`, advanced order types and conditional triggers. Execution instructions `post-only`, `reduce-only`, and icebergs. Contingency order lists including `OCO`, `OTO`
-- **Customizable** - Add user defined custom components, or assemble entire systems from scratch leveraging the cache and message bus
-- **Backtesting** - Run with multiple venues, instruments and strategies simultaneously using historical quote tick, trade tick, bar, order book and custom data with nanosecond resolution
-- **Live** - Use identical strategy implementations between backtesting and live deployments
-- **Multi-venue** - Multiple venue capabilities facilitate market making and statistical arbitrage strategies
-- **AI Agent Training** - Backtest engine fast enough to be used to train AI trading agents (RL/ES)
+- **Fast:** Core written in Rust with asynchronous networking using [tokio](https://crates.io/crates/tokio)
+- **Reliable:** Type safety and thread safety through Rust. Redis backed performant state persistence
+- **Portable:** OS independent, runs on Linux, macOS, Windows. Deploy using Docker
+- **Flexible:** Modular adapters mean any REST, WebSocket, or FIX API can be integrated
+- **Advanced:** Time in force `IOC`, `FOK`, `GTD`, `AT_THE_OPEN`, `AT_THE_CLOSE`, advanced order types and conditional triggers. Execution instructions `post-only`, `reduce-only`, and icebergs. Contingency order lists including `OCO`, `OTO`
+- **Customizable:** Add user defined custom components, or assemble entire systems from scratch leveraging the cache and message bus
+- **Backtesting:** Run with multiple venues, instruments and strategies simultaneously using historical quote tick, trade tick, bar, order book and custom data with nanosecond resolution
+- **Live:** Use identical strategy implementations between backtesting and live deployments
+- **Multi-venue:** Multiple venue capabilities facilitate market making and statistical arbitrage strategies
+- **AI Training:** Backtest engine fast enough to be used to train AI trading agents (RL/ES)
 
 ![Alt text](https://github.com/nautechsystems/nautilus_trader/blob/develop/docs/_images/nautilus-art.png?raw=true "nautilus")
 
 > _nautilus - from ancient Greek 'sailor' and naus 'ship'._
 >
 > _The nautilus shell consists of modular chambers with a growth factor which approximates a logarithmic spiral.
 > The idea is that this can be translated to the aesthetics of design and architecture._
 
 ## Why NautilusTrader?
 
-- **Highly performant event-driven Python** - native binary core components
-- **Parity between backtesting and live trading** - identical strategy code
-- **Reduced operational risk** - risk management functionality, logical correctness and type safety
-- **Highly extendable** - message bus, custom components and actors, custom data, custom adapters
+- **Highly performant event-driven Python:** Native binary core components
+- **Parity between backtesting and live trading:** Identical strategy code
+- **Reduced operational risk:** Risk management functionality, logical correctness and type safety
+- **Highly extendable:** Message bus, custom components and actors, custom data, custom adapters
 
 Traditionally, trading strategy research and backtesting might be conducted in Python (or other suitable language)
 using vectorized methods, with the strategy then needing to be reimplemented in a more event-drive way
 using C++, C#, Java or other statically typed language(s). The reasoning here is that vectorized backtesting code cannot
 express the granular time and event dependent complexity of real-time trading, where compiled languages have
 proven to be more suitable due to their inherently higher performance, and type safety.
 
@@ -125,16 +125,16 @@
 | [Binance](https://binance.com)                            | `BINANCE`             | Crypto Exchange (CEX)   | ![status](https://img.shields.io/badge/stable-green)    | [Guide](https://docs.nautilustrader.io/integrations/binance.html)   |
 | [Binance US](https://binance.us)                          | `BINANCE`             | Crypto Exchange (CEX)   | ![status](https://img.shields.io/badge/stable-green)    | [Guide](https://docs.nautilustrader.io/integrations/binance.html)   |
 | [Binance Futures](https://www.binance.com/en/futures)     | `BINANCE`             | Crypto Exchange (CEX)   | ![status](https://img.shields.io/badge/stable-green)    | [Guide](https://docs.nautilustrader.io/integrations/binance.html)   |
 | [Bybit](https://www.bybit.com)                            | `BYBIT`               | Crypto Exchange (CEX)   | ![status](https://img.shields.io/badge/beta-yellow)     | [Guide](https://docs.nautilustrader.io/integrations/bybit.html)     |
 | [Databento](https://databento.com)                        | `DATABENTO`           | Data Provider           | ![status](https://img.shields.io/badge/beta-yellow)     | [Guide](https://docs.nautilustrader.io/integrations/databento.html) |
 | [Interactive Brokers](https://www.interactivebrokers.com) | `INTERACTIVE_BROKERS` | Brokerage (multi-venue) | ![status](https://img.shields.io/badge/stable-green)    | [Guide](https://docs.nautilustrader.io/integrations/ib.html)        |
 
-- `ID:` The default client ID for the integrations adapter clients
-- `Type:` The type of integration (often the venue type)
+- **ID:** The default client ID for the integrations adapter clients
+- **Type:** The type of integration (often the venue type)
 
 ### Status
 - `building` - Under construction and likely not in a usable state
 - `beta` - Completed to a minimally working state and in a 'beta' testing phase
 - `stable` - Stabilized feature set and API, the integration has been tested by both developers and users to a reasonable level (some bugs may still remain)
 
 Refer to the [Integrations](https://docs.nautilustrader.io/integrations/index.html) documentation for further details.
@@ -192,27 +192,31 @@
    cd nautilus_trader
    poetry install --only main --all-extras
 
 Refer to the [Installation Guide](https://docs.nautilustrader.io/getting_started/installation.html) for other options and further details.
 
 ## Versioning and releases
 
-NautilusTrader is currently following a bi-weekly beta release schedule.
+NautilusTrader is currently targeting a weekly release schedule, occasionally there may be experimental
+or larger features which will delay a release by several weeks.
+
 The API is becoming more stable, however breaking changes are still possible between releases.
 Documentation of these changes in the release notes are made on a best-effort basis.
 
 ### Branches
 
+We aim to maintain a stable passing build on all branches.
+
 - `master` branch will always reflect the source code for the latest released version
 - `nightly` branch may contain experimental features and is generally merged from `develop` branch daily, and also when required
-- `develop` branch is normally very active with frequent commits and may contain experimental features. We aim to maintain a stable
-  passing build on this branch
+- `develop` branch is normally very active with frequent commits and may contain experimental features
 
-The current roadmap has a goal of achieving a stable API for a `2.x` version. From this
-point we will follow a formal process for releases, with deprecation periods for any API changes.
+The current roadmap has a goal of achieving a stable API for a `2.x` version (likely post Rust port).
+From this point we will follow a formal process for releases, with deprecation periods for any API changes.
+This allows us to maintain a maximum pace of development for now.
 
 ## Makefile
 
 A `Makefile` is provided to automate most installation and build tasks for development. It provides the following targets:
 
 - `make install` -- Installs in `release` build mode with `main`, `dev` and `test` dependencies then installs the package using poetry (default)
 - `make install-debug` -- Same as `make install` but with `debug` build mode
```

### Comparing `nautilus_trader-1.193.0/build.py` & `nautilus_trader-1.194.0/build.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/.cargo/config.toml` & `nautilus_trader-1.194.0/nautilus_core/.cargo/config.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/Cargo.lock` & `nautilus_trader-1.194.0/nautilus_core/Cargo.lock`

 * *Files 1% similar despite different names*

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
@@ -380,17 +380,17 @@
  "num",
  "regex",
  "regex-syntax 0.8.3",
 ]
 
 [[package]]
 name = "async-compression"
-version = "0.4.10"
+version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c90a406b4495d129f00461241616194cb8a032c8d1c53c657f0961d5f8e0498"
+checksum = "cd066d0b4ef8ecb03a55319dc13aa6910616d0f44008a045bb1835af830abff5"
 dependencies = [
  "bzip2",
  "flate2",
  "futures-core",
  "futures-io",
  "memchr",
  "pin-project-lite",
@@ -496,17 +496,17 @@
  "tower-layer",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
 name = "backtrace"
-version = "0.3.71"
+version = "0.3.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
+checksum = "17c6a35df3749d2e8bb1b7b21a976d82b15548788d2735b9d82f329268f71a11"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -1634,20 +1634,14 @@
 [[package]]
 name = "fastrand"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
-name = "finl_unicode"
-version = "1.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8fcfdc7a0362c9f4444381a9e697c79d435fe65b52a37466fc2c1184cee9edc6"
-
-[[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
 name = "flatbuffers"
@@ -1850,17 +1844,17 @@
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
 
@@ -2072,17 +2066,17 @@
  "tokio",
  "tokio-native-tls",
  "tower-service",
 ]
 
 [[package]]
 name = "hyper-util"
-version = "0.1.3"
+version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca38ef113da30126bbff9cd1705f9273e15d45498615d138b0c20279ac7a76aa"
+checksum = "7b875924a60b96e5d7b9ae7b066540b1dd1cbd90d1828f54c92e02a283351c56"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-util",
  "http",
  "http-body",
  "hyper",
@@ -2471,33 +2465,32 @@
  "libc",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "native-tls"
-version = "0.2.11"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
+checksum = "a8614eb2c83d59d1c8cc974dd3f920198647674a0a035e1af1fa58707e317466"
 dependencies = [
- "lazy_static",
  "libc",
  "log",
  "openssl",
  "openssl-probe",
  "openssl-sys",
  "schannel",
  "security-framework",
  "security-framework-sys",
  "tempfile",
 ]
 
 [[package]]
 name = "nautilus-accounting"
-version = "0.23.0"
+version = "0.24.0"
 dependencies = [
  "anyhow",
  "cbindgen",
  "nautilus-common",
  "nautilus-core",
  "nautilus-model",
  "pyo3",
@@ -2505,15 +2498,15 @@
  "rust_decimal",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "nautilus-adapters"
-version = "0.23.0"
+version = "0.24.0"
 dependencies = [
  "anyhow",
  "chrono",
  "criterion",
  "databento",
  "fallible-streaming-iterator",
  "indexmap 2.2.6",
@@ -2536,15 +2529,15 @@
  "tokio",
  "tracing",
  "ustr",
 ]
 
 [[package]]
 name = "nautilus-backtest"
-version = "0.23.0"
+version = "0.24.0"
 dependencies = [
  "anyhow",
  "cbindgen",
  "log",
  "nautilus-common",
  "nautilus-core",
  "nautilus-execution",
@@ -2553,15 +2546,15 @@
  "rstest",
  "tempfile",
  "ustr",
 ]
 
 [[package]]
 name = "nautilus-cli"
-version = "0.23.0"
+version = "0.24.0"
 dependencies = [
  "anyhow",
  "clap 4.5.4",
  "clap_derive",
  "dotenvy",
  "log",
  "nautilus-common",
@@ -2570,15 +2563,15 @@
  "nautilus-model",
  "simple_logger",
  "tokio",
 ]
 
 [[package]]
 name = "nautilus-common"
-version = "0.23.0"
+version = "0.24.0"
 dependencies = [
  "anyhow",
  "cbindgen",
  "chrono",
  "indexmap 2.2.6",
  "itertools 0.12.1",
  "log",
@@ -2598,15 +2591,15 @@
  "tracing",
  "tracing-subscriber",
  "ustr",
 ]
 
 [[package]]
 name = "nautilus-core"
-version = "0.23.0"
+version = "0.24.0"
 dependencies = [
  "anyhow",
  "cbindgen",
  "chrono",
  "criterion",
  "heck 0.5.0",
  "iai",
@@ -2618,15 +2611,15 @@
  "serde_json",
  "ustr",
  "uuid",
 ]
 
 [[package]]
 name = "nautilus-execution"
-version = "0.23.0"
+version = "0.24.0"
 dependencies = [
  "anyhow",
  "criterion",
  "derive_builder",
  "indexmap 2.2.6",
  "log",
  "nautilus-common",
@@ -2643,27 +2636,27 @@
  "thiserror",
  "tracing",
  "ustr",
 ]
 
 [[package]]
 name = "nautilus-indicators"
-version = "0.23.0"
+version = "0.24.0"
 dependencies = [
  "anyhow",
  "nautilus-core",
  "nautilus-model",
  "pyo3",
  "rstest",
  "strum",
 ]
 
 [[package]]
 name = "nautilus-infrastructure"
-version = "0.23.0"
+version = "0.24.0"
 dependencies = [
  "anyhow",
  "log",
  "nautilus-common",
  "nautilus-core",
  "nautilus-model",
  "pyo3",
@@ -2678,15 +2671,15 @@
  "tokio",
  "tracing",
  "ustr",
 ]
 
 [[package]]
 name = "nautilus-model"
-version = "0.23.0"
+version = "0.24.0"
 dependencies = [
  "anyhow",
  "cbindgen",
  "chrono",
  "criterion",
  "derive_builder",
  "evalexpr",
@@ -2706,15 +2699,15 @@
  "thiserror",
  "thousands",
  "ustr",
 ]
 
 [[package]]
 name = "nautilus-network"
-version = "0.23.0"
+version = "0.24.0"
 dependencies = [
  "anyhow",
  "axum",
  "criterion",
  "dashmap",
  "futures",
  "futures-util",
@@ -2731,15 +2724,15 @@
  "tokio-tungstenite",
  "tracing",
  "tracing-test",
 ]
 
 [[package]]
 name = "nautilus-persistence"
-version = "0.23.0"
+version = "0.24.0"
 dependencies = [
  "anyhow",
  "binary-heap-plus",
  "compare",
  "criterion",
  "datafusion",
  "dotenv",
@@ -2754,15 +2747,15 @@
  "rstest",
  "thiserror",
  "tokio",
 ]
 
 [[package]]
 name = "nautilus-pyo3"
-version = "0.23.0"
+version = "0.24.0"
 dependencies = [
  "nautilus-accounting",
  "nautilus-adapters",
  "nautilus-common",
  "nautilus-core",
  "nautilus-indicators",
  "nautilus-infrastructure",
@@ -2942,17 +2935,17 @@
 checksum = "5c7398b9c8b70908f6371f47ed36737907c87c52af34c268fed0bf0ceb92ead9"
 dependencies = [
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
 name = "object_store"
 version = "0.9.1"
@@ -3070,17 +3063,17 @@
  "bytecount",
  "fnv",
  "unicode-width",
 ]
 
 [[package]]
 name = "parking_lot"
-version = "0.12.2"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
@@ -3354,17 +3347,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.83"
+version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b33eb56c327dec362a9e55b3ad14f9d2f0904fb5a5b03b513ab5465399e9f43"
+checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "procfs"
 version = "0.16.0"
@@ -3585,17 +3578,17 @@
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "redis"
-version = "0.25.3"
+version = "0.25.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6472825949c09872e8f2c50bde59fcefc17748b6be5c90fd67cd8b4daca73bfd"
+checksum = "e0d7a6955c7511f60f3ba9e86c6d02b3c3f144f8c24b288d1f4e18074ab8bbec"
 dependencies = [
  "arc-swap",
  "async-trait",
  "bytes",
  "combine",
  "futures",
  "futures-util",
@@ -4051,26 +4044,26 @@
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.202"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "226b61a0d411b2ba5ff6d7f73a476ac4f8bb900373459cd00fab8512828ba395"
+checksum = "7253ab4de971e72fb7be983802300c30b5a7f0c2e56fab8abfc6a214307c0094"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.202"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6048858004bcff69094cd972ed40a32500f153bd3be9f716b2eed2e8217c4838"
+checksum = "500cbc0ebeb6f46627f50f3f5811ccf6bf00643be300b4c3eabc0ef55dc5b5ba"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.66",
 ]
 
 [[package]]
@@ -4519,21 +4512,21 @@
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
 name = "stringprep"
-version = "0.1.4"
+version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb41d74e231a107a1b4ee36bd1214b11285b77768d2e3824aedafa988fd36ee6"
+checksum = "7b4df3d392d81bd458a8a621b8bffbd2302a12ffe288a9d931670948749463b1"
 dependencies = [
- "finl_unicode",
  "unicode-bidi",
  "unicode-normalization",
+ "unicode-properties",
 ]
 
 [[package]]
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
@@ -4829,17 +4822,17 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.37.0"
+version = "1.38.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
+checksum = "ba4f4a02a7a80d6f274636f0aa95c7e383b912d41fe721a31f29e29698585a4a"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
@@ -4848,17 +4841,17 @@
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
  "syn 2.0.66",
 ]
 
 [[package]]
@@ -5155,14 +5148,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
+name = "unicode-properties"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e4259d9d4425d9f0661581b804cb85fe66a4c631cadd8f490d1c13a35d5d9291"
+
+[[package]]
 name = "unicode-segmentation"
 version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
 
 [[package]]
 name = "unicode-width"
@@ -5652,17 +5651,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.66",
 ]
 
 [[package]]
 name = "zeroize"
-version = "1.7.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
+checksum = "ced3678a2879b30306d323f4542626697a464a97c0a07c9aebf7ebca65cd4dde"
 
 [[package]]
 name = "zstd"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
 dependencies = [
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/Cargo.toml` & `nautilus_trader-1.194.0/nautilus_core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "persistence",
     "pyo3",
     "cli"
 ]
 
 [workspace.package]
 rust-version = "1.78.0"
-version = "0.23.0"
+version = "0.24.0"
 edition = "2021"
 authors = ["Nautech Systems <info@nautechsystems.io>"]
 description = "A high-performance algorithmic trading platform and event-driven backtester"
 documentation = "https://docs.nautilustrader.io"
 
 [workspace.dependencies]
 anyhow = "1.0.86"
@@ -38,21 +38,21 @@
 pyo3 = { version = "0.20.3", features = ["rust_decimal"] }
 pyo3-asyncio = { version = "0.20.0", features = ["tokio-runtime", "tokio", "attributes"] }
 rand = "0.8.5"
 rmp-serde = "1.3.0"
 rust_decimal = "1.35.0"
 rust_decimal_macros = "1.34.2"
 semver = "1.0.23"
-serde = { version = "1.0.202", features = ["derive"] }
+serde = { version = "1.0.203", features = ["derive"] }
 serde_json = "1.0.117"
 strum = { version = "0.26.2", features = ["derive"] }
 thiserror = "1.0.61"
 thousands = "0.2.0"
 tracing = "0.1.40"
-tokio = { version = "1.37.0", features = ["full"] }
+tokio = { version = "1.38.0", features = ["full"] }
 ustr = { version = "1.0.0", features = ["serde"] }
 uuid = { version = "1.8.0", features = ["v4"] }
 
 # dev-dependencies
 criterion = "0.5.1"
 float-cmp = "0.9.0"
 iai = "0.1.1"
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/LICENSE` & `nautilus_trader-1.194.0/nautilus_core/LICENSE`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/README.md` & `nautilus_trader-1.194.0/nautilus_core/README.md`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/accounting/Cargo.toml` & `nautilus_trader-1.194.0/nautilus_core/accounting/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/accounting/src/account/base.rs` & `nautilus_trader-1.194.0/nautilus_core/accounting/src/account/base.rs`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     pub events: Vec<AccountState>,
     pub commissions: HashMap<Currency, f64>,
     pub balances: HashMap<Currency, AccountBalance>,
     pub balances_starting: HashMap<Currency, Money>,
 }
 
 impl BaseAccount {
+    /// Creates a new [`BaseAccount`] instance.
     pub fn new(event: AccountState, calculate_account_state: bool) -> anyhow::Result<Self> {
         let mut balances_starting: HashMap<Currency, Money> = HashMap::new();
         let mut balances: HashMap<Currency, AccountBalance> = HashMap::new();
         event.balances.iter().for_each(|balance| {
             balances_starting.insert(balance.currency, balance.total);
             balances.insert(balance.currency, *balance);
         });
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/accounting/src/account/cash.rs` & `nautilus_trader-1.194.0/nautilus_core/accounting/src/account/cash.rs`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.accounting")
 )]
 pub struct CashAccount {
     pub base: BaseAccount,
 }
 
 impl CashAccount {
+    /// Creates a new [`CashAccount`] instance.
     pub fn new(event: AccountState, calculate_account_state: bool) -> anyhow::Result<Self> {
         Ok(Self {
             base: BaseAccount::new(event, calculate_account_state)?,
         })
     }
 
     #[must_use]
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/accounting/src/account/margin.rs` & `nautilus_trader-1.194.0/nautilus_core/accounting/src/account/margin.rs`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     pub base: BaseAccount,
     pub leverages: HashMap<InstrumentId, f64>,
     pub margins: HashMap<InstrumentId, MarginBalance>,
     pub default_leverage: f64,
 }
 
 impl MarginAccount {
+    /// Creates a new [`MarginAccount`] instance.
     pub fn new(event: AccountState, calculate_account_state: bool) -> anyhow::Result<Self> {
         Ok(Self {
             base: BaseAccount::new(event, calculate_account_state)?,
             leverages: HashMap::new(),
             margins: HashMap::new(),
             default_leverage: 1.0,
         })
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/accounting/src/account/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/accounting/src/account/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides account types and accounting functionality.
+//! Account implementations and accounting functionality.
 
 pub mod base;
 pub mod cash;
 pub mod margin;
 
 #[cfg(test)]
 pub mod stubs;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/accounting/src/account/stubs.rs` & `nautilus_trader-1.194.0/nautilus_core/accounting/src/account/stubs.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/accounting/src/lib.rs` & `nautilus_trader-1.194.0/nautilus_core/accounting/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/accounting/src/python/cash.rs` & `nautilus_trader-1.194.0/nautilus_core/accounting/src/python/cash.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/accounting/src/python/margin.rs` & `nautilus_trader-1.194.0/nautilus_core/accounting/src/python/margin.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/accounting/src/python/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/accounting/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/accounting/src/python/transformer.rs` & `nautilus_trader-1.194.0/nautilus_core/accounting/src/python/transformer.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/accounting/src/stubs.rs` & `nautilus_trader-1.194.0/nautilus_core/accounting/src/stubs.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/Cargo.toml` & `nautilus_trader-1.194.0/nautilus_core/adapters/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/bin/sandbox.rs` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/bin/sandbox.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/common.rs` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/common.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/decode.rs` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/decode.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/enums.rs` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/enums.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines enumerations for the Databento integration.
+//! Enumerations for the Databento integration.
 
 use std::str::FromStr;
 
 use nautilus_model::{enum_strum_serde, enums::FromU8};
 use serde::{Deserialize, Deserializer, Serialize, Serializer};
 use strum::{AsRefStr, Display, EnumIter, EnumString, FromRepr};
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/live.rs` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/live.rs`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     cmd_rx: mpsc::UnboundedReceiver<LiveCommand>,
     msg_tx: mpsc::Sender<LiveMessage>,
     publisher_venue_map: IndexMap<PublisherId, Venue>,
     replay: bool,
 }
 
 impl DatabentoFeedHandler {
-    /// Initialize a new instance of the [`DatabentoFeedHandler`].
+    /// Creates a new [`DatabentoFeedHandler`] instance.
     #[must_use]
     pub fn new(
         key: String,
         dataset: String,
         rx: mpsc::UnboundedReceiver<LiveCommand>,
         tx: mpsc::Sender<LiveMessage>,
         publisher_venue_map: IndexMap<PublisherId, Venue>,
@@ -261,15 +261,15 @@
                             "Buffering delta: {} {} {:?} flags={}",
                             deltas_count,
                             delta.ts_event,
                             buffering_start,
                             msg.flags.raw(),
                         );
 
-                        // Check if last message in the packet
+                        // Check if last message in the book event
                         if !RecordFlag::F_LAST.matches(msg.flags.raw()) {
                             continue; // NOT last message
                         }
 
                         // Check if snapshot
                         if RecordFlag::F_SNAPSHOT.matches(msg.flags.raw()) {
                             continue; // Buffer snapshot
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/loader.rs` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/loader.rs`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         decode_imbalance_msg, decode_instrument_def_msg_v1, decode_record, decode_statistics_msg,
         raw_ptr_to_ustr,
     },
     symbology::decode_nautilus_instrument_id,
     types::{DatabentoImbalance, DatabentoPublisher, DatabentoStatistics, Dataset, PublisherId},
 };
 
-/// Provides a Nautilus data loader for Databento Binary Encoding (DBN) format data.
+/// A Nautilus data loader for Databento Binary Encoding (DBN) format data.
 ///
 /// # Supported schemas:
 ///  - MBO -> `OrderBookDelta`
 ///  - MBP_1 -> `(QuoteTick, Option<TradeTick>)`
 ///  - MBP_10 -> `OrderBookDepth10`
 ///  - TBBO -> `(QuoteTick, TradeTick)`
 ///  - TRADES -> `TradeTick`
@@ -64,14 +64,15 @@
 pub struct DatabentoDataLoader {
     publishers_map: IndexMap<PublisherId, DatabentoPublisher>,
     venue_dataset_map: IndexMap<Venue, Dataset>,
     publisher_venue_map: IndexMap<PublisherId, Venue>,
 }
 
 impl DatabentoDataLoader {
+    /// Creates a new [`DatabentoDataLoader`] instance.
     pub fn new(path: Option<PathBuf>) -> anyhow::Result<Self> {
         let mut loader = Self {
             publishers_map: IndexMap::new(),
             venue_dataset_map: IndexMap::new(),
             publisher_venue_map: IndexMap::new(),
         };
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/data/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides the [Databento](https://databento.com) integration adapter.
-
-pub mod common;
-pub mod decode;
-pub mod enums;
-pub mod live;
-pub mod loader;
-pub mod symbology;
-pub mod types;
-
-#[cfg(feature = "python")]
-pub mod python;
+pub mod bar;
+pub mod delta;
+pub mod deltas;
+pub mod depth;
+pub mod order;
+pub mod quote;
+pub mod trade;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/publishers.json` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/publishers.json`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/enums.rs` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/python/enums.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/historical.rs` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/python/historical.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/live.rs` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/python/live.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/loader.rs` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/python/loader.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/python/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/python/types.rs` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/python/types.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/symbology.rs` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/symbology.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.definition.dbn.zst` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.definition.dbn.zst`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.definition.v1.dbn.zst` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.definition.v1.dbn.zst`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/test_data/test_data.imbalance.dbn.zst` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/test_data/test_data.imbalance.dbn.zst`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/databento/types.rs` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/databento/types.rs`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
     // The UNIX timestamp (nanoseconds) when the data object was received by Databento.
     pub ts_recv: UnixNanos,
     // The UNIX timestamp (nanoseconds) when the data object was initialized.
     pub ts_init: UnixNanos,
 }
 
 impl DatabentoImbalance {
+    /// Creates a new [`DatabentoImbalance`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         instrument_id: InstrumentId,
         ref_price: Price,
         cont_book_clr_price: Price,
         auct_interest_clr_price: Price,
         paired_qty: Quantity,
@@ -150,14 +151,15 @@
     // The UNIX timestamp (nanoseconds) when the data object was received by Databento.
     pub ts_recv: UnixNanos,
     // The UNIX timestamp (nanoseconds) when the data object was initialized.
     pub ts_init: UnixNanos,
 }
 
 impl DatabentoStatistics {
+    /// Creates a new [`DatabentoStatistics`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         instrument_id: InstrumentId,
         stat_type: DatabentoStatisticType,
         update_action: DatabentoStatisticUpdateAction,
         price: Option<Price>,
         quantity: Option<Quantity>,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/adapters/src/lib.rs` & `nautilus_trader-1.194.0/nautilus_core/adapters/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/backtest/Cargo.toml` & `nautilus_trader-1.194.0/nautilus_core/backtest/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/backtest/build.rs` & `nautilus_trader-1.194.0/nautilus_core/backtest/build.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/backtest/cbindgen_cython.toml` & `nautilus_trader-1.194.0/nautilus_core/backtest/cbindgen_cython.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/backtest/src/engine.rs` & `nautilus_trader-1.194.0/nautilus_core/backtest/src/engine.rs`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 /// Provides a means of accumulating and draining time event handlers.
 pub struct TimeEventAccumulator {
     event_handlers: Vec<TimeEventHandler>,
 }
 
 impl TimeEventAccumulator {
-    /// Creates a new `TimeEventAccumulator` instance.
+    /// Creates a new [`TimeEventAccumulator`] instance.
     #[must_use]
     pub fn new() -> Self {
         Self {
             event_handlers: Vec::new(),
         }
     }
 
@@ -51,14 +51,15 @@
         self.event_handlers
             .sort_unstable_by_key(|v| v.event.ts_event);
         self.event_handlers.drain(..).collect()
     }
 }
 
 impl Default for TimeEventAccumulator {
+    /// Creates a new default [`TimeEventAccumulator`] instance.
     fn default() -> Self {
         Self::new()
     }
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // C API
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/backtest/src/lib.rs` & `nautilus_trader-1.194.0/nautilus_core/backtest/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/backtest/src/matching_engine.rs` & `nautilus_trader-1.194.0/nautilus_core/backtest/src/matching_engine.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides an `OrderMatchingEngine` for use in research, backtesting and sandbox environments.
+//! An `OrderMatchingEngine` for use in research, backtesting and sandbox environments.
 
 // Under development
 #![allow(dead_code)]
 #![allow(unused_variables)]
 
 use std::collections::HashMap;
 
@@ -51,15 +51,15 @@
     pub support_gtd_orders: bool,
     pub support_contingent_orders: bool,
     pub use_position_ids: bool,
     pub use_random_ids: bool,
     pub use_reduce_only: bool,
 }
 
-/// Provides an order matching engine for a single market.
+/// An order matching engine for a single market.
 pub struct OrderMatchingEngine {
     /// The venue for the matching engine.
     pub venue: Venue,
     /// The instrument for the matching engine.
     pub instrument: Box<dyn Instrument>,
     /// The instruments raw integer ID for the venue.
     pub raw_id: u32,
@@ -87,16 +87,17 @@
     execution_bar_deltas: HashMap<InstrumentId, u64>,
     account_ids: HashMap<TraderId, AccountId>,
     position_count: usize,
     order_count: usize,
     execution_count: usize,
 }
 
-// Note: we'll probably be changing the `FillModel` (don't add for now)
+// TODO: we'll probably be changing the `FillModel` (don't add for now)
 impl OrderMatchingEngine {
+    /// Creates a new [`OrderMatchingEngine`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         instrument: Box<dyn Instrument>,
         raw_id: u32,
         book_type: BookType,
         oms_type: OmsType,
         account_type: AccountType,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/cli/Cargo.toml` & `nautilus_trader-1.194.0/nautilus_core/cli/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/cli/src/bin/cli.rs` & `nautilus_trader-1.194.0/nautilus_core/cli/src/bin/cli.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/cli/src/database/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/cli/src/database/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/cli/src/database/postgres.rs` & `nautilus_trader-1.194.0/nautilus_core/cli/src/database/postgres.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/cli/src/lib.rs` & `nautilus_trader-1.194.0/nautilus_core/cli/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/cli/src/opt.rs` & `nautilus_trader-1.194.0/nautilus_core/cli/src/opt.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/Cargo.toml` & `nautilus_trader-1.194.0/nautilus_core/common/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/build.rs` & `nautilus_trader-1.194.0/nautilus_core/common/build.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/cbindgen.toml` & `nautilus_trader-1.194.0/nautilus_core/common/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/cbindgen_cython.toml` & `nautilus_trader-1.194.0/nautilus_core/common/cbindgen_cython.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/cache/core.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/cache/core.rs`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! The core cache in-memory structure.
+
 use std::{
     collections::{HashMap, HashSet, VecDeque},
     time::{SystemTime, UNIX_EPOCH},
 };
 
 use log::{debug, error, info, warn};
 use nautilus_core::correctness::{check_key_not_in_map, check_slice_not_empty, check_valid_string};
@@ -45,27 +47,28 @@
     types::{currency::Currency, price::Price, quantity::Quantity},
 };
 use ustr::Ustr;
 
 use super::database::CacheDatabaseAdapter;
 use crate::{enums::SerializationEncoding, interface::account::Account};
 
-/// The configuration for `Cache` instances.
+/// Configuration for `Cache` instances.
 pub struct CacheConfig {
     pub encoding: SerializationEncoding,
     pub timestamps_as_iso8601: bool,
     pub use_trader_prefix: bool,
     pub use_instance_id: bool,
     pub flush_on_start: bool,
     pub drop_instruments_on_reset: bool,
     pub tick_capacity: usize,
     pub bar_capacity: usize,
 }
 
 impl CacheConfig {
+    /// Creates a new [`CacheConfig`] instance.
     #[allow(clippy::too_many_arguments)]
     #[must_use]
     pub fn new(
         encoding: SerializationEncoding,
         timestamps_as_iso8601: bool,
         use_trader_prefix: bool,
         use_instance_id: bool,
@@ -84,14 +87,15 @@
             tick_capacity,
             bar_capacity,
         }
     }
 }
 
 impl Default for CacheConfig {
+    /// Creates a new default [`CacheConfig`] instance.
     fn default() -> Self {
         Self::new(
             SerializationEncoding::MsgPack,
             false,
             true,
             false,
             false,
@@ -131,15 +135,15 @@
     positions_closed: HashSet<PositionId>,
     actors: HashSet<ComponentId>,
     strategies: HashSet<StrategyId>,
     exec_algorithms: HashSet<ExecAlgorithmId>,
 }
 
 impl CacheIndex {
-    /// Clear the index which will clear/reset all internal state.
+    /// Clears the index which will clear/reset all internal state.
     pub fn clear(&mut self) {
         self.venue_account.clear();
         self.venue_orders.clear();
         self.venue_positions.clear();
         self.venue_order_ids.clear();
         self.client_order_ids.clear();
         self.order_position.clear();
@@ -168,15 +172,15 @@
     }
 }
 
 /// A common in-memory `Cache` for market and execution related data.
 pub struct Cache {
     config: CacheConfig,
     index: CacheIndex,
-    database: Option<CacheDatabaseAdapter>,
+    database: Option<Box<dyn CacheDatabaseAdapter>>,
     general: HashMap<String, Vec<u8>>,
     quotes: HashMap<InstrumentId, VecDeque<QuoteTick>>,
     trades: HashMap<InstrumentId, VecDeque<TradeTick>>,
     books: HashMap<InstrumentId, OrderBook>,
     bars: HashMap<BarType, VecDeque<Bar>>,
     currencies: HashMap<Ustr, Currency>,
     instruments: HashMap<InstrumentId, InstrumentAny>,
@@ -185,22 +189,24 @@
     orders: HashMap<ClientOrderId, OrderAny>,
     order_lists: HashMap<OrderListId, OrderList>,
     positions: HashMap<PositionId, Position>,
     position_snapshots: HashMap<PositionId, Vec<u8>>,
 }
 
 impl Default for Cache {
+    /// Creates a new default [`Cache`] instance.
     fn default() -> Self {
         Self::new(CacheConfig::default(), None)
     }
 }
 
 impl Cache {
+    /// Creates a new [`Cache`] instance.
     #[must_use]
-    pub fn new(config: CacheConfig, database: Option<CacheDatabaseAdapter>) -> Self {
+    pub fn new(config: CacheConfig, database: Option<Box<dyn CacheDatabaseAdapter>>) -> Self {
         let index = CacheIndex {
             venue_account: HashMap::new(),
             venue_orders: HashMap::new(),
             venue_positions: HashMap::new(),
             venue_order_ids: HashMap::new(),
             client_order_ids: HashMap::new(),
             order_position: HashMap::new(),
@@ -246,102 +252,102 @@
             positions: HashMap::new(),
             position_snapshots: HashMap::new(),
         }
     }
 
     // -- COMMANDS --------------------------------------------------------------------------------
 
-    /// Clear the current general cache and load the general objects from the cache database.
+    /// Clears the current general cache and loads the general objects from the cache database.
     pub fn cache_general(&mut self) -> anyhow::Result<()> {
-        self.general = match &self.database {
+        self.general = match &mut self.database {
             Some(db) => db.load()?,
             None => HashMap::new(),
         };
 
         info!(
             "Cached {} general object(s) from database",
             self.general.len()
         );
         Ok(())
     }
 
-    /// Clear the current currencies cache and load currencies from the cache database.
+    /// Clears the current currencies cache and loads currencies from the cache database.
     pub fn cache_currencies(&mut self) -> anyhow::Result<()> {
-        self.currencies = match &self.database {
+        self.currencies = match &mut self.database {
             Some(db) => db.load_currencies()?,
             None => HashMap::new(),
         };
 
         info!("Cached {} currencies from database", self.general.len());
         Ok(())
     }
 
-    /// Clear the current instruments cache and load instruments from the cache database.
+    /// Clears the current instruments cache and loads instruments from the cache database.
     pub fn cache_instruments(&mut self) -> anyhow::Result<()> {
-        self.instruments = match &self.database {
+        self.instruments = match &mut self.database {
             Some(db) => db.load_instruments()?,
             None => HashMap::new(),
         };
 
         info!("Cached {} instruments from database", self.general.len());
         Ok(())
     }
 
-    /// Clear the current synthetic instruments cache and load synthetic instruments from the cache
+    /// Clears the current synthetic instruments cache and loads synthetic instruments from the cache
     /// database.
     pub fn cache_synthetics(&mut self) -> anyhow::Result<()> {
-        self.synthetics = match &self.database {
+        self.synthetics = match &mut self.database {
             Some(db) => db.load_synthetics()?,
             None => HashMap::new(),
         };
 
         info!(
             "Cached {} synthetic instruments from database",
             self.general.len()
         );
         Ok(())
     }
 
-    /// Clear the current accounts cache and load accounts from the cache database.
+    /// Clears the current accounts cache and loads accounts from the cache database.
     pub fn cache_accounts(&mut self) -> anyhow::Result<()> {
-        self.accounts = match &self.database {
+        self.accounts = match &mut self.database {
             Some(db) => db.load_accounts()?,
             None => HashMap::new(),
         };
 
         info!(
             "Cached {} synthetic instruments from database",
             self.general.len()
         );
         Ok(())
     }
 
-    /// Clear the current orders cache and load orders from the cache database.
+    /// Clears the current orders cache and loads orders from the cache database.
     pub fn cache_orders(&mut self) -> anyhow::Result<()> {
-        self.orders = match &self.database {
+        self.orders = match &mut self.database {
             Some(db) => db.load_orders()?,
             None => HashMap::new(),
         };
 
         info!("Cached {} orders from database", self.general.len());
         Ok(())
     }
 
-    /// Clear the current positions cache and load positions from the cache database.
+    /// Clears the current positions cache and loads positions from the cache database.
     pub fn cache_positions(&mut self) -> anyhow::Result<()> {
-        self.positions = match &self.database {
+        self.positions = match &mut self.database {
             Some(db) => db.load_positions()?,
             None => HashMap::new(),
         };
 
         info!("Cached {} positions from database", self.general.len());
         Ok(())
     }
 
-    /// Clear the current cache index and re-build.
+    /// Clears the current cache index and re-build.
     pub fn build_index(&mut self) {
         self.index.clear();
         debug!("Building index");
 
         // Index accounts
         for account_id in self.accounts.keys() {
             self.index
@@ -500,15 +506,15 @@
             }
 
             // 9: Build index.strategies -> {StrategyId}
             self.index.strategies.insert(strategy_id);
         }
     }
 
-    /// Check integrity of data within the cache.
+    /// Checks integrity of data within the cache.
     ///
     /// All data should be loaded from the database prior to this call.
     /// If an error is found then a log error message will also be produced.
     #[must_use]
     fn check_integrity(&mut self) -> bool {
         let mut error_count = 0;
         let failure = "Integrity failure";
@@ -873,15 +879,15 @@
                 if error_count == 1 { "" } else { "s" },
                 total_us
             );
             false
         }
     }
 
-    /// Check for any residual open state and log warnings if any are found.
+    /// Checks for any residual open state and log warnings if any are found.
     ///
     ///'Open state' is considered to be open orders and open positions.
     #[must_use]
     pub fn check_residuals(&self) -> bool {
         debug!("Checking residuals");
 
         let mut residuals = false;
@@ -897,21 +903,21 @@
             residuals = true;
             warn!("Residual {}", position);
         }
 
         residuals
     }
 
-    /// Clear the caches index.
+    /// Clears the caches index.
     pub fn clear_index(&mut self) {
         self.index.clear();
         debug!("Cleared index");
     }
 
-    /// Reset the cache.
+    /// Resets the cache.
     ///
     /// All stateful fields are reset to their initial value.
     pub fn reset(&mut self) {
         debug!("Resetting cache");
 
         self.general.clear();
         self.quotes.clear();
@@ -928,67 +934,67 @@
 
         self.clear_index();
 
         info!("Reset cache");
     }
 
     /// Dispose of the cache which will close any underlying database adapter.
-    pub fn dispose(&self) -> anyhow::Result<()> {
-        if let Some(database) = &self.database {
+    pub fn dispose(&mut self) -> anyhow::Result<()> {
+        if let Some(database) = &mut self.database {
             // TODO: Log operations in database adapter
             database.close()?;
         }
         Ok(())
     }
 
-    /// Flush the caches database which permanently removes all persisted data.
-    pub fn flush_db(&self) -> anyhow::Result<()> {
-        if let Some(database) = &self.database {
+    /// Flushes the caches database which permanently removes all persisted data.
+    pub fn flush_db(&mut self) -> anyhow::Result<()> {
+        if let Some(database) = &mut self.database {
             // TODO: Log operations in database adapter
             database.flush()?;
         }
         Ok(())
     }
 
-    /// Add the given general object to the cache.
+    /// Adds a general object `value` (as bytes) to the cache at the given `key`.
     ///
-    /// The cache is agnostic to what the object actually is (and how it may be serialized),
-    /// offering maximum flexibility.
+    /// The cache is agnostic to what the bytes actually represent (and how it may be serialized),
+    /// which provides maximum flexibility.
     pub fn add(&mut self, key: &str, value: Vec<u8>) -> anyhow::Result<()> {
         check_valid_string(key, stringify!(key))?;
         check_slice_not_empty(value.as_slice(), stringify!(value))?;
 
         debug!("Adding general {key}");
         self.general.insert(key.to_string(), value.clone());
 
-        if let Some(database) = &self.database {
+        if let Some(database) = &mut self.database {
             database.add(key.to_string(), value)?;
         }
         Ok(())
     }
 
-    /// Add the given order `book` to the cache.
+    /// Adds the given order `book` to the cache.
     pub fn add_order_book(&mut self, book: OrderBook) -> anyhow::Result<()> {
         debug!("Adding `OrderBook` {}", book.instrument_id);
         self.books.insert(book.instrument_id, book);
         Ok(())
     }
 
-    /// Add the given `quote` tick to the cache.
+    /// Adds the given `quote` tick to the cache.
     pub fn add_quote(&mut self, quote: QuoteTick) -> anyhow::Result<()> {
         debug!("Adding `QuoteTick` {}", quote.instrument_id);
         let quotes_deque = self
             .quotes
             .entry(quote.instrument_id)
             .or_insert_with(|| VecDeque::with_capacity(self.config.tick_capacity));
         quotes_deque.push_front(quote);
         Ok(())
     }
 
-    /// Add the given `quotes` to the cache.
+    /// Adds the given `quotes` to the cache.
     pub fn add_quotes(&mut self, quotes: &[QuoteTick]) -> anyhow::Result<()> {
         check_slice_not_empty(quotes, stringify!(quotes))?;
 
         let instrument_id = quotes[0].instrument_id;
         debug!("Adding `QuoteTick`[{}] {}", quotes.len(), instrument_id);
         let quotes_deque = self
             .quotes
@@ -997,26 +1003,26 @@
 
         for quote in quotes {
             quotes_deque.push_front(*quote);
         }
         Ok(())
     }
 
-    /// Add the given `trade` tick to the cache.
+    /// Adds the given `trade` tick to the cache.
     pub fn add_trade(&mut self, trade: TradeTick) -> anyhow::Result<()> {
         debug!("Adding `TradeTick` {}", trade.instrument_id);
         let trades_deque = self
             .trades
             .entry(trade.instrument_id)
             .or_insert_with(|| VecDeque::with_capacity(self.config.tick_capacity));
         trades_deque.push_front(trade);
         Ok(())
     }
 
-    /// Add the give `trades` to the cache.
+    /// Adds the give `trades` to the cache.
     pub fn add_trades(&mut self, trades: &[TradeTick]) -> anyhow::Result<()> {
         check_slice_not_empty(trades, stringify!(trades))?;
 
         let instrument_id = trades[0].instrument_id;
         debug!("Adding `TradeTick`[{}] {}", trades.len(), instrument_id);
         let trades_deque = self
             .trades
@@ -1025,26 +1031,26 @@
 
         for trade in trades {
             trades_deque.push_front(*trade);
         }
         Ok(())
     }
 
-    /// Add the given `bar` to the cache.
+    /// Adds the given `bar` to the cache.
     pub fn add_bar(&mut self, bar: Bar) -> anyhow::Result<()> {
         debug!("Adding `Bar` {}", bar.bar_type);
         let bars = self
             .bars
             .entry(bar.bar_type)
             .or_insert_with(|| VecDeque::with_capacity(self.config.bar_capacity));
         bars.push_front(bar);
         Ok(())
     }
 
-    /// Add the given `bars` to the cache.
+    /// Adds the given `bars` to the cache.
     pub fn add_bars(&mut self, bars: &[Bar]) -> anyhow::Result<()> {
         check_slice_not_empty(bars, stringify!(bars))?;
 
         let bar_type = bars[0].bar_type;
         debug!("Adding `Bar`[{}] {}", bars.len(), bar_type);
         let bars_deque = self
             .bars
@@ -1053,63 +1059,65 @@
 
         for bar in bars {
             bars_deque.push_front(*bar);
         }
         Ok(())
     }
 
-    /// Add the given `currency` to the cache.
+    /// Adds the given `currency` to the cache.
     pub fn add_currency(&mut self, currency: Currency) -> anyhow::Result<()> {
         debug!("Adding `Currency` {}", currency.code);
 
-        if let Some(database) = &self.database {
+        if let Some(database) = &mut self.database {
             database.add_currency(&currency)?;
         }
 
         self.currencies.insert(currency.code, currency);
         Ok(())
     }
 
-    /// Add the given `instrument` to the cache.
+    /// Adds the given `instrument` to the cache.
     pub fn add_instrument(&mut self, instrument: InstrumentAny) -> anyhow::Result<()> {
         debug!("Adding `Instrument` {}", instrument.id());
 
-        if let Some(database) = &self.database {
+        if let Some(database) = &mut self.database {
             database.add_instrument(&instrument)?;
         }
 
         self.instruments.insert(instrument.id(), instrument);
         Ok(())
     }
 
-    /// Add the given `synthetic` instrument to the cache.
+    /// Adds the given `synthetic` instrument to the cache.
     pub fn add_synthetic(&mut self, synthetic: SyntheticInstrument) -> anyhow::Result<()> {
         debug!("Adding `SyntheticInstrument` {}", synthetic.id);
 
-        if let Some(database) = &self.database {
+        if let Some(database) = &mut self.database {
             database.add_synthetic(&synthetic)?;
         }
 
         self.synthetics.insert(synthetic.id, synthetic);
         Ok(())
     }
 
-    /// Add the given `account` to the cache.
+    /// Adds the given `account` to the cache.
     pub fn add_account(&mut self, account: Box<dyn Account>) -> anyhow::Result<()> {
         debug!("Adding `Account` {}", account.id());
 
-        if let Some(database) = &self.database {
+        if let Some(database) = &mut self.database {
             database.add_account(account.as_ref())?;
         }
 
         self.accounts.insert(account.id(), account);
         Ok(())
     }
 
-    /// Index the given client order ID with the given venue order ID.
+    /// Indexes the given `client_order_id` with the given `venue_order_id`.
+    ///
+    /// The `overwrite` parameter determines whether to overwrite any existing cached identifier.
     pub fn add_venue_order_id(
         &mut self,
         client_order_id: &ClientOrderId,
         venue_order_id: &VenueOrderId,
         overwrite: bool,
     ) -> anyhow::Result<()> {
         if let Some(existing_venue_order_id) = self.index.client_order_ids.get(client_order_id) {
@@ -1129,15 +1137,15 @@
         self.index
             .venue_order_ids
             .insert(*venue_order_id, *client_order_id);
 
         Ok(())
     }
 
-    /// Add the order to the cache indexed with any given identifiers.
+    /// Adds the given `order` to the cache indexed with any given identifiers.
     ///
     /// # Parameters
     ///
     /// `override_existing`: If the added order should 'override' any existing order and replace
     /// it in the cache. This is currently used for emulated orders which are
     /// being released and transformed into another type.
     ///
@@ -1267,15 +1275,15 @@
         }
 
         self.orders.insert(client_order_id, order);
 
         Ok(())
     }
 
-    /// Index the given `position_id` with the other given IDs.
+    /// Indexes the given `position_id` with the other given IDs.
     pub fn add_position_id(
         &mut self,
         position_id: &PositionId,
         venue: &Venue,
         client_order_id: &ClientOrderId,
         strategy_id: &StrategyId,
     ) -> anyhow::Result<()> {
@@ -1306,14 +1314,15 @@
             .entry(*strategy_id)
             .or_default()
             .insert(*position_id);
 
         Ok(())
     }
 
+    /// Adds the given `position` to the cache.
     pub fn add_position(&mut self, position: Position, oms_type: OmsType) -> anyhow::Result<()> {
         self.positions.insert(position.id, position.clone());
         self.index.positions.insert(position.id);
         self.index.positions_open.insert(position.id);
 
         log::debug!("Adding {position}");
 
@@ -1348,23 +1357,23 @@
             //     )?;
             // }
         }
 
         Ok(())
     }
 
-    /// Update the given `account` in the cache.
+    /// Updates the given `account` in the cache.
     pub fn update_account(&mut self, account: &dyn Account) -> anyhow::Result<()> {
         if let Some(database) = &mut self.database {
             database.update_account(account)?;
         }
         Ok(())
     }
 
-    /// Update the given `order` in the cache.
+    /// Updates the given `order` in the cache.
     pub fn update_order(&mut self, order: &OrderAny) -> anyhow::Result<()> {
         let client_order_id = order.client_order_id();
 
         // Update venue order ID
         if let Some(venue_order_id) = order.venue_order_id() {
             // If the order is being modified then we allow a changing `VenueOrderId` to accommodate
             // venues which use a cancel+replace update strategy.
@@ -1406,22 +1415,22 @@
             //     database.snapshot_order_state(order)?;
             // }
         }
 
         Ok(())
     }
 
-    /// Update the given `order` as pending cancel locally.
+    /// Updates the given `order` as pending cancel locally.
     pub fn update_order_pending_cancel_local(&mut self, order: &OrderAny) {
         self.index
             .orders_pending_cancel
             .insert(order.client_order_id());
     }
 
-    /// Update the given `position` in the cache.
+    /// Updates the given `position` in the cache.
     pub fn update_position(&mut self, position: &Position) -> anyhow::Result<()> {
         // Update open/closed state
         if position.is_open() {
             self.index.positions_open.insert(position.id);
             self.index.positions_closed.remove(&position.id);
         } else {
             self.index.positions_closed.insert(position.id);
@@ -1590,28 +1599,30 @@
                 positions.push(position);
             };
         }
 
         positions
     }
 
+    /// Returns the `ClientOrderId`s of all orders.
     #[must_use]
     pub fn client_order_ids(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
     ) -> HashSet<ClientOrderId> {
         let query = self.build_order_query_filter_set(venue, instrument_id, strategy_id);
         match query {
             Some(query) => self.index.orders.intersection(&query).copied().collect(),
             None => self.index.orders.clone(),
         }
     }
 
+    /// Returns the `ClientOrderId`s of all open orders.
     #[must_use]
     pub fn client_order_ids_open(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
     ) -> HashSet<ClientOrderId> {
@@ -1623,14 +1634,15 @@
                 .intersection(&query)
                 .copied()
                 .collect(),
             None => self.index.orders_open.clone(),
         }
     }
 
+    /// Returns the `ClientOrderId`s of all closed orders.
     #[must_use]
     pub fn client_order_ids_closed(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
     ) -> HashSet<ClientOrderId> {
@@ -1642,14 +1654,15 @@
                 .intersection(&query)
                 .copied()
                 .collect(),
             None => self.index.orders_closed.clone(),
         }
     }
 
+    /// Returns the `ClientOrderId`s of all emulated orders.
     #[must_use]
     pub fn client_order_ids_emulated(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
     ) -> HashSet<ClientOrderId> {
@@ -1661,14 +1674,15 @@
                 .intersection(&query)
                 .copied()
                 .collect(),
             None => self.index.orders_emulated.clone(),
         }
     }
 
+    /// Returns the `ClientOrderId`s of all in-flight orders.
     #[must_use]
     pub fn client_order_ids_inflight(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
     ) -> HashSet<ClientOrderId> {
@@ -1680,28 +1694,30 @@
                 .intersection(&query)
                 .copied()
                 .collect(),
             None => self.index.orders_inflight.clone(),
         }
     }
 
+    /// Returns `PositionId`s of all positions.
     #[must_use]
     pub fn position_ids(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
     ) -> HashSet<PositionId> {
         let query = self.build_position_query_filter_set(venue, instrument_id, strategy_id);
         match query {
             Some(query) => self.index.positions.intersection(&query).copied().collect(),
             None => self.index.positions.clone(),
         }
     }
 
+    /// Returns the `PositionId`s of all open positions.
     #[must_use]
     pub fn position_open_ids(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
     ) -> HashSet<PositionId> {
@@ -1713,14 +1729,15 @@
                 .intersection(&query)
                 .copied()
                 .collect(),
             None => self.index.positions_open.clone(),
         }
     }
 
+    /// Returns the `PositionId`s of all closed positions.
     #[must_use]
     pub fn position_closed_ids(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
     ) -> HashSet<PositionId> {
@@ -1732,216 +1749,242 @@
                 .intersection(&query)
                 .copied()
                 .collect(),
             None => self.index.positions_closed.clone(),
         }
     }
 
+    /// Returns the `ComponentId`s of all actors.
     #[must_use]
     pub fn actor_ids(&self) -> HashSet<ComponentId> {
         self.index.actors.clone()
     }
 
+    /// Returns the `StrategyId`s of all strategies.
     #[must_use]
     pub fn strategy_ids(&self) -> HashSet<StrategyId> {
         self.index.strategies.clone()
     }
 
+    /// Returns the `ExecAlgorithmId`s of all execution algorithms.
     #[must_use]
     pub fn exec_algorithm_ids(&self) -> HashSet<ExecAlgorithmId> {
         self.index.exec_algorithms.clone()
     }
 
     // -- ORDER QUERIES ---------------------------------------------------------------------------
 
+    /// Gets a reference to the order with the given `client_order_id` (if found).
     #[must_use]
     pub fn order(&self, client_order_id: &ClientOrderId) -> Option<&OrderAny> {
         self.orders.get(client_order_id)
     }
 
+    /// Gets a reference to the client order ID for given `venue_order_id` (if found).
     #[must_use]
     pub fn client_order_id(&self, venue_order_id: &VenueOrderId) -> Option<&ClientOrderId> {
         self.index.venue_order_ids.get(venue_order_id)
     }
 
+    /// Gets a reference to the venue order ID for given `client_order_id` (if found).
     #[must_use]
     pub fn venue_order_id(&self, client_order_id: &ClientOrderId) -> Option<&VenueOrderId> {
         self.index.client_order_ids.get(client_order_id)
     }
 
+    /// Gets a reference to the client ID indexed for given `client_order_id` (if found).
     #[must_use]
     pub fn client_id(&self, client_order_id: &ClientOrderId) -> Option<&ClientId> {
         self.index.order_client.get(client_order_id)
     }
 
+    /// Returns references to all orders matching the given optional filter parameters.
     #[must_use]
     pub fn orders(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
         side: Option<OrderSide>,
     ) -> Vec<&OrderAny> {
         let client_order_ids = self.client_order_ids(venue, instrument_id, strategy_id);
         self.get_orders_for_ids(&client_order_ids, side)
     }
 
+    /// Returns references to all open orders matching the given optional filter parameters.
     #[must_use]
     pub fn orders_open(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
         side: Option<OrderSide>,
     ) -> Vec<&OrderAny> {
         let client_order_ids = self.client_order_ids_open(venue, instrument_id, strategy_id);
         self.get_orders_for_ids(&client_order_ids, side)
     }
 
+    /// Returns references to all closed orders matching the given optional filter parameters.
     #[must_use]
     pub fn orders_closed(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
         side: Option<OrderSide>,
     ) -> Vec<&OrderAny> {
         let client_order_ids = self.client_order_ids_closed(venue, instrument_id, strategy_id);
         self.get_orders_for_ids(&client_order_ids, side)
     }
 
+    /// Returns references to all emulated orders matching the given optional filter parameters.
     #[must_use]
     pub fn orders_emulated(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
         side: Option<OrderSide>,
     ) -> Vec<&OrderAny> {
         let client_order_ids = self.client_order_ids_emulated(venue, instrument_id, strategy_id);
         self.get_orders_for_ids(&client_order_ids, side)
     }
 
+    /// Returns references to all in-flight orders matching the given optional filter parameters.
     #[must_use]
     pub fn orders_inflight(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
         side: Option<OrderSide>,
     ) -> Vec<&OrderAny> {
         let client_order_ids = self.client_order_ids_inflight(venue, instrument_id, strategy_id);
         self.get_orders_for_ids(&client_order_ids, side)
     }
 
+    /// Returns references to all orders for the given `position_id`.
     #[must_use]
     pub fn orders_for_position(&self, position_id: &PositionId) -> Vec<&OrderAny> {
         let client_order_ids = self.index.position_orders.get(position_id);
         match client_order_ids {
             Some(client_order_ids) => {
                 self.get_orders_for_ids(&client_order_ids.iter().copied().collect(), None)
             }
             None => Vec::new(),
         }
     }
 
+    /// Returns whether an order with the given `client_order_id` exists.
     #[must_use]
     pub fn order_exists(&self, client_order_id: &ClientOrderId) -> bool {
         self.index.orders.contains(client_order_id)
     }
 
+    /// Returns whether an order with the given `client_order_id` is open.
     #[must_use]
     pub fn is_order_open(&self, client_order_id: &ClientOrderId) -> bool {
         self.index.orders_open.contains(client_order_id)
     }
 
+    /// Returns whether an order with the given `client_order_id` is closed.
     #[must_use]
     pub fn is_order_closed(&self, client_order_id: &ClientOrderId) -> bool {
         self.index.orders_closed.contains(client_order_id)
     }
 
+    /// Returns whether an order with the given `client_order_id` is emulated.
     #[must_use]
     pub fn is_order_emulated(&self, client_order_id: &ClientOrderId) -> bool {
         self.index.orders_emulated.contains(client_order_id)
     }
 
+    /// Returns whether an order with the given `client_order_id` is in-flight.
     #[must_use]
     pub fn is_order_inflight(&self, client_order_id: &ClientOrderId) -> bool {
         self.index.orders_inflight.contains(client_order_id)
     }
 
+    /// Returns whether an order with the given `client_order_id` is `PENDING_CANCEL` locally.
     #[must_use]
     pub fn is_order_pending_cancel_local(&self, client_order_id: &ClientOrderId) -> bool {
         self.index.orders_pending_cancel.contains(client_order_id)
     }
 
+    /// Returns the count of all open orders.
     #[must_use]
     pub fn orders_open_count(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
         side: Option<OrderSide>,
     ) -> usize {
         self.orders_open(venue, instrument_id, strategy_id, side)
             .len()
     }
 
+    /// Returns the count of all closed orders.
     #[must_use]
     pub fn orders_closed_count(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
         side: Option<OrderSide>,
     ) -> usize {
         self.orders_closed(venue, instrument_id, strategy_id, side)
             .len()
     }
 
+    /// Returns the count of all emulated orders.
     #[must_use]
     pub fn orders_emulated_count(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
         side: Option<OrderSide>,
     ) -> usize {
         self.orders_emulated(venue, instrument_id, strategy_id, side)
             .len()
     }
 
+    /// Returns the count of all in-flight orders.
     #[must_use]
     pub fn orders_inflight_count(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
         side: Option<OrderSide>,
     ) -> usize {
         self.orders_inflight(venue, instrument_id, strategy_id, side)
             .len()
     }
 
+    /// Returns the count of all orders.
     #[must_use]
     pub fn orders_total_count(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
         side: Option<OrderSide>,
     ) -> usize {
         self.orders(venue, instrument_id, strategy_id, side).len()
     }
 
+    /// Returns the order list for the given `order_list_id`.
     #[must_use]
     pub fn order_list(&self, order_list_id: &OrderListId) -> Option<&OrderList> {
         self.order_lists.get(order_list_id)
     }
 
+    /// Returns all order lists matching the given optional filter parameters.
     #[must_use]
     pub fn order_lists(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
     ) -> Vec<&OrderList> {
@@ -1958,21 +2001,24 @@
         if let Some(strategy_id) = strategy_id {
             order_lists.retain(|ol| &ol.strategy_id == strategy_id);
         }
 
         order_lists
     }
 
+    /// Returns whether an order list with the given `order_list_id` exists.
     #[must_use]
     pub fn order_list_exists(&self, order_list_id: &OrderListId) -> bool {
         self.order_lists.contains_key(order_list_id)
     }
 
     // -- EXEC ALGORITHM QUERIES ------------------------------------------------------------------
 
+    /// Returns references to all orders associated with the given `exec_algorithm_id` matching the given
+    /// optional filter parameters.
     #[must_use]
     pub fn orders_for_exec_algorithm(
         &self,
         exec_algorithm_id: &ExecAlgorithmId,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
@@ -1990,25 +2036,27 @@
         if let Some(exec_algorithm_order_ids) = exec_algorithm_order_ids {
             self.get_orders_for_ids(exec_algorithm_order_ids, side)
         } else {
             Vec::new()
         }
     }
 
+    /// Returns references to all orders with the given `exec_spawn_id`.
     #[must_use]
     pub fn orders_for_exec_spawn(&self, exec_spawn_id: &ClientOrderId) -> Vec<&OrderAny> {
         self.get_orders_for_ids(
             self.index
                 .exec_spawn_orders
                 .get(exec_spawn_id)
                 .unwrap_or(&HashSet::new()),
             None,
         )
     }
 
+    /// Returns the total order quantity for the given `exec_spawn_id`.
     #[must_use]
     pub fn exec_spawn_total_quantity(
         &self,
         exec_spawn_id: &ClientOrderId,
         active_only: bool,
     ) -> Option<Quantity> {
         let exec_spawn_orders = self.orders_for_exec_spawn(exec_spawn_id);
@@ -2024,14 +2072,15 @@
                 total_quantity = Some(spawn_order.quantity());
             }
         }
 
         total_quantity
     }
 
+    /// Returns the total filled quantity for all orders with the given `exec_spawn_id`.
     #[must_use]
     pub fn exec_spawn_total_filled_qty(
         &self,
         exec_spawn_id: &ClientOrderId,
         active_only: bool,
     ) -> Option<Quantity> {
         let exec_spawn_orders = self.orders_for_exec_spawn(exec_spawn_id);
@@ -2047,14 +2096,15 @@
                 total_quantity = Some(spawn_order.filled_qty());
             }
         }
 
         total_quantity
     }
 
+    /// Returns the total leaves quantity for all orders with the given `exec_spawn_id`.
     #[must_use]
     pub fn exec_spawn_total_leaves_qty(
         &self,
         exec_spawn_id: &ClientOrderId,
         active_only: bool,
     ) -> Option<Quantity> {
         let exec_spawn_orders = self.orders_for_exec_spawn(exec_spawn_id);
@@ -2072,141 +2122,157 @@
         }
 
         total_quantity
     }
 
     // -- POSITION QUERIES ------------------------------------------------------------------------
 
+    /// Returns a reference to the position with the given `position_id` (if found).
     #[must_use]
     pub fn position(&self, position_id: &PositionId) -> Option<&Position> {
         self.positions.get(position_id)
     }
 
+    /// Returns a reference to the position for the given `client_order_id` (if found).
     #[must_use]
     pub fn position_for_order(&self, client_order_id: &ClientOrderId) -> Option<&Position> {
         self.index
             .order_position
             .get(client_order_id)
             .and_then(|position_id| self.positions.get(position_id))
     }
 
+    /// Returns a reference to the position ID for the given `client_order_id` (if found).
     #[must_use]
     pub fn position_id(&self, client_order_id: &ClientOrderId) -> Option<&PositionId> {
         self.index.order_position.get(client_order_id)
     }
 
+    /// Returns a reference to all positions matching the given optional filter parameters.
     #[must_use]
     pub fn positions(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
         side: Option<PositionSide>,
     ) -> Vec<&Position> {
         let position_ids = self.position_ids(venue, instrument_id, strategy_id);
         self.get_positions_for_ids(&position_ids, side)
     }
 
+    /// Returns a reference to all open positions matching the given optional filter parameters.
     #[must_use]
     pub fn positions_open(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
         side: Option<PositionSide>,
     ) -> Vec<&Position> {
         let position_ids = self.position_open_ids(venue, instrument_id, strategy_id);
         self.get_positions_for_ids(&position_ids, side)
     }
 
+    /// Returns a reference to all closed positions matching the given optional filter parameters.
     #[must_use]
     pub fn positions_closed(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
         side: Option<PositionSide>,
     ) -> Vec<&Position> {
         let position_ids = self.position_closed_ids(venue, instrument_id, strategy_id);
         self.get_positions_for_ids(&position_ids, side)
     }
 
+    /// Returns whether a position with the given `position_id` exists.
     #[must_use]
     pub fn position_exists(&self, position_id: &PositionId) -> bool {
         self.index.positions.contains(position_id)
     }
 
+    /// Returns whether a position with the given `position_id` is open.
     #[must_use]
     pub fn is_position_open(&self, position_id: &PositionId) -> bool {
         self.index.positions_open.contains(position_id)
     }
 
+    /// Returns whether a position with the given `position_id` is closed.
     #[must_use]
     pub fn is_position_closed(&self, position_id: &PositionId) -> bool {
         self.index.positions_closed.contains(position_id)
     }
 
+    /// Returns the count of all open positions.
     #[must_use]
     pub fn positions_open_count(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
         side: Option<PositionSide>,
-    ) -> u64 {
+    ) -> usize {
         self.positions_open(venue, instrument_id, strategy_id, side)
-            .len() as u64
+            .len()
     }
 
+    /// Returns the count of all closed positions.
     #[must_use]
     pub fn positions_closed_count(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
         side: Option<PositionSide>,
-    ) -> u64 {
+    ) -> usize {
         self.positions_closed(venue, instrument_id, strategy_id, side)
-            .len() as u64
+            .len()
     }
 
+    /// Returns the count of all positions.
     #[must_use]
     pub fn positions_total_count(
         &self,
         venue: Option<&Venue>,
         instrument_id: Option<&InstrumentId>,
         strategy_id: Option<&StrategyId>,
         side: Option<PositionSide>,
-    ) -> u64 {
+    ) -> usize {
         self.positions(venue, instrument_id, strategy_id, side)
-            .len() as u64
+            .len()
     }
 
     // -- STRATEGY QUERIES ------------------------------------------------------------------------
 
+    /// Gets a reference to the strategy ID for the given `client_order_id` (if found).
     #[must_use]
     pub fn strategy_id_for_order(&self, client_order_id: &ClientOrderId) -> Option<&StrategyId> {
         self.index.order_strategy.get(client_order_id)
     }
 
+    /// Gets a reference to the strategy ID for the given `position_id` (if found).
     #[must_use]
     pub fn strategy_id_for_position(&self, position_id: &PositionId) -> Option<&StrategyId> {
         self.index.position_strategy.get(position_id)
     }
 
     // -- GENERAL ---------------------------------------------------------------------------------
 
+    /// Gets a reference to the general object value for the given `key` (if found).
     pub fn get(&self, key: &str) -> anyhow::Result<Option<&[u8]>> {
         check_valid_string(key, stringify!(key))?;
 
         Ok(self.general.get(key).map(std::vec::Vec::as_slice))
     }
 
     // -- DATA QUERIES ----------------------------------------------------------------------------
 
+    /// Returns the price for the given `instrument_id` and `price_type` (if found).
     #[must_use]
     pub fn price(&self, instrument_id: &InstrumentId, price_type: PriceType) -> Option<Price> {
         match price_type {
             PriceType::Bid => self
                 .quotes
                 .get(instrument_id)
                 .and_then(|quotes| quotes.front().map(|quote| quote.bid_price)),
@@ -2226,128 +2292,147 @@
             PriceType::Last => self
                 .trades
                 .get(instrument_id)
                 .and_then(|trades| trades.front().map(|trade| trade.price)),
         }
     }
 
+    /// Gets all quote ticks for the given `instrument_id`.
     #[must_use]
     pub fn quote_ticks(&self, instrument_id: &InstrumentId) -> Option<Vec<QuoteTick>> {
         self.quotes
             .get(instrument_id)
             .map(|quotes| quotes.iter().copied().collect())
     }
 
+    /// Gets all trade ticks for the given `instrument_id`.
     #[must_use]
     pub fn trade_ticks(&self, instrument_id: &InstrumentId) -> Option<Vec<TradeTick>> {
         self.trades
             .get(instrument_id)
             .map(|trades| trades.iter().copied().collect())
     }
 
+    /// Gets all bars for the given `bar_type`.
     #[must_use]
     pub fn bars(&self, bar_type: &BarType) -> Option<Vec<Bar>> {
         self.bars
             .get(bar_type)
             .map(|bars| bars.iter().copied().collect())
     }
 
+    /// Gets a reference to the order book for the given `instrument_id`.
     #[must_use]
     pub fn order_book(&self, instrument_id: &InstrumentId) -> Option<&OrderBook> {
         self.books.get(instrument_id)
     }
 
+    /// Gets a reference to the latest quote tick for the given `instrument_id`.
     #[must_use]
     pub fn quote_tick(&self, instrument_id: &InstrumentId) -> Option<&QuoteTick> {
         self.quotes
             .get(instrument_id)
             .and_then(|quotes| quotes.front())
     }
 
+    /// Gets a refernece to the latest trade tick for the given `instrument_id`.
     #[must_use]
     pub fn trade_tick(&self, instrument_id: &InstrumentId) -> Option<&TradeTick> {
         self.trades
             .get(instrument_id)
             .and_then(|trades| trades.front())
     }
 
+    /// Gets a reference to the latest bar for the given `bar_type`.
     #[must_use]
     pub fn bar(&self, bar_type: &BarType) -> Option<&Bar> {
         self.bars.get(bar_type).and_then(|bars| bars.front())
     }
 
+    /// Gets the order book update count for the given `instrument_id`.
     #[must_use]
-    pub fn book_update_count(&self, instrument_id: &InstrumentId) -> u64 {
-        self.books.get(instrument_id).map_or(0, |book| book.count)
+    pub fn book_update_count(&self, instrument_id: &InstrumentId) -> usize {
+        self.books.get(instrument_id).map_or(0, |book| book.count) as usize
     }
 
+    /// Gets the quote tick count for the given `instrument_id`.
     #[must_use]
-    pub fn quote_tick_count(&self, instrument_id: &InstrumentId) -> u64 {
+    pub fn quote_tick_count(&self, instrument_id: &InstrumentId) -> usize {
         self.quotes
             .get(instrument_id)
-            .map_or(0, std::collections::VecDeque::len) as u64
+            .map_or(0, std::collections::VecDeque::len)
     }
 
+    /// Gets the trade tick count for the given `instrument_id`.
     #[must_use]
-    pub fn trade_tick_count(&self, instrument_id: &InstrumentId) -> u64 {
+    pub fn trade_tick_count(&self, instrument_id: &InstrumentId) -> usize {
         self.trades
             .get(instrument_id)
-            .map_or(0, std::collections::VecDeque::len) as u64
+            .map_or(0, std::collections::VecDeque::len)
     }
 
+    /// Gets the bar count for the given `instrument_id`.
     #[must_use]
-    pub fn bar_count(&self, bar_type: &BarType) -> u64 {
+    pub fn bar_count(&self, bar_type: &BarType) -> usize {
         self.bars
             .get(bar_type)
-            .map_or(0, std::collections::VecDeque::len) as u64
+            .map_or(0, std::collections::VecDeque::len)
     }
 
+    /// Returns whether the cache contains an order book for the given `instrument_id`.
     #[must_use]
     pub fn has_order_book(&self, instrument_id: &InstrumentId) -> bool {
         self.books.contains_key(instrument_id)
     }
 
+    /// Returns whether the cache contains quote ticks for the given `instrument_id`.
     #[must_use]
     pub fn has_quote_ticks(&self, instrument_id: &InstrumentId) -> bool {
         self.quote_tick_count(instrument_id) > 0
     }
 
+    /// Returns whether the cache contains trade ticks for the given `instrument_id`.
     #[must_use]
     pub fn has_trade_ticks(&self, instrument_id: &InstrumentId) -> bool {
         self.trade_tick_count(instrument_id) > 0
     }
 
+    /// Returns whether the cache contains bars for the given `bar_type`.
     #[must_use]
     pub fn has_bars(&self, bar_type: &BarType) -> bool {
         self.bar_count(bar_type) > 0
     }
 
     // -- INSTRUMENT QUERIES ----------------------------------------------------------------------
 
+    /// Returns a reference to the instrument for the given `instrument_id` (if found).
     #[must_use]
     pub fn instrument(&self, instrument_id: &InstrumentId) -> Option<&InstrumentAny> {
         self.instruments.get(instrument_id)
     }
 
+    /// Returns references to all instrument IDs for the given `venue`.
     #[must_use]
     pub fn instrument_ids(&self, venue: &Venue) -> Vec<&InstrumentId> {
         self.instruments
             .keys()
             .filter(|i| &i.venue == venue)
             .collect()
     }
 
+    /// Returns references to all instruments for the given `venue`.
     #[must_use]
     pub fn instruments(&self, venue: &Venue) -> Vec<&InstrumentAny> {
         self.instruments
             .values()
             .filter(|i| &i.id().venue == venue)
             .collect()
     }
 
+    /// Returns references to all bar types contained in the cache.
     #[must_use]
     pub fn bar_types(
         &self,
         instrument_id: Option<&InstrumentId>,
         price_type: Option<&PriceType>,
         aggregation_source: AggregationSource,
     ) -> Vec<&BarType> {
@@ -2366,52 +2451,59 @@
         }
 
         bar_types
     }
 
     // -- SYNTHETIC QUERIES -----------------------------------------------------------------------
 
+    /// Returns a reference to the synthetic instrument for the given `instrument_id` (if found).
     #[must_use]
     pub fn synthetic(&self, instrument_id: &InstrumentId) -> Option<&SyntheticInstrument> {
         self.synthetics.get(instrument_id)
     }
 
+    /// Returns references to instrument IDs for all synthetic instruments contained in the cache.
     #[must_use]
     pub fn synthetic_ids(&self) -> Vec<&InstrumentId> {
         self.synthetics.keys().collect()
     }
 
+    /// Returns references to all synthetic instruments contained in the cache.
     #[must_use]
     pub fn synthetics(&self) -> Vec<&SyntheticInstrument> {
         self.synthetics.values().collect()
     }
 
     // -- ACCOUNT QUERIES -----------------------------------------------------------------------
 
+    /// Returns a reference to the account for the given `account_id` (if found).
     #[must_use]
     pub fn account(&self, account_id: &AccountId) -> Option<&dyn Account> {
         self.accounts
             .get(account_id)
             .map(std::convert::AsRef::as_ref)
     }
 
+    /// Returns a reference to the account for the given `venue` (if found).
     #[must_use]
     pub fn account_for_venue(&self, venue: &Venue) -> Option<&dyn Account> {
         self.index
             .venue_account
             .get(venue)
             .and_then(|account_id| self.accounts.get(account_id))
             .map(std::convert::AsRef::as_ref)
     }
 
+    /// Returns a reference to the account ID for the given `venue` (if found).
     #[must_use]
     pub fn account_id(&self, venue: &Venue) -> Option<&AccountId> {
         self.index.venue_account.get(venue)
     }
 
+    /// Returns references to all accounts for the given `account_id`.
     #[must_use]
     pub fn accounts(&self, account_id: &AccountId) -> Vec<&dyn Account> {
         self.accounts
             .values()
             .map(std::convert::AsRef::as_ref)
             .collect()
     }
@@ -2421,28 +2513,28 @@
 // Tests
 ////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
 mod tests {
     use nautilus_core::{nanos::UnixNanos, uuid::UUID4};
     use nautilus_model::{
         data::{bar::Bar, quote::QuoteTick, trade::TradeTick},
-        enums::OrderSide,
+        enums::{OrderSide, OrderStatus},
         events::order::{accepted::OrderAccepted, event::OrderEventAny, submitted::OrderSubmitted},
         identifiers::{
             account_id::AccountId, client_order_id::ClientOrderId, position_id::PositionId,
             venue_order_id::VenueOrderId,
         },
         instruments::{
             any::InstrumentAny, currency_pair::CurrencyPair, stubs::*,
             synthetic::SyntheticInstrument,
         },
         orders::{any::OrderAny, stubs::TestOrderStubs},
         polymorphism::{
-            ApplyOrderEventAny, GetAccountId, GetClientOrderId, GetInstrumentId, GetStrategyId,
-            GetTraderId, GetVenueOrderId, IsOpen,
+            ApplyOrderEventAny, GetAccountId, GetClientOrderId, GetInstrumentId, GetOrderStatus,
+            GetStrategyId, GetTraderId, GetVenueOrderId, IsOpen,
         },
         types::{price::Price, quantity::Quantity},
     };
     use rstest::*;
 
     use super::Cache;
 
@@ -2463,29 +2555,29 @@
 
     #[rstest]
     fn test_reset_when_empty(mut cache: Cache) {
         cache.reset();
     }
 
     #[rstest]
-    fn test_dispose_when_empty(cache: Cache) {
+    fn test_dispose_when_empty(mut cache: Cache) {
         let result = cache.dispose();
         assert!(result.is_ok());
     }
 
     #[rstest]
-    fn test_flush_db_when_empty(cache: Cache) {
+    fn test_flush_db_when_empty(mut cache: Cache) {
         let result = cache.flush_db();
         assert!(result.is_ok());
     }
 
     #[rstest]
     fn test_check_residuals_when_empty(cache: Cache) {
-        let result = cache.flush_db();
-        assert!(result.is_ok());
+        let result = cache.check_residuals();
+        assert!(!result);
     }
 
     #[rstest]
     fn test_cache_general_load_when_no_database(mut cache: Cache) {
         assert!(cache.cache_general().is_ok());
     }
 
@@ -2595,30 +2687,31 @@
         )
         .unwrap(); // TODO: Should event generation be fallible?
         order.apply(OrderEventAny::Submitted(submitted)).unwrap();
         cache.update_order(&order).unwrap();
 
         let result = cache.order(&order.client_order_id()).unwrap();
 
+        assert_eq!(order.status(), OrderStatus::Submitted);
         assert_eq!(result, &order);
         assert_eq!(cache.orders(None, None, None, None), vec![&order]);
         assert!(cache.orders_open(None, None, None, None).is_empty());
         assert!(cache.orders_closed(None, None, None, None).is_empty());
         assert!(cache.orders_emulated(None, None, None, None).is_empty());
-        assert!(cache.orders_inflight(None, None, None, None).is_empty());
+        assert!(!cache.orders_inflight(None, None, None, None).is_empty());
         assert!(cache.order_exists(&order.client_order_id()));
         assert!(!cache.is_order_open(&order.client_order_id()));
         assert!(!cache.is_order_closed(&order.client_order_id()));
         assert!(!cache.is_order_emulated(&order.client_order_id()));
-        assert!(!cache.is_order_inflight(&order.client_order_id()));
+        assert!(cache.is_order_inflight(&order.client_order_id()));
         assert!(!cache.is_order_pending_cancel_local(&order.client_order_id()));
         assert_eq!(cache.orders_open_count(None, None, None, None), 0);
         assert_eq!(cache.orders_closed_count(None, None, None, None), 0);
         assert_eq!(cache.orders_emulated_count(None, None, None, None), 0);
-        assert_eq!(cache.orders_inflight_count(None, None, None, None), 0);
+        assert_eq!(cache.orders_inflight_count(None, None, None, None), 1);
         assert_eq!(cache.orders_total_count(None, None, None, None), 1);
         assert_eq!(cache.venue_order_id(&order.client_order_id()), None);
     }
 
     #[rstest]
     fn test_order_when_accepted_open(mut cache: Cache, audusd_sim: CurrencyPair) {
         let order = TestOrderStubs::limit_order(
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/cache/database.rs` & `nautilus_trader-1.194.0/nautilus_core/execution/src/engine.rs`

 * *Files 27% similar despite different names*

```diff
@@ -9,279 +9,280 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides a `Cache` database backing.
+//! Provides a generic `ExecutionEngine` for backtesting and live environments.
 
 // Under development
 #![allow(dead_code)]
 #![allow(unused_variables)]
 
-use std::{collections::HashMap, sync::mpsc::Receiver};
+use std::collections::{HashMap, HashSet};
 
-use nautilus_core::{nanos::UnixNanos, uuid::UUID4};
+use log::debug;
+use nautilus_common::{cache::Cache, generators::position_id::PositionIdGenerator};
 use nautilus_model::{
+    enums::{OmsType, OrderSide},
+    events::order::{event::OrderEventAny, filled::OrderFilled},
     identifiers::{
-        account_id::AccountId, client_id::ClientId, client_order_id::ClientOrderId,
-        component_id::ComponentId, instrument_id::InstrumentId, position_id::PositionId,
-        strategy_id::StrategyId, trader_id::TraderId, venue_order_id::VenueOrderId,
+        client_id::ClientId, instrument_id::InstrumentId, strategy_id::StrategyId, venue::Venue,
     },
-    instruments::{any::InstrumentAny, synthetic::SyntheticInstrument},
-    orders::{any::OrderAny, base::Order},
+    instruments::any::InstrumentAny,
+    orders::any::OrderAny,
     position::Position,
-    types::currency::Currency,
+    types::quantity::Quantity,
 };
-use ustr::Ustr;
 
-use crate::{enums::SerializationEncoding, interface::account::Account};
+use crate::{
+    client::ExecutionClient,
+    messages::{
+        cancel::CancelOrder, cancel_all::CancelAllOrders, cancel_batch::BatchCancelOrders,
+        modify::ModifyOrder, query::QueryOrder, submit::SubmitOrder, submit_list::SubmitOrderList,
+        TradingCommand,
+    },
+};
 
-/// A type of database operation.
-#[derive(Clone, Debug)]
-pub enum DatabaseOperation {
-    Insert,
-    Update,
-    Delete,
-    Close,
+pub struct ExecutionEngineConfig {
+    pub debug: bool,
 }
 
-/// Represents a database command to be performed which may be executed in another thread.
-#[derive(Clone, Debug)]
-pub struct DatabaseCommand {
-    /// The database operation type.
-    pub op_type: DatabaseOperation,
-    /// The primary key for the operation.
-    pub key: Option<String>,
-    /// The data payload for the operation.
-    pub payload: Option<Vec<Vec<u8>>>,
+pub struct ExecutionEngine {
+    pub command_count: u64,
+    pub event_count: u64,
+    pub report_count: u64,
+    cache: &'static Cache,
+    default_client: Option<ExecutionClient>,
+    pos_id_generator: PositionIdGenerator,
+    clients: HashMap<ClientId, ExecutionClient>,
+    routing_map: HashMap<Venue, ClientId>,
+    oms_overrides: HashMap<StrategyId, OmsType>,
+    external_order_claims: HashMap<InstrumentId, StrategyId>,
+    config: ExecutionEngineConfig,
 }
 
-impl DatabaseCommand {
+impl ExecutionEngine {
     #[must_use]
-    pub fn new(op_type: DatabaseOperation, key: String, payload: Option<Vec<Vec<u8>>>) -> Self {
-        Self {
-            op_type,
-            key: Some(key),
-            payload,
-        }
+    pub fn position_id_count(&self, strategy_id: StrategyId) -> u64 {
+        todo!();
     }
 
-    /// Initialize a `Close` database command, this is meant to close the database cache channel.
     #[must_use]
-    pub fn close() -> Self {
-        Self {
-            op_type: DatabaseOperation::Close,
-            key: None,
-            payload: None,
-        }
+    pub fn check_integrity(&self) -> bool {
+        todo!();
     }
-}
-
-/// Provides a generic cache database facade.
-///
-/// The main operations take a consistent `key` and `payload` which should provide enough
-/// information to implement the cache database in many different technologies.
-///
-/// Delete operations may need a `payload` to target specific values.
-pub trait CacheDatabase {
-    type DatabaseType;
-
-    fn new(
-        trader_id: TraderId,
-        instance_id: UUID4,
-        config: HashMap<String, serde_json::Value>,
-    ) -> anyhow::Result<Self::DatabaseType>;
-    fn close(&mut self) -> anyhow::Result<()>;
-    fn flushdb(&mut self) -> anyhow::Result<()>;
-    fn keys(&mut self, pattern: &str) -> anyhow::Result<Vec<String>>;
-    fn read(&mut self, key: &str) -> anyhow::Result<Vec<Vec<u8>>>;
-    fn insert(&mut self, key: String, payload: Option<Vec<Vec<u8>>>) -> anyhow::Result<()>;
-    fn update(&mut self, key: String, payload: Option<Vec<Vec<u8>>>) -> anyhow::Result<()>;
-    fn delete(&mut self, key: String, payload: Option<Vec<Vec<u8>>>) -> anyhow::Result<()>;
-    fn handle_messages(
-        rx: Receiver<DatabaseCommand>,
-        trader_key: String,
-        config: HashMap<String, serde_json::Value>,
-    );
-}
 
-pub struct CacheDatabaseAdapter {
-    pub encoding: SerializationEncoding,
-    // database: Box<dyn CacheDatabase>,  // TBD
-}
-
-impl CacheDatabaseAdapter {
-    pub fn close(&self) -> anyhow::Result<()> {
-        Ok(()) // TODO
+    #[must_use]
+    pub fn check_connected(&self) -> bool {
+        todo!();
     }
 
-    pub fn flush(&self) -> anyhow::Result<()> {
-        Ok(()) // TODO
+    #[must_use]
+    pub fn check_disconnected(&self) -> bool {
+        todo!();
     }
 
-    pub fn keys(&self) -> anyhow::Result<Vec<String>> {
-        Ok(vec![])
+    #[must_use]
+    pub fn check_residuals(&self) -> bool {
+        todo!();
     }
 
-    pub fn load(&self) -> anyhow::Result<HashMap<String, Vec<u8>>> {
-        Ok(HashMap::new()) // TODO
+    #[must_use]
+    pub fn get_external_order_claims_instruments(&self) -> HashSet<InstrumentId> {
+        todo!();
     }
 
-    pub fn load_currencies(&self) -> anyhow::Result<HashMap<Ustr, Currency>> {
-        Ok(HashMap::new()) // TODO
-    }
+    // -- REGISTRATION --------------------------------------------------------
 
-    pub fn load_instruments(&self) -> anyhow::Result<HashMap<InstrumentId, InstrumentAny>> {
-        Ok(HashMap::new()) // TODO
+    pub fn register_client(&mut self, client: ExecutionClient) -> anyhow::Result<()> {
+        todo!();
     }
 
-    pub fn load_synthetics(&self) -> anyhow::Result<HashMap<InstrumentId, SyntheticInstrument>> {
-        Ok(HashMap::new()) // TODO
+    pub fn register_default_client(&mut self, client: ExecutionClient) -> anyhow::Result<()> {
+        todo!();
     }
 
-    pub fn load_accounts(&self) -> anyhow::Result<HashMap<AccountId, Box<dyn Account>>> {
-        Ok(HashMap::new()) // TODO
+    pub fn register_venue_routing(
+        &mut self,
+        client_id: ClientId,
+        venue: Venue,
+    ) -> anyhow::Result<()> {
+        todo!();
     }
 
-    pub fn load_orders(&self) -> anyhow::Result<HashMap<ClientOrderId, OrderAny>> {
-        Ok(HashMap::new()) // TODO
-    }
+    // TODO: Implement `Strategy`
+    // pub fn register_external_order_claims(&mut self, strategy: Strategy) -> anyhow::Result<()> {
+    //     todo!();
+    // }
 
-    pub fn load_positions(&self) -> anyhow::Result<HashMap<PositionId, Position>> {
-        Ok(HashMap::new()) // TODO
+    pub fn deregister_client(&mut self, client_id: ClientId) -> anyhow::Result<()> {
+        todo!();
     }
 
-    pub fn load_index_order_position(&self) -> anyhow::Result<HashMap<ClientOrderId, Position>> {
-        Ok(HashMap::new()) // TODO
+    // -- COMMANDS ------------------------------------------------------------
+
+    pub fn load_cache(&self) {
+        todo!();
     }
 
-    pub fn load_index_order_client(&self) -> anyhow::Result<HashMap<ClientOrderId, ClientId>> {
-        Ok(HashMap::new()) // TODO
+    pub fn flush_db(&self) {
+        todo!();
     }
 
-    pub fn load_currency(&self, code: &Ustr) -> anyhow::Result<Currency> {
-        todo!() // TODO
+    pub fn execute(&mut self, command: TradingCommand) {
+        self.execute_command(command);
     }
 
-    pub fn load_instrument(&self, instrument_id: &InstrumentId) -> anyhow::Result<InstrumentAny> {
-        todo!() // TODO
+    pub fn process(&self, event: &OrderEventAny) {
+        todo!();
     }
 
-    pub fn load_synthetic(
-        &self,
-        instrument_id: &InstrumentId,
-    ) -> anyhow::Result<SyntheticInstrument> {
-        todo!() // TODO
+    // -- COMMAND HANDLERS ----------------------------------------------------
+
+    fn execute_command(&mut self, command: TradingCommand) {
+        debug!("<--[CMD] {:?}", command); // TODO: Log constants
+        self.command_count += 1;
+
+        // TODO: Refine getting the client (no need for two expects)
+        let client = if let Some(client) = self.clients.get(&command.client_id()) {
+            client
+        } else if let Some(client_id) = self.routing_map.get(&command.instrument_id().venue) {
+            if let Some(client) = self.clients.get(client_id) {
+                client
+            } else {
+                self.default_client.as_ref().expect("No client found")
+            }
+        } else {
+            self.default_client.as_ref().expect("No client found")
+        };
+
+        match command {
+            TradingCommand::SubmitOrder(cmd) => self.handle_submit_order(client, cmd),
+            TradingCommand::SubmitOrderList(cmd) => self.handle_submit_order_list(client, cmd),
+            TradingCommand::ModifyOrder(cmd) => self.handle_modify_order(client, cmd),
+            TradingCommand::CancelOrder(cmd) => self.handle_cancel_order(client, cmd),
+            TradingCommand::CancelAllOrders(cmd) => self.handle_cancel_all_orders(client, cmd),
+            TradingCommand::BatchCancelOrders(cmd) => self.handle_batch_cancel_orders(client, cmd),
+            TradingCommand::QueryOrder(cmd) => self.handle_query_order(client, cmd),
+        }
     }
 
-    pub fn load_account(&self, account_id: &AccountId) -> anyhow::Result<()> {
-        todo!() // TODO
+    fn handle_submit_order(&self, client: &ExecutionClient, command: SubmitOrder) {
+        todo!();
     }
 
-    pub fn load_order(&self, client_order_id: &ClientOrderId) -> anyhow::Result<Box<dyn Order>> {
-        todo!() // TODO
+    fn handle_submit_order_list(&self, client: &ExecutionClient, command: SubmitOrderList) {
+        todo!();
     }
 
-    pub fn load_position(&self, position_id: &PositionId) -> anyhow::Result<Position> {
-        todo!() // TODO
+    fn handle_modify_order(&self, client: &ExecutionClient, command: ModifyOrder) {
+        todo!();
     }
 
-    pub fn load_actor(
-        &self,
-        component_id: &ComponentId,
-    ) -> anyhow::Result<HashMap<String, Vec<u8>>> {
-        todo!() // TODO
+    fn handle_cancel_order(&self, client: &ExecutionClient, command: CancelOrder) {
+        todo!();
     }
 
-    pub fn delete_actor(&self, component_id: &ComponentId) -> anyhow::Result<()> {
-        todo!() // TODO
+    fn handle_cancel_all_orders(&self, client: &ExecutionClient, command: CancelAllOrders) {
+        todo!();
     }
 
-    pub fn load_strategy(
-        &self,
-        strategy_id: &StrategyId,
-    ) -> anyhow::Result<HashMap<String, Vec<u8>>> {
-        todo!() // TODO
+    fn handle_batch_cancel_orders(&self, client: &ExecutionClient, command: BatchCancelOrders) {
+        todo!();
     }
 
-    pub fn delete_strategy(&self, component_id: &StrategyId) -> anyhow::Result<()> {
-        todo!() // TODO
+    fn handle_query_order(&self, client: &ExecutionClient, command: QueryOrder) {
+        todo!();
     }
 
-    pub fn add(&self, key: String, value: Vec<u8>) -> anyhow::Result<()> {
-        todo!() // TODO
+    // -- EVENT HANDLERS ----------------------------------------------------
+
+    fn handle_event(&self, event: OrderEventAny) {
+        todo!();
     }
 
-    pub fn add_currency(&self, currency: &Currency) -> anyhow::Result<()> {
-        todo!() // TODO
+    fn determine_oms_type(&self, fill: OrderFilled) {
+        todo!();
     }
 
-    pub fn add_instrument(&self, instrument: &InstrumentAny) -> anyhow::Result<()> {
-        todo!() // TODO
+    fn determine_position_id(&self, fill: OrderFilled, oms_type: OmsType) {
+        todo!();
     }
 
-    pub fn add_synthetic(&self, synthetic: &SyntheticInstrument) -> anyhow::Result<()> {
-        todo!() // TODO
+    fn determine_hedging_position_id(&self, fill: OrderFilled) {
+        todo!();
     }
 
-    pub fn add_account(&self, account: &dyn Account) -> anyhow::Result<Box<dyn Account>> {
-        todo!() // TODO
+    fn determine_netting_position_id(&self, fill: OrderFilled) {
+        todo!();
     }
 
-    pub fn add_order(&self, order: &OrderAny) -> anyhow::Result<()> {
-        todo!() // TODO
+    fn apply_event_to_order(&self, order: &OrderAny, event: OrderEventAny) {
+        todo!();
     }
 
-    pub fn add_position(&self, position: &Position) -> anyhow::Result<()> {
-        todo!() // TODO
+    fn handle_order_fill(&self, order: &OrderAny, fill: OrderFilled, oms_type: OmsType) {
+        todo!();
     }
 
-    pub fn index_venue_order_id(
+    fn open_position(
         &self,
-        client_order_id: ClientOrderId,
-        venue_order_id: VenueOrderId,
-    ) -> anyhow::Result<()> {
-        todo!() // TODO
+        instrument: InstrumentAny,
+        position: &Position,
+        fill: OrderFilled,
+        oms_type: OmsType,
+    ) {
+        todo!();
     }
 
-    pub fn index_order_position(
+    fn update_position(
         &self,
-        client_order_id: ClientOrderId,
-        position_id: PositionId,
-    ) -> anyhow::Result<()> {
-        todo!() // TODO
+        instrument: InstrumentAny,
+        position: &Position,
+        fill: OrderFilled,
+        oms_type: OmsType,
+    ) {
+        todo!();
     }
 
-    pub fn update_actor(&self) -> anyhow::Result<()> {
-        todo!() // TODO
+    fn will_flip_position(&self, position: &Position, fill: OrderFilled) {
+        todo!();
     }
 
-    pub fn update_strategy(&self) -> anyhow::Result<()> {
-        todo!() // TODO
+    fn flip_position(
+        &self,
+        instrument: InstrumentAny,
+        position: &Position,
+        fill: OrderFilled,
+        oms_type: OmsType,
+    ) {
+        todo!();
     }
 
-    pub fn update_account(&self, account: &dyn Account) -> anyhow::Result<()> {
-        todo!() // TODO
+    fn publish_order_snapshot(&self, order: &OrderAny) {
+        todo!();
     }
 
-    pub fn update_order(&self, order: &OrderAny) -> anyhow::Result<()> {
-        todo!() // TODO
+    fn publish_position_snapshot(&self, position: &Position) {
+        todo!();
     }
 
-    pub fn update_position(&self, position: &Position) -> anyhow::Result<()> {
-        todo!() // TODO
+    // -- INTERNAL ------------------------------------------------------------
+
+    fn set_position_id_counts(&self) {
+        todo!();
     }
 
-    pub fn snapshot_order_state(&self, order: &OrderAny) -> anyhow::Result<()> {
-        todo!() // TODO
+    fn last_px_for_conversion(&self, instrument_id: InstrumentId, side: OrderSide) {
+        todo!();
     }
 
-    pub fn snapshot_position_state(&self, position: &Position) -> anyhow::Result<()> {
-        todo!() // TODO
+    fn set_order_base_qty(&self, order: &OrderAny, base_qty: Quantity) {
+        todo!();
     }
 
-    pub fn heartbeat(&self, timestamp: UnixNanos) -> anyhow::Result<()> {
-        todo!() // TODO
+    fn deny_order(&self, order: &OrderAny, reason: &str) {
+        todo!();
     }
 }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/cache/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/clock.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/clock.rs`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides real-time and static test `Clock` implementations.
+//! Real-time and static test `Clock` implementations.
 
 use std::{collections::HashMap, ops::Deref};
 
 use nautilus_core::{
     correctness::{check_positive_u64, check_predicate_true, check_valid_string},
     nanos::UnixNanos,
     time::{get_atomic_clock_realtime, AtomicTime},
@@ -67,22 +67,26 @@
     ) -> anyhow::Result<()>;
 
     fn next_time_ns(&self, name: &str) -> UnixNanos;
     fn cancel_timer(&mut self, name: &str);
     fn cancel_timers(&mut self);
 }
 
+/// A static test clock.
+///
+/// Stores the current timestamp internally which can be advanced.
 pub struct TestClock {
     time: AtomicTime,
     timers: HashMap<Ustr, TestTimer>,
     default_callback: Option<EventHandler>,
     callbacks: HashMap<Ustr, EventHandler>,
 }
 
 impl TestClock {
+    /// Creates a new [`TestClock`] instance.
     #[must_use]
     pub fn new() -> Self {
         Self {
             time: AtomicTime::new(false, UnixNanos::default()),
             timers: HashMap::new(),
             default_callback: None,
             callbacks: HashMap::new(),
@@ -145,14 +149,15 @@
     TimeEventHandler {
         event,
         callback_ptr: handler.callback.as_ptr().cast::<c_char>(),
     }
 }
 
 impl Default for TestClock {
+    /// Creates a new default [`TestClock`] instance.
     fn default() -> Self {
         Self::new()
     }
 }
 
 impl Deref for TestClock {
     type Target = AtomicTime;
@@ -257,21 +262,25 @@
         for timer in &mut self.timers.values_mut() {
             timer.cancel();
         }
         self.timers = HashMap::new();
     }
 }
 
+/// A real-time clock which uses system time.
+///
+/// Timestamps are guaranteed to be unique and monotonically increasing.
 pub struct LiveClock {
     time: &'static AtomicTime,
     timers: HashMap<Ustr, LiveTimer>,
     default_callback: Option<EventHandler>,
 }
 
 impl LiveClock {
+    /// Creates a new [`LiveClock`] instance.
     #[must_use]
     pub fn new() -> Self {
         Self {
             time: get_atomic_clock_realtime(),
             timers: HashMap::new(),
             default_callback: None,
         }
@@ -280,14 +289,15 @@
     #[must_use]
     pub fn get_timers(&self) -> &HashMap<Ustr, LiveTimer> {
         &self.timers
     }
 }
 
 impl Default for LiveClock {
+    /// Creates a new default [`LiveClock`] instance.
     fn default() -> Self {
         Self::new()
     }
 }
 
 impl Deref for LiveClock {
     type Target = AtomicTime;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/enums.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/enums.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines common enumerations.
+//! Enumerations for common components.
 
 use std::fmt::Debug;
 
 use serde::{Deserialize, Serialize};
 use strum::{Display, EnumIter, EnumString, FromRepr};
 
 /// The state of a component within the system.
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/factories.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/factories.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides factories for constructing domain objects such as orders.
+//! Factories for constructing domain objects such as orders.
 
 use std::collections::HashMap;
 
 use nautilus_core::{time::AtomicTime, uuid::UUID4};
 use nautilus_model::{
     enums::{ContingencyType, OrderSide, TimeInForce},
     identifiers::{
@@ -40,14 +40,15 @@
     trader_id: TraderId,
     strategy_id: StrategyId,
     order_id_generator: ClientOrderIdGenerator,
     order_list_id_generator: OrderListIdGenerator,
 }
 
 impl OrderFactory {
+    /// Creates a new [`OrderFactory`] instance.
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         init_order_id_count: Option<usize>,
         init_order_list_id_count: Option<usize>,
         clock: &'static AtomicTime,
     ) -> Self {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/ffi/clock.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/ffi/clock.rs`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 use crate::{
     clock::{Clock, LiveClock, TestClock},
     handlers::EventHandler,
     timer::{TimeEvent, TimeEventHandler},
 };
 
-/// Provides a C compatible Foreign Function Interface (FFI) for an underlying [`TestClock`].
+/// C compatible Foreign Function Interface (FFI) for an underlying [`TestClock`].
 ///
 /// This struct wraps `TestClock` in a way that makes it compatible with C function
 /// calls, enabling interaction with `TestClock` in a C environment.
 ///
 /// It implements the `Deref` trait, allowing instances of `TestClock_API` to be
 /// dereferenced to `TestClock`, providing access to `TestClock`'s methods without
 /// having to manually access the underlying `TestClock` instance.
@@ -239,15 +239,15 @@
 }
 
 #[no_mangle]
 pub extern "C" fn test_clock_cancel_timers(clock: &mut TestClock_API) {
     clock.cancel_timers();
 }
 
-/// Provides a C compatible Foreign Function Interface (FFI) for an underlying [`LiveClock`].
+/// C compatible Foreign Function Interface (FFI) for an underlying [`LiveClock`].
 ///
 /// This struct wraps `LiveClock` in a way that makes it compatible with C function
 /// calls, enabling interaction with `LiveClock` in a C environment.
 ///
 /// It implements the `Deref` and `DerefMut` traits, allowing instances of `LiveClock_API` to be
 /// dereferenced to `LiveClock`, providing access to `LiveClock`'s methods without
 /// having to manually access the underlying `LiveClock` instance. This includes
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/ffi/enums.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/ffi/enums.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/ffi/logging.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/ffi/logging.rs`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self, headers,
         logger::{self, LogGuard, LoggerConfig},
         logging_set_bypass, map_log_level_to_filter, parse_component_levels,
         writer::FileWriterConfig,
     },
 };
 
-/// Provides a C compatible Foreign Function Interface (FFI) for an underlying [`LogGuard`].
+/// C compatible Foreign Function Interface (FFI) for an underlying [`LogGuard`].
 ///
 /// This struct wraps `LogGuard` in a way that makes it compatible with C function
 /// calls, enabling interaction with `LogGuard` in a C environment.
 ///
 /// It implements the `Deref` trait, allowing instances of `LogGuard_API` to be
 /// dereferenced to `LogGuard`, providing access to `LogGuard`'s methods without
 /// having to manually access the underlying `LogGuard` instance.
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/ffi/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/momentum/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -9,13 +9,12 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides a C foreign function interface (FFI) from `cbindgen`.
-
-pub mod clock;
-pub mod enums;
-pub mod logging;
-pub mod timer;
+pub mod aroon;
+pub mod bias;
+pub mod cmo;
+pub mod rsi;
+pub mod vhf;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/ffi/timer.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/ffi/timer.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/generators/client_order_id.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/generators/client_order_id.rs`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     clock: &'static AtomicTime,
     trader_id: TraderId,
     strategy_id: StrategyId,
     count: usize,
 }
 
 impl ClientOrderIdGenerator {
+    /// Creates a new [`ClientOrderIdGenerator`] instance.
     #[must_use]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         initial_count: usize,
         clock: &'static AtomicTime,
     ) -> Self {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/generators/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/generators/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/generators/order_list_id.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/generators/order_list_id.rs`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     clock: &'static AtomicTime,
     trader_id: TraderId,
     strategy_id: StrategyId,
     count: usize,
 }
 
 impl OrderListIdGenerator {
+    /// Creates a new [`OrderListIdGenerator`] instance.
     #[must_use]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         initial_count: usize,
         clock: &'static AtomicTime,
     ) -> Self {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/generators/position_id.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/generators/position_id.rs`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 pub struct PositionIdGenerator {
     clock: &'static AtomicTime,
     trader_id: TraderId,
     counts: HashMap<StrategyId, usize>,
 }
 
 impl PositionIdGenerator {
+    /// Creates a new [`PositionIdGenerator`] instance.
     #[must_use]
     pub fn new(trader_id: TraderId, clock: &'static AtomicTime) -> Self {
         Self {
             clock,
             trader_id,
             counts: HashMap::new(),
         }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/handlers.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/handlers.rs`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides common message handlers.
+//! Common message handlers.
 
 #[cfg(not(feature = "python"))]
 use std::ffi::c_char;
 use std::{fmt, sync::Arc};
 
 #[cfg(not(feature = "python"))]
 use nautilus_core::message::Message;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/interface/account.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/interface/account.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/interface/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/interface/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/lib.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/logging/headers.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/logging/headers.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/logging/logger.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/logging/logger.rs`

 * *Files 4% similar despite different names*

```diff
@@ -60,26 +60,28 @@
     /// If logger is using ANSI color codes.
     pub is_colored: bool,
     /// If the configuration should be printed to stdout at initialization.
     pub print_config: bool,
 }
 
 impl Default for LoggerConfig {
+    /// Creates a new default [`LoggerConfig`] instance.
     fn default() -> Self {
         Self {
             stdout_level: LevelFilter::Info,
             fileout_level: LevelFilter::Off,
             component_level: HashMap::new(),
             is_colored: false,
             print_config: false,
         }
     }
 }
 
 impl LoggerConfig {
+    /// Creates a new [`LoggerConfig`] instance.
     #[must_use]
     pub fn new(
         stdout_level: LevelFilter,
         fileout_level: LevelFilter,
         component_level: HashMap<Ustr, LevelFilter>,
         is_colored: bool,
         print_config: bool,
@@ -142,15 +144,15 @@
 
 /// Initialize tracing.
 ///
 /// Tracing is meant to be used to trace/debug async Rust code. It can be
 /// configured to filter modules and write up to a specific level only using
 /// by passing a configuration using the `RUST_LOG` environment variable.
 
-/// Provides a high-performance logger utilizing a MPSC channel under the hood.
+/// A high-performance logger utilizing a MPSC channel under the hood.
 ///
 /// A separate thead is spawned at initialization which receives [`LogEvent`] structs over the
 /// channel.
 #[derive(Debug)]
 pub struct Logger {
     /// Configure maximum levels for components and IO.
     pub config: LoggerConfig,
@@ -190,14 +192,15 @@
     cache: Option<String>,
     colored: Option<String>,
     timestamp: String,
     trader_id: Ustr,
 }
 
 impl LogLineWrapper {
+    /// Creates a new [`LogLineWrapper`] instance.
     #[must_use]
     pub fn new(line: LogLine, trader_id: Ustr, timestamp: UnixNanos) -> Self {
         Self {
             line,
             cache: None,
             colored: None,
             timestamp: unix_nanos_to_iso8601(timestamp),
@@ -475,21 +478,23 @@
 )]
 #[derive(Debug)]
 pub struct LogGuard {
     handle: Option<JoinHandle<()>>,
 }
 
 impl LogGuard {
+    /// Creates a new [`LogGuard`] instance.
     #[must_use]
     pub fn new(handle: Option<JoinHandle<()>>) -> Self {
         Self { handle }
     }
 }
 
 impl Default for LogGuard {
+    /// Creates a new default [`LogGuard`] instance.
     fn default() -> Self {
         Self::new(None)
     }
 }
 
 impl Drop for LogGuard {
     fn drop(&mut self) {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/logging/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/logging/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/logging/writer.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/logging/writer.rs`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 pub struct StdoutWriter {
     pub is_colored: bool,
     buf: BufWriter<Stdout>,
     level: LevelFilter,
 }
 
 impl StdoutWriter {
+    /// Creates a new [`StdoutWriter`] instance.
     #[must_use]
     pub fn new(level: LevelFilter, is_colored: bool) -> Self {
         Self {
             buf: BufWriter::new(io::stdout()),
             level,
             is_colored,
         }
@@ -76,14 +77,15 @@
 #[derive(Debug)]
 pub struct StderrWriter {
     pub is_colored: bool,
     buf: BufWriter<Stderr>,
 }
 
 impl StderrWriter {
+    /// Creates a new [`StderrWriter`] instance.
     #[must_use]
     pub fn new(is_colored: bool) -> Self {
         Self {
             buf: BufWriter::new(io::stderr()),
             is_colored,
         }
     }
@@ -117,14 +119,15 @@
 pub struct FileWriterConfig {
     pub directory: Option<String>,
     pub file_name: Option<String>,
     pub file_format: Option<String>,
 }
 
 impl FileWriterConfig {
+    /// Creates a new [`FileWriterConfig`] instance.
     #[must_use]
     pub fn new(
         directory: Option<String>,
         file_name: Option<String>,
         file_format: Option<String>,
     ) -> Self {
         Self {
@@ -143,14 +146,15 @@
     file_config: FileWriterConfig,
     trader_id: String,
     instance_id: String,
     level: LevelFilter,
 }
 
 impl FileWriter {
+    /// Creates a new [`FileWriter`] instance.
     pub fn new(
         trader_id: String,
         instance_id: String,
         file_config: FileWriterConfig,
         fileout_level: LevelFilter,
     ) -> Option<Self> {
         // Setup log file
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/msgbus/core.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/msgbus/core.rs`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     pub handler: MessageHandler,
     pub topic: Ustr,
     pub sequence: usize,
     pub priority: u8,
 }
 
 impl Subscription {
+    /// Creates a new [`Subscription`] instance.
     #[must_use]
     pub fn new(
         topic: Ustr,
         handler: MessageHandler,
         sequence: usize,
         priority: Option<u8>,
     ) -> Self {
@@ -105,15 +106,15 @@
             "[{}] {}",
             self.topic,
             String::from_utf8_lossy(&self.payload)
         )
     }
 }
 
-/// Provides a generic message bus to facilitate various messaging patterns.
+/// A generic message bus to facilitate various messaging patterns.
 ///
 /// The bus provides both a producer and consumer API for Pub/Sub, Req/Rep, as
 /// well as direct point-to-point messaging to registered endpoints.
 ///
 /// Pub/Sub wildcard patterns for hierarchical topics are possible:
 ///  - `*` asterisk represents one or more characters in a pattern.
 ///  - `?` question mark represents a single character in a pattern.
@@ -161,15 +162,15 @@
     /// Relates a request with a response
     /// a request maps it's id to a handler so that a response
     /// with the same id can later be handled.
     correlation_index: IndexMap<UUID4, MessageHandler>,
 }
 
 impl MessageBus {
-    /// Creates a new `MessageBus` instance.
+    /// Creates a new [`MessageBus`] instance.
     pub fn new(
         trader_id: TraderId,
         instance_id: UUID4,
         name: Option<String>,
         _config: Option<HashMap<String, serde_json::Value>>,
     ) -> anyhow::Result<Self> {
         Ok(Self {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/msgbus/database.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/msgbus/database.rs`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 // -------------------------------------------------------------------------------------------------
 
 use std::collections::HashMap;
 
 use nautilus_core::uuid::UUID4;
 use nautilus_model::identifiers::trader_id::TraderId;
 
-/// Provides a generic message bus database facade.
+/// A generic message bus database facade.
 ///
 /// The main operations take a consistent `key` and `payload` which should provide enough
 /// information to implement the message bus database in many different technologies.
 ///
 /// Delete operations may need a `payload` to target specific values.
 pub trait MessageBusDatabaseAdapter {
     type DatabaseType;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/msgbus/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/msgbus/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/python/clock.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/python/clock.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/python/enums.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/python/enums.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/python/logging.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/python/logging.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/python/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/python/timer.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/python/timer.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/python/versioning.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/python/versioning.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/runtime.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/runtime.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/stubs.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/stubs.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/testing.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/testing.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/timer.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/timer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides real-time and test timers for use with `Clock` implementations.
+//! Real-time and test timers for use with `Clock` implementations.
 
 use std::{
     cmp::Ordering,
     ffi::c_char,
     fmt::{Display, Formatter},
     num::NonZeroU64,
     sync::{
@@ -55,16 +55,18 @@
     pub event_id: UUID4,
     /// The message category
     pub ts_event: UnixNanos,
     /// The UNIX timestamp (nanoseconds) when the object was initialized.
     pub ts_init: UnixNanos,
 }
 
-/// Assumes `name` is a valid string.
 impl TimeEvent {
+    /// Creates a new [`TimeEvent`] instance.
+    ///
+    /// Assumes `name` is a valid string.
     #[must_use]
     pub fn new(name: Ustr, event_id: UUID4, ts_event: UnixNanos, ts_init: UnixNanos) -> Self {
         Self {
             name,
             event_id,
             ts_event,
             ts_init,
@@ -88,15 +90,15 @@
     }
 }
 
 #[repr(C)]
 #[derive(Clone, Debug)]
 /// Represents a time event and its associated handler.
 pub struct TimeEventHandler {
-    /// The event.
+    /// The time event.
     pub event: TimeEvent,
     /// The callable raw pointer.
     pub callback_ptr: *mut c_char,
 }
 
 impl PartialOrd for TimeEventHandler {
     fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
@@ -114,27 +116,27 @@
 
 impl Ord for TimeEventHandler {
     fn cmp(&self, other: &Self) -> Ordering {
         self.event.ts_event.cmp(&other.event.ts_event)
     }
 }
 
-/// Provides a test timer for user with a `TestClock`.
+/// A test timer for user with a `TestClock`.
 #[derive(Clone, Copy, Debug)]
 pub struct TestTimer {
     pub name: Ustr,
     pub interval_ns: NonZeroU64,
     pub start_time_ns: UnixNanos,
     pub stop_time_ns: Option<UnixNanos>,
     next_time_ns: UnixNanos,
     is_expired: bool,
 }
 
 impl TestTimer {
-    /// Creates a new `TestTimer`.
+    /// Creates a new [`TestTimer`] instance.
     pub fn new(
         name: &str,
         interval_ns: u64,
         start_time_ns: UnixNanos,
         stop_time_ns: Option<UnixNanos>,
     ) -> anyhow::Result<Self> {
         check_valid_string(name, stringify!(name))?;
@@ -216,28 +218,28 @@
             self.next_time_ns += self.interval_ns;
 
             Some(item)
         }
     }
 }
 
-/// Provides a live timer for use with a `LiveClock`.
+/// A live timer for use with a `LiveClock`.
 pub struct LiveTimer {
     pub name: Ustr,
     pub interval_ns: NonZeroU64,
     pub start_time_ns: UnixNanos,
     pub stop_time_ns: Option<UnixNanos>,
     next_time_ns: Arc<AtomicU64>,
     is_expired: Arc<AtomicBool>,
     callback: EventHandler,
     canceler: Option<oneshot::Sender<()>>,
 }
 
 impl LiveTimer {
-    /// Creates a new `LiveTimer`.
+    /// Creates a new [`LiveTimer`] instance.
     pub fn new(
         name: &str,
         interval_ns: u64,
         start_time_ns: UnixNanos,
         stop_time_ns: Option<UnixNanos>,
         callback: EventHandler,
     ) -> anyhow::Result<Self> {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/common/src/xrate.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/xrate.rs`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 // -------------------------------------------------------------------------------------------------
 
 // ****************************************************************************
 // The design of exchange rate calculations needs to be revisited,
 // as its not efficient to be allocating so many structures and doing so many recalculations"
 // ****************************************************************************
 
-//! Provides exchange rate calculations between currencies.
+//! Exchange rate calculations between currencies.
 //!
 //! An exchange rate is the value of one asset versus that of another.
 use std::collections::{HashMap, HashSet};
 
 use itertools::Itertools;
 use nautilus_core::correctness::{check_equal_usize, check_map_not_empty};
 use nautilus_model::{enums::PriceType, identifiers::symbol::Symbol, types::currency::Currency};
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/Cargo.toml` & `nautilus_trader-1.194.0/nautilus_core/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/build.rs` & `nautilus_trader-1.194.0/nautilus_core/core/build.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/cbindgen.toml` & `nautilus_trader-1.194.0/nautilus_core/core/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/cbindgen_cython.toml` & `nautilus_trader-1.194.0/nautilus_core/core/cbindgen_cython.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/correctness.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/correctness.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides static condition checks similar to the *design by contract* philosophy
+//! Functions for static condition checks similar to the *design by contract* philosophy
 //! to help ensure logical correctness.
 //!
 //! This module provides validation checking of function or method conditions.
 //!
 //! A condition is a predicate which must be true just prior to the execution of
 //! some section of code - for correct behavior as per the design specification.
 //!
@@ -159,18 +159,20 @@
         anyhow::bail!("{FAILED} invalid i64 for '{param}' not in range [{l}, {r}], was {value}")
     }
     Ok(())
 }
 
 /// Checks the `f64` value is in range [`l`, `r`] (inclusive).
 pub fn check_in_range_inclusive_f64(value: f64, l: f64, r: f64, param: &str) -> anyhow::Result<()> {
+    const EPSILON: f64 = 1e-15; // Epsilon to account for floating-point precision issues
+
     if value.is_nan() || value.is_infinite() {
         anyhow::bail!("{FAILED} invalid f64 for '{param}', was {value}")
     }
-    if value < l || value > r {
+    if value < l - EPSILON || value > r + EPSILON {
         anyhow::bail!("{FAILED} invalid f64 for '{param}' not in range [{l}, {r}], was {value}")
     }
     Ok(())
 }
 
 /// Checks the `usize` value is in range [`l`, `r`] (inclusive).
 pub fn check_in_range_inclusive_usize(
@@ -192,15 +194,15 @@
             "{FAILED} the '{param}' slice `&[{}]` was not empty",
             std::any::type_name::<T>()
         )
     }
     Ok(())
 }
 
-/// Checks the slice is *not* empty.
+/// Checks the slice is **not** empty.
 pub fn check_slice_not_empty<T>(slice: &[T], param: &str) -> anyhow::Result<()> {
     if slice.is_empty() {
         anyhow::bail!(
             "{FAILED} the '{param}' slice `&[{}]` was empty",
             std::any::type_name::<T>()
         )
     }
@@ -215,15 +217,15 @@
             std::any::type_name::<K>(),
             std::any::type_name::<V>(),
         )
     }
     Ok(())
 }
 
-/// Checks the map is *not* empty.
+/// Checks the map is **not** empty.
 pub fn check_map_not_empty<K, V>(map: &HashMap<K, V>, param: &str) -> anyhow::Result<()> {
     if map.is_empty() {
         anyhow::bail!(
             "{FAILED} the '{param}' map `&<{}, {}>` was empty",
             std::any::type_name::<K>(),
             std::any::type_name::<V>(),
         )
@@ -475,14 +477,39 @@
         #[case] r: i64,
         #[case] param: &str,
     ) {
         assert!(check_in_range_inclusive_i64(value, l, r, param).is_ok());
     }
 
     #[rstest]
+    #[case(0.0, 0.0, 0.0, "value")]
+    #[case(0.0, 0.0, 1.0, "value")]
+    #[case(1.0, 0.0, 1.0, "value")]
+    fn test_check_in_range_inclusive_f64_when_in_range(
+        #[case] value: f64,
+        #[case] l: f64,
+        #[case] r: f64,
+        #[case] param: &str,
+    ) {
+        assert!(check_in_range_inclusive_f64(value, l, r, param).is_ok());
+    }
+
+    #[rstest]
+    #[case(-1e16, 0.0, 0.0, "value")]
+    #[case(1.0 + 1e16, 0.0, 1.0, "value")]
+    fn test_check_in_range_inclusive_f64_when_out_of_range(
+        #[case] value: f64,
+        #[case] l: f64,
+        #[case] r: f64,
+        #[case] param: &str,
+    ) {
+        assert!(check_in_range_inclusive_f64(value, l, r, param).is_err());
+    }
+
+    #[rstest]
     #[case(0, 1, 2, "value")]
     #[case(3, 1, 2, "value")]
     fn test_check_in_range_inclusive_i64_when_out_of_range(
         #[case] value: i64,
         #[case] l: i64,
         #[case] r: i64,
         #[case] param: &str,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/datetime.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/datetime.rs`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides common data and time functions.
+//! Common data and time functions.
 
 use std::time::{Duration, UNIX_EPOCH};
 
 use chrono::{
     prelude::{DateTime, Utc},
     Datelike, NaiveDate, SecondsFormat, TimeDelta, Weekday,
 };
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/deserialization.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/parsing.rs`

 * *Files 26% similar despite different names*

```diff
@@ -9,83 +9,92 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-use std::fmt;
+//! Core parsing functions.
 
-use serde::{
-    de::{Unexpected, Visitor},
-    Deserializer,
-};
-
-struct BoolVisitor;
-
-impl<'de> Visitor<'de> for BoolVisitor {
-    type Value = u8;
-
-    fn expecting(&self, formatter: &mut fmt::Formatter) -> fmt::Result {
-        formatter.write_str("a boolean as u8")
-    }
-
-    fn visit_bool<E>(self, value: bool) -> Result<Self::Value, E>
-    where
-        E: serde::de::Error,
-    {
-        Ok(u8::from(value))
-    }
-
-    fn visit_u64<E>(self, value: u64) -> Result<Self::Value, E>
-    where
-        E: serde::de::Error,
-    {
-        if value > u64::from(u8::MAX) {
-            Err(E::invalid_value(Unexpected::Unsigned(value), &self))
-        } else {
-            Ok(value as u8)
-        }
+/// Returns the decimal precision inferred from the given string.
+#[must_use]
+pub fn precision_from_str(s: &str) -> u8 {
+    let lower_s = s.to_lowercase();
+    // Handle scientific notation
+    if lower_s.contains("e-") {
+        return lower_s.split("e-").last().unwrap().parse::<u8>().unwrap();
     }
+    if !lower_s.contains('.') {
+        return 0;
+    }
+    return lower_s.split('.').last().unwrap().len() as u8;
 }
 
-pub fn from_bool_as_u8<'de, D>(deserializer: D) -> Result<u8, D::Error>
-where
-    D: Deserializer<'de>,
-{
-    deserializer.deserialize_any(BoolVisitor)
+/// Returns a `usize` from the given bytes.
+pub fn bytes_to_usize(bytes: &[u8]) -> anyhow::Result<usize> {
+    // Check bytes width
+    if bytes.len() >= std::mem::size_of::<usize>() {
+        let mut buffer = [0u8; std::mem::size_of::<usize>()];
+        buffer.copy_from_slice(&bytes[..std::mem::size_of::<usize>()]);
+
+        Ok(usize::from_le_bytes(buffer))
+    } else {
+        Err(anyhow::anyhow!("Not enough bytes to represent a `usize`"))
+    }
 }
 
+////////////////////////////////////////////////////////////////////////////////
+// Tests
+////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
 mod tests {
-    use serde::Deserialize;
-
-    use super::from_bool_as_u8;
-
-    #[derive(Deserialize)]
-    pub struct TestStruct {
-        #[serde(deserialize_with = "from_bool_as_u8")]
-        pub value: u8,
-    }
-
-    #[test]
-    fn test_deserialize_bool_as_u8_with_boolean() {
-        let json_true = r#"{"value": true}"#;
-        let test_struct: TestStruct = serde_json::from_str(json_true).unwrap();
-        assert_eq!(test_struct.value, 1);
-
-        let json_false = r#"{"value": false}"#;
-        let test_struct: TestStruct = serde_json::from_str(json_false).unwrap();
-        assert_eq!(test_struct.value, 0);
-    }
+    use rstest::rstest;
 
-    #[test]
-    fn test_deserialize_bool_as_u8_with_u64() {
-        let json_true = r#"{"value": 1}"#;
-        let test_struct: TestStruct = serde_json::from_str(json_true).unwrap();
-        assert_eq!(test_struct.value, 1);
+    use super::*;
 
-        let json_false = r#"{"value": 0}"#;
-        let test_struct: TestStruct = serde_json::from_str(json_false).unwrap();
-        assert_eq!(test_struct.value, 0);
+    #[rstest]
+    #[case("", 0)]
+    #[case("0", 0)]
+    #[case("1.0", 1)]
+    #[case("1.00", 2)]
+    #[case("1.23456789", 8)]
+    #[case("123456.789101112", 9)]
+    #[case("0.000000001", 9)]
+    #[case("1e-1", 1)]
+    #[case("1e-2", 2)]
+    #[case("1e-3", 3)]
+    #[case("1e8", 0)]
+    fn test_precision_from_str(#[case] s: &str, #[case] expected: u8) {
+        let result = precision_from_str(s);
+        assert_eq!(result, expected);
+    }
+
+    #[rstest]
+    fn test_bytes_to_usize_empty() {
+        let payload: Vec<u8> = vec![];
+        let result = bytes_to_usize(&payload);
+        assert!(result.is_err());
+        assert_eq!(
+            result.err().unwrap().to_string(),
+            "Not enough bytes to represent a `usize`"
+        );
+    }
+
+    #[rstest]
+    fn test_bytes_to_usize_invalid() {
+        let payload: Vec<u8> = vec![0x01, 0x02, 0x03];
+        let result = bytes_to_usize(&payload);
+        assert!(result.is_err());
+        assert_eq!(
+            result.err().unwrap().to_string(),
+            "Not enough bytes to represent a `usize`"
+        );
+    }
+
+    #[rstest]
+    fn test_bytes_to_usize_valid() {
+        let payload: Vec<u8> = vec![0x01, 0x02, 0x03, 0x04, 0x05, 0x06, 0x07, 0x08];
+        let result = bytes_to_usize(&payload).unwrap();
+        assert_eq!(result, 0x0807_0605_0403_0201);
+        assert_eq!(result, 578_437_695_752_307_201);
     }
 }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/equality.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/equality.rs`

 * *Files 14% similar despite different names*

```diff
@@ -9,16 +9,21 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Functions to evaluation total equality of two instances.
+
 use pretty_assertions::assert_eq;
 use serde::Serialize;
 
+/// Return whether `a` and `b` are entirely equal (all fields).
+///
+/// Serializes the input values to JSON and compares the resulting strings.
 pub fn entirely_equal<T: Serialize>(a: T, b: T) {
     let a_serialized = serde_json::to_string(&a).unwrap();
     let b_serialized = serde_json::to_string(&b).unwrap();
 
     assert_eq!(a_serialized, b_serialized);
 }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/ffi/cvec.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/ffi/cvec.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/ffi/datetime.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/ffi/datetime.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/ffi/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides a C foreign function interface (FFI) from `cbindgen`.
+//! C foreign function interface (FFI) from `cbindgen`.
 
-pub mod cvec;
-pub mod datetime;
-pub mod parsing;
-pub mod string;
-pub mod uuid;
+pub mod data;
+pub mod enums;
+pub mod events;
+pub mod identifiers;
+pub mod instruments;
+pub mod orderbook;
+pub mod types;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/ffi/parsing.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/ffi/parsing.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/ffi/string.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/ffi/string.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/ffi/uuid.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/ffi/uuid.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/lib.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 //! for the main `nautilus_trader` Python package, or as part of a Rust only build.
 //!
 //! - `ffi`: Enables the C foreign function interface (FFI) from `cbindgen`
 //! - `python`: Enables Python bindings from `pyo3`
 
 pub mod correctness;
 pub mod datetime;
-pub mod deserialization;
 pub mod equality;
 pub mod message;
 pub mod nanos;
 pub mod parsing;
 pub mod serialization;
 pub mod time;
 pub mod uuid;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/message.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/message.rs`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines common message types.
+//! Common message types.
 
 use crate::{nanos::UnixNanos, uuid::UUID4};
 
 #[derive(Debug, Clone)]
 pub enum Message {
     Command {
         id: UUID4,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/nanos.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/nanos.rs`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines `UnixNanos` type for working with UNIX epoch (nanoseconds).
+//! A `UnixNanos` type for working with UNIX epoch (nanoseconds).
 
 use std::{
     cmp::Ordering,
     fmt::Display,
     ops::{Add, AddAssign, Deref, Sub, SubAssign},
     str::FromStr,
 };
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/python/casing.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/python/casing.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/python/datetime.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/python/datetime.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/python/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/python/serialization.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/python/serialization.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/python/uuid.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/python/uuid.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/serialization.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/macros.rs`

 * *Files 26% similar despite different names*

```diff
@@ -9,33 +9,32 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines common serialization traits.
+//! Model specific macros.
 
-use serde::{Deserialize, Serialize};
-
-/// Represents types which are serializable for JSON and `MsgPack` specifications.
-pub trait Serializable: Serialize + for<'de> Deserialize<'de> {
-    /// Deserialize an object from JSON encoded bytes.
-    fn from_json_bytes(data: Vec<u8>) -> Result<Self, serde_json::Error> {
-        serde_json::from_slice(&data)
-    }
-
-    /// Deserialize an object from `MsgPack` encoded bytes.
-    fn from_msgpack_bytes(data: Vec<u8>) -> Result<Self, rmp_serde::decode::Error> {
-        rmp_serde::from_slice(&data)
-    }
-
-    /// Serialize an object to JSON encoded bytes.
-    fn as_json_bytes(&self) -> Result<Vec<u8>, serde_json::Error> {
-        serde_json::to_vec(self)
-    }
-
-    /// Serialize an object to `MsgPack` encoded bytes.
-    fn as_msgpack_bytes(&self) -> Result<Vec<u8>, rmp_serde::encode::Error> {
-        rmp_serde::to_vec_named(self)
-    }
+#[macro_export]
+macro_rules! enum_strum_serde {
+    ($type:ty) => {
+        impl Serialize for $type {
+            fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
+            where
+                S: Serializer,
+            {
+                serializer.serialize_str(&self.to_string())
+            }
+        }
+
+        impl<'de> Deserialize<'de> for $type {
+            fn deserialize<D>(deserializer: D) -> Result<Self, D::Error>
+            where
+                D: Deserializer<'de>,
+            {
+                let s = String::deserialize(deserializer)?;
+                <$type>::from_str(&s).map_err(serde::de::Error::custom)
+            }
+        }
+    };
 }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/time.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/time.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides the core `AtomicTime` real-time and static clocks.
+//! The core `AtomicTime` real-time and static clocks.
 
 use std::{
     ops::Deref,
     sync::{
         atomic::{AtomicBool, AtomicU64, Ordering},
         OnceLock,
     },
@@ -25,18 +25,18 @@
 };
 
 use crate::{
     datetime::{NANOSECONDS_IN_MICROSECOND, NANOSECONDS_IN_MILLISECOND, NANOSECONDS_IN_SECOND},
     nanos::UnixNanos,
 };
 
-/// Provides a global atomic time in real-time mode for use across the system.
+/// Global atomic time in real-time mode for use across the system.
 pub static ATOMIC_CLOCK_REALTIME: OnceLock<AtomicTime> = OnceLock::new();
 
-/// Provides a global atomic time in static mode for use across the system.
+/// Global atomic time in static mode for use across the system.
 pub static ATOMIC_CLOCK_STATIC: OnceLock<AtomicTime> = OnceLock::new();
 
 /// Returns a static reference to the global atomic clock in real-time mode.
 pub fn get_atomic_clock_realtime() -> &'static AtomicTime {
     ATOMIC_CLOCK_REALTIME.get_or_init(AtomicTime::default)
 }
 
@@ -81,21 +81,25 @@
 
     fn deref(&self) -> &Self::Target {
         &self.timestamp_ns
     }
 }
 
 impl Default for AtomicTime {
+    /// Creates a new default [`AtomicTime`] instance.
     fn default() -> Self {
         Self::new(true, UnixNanos::default())
     }
 }
 
 impl AtomicTime {
-    /// New atomic clock set with the given UNIX time (nanoseconds).
+    /// Creates a new [`AtomicTime`] instance.
+    ///
+    /// The `realtime` flag will determine whether the atomic time is based off system time.
+    /// The time will be set to the given UNIX `time` (nanoseconds).
     #[must_use]
     pub fn new(realtime: bool, time: UnixNanos) -> Self {
         Self {
             realtime: AtomicBool::new(realtime),
             timestamp_ns: AtomicU64::new(time.into()),
         }
     }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/core/src/uuid.rs` & `nautilus_trader-1.194.0/nautilus_core/core/src/uuid.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! A core `UUID4` universally unique identifier (UUID) version 4 based on a 128-bit
+//! A `UUID4` universally unique identifier (UUID) version 4 based on a 128-bit
 //! label (RFC 4122).
 
 use std::{
     ffi::{CStr, CString},
     fmt::{Debug, Display, Formatter},
     hash::Hash,
     str::FromStr,
@@ -39,15 +39,15 @@
 )]
 pub struct UUID4 {
     /// The UUID v4 value as a fixed-length C string byte array (includes null terminator).
     pub(crate) value: [u8; 37], // cbindgen issue using the constant in the array
 }
 
 impl UUID4 {
-    /// Creates a new `UUID4`.
+    /// Creates a new [`UUID4`] instance.
     #[must_use]
     pub fn new() -> Self {
         let uuid = Uuid::new_v4();
         let c_string = CString::new(uuid.to_string()).expect("`CString` conversion failed");
         let bytes = c_string.as_bytes_with_nul();
         let mut value = [0; UUID4_LEN];
         value[..bytes.len()].copy_from_slice(bytes);
@@ -80,14 +80,15 @@
 impl From<&str> for UUID4 {
     fn from(input: &str) -> Self {
         input.parse().unwrap_or_else(|err| panic!("{}", err))
     }
 }
 
 impl Default for UUID4 {
+    /// Creates a new default [`UUID4`] instance.
     fn default() -> Self {
         Self::new()
     }
 }
 
 impl Debug for UUID4 {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/execution/Cargo.toml` & `nautilus_trader-1.194.0/nautilus_core/execution/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/execution/src/client.rs` & `nautilus_trader-1.194.0/nautilus_core/execution/src/client.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides execution client base functionality.
+//! Base execution client functionality.
 
 // Under development
 #![allow(dead_code)]
 #![allow(unused_variables)]
 
 use nautilus_common::cache::Cache;
 use nautilus_core::nanos::UnixNanos;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/execution/src/engine.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/accepted.rs`

 * *Files 21% similar despite different names*

```diff
@@ -9,280 +9,303 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides a generic `ExecutionEngine` for backtesting and live environments.
+use std::fmt::{Debug, Display};
 
-// Under development
-#![allow(dead_code)]
-#![allow(unused_variables)]
-
-use std::collections::{HashMap, HashSet};
-
-use log::debug;
-use nautilus_common::{cache::Cache, generators::position_id::PositionIdGenerator};
-use nautilus_model::{
-    enums::{OmsType, OrderSide},
-    events::order::{event::OrderEventAny, filled::OrderFilled},
-    identifiers::{
-        client_id::ClientId, instrument_id::InstrumentId, strategy_id::StrategyId, venue::Venue,
-    },
-    instruments::any::InstrumentAny,
-    orders::any::OrderAny,
-    position::Position,
-    types::quantity::Quantity,
-};
+use derive_builder::Builder;
+use nautilus_core::{nanos::UnixNanos, serialization::from_bool_as_u8, uuid::UUID4};
+use serde::{Deserialize, Serialize};
+use ustr::Ustr;
 
 use crate::{
-    client::ExecutionClient,
-    messages::{
-        cancel::CancelOrder, cancel_all::CancelAllOrders, cancel_batch::BatchCancelOrders,
-        modify::ModifyOrder, query::QueryOrder, submit::SubmitOrder, submit_list::SubmitOrderList,
-        TradingCommand,
+    enums::{
+        ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
+        TriggerType,
+    },
+    events::order::OrderEvent,
+    identifiers::{
+        account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
+        instrument_id::InstrumentId, order_list_id::OrderListId, position_id::PositionId,
+        strategy_id::StrategyId, trade_id::TradeId, trader_id::TraderId,
+        venue_order_id::VenueOrderId,
     },
+    types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
-pub struct ExecutionEngineConfig {
-    pub debug: bool,
+#[repr(C)]
+#[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
+#[builder(default)]
+#[serde(tag = "type")]
+#[cfg_attr(
+    feature = "python",
+    pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
+)]
+pub struct OrderAccepted {
+    pub trader_id: TraderId,
+    pub strategy_id: StrategyId,
+    pub instrument_id: InstrumentId,
+    pub client_order_id: ClientOrderId,
+    pub venue_order_id: VenueOrderId,
+    pub account_id: AccountId,
+    pub event_id: UUID4,
+    pub ts_event: UnixNanos,
+    pub ts_init: UnixNanos,
+    #[serde(deserialize_with = "from_bool_as_u8")]
+    pub reconciliation: u8, // TODO: Change to bool once Cython removed
 }
 
-pub struct ExecutionEngine {
-    pub command_count: u64,
-    pub event_count: u64,
-    pub report_count: u64,
-    cache: &'static Cache,
-    default_client: Option<ExecutionClient>,
-    pos_id_generator: PositionIdGenerator,
-    clients: HashMap<ClientId, ExecutionClient>,
-    routing_map: HashMap<Venue, ClientId>,
-    oms_overrides: HashMap<StrategyId, OmsType>,
-    external_order_claims: HashMap<InstrumentId, StrategyId>,
-    config: ExecutionEngineConfig,
+impl OrderAccepted {
+    /// Creates a new [`OrderAccepted`] instance.
+    #[allow(clippy::too_many_arguments)]
+    pub fn new(
+        trader_id: TraderId,
+        strategy_id: StrategyId,
+        instrument_id: InstrumentId,
+        client_order_id: ClientOrderId,
+        venue_order_id: VenueOrderId,
+        account_id: AccountId,
+        event_id: UUID4,
+        ts_event: UnixNanos,
+        ts_init: UnixNanos,
+        reconciliation: bool,
+    ) -> anyhow::Result<Self> {
+        Ok(Self {
+            trader_id,
+            strategy_id,
+            instrument_id,
+            client_order_id,
+            venue_order_id,
+            account_id,
+            event_id,
+            ts_event,
+            ts_init,
+            reconciliation: u8::from(reconciliation),
+        })
+    }
 }
 
-impl ExecutionEngine {
-    #[must_use]
-    pub fn position_id_count(&self, strategy_id: StrategyId) -> u64 {
-        todo!();
+impl Debug for OrderAccepted {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        write!(f,
+            "{}(trader_id={}, strategy_id={}, instrument_id={}, client_order_id={}, venue_order_id={}, account_id={}, event_id={}, ts_event={}, ts_init={})",
+            stringify!(OrderAccepted),
+            self.trader_id,
+            self.strategy_id,
+            self.instrument_id,
+            self.client_order_id,
+            self.venue_order_id,
+            self.account_id,
+            self.event_id,
+            self.ts_event,
+            self.ts_init
+        )
     }
+}
 
-    #[must_use]
-    pub fn check_integrity(&self) -> bool {
-        todo!();
+impl Display for OrderAccepted {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        write!(
+            f,
+            "{}(instrument_id={}, client_order_id={}, venue_order_id={}, account_id={}, ts_event={})",
+            stringify!(OrderAccepted),
+            self.instrument_id,
+            self.client_order_id,
+            self.venue_order_id,
+            self.account_id,
+            self.ts_event
+        )
     }
+}
 
-    #[must_use]
-    pub fn check_connected(&self) -> bool {
-        todo!();
+impl OrderEvent for OrderAccepted {
+    fn id(&self) -> UUID4 {
+        self.event_id
     }
 
-    #[must_use]
-    pub fn check_disconnected(&self) -> bool {
-        todo!();
+    fn kind(&self) -> &str {
+        stringify!(OrderAccepted)
     }
 
-    #[must_use]
-    pub fn check_residuals(&self) -> bool {
-        todo!();
+    fn order_type(&self) -> Option<OrderType> {
+        None
     }
 
-    #[must_use]
-    pub fn get_external_order_claims_instruments(&self) -> HashSet<InstrumentId> {
-        todo!();
+    fn order_side(&self) -> Option<OrderSide> {
+        None
     }
 
-    // -- REGISTRATION --------------------------------------------------------
-
-    pub fn register_client(&mut self, client: ExecutionClient) -> anyhow::Result<()> {
-        todo!();
+    fn trader_id(&self) -> TraderId {
+        self.trader_id
     }
 
-    pub fn register_default_client(&mut self, client: ExecutionClient) -> anyhow::Result<()> {
-        todo!();
+    fn strategy_id(&self) -> StrategyId {
+        self.strategy_id
     }
 
-    pub fn register_venue_routing(
-        &mut self,
-        client_id: ClientId,
-        venue: Venue,
-    ) -> anyhow::Result<()> {
-        todo!();
+    fn instrument_id(&self) -> InstrumentId {
+        self.instrument_id
     }
 
-    // TODO: Implement `Strategy`
-    // pub fn register_external_order_claims(&mut self, strategy: Strategy) -> anyhow::Result<()> {
-    //     todo!();
-    // }
-
-    pub fn deregister_client(&mut self, client_id: ClientId) -> anyhow::Result<()> {
-        todo!();
+    fn trade_id(&self) -> Option<TradeId> {
+        None
     }
 
-    // -- COMMANDS ------------------------------------------------------------
+    fn currency(&self) -> Option<Currency> {
+        None
+    }
 
-    pub fn load_cache(&self) {
-        todo!();
+    fn client_order_id(&self) -> ClientOrderId {
+        self.client_order_id
     }
 
-    pub fn flush_db(&self) {
-        todo!();
+    fn reason(&self) -> Option<Ustr> {
+        None
     }
 
-    pub fn execute(&mut self, command: TradingCommand) {
-        self.execute_command(command);
+    fn quantity(&self) -> Option<Quantity> {
+        None
     }
 
-    pub fn process(&self, event: &OrderEventAny) {
-        todo!();
+    fn time_in_force(&self) -> Option<TimeInForce> {
+        None
     }
 
-    // -- COMMAND HANDLERS ----------------------------------------------------
+    fn liquidity_side(&self) -> Option<LiquiditySide> {
+        None
+    }
 
-    fn execute_command(&mut self, command: TradingCommand) {
-        debug!("<--[CMD] {:?}", command); // TODO: Log constants
-        self.command_count += 1;
+    fn post_only(&self) -> Option<bool> {
+        None
+    }
 
-        // TODO: Refine getting the client (no need for two expects)
-        let client = if let Some(client) = self.clients.get(&command.client_id()) {
-            client
-        } else if let Some(client_id) = self.routing_map.get(&command.instrument_id().venue) {
-            if let Some(client) = self.clients.get(client_id) {
-                client
-            } else {
-                self.default_client.as_ref().expect("No client found")
-            }
-        } else {
-            self.default_client.as_ref().expect("No client found")
-        };
+    fn reduce_only(&self) -> Option<bool> {
+        None
+    }
 
-        match command {
-            TradingCommand::SubmitOrder(cmd) => self.handle_submit_order(client, cmd),
-            TradingCommand::SubmitOrderList(cmd) => self.handle_submit_order_list(client, cmd),
-            TradingCommand::ModifyOrder(cmd) => self.handle_modify_order(client, cmd),
-            TradingCommand::CancelOrder(cmd) => self.handle_cancel_order(client, cmd),
-            TradingCommand::CancelAllOrders(cmd) => self.handle_cancel_all_orders(client, cmd),
-            TradingCommand::BatchCancelOrders(cmd) => self.handle_batch_cancel_orders(client, cmd),
-            TradingCommand::QueryOrder(cmd) => self.handle_query_order(client, cmd),
-        }
+    fn quote_quantity(&self) -> Option<bool> {
+        None
     }
 
-    fn handle_submit_order(&self, client: &ExecutionClient, command: SubmitOrder) {
-        todo!();
+    fn reconciliation(&self) -> bool {
+        false
     }
 
-    fn handle_submit_order_list(&self, client: &ExecutionClient, command: SubmitOrderList) {
-        todo!();
+    fn price(&self) -> Option<Price> {
+        None
     }
 
-    fn handle_modify_order(&self, client: &ExecutionClient, command: ModifyOrder) {
-        todo!();
+    fn last_px(&self) -> Option<Price> {
+        None
     }
 
-    fn handle_cancel_order(&self, client: &ExecutionClient, command: CancelOrder) {
-        todo!();
+    fn last_qty(&self) -> Option<Quantity> {
+        None
     }
 
-    fn handle_cancel_all_orders(&self, client: &ExecutionClient, command: CancelAllOrders) {
-        todo!();
+    fn trigger_price(&self) -> Option<Price> {
+        None
     }
 
-    fn handle_batch_cancel_orders(&self, client: &ExecutionClient, command: BatchCancelOrders) {
-        todo!();
+    fn trigger_type(&self) -> Option<TriggerType> {
+        None
     }
 
-    fn handle_query_order(&self, client: &ExecutionClient, command: QueryOrder) {
-        todo!();
+    fn limit_offset(&self) -> Option<Price> {
+        None
     }
 
-    // -- EVENT HANDLERS ----------------------------------------------------
+    fn trailing_offset(&self) -> Option<Price> {
+        None
+    }
 
-    fn handle_event(&self, event: OrderEventAny) {
-        todo!();
+    fn trailing_offset_type(&self) -> Option<TrailingOffsetType> {
+        None
     }
 
-    fn determine_oms_type(&self, fill: OrderFilled) {
-        todo!();
+    fn expire_time(&self) -> Option<UnixNanos> {
+        None
     }
 
-    fn determine_position_id(&self, fill: OrderFilled, oms_type: OmsType) {
-        todo!();
+    fn display_qty(&self) -> Option<Quantity> {
+        None
     }
 
-    fn determine_hedging_position_id(&self, fill: OrderFilled) {
-        todo!();
+    fn emulation_trigger(&self) -> Option<TriggerType> {
+        None
     }
 
-    fn determine_netting_position_id(&self, fill: OrderFilled) {
-        todo!();
+    fn trigger_instrument_id(&self) -> Option<InstrumentId> {
+        None
     }
 
-    fn apply_event_to_order(&self, order: &OrderAny, event: OrderEventAny) {
-        todo!();
+    fn contingency_type(&self) -> Option<ContingencyType> {
+        None
     }
 
-    fn handle_order_fill(&self, order: &OrderAny, fill: OrderFilled, oms_type: OmsType) {
-        todo!();
+    fn order_list_id(&self) -> Option<OrderListId> {
+        None
     }
 
-    fn open_position(
-        &self,
-        instrument: InstrumentAny,
-        position: &Position,
-        fill: OrderFilled,
-        oms_type: OmsType,
-    ) {
-        todo!();
+    fn linked_order_ids(&self) -> Option<Vec<ClientOrderId>> {
+        None
     }
 
-    fn update_position(
-        &self,
-        instrument: InstrumentAny,
-        position: &Position,
-        fill: OrderFilled,
-        oms_type: OmsType,
-    ) {
-        todo!();
+    fn parent_order_id(&self) -> Option<ClientOrderId> {
+        None
     }
 
-    fn will_flip_position(&self, position: &Position, fill: OrderFilled) {
-        todo!();
+    fn exec_algorithm_id(&self) -> Option<ExecAlgorithmId> {
+        None
     }
 
-    fn flip_position(
-        &self,
-        instrument: InstrumentAny,
-        position: &Position,
-        fill: OrderFilled,
-        oms_type: OmsType,
-    ) {
-        todo!();
+    fn exec_spawn_id(&self) -> Option<ClientOrderId> {
+        None
     }
 
-    fn publish_order_snapshot(&self, order: &OrderAny) {
-        todo!();
+    fn venue_order_id(&self) -> Option<VenueOrderId> {
+        Some(self.venue_order_id)
     }
 
-    fn publish_position_snapshot(&self, position: &Position) {
-        todo!();
+    fn account_id(&self) -> Option<AccountId> {
+        Some(self.account_id)
     }
 
-    // -- INTERNAL ------------------------------------------------------------
+    fn position_id(&self) -> Option<PositionId> {
+        None
+    }
 
-    fn set_position_id_counts(&self) {
-        todo!();
+    fn commission(&self) -> Option<Money> {
+        None
     }
 
-    fn last_px_for_conversion(&self, instrument_id: InstrumentId, side: OrderSide) {
-        todo!();
+    fn ts_event(&self) -> UnixNanos {
+        self.ts_event
     }
 
-    fn set_order_base_qty(&self, order: &OrderAny, base_qty: Quantity) {
-        todo!();
+    fn ts_init(&self) -> UnixNanos {
+        self.ts_init
     }
+}
 
-    fn deny_order(&self, order: &OrderAny, reason: &str) {
-        todo!();
+////////////////////////////////////////////////////////////////////////////////
+// Tests
+////////////////////////////////////////////////////////////////////////////////
+#[cfg(test)]
+mod tests {
+    use rstest::rstest;
+
+    use super::*;
+    use crate::events::order::stubs::*;
+
+    #[rstest]
+    fn test_order_accepted_display(order_accepted: OrderAccepted) {
+        let display = format!("{order_accepted}");
+        assert_eq!(
+            display,
+            "OrderAccepted(instrument_id=BTCUSDT.COINBASE, client_order_id=O-19700101-0000-000-001-1, venue_order_id=001, account_id=SIM-001, ts_event=0)"
+        );
     }
 }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/execution/src/lib.rs` & `nautilus_trader-1.194.0/nautilus_core/execution/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/execution/src/matching_core.rs` & `nautilus_trader-1.194.0/nautilus_core/execution/src/matching_core.rs`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         base::OrderError,
         market::MarketOrder,
     },
     polymorphism::{GetClientOrderId, GetLimitPrice, GetOrderSideSpecified, GetStopPrice},
     types::price::Price,
 };
 
-/// Provides a generic order matching core.
+/// A generic order matching core.
 pub struct OrderMatchingCore {
     /// The instrument ID for the matching core.
     pub instrument_id: InstrumentId,
     /// The price increment for the matching core.
     pub price_increment: Price,
     /// The current bid price for the matching core.
     pub bid: Option<Price>,
@@ -47,14 +47,15 @@
     orders_ask: Vec<PassiveOrderAny>,
     trigger_stop_order: Option<fn(StopOrderAny)>,
     fill_market_order: Option<fn(MarketOrder)>,
     fill_limit_order: Option<fn(LimitOrderAny)>,
 }
 
 impl OrderMatchingCore {
+    // Creates a new [`OrderMatchingCore`] instance.
     #[must_use]
     pub fn new(
         instrument_id: InstrumentId,
         price_increment: Price,
         trigger_stop_order: Option<fn(StopOrderAny)>,
         fill_market_order: Option<fn(MarketOrder)>,
         fill_limit_order: Option<fn(LimitOrderAny)>,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/execution/src/messages/cancel.rs` & `nautilus_trader-1.194.0/nautilus_core/execution/src/messages/cancel.rs`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     pub client_order_id: ClientOrderId,
     pub venue_order_id: VenueOrderId,
     pub command_id: UUID4,
     pub ts_init: UnixNanos,
 }
 
 impl CancelOrder {
+    /// Creates a new [`CancelOrder`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         client_id: ClientId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/execution/src/messages/cancel_all.rs` & `nautilus_trader-1.194.0/nautilus_core/execution/src/messages/cancel_all.rs`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     pub instrument_id: InstrumentId,
     pub order_side: OrderSide,
     pub command_id: UUID4,
     pub ts_init: UnixNanos,
 }
 
 impl CancelAllOrders {
+    /// Creates a new [`CancelAllOrders`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         client_id: ClientId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         order_side: OrderSide,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/execution/src/messages/cancel_batch.rs` & `nautilus_trader-1.194.0/nautilus_core/execution/src/messages/cancel_batch.rs`

 * *Files 9% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     pub instrument_id: InstrumentId,
     pub cancels: Vec<CancelOrder>,
     pub command_id: UUID4,
     pub ts_init: UnixNanos,
 }
 
 impl BatchCancelOrders {
+    /// Creates a new [`BatchCancelOrders`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         client_id: ClientId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         cancels: Vec<CancelOrder>,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/execution/src/messages/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/execution/src/messages/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines execution specific messages such as order commands.
+//! Execution specific messages such as order commands.
 
 use nautilus_model::identifiers::{client_id::ClientId, instrument_id::InstrumentId};
 use strum::Display;
 
 use self::{
     cancel::CancelOrder, cancel_all::CancelAllOrders, cancel_batch::BatchCancelOrders,
     modify::ModifyOrder, query::QueryOrder, submit::SubmitOrder, submit_list::SubmitOrderList,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/execution/src/messages/modify.rs` & `nautilus_trader-1.194.0/nautilus_core/execution/src/messages/modify.rs`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     pub price: Option<Price>,
     pub trigger_price: Option<Price>,
     pub command_id: UUID4,
     pub ts_init: UnixNanos,
 }
 
 impl ModifyOrder {
+    /// Creates a new [`ModifyOrder`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         client_id: ClientId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/execution/src/messages/query.rs` & `nautilus_trader-1.194.0/nautilus_core/execution/src/messages/query.rs`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     pub client_order_id: ClientOrderId,
     pub venue_order_id: VenueOrderId,
     pub command_id: UUID4,
     pub ts_init: UnixNanos,
 }
 
 impl QueryOrder {
+    /// Creates a new [`QueryOrder`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         client_id: ClientId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/execution/src/messages/submit.rs` & `nautilus_trader-1.194.0/nautilus_core/execution/src/messages/submit.rs`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     pub exec_algorith_id: Option<ExecAlgorithmId>,
     pub position_id: Option<PositionId>,
     pub command_id: UUID4,
     pub ts_init: UnixNanos,
 }
 
 impl SubmitOrder {
+    /// Creates a new [`SubmitOrder`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         client_id: ClientId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/execution/src/messages/submit_list.rs` & `nautilus_trader-1.194.0/nautilus_core/execution/src/messages/submit_list.rs`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     pub exec_algorith_id: Option<ExecAlgorithmId>,
     pub position_id: Option<PositionId>,
     pub command_id: UUID4,
     pub ts_init: UnixNanos,
 }
 
 impl SubmitOrderList {
+    /// Creates a new [`SubmitOrderList`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         client_id: ClientId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/Cargo.toml` & `nautilus_trader-1.194.0/nautilus_core/indicators/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/ama.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/average/ama.rs`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
         self.count = 0;
         self.has_inputs = false;
         self.initialized = false;
     }
 }
 
 impl AdaptiveMovingAverage {
+    /// Creates a new [`AdaptiveMovingAverage`] instance.
     pub fn new(
         period_efficiency_ratio: usize,
         period_fast: usize,
         period_slow: usize,
         price_type: Option<PriceType>,
     ) -> anyhow::Result<Self> {
         // Inputs don't require validation, however we return a `Result`
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/dema.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/average/dema.rs`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
         self.count = 0;
         self.has_inputs = false;
         self.initialized = false;
     }
 }
 
 impl DoubleExponentialMovingAverage {
+    /// Creates a new [`DoubleExponentialMovingAverage`] instance.
     pub fn new(period: usize, price_type: Option<PriceType>) -> anyhow::Result<Self> {
         Ok(Self {
             period,
             price_type: price_type.unwrap_or(PriceType::Last),
             value: 0.0,
             count: 0,
             has_inputs: false,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/ema.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/average/ema.rs`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         self.count = 0;
         self.has_inputs = false;
         self.initialized = false;
     }
 }
 
 impl ExponentialMovingAverage {
+    /// Creates a new [`ExponentialMovingAverage`] instance.
     pub fn new(period: usize, price_type: Option<PriceType>) -> anyhow::Result<Self> {
         // Inputs don't require validation, however we return a `Result`
         // to standardize with other indicators which do need validation.
         Ok(Self {
             period,
             price_type: price_type.unwrap_or(PriceType::Last),
             alpha: 2.0 / (period as f64 + 1.0),
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/hma.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/average/hma.rs`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     let mut weights: Vec<f64> = (1..size + 1).map(|x| x as f64).collect();
     let divisor: f64 = weights.iter().sum();
     weights = weights.iter().map(|x| x / divisor).collect();
     weights
 }
 
 impl HullMovingAverage {
+    /// Creates a new [`HullMovingAverage`] instance.
     pub fn new(period: usize, price_type: Option<PriceType>) -> anyhow::Result<Self> {
         let period_halved = period / 2;
         let period_sqrt = (period as f64).sqrt() as usize;
 
         let w1 = _get_weights(period_halved);
         let w2 = _get_weights(period);
         let w3 = _get_weights(period_sqrt);
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/average/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 pub mod ama;
 pub mod dema;
 pub mod ema;
 pub mod hma;
 pub mod rma;
 pub mod sma;
 pub mod vidya;
+pub mod vwap;
 pub mod wma;
 
 #[repr(C)]
 #[derive(
     Copy,
     Clone,
     Debug,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/rma.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/average/rma.rs`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         self.count = 0;
         self.has_inputs = false;
         self.initialized = false;
     }
 }
 
 impl WilderMovingAverage {
+    /// Creates a new [`WilderMovingAverage`] instance.
     pub fn new(period: usize, price_type: Option<PriceType>) -> anyhow::Result<Self> {
         // Inputs don't require validation, however we return a `Result`
         // to standardize with other indicators which do need validation.
         // The Wilder Moving Average is The Wilder's Moving Average is simply
         // an Exponential Moving Average (EMA) with a modified alpha.
         // alpha = 1 / period
         Ok(Self {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/sma.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/average/sma.rs`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         self.count = 0;
         self.inputs.clear();
         self.initialized = false;
     }
 }
 
 impl SimpleMovingAverage {
+    /// Creates a new [`SimpleMovingAverage`] instance.
     pub fn new(period: usize, price_type: Option<PriceType>) -> anyhow::Result<Self> {
         // Inputs don't require validation, however we return a `Result`
         // to standardize with other indicators which do need validation.
         Ok(Self {
             period,
             price_type: price_type.unwrap_or(PriceType::Last),
             value: 0.0,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/vidya.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/average/vidya.rs`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     pub alpha: f64,
     pub price_type: PriceType,
     pub value: f64,
     pub count: usize,
     pub initialized: bool,
     has_inputs: bool,
     pub cmo: ChandeMomentumOscillator,
-    cmo_pct: f64,
+    pub cmo_pct: f64,
 }
 
 impl Display for VariableIndexDynamicAverage {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}({})", self.name(), self.period)
     }
 }
@@ -82,14 +82,15 @@
         self.alpha = 0.0;
         self.has_inputs = false;
         self.initialized = false;
     }
 }
 
 impl VariableIndexDynamicAverage {
+    /// Creates a new [`VariableIndexDynamicAverage`] instance.
     pub fn new(
         period: usize,
         price_type: Option<PriceType>,
         cmo_ma_type: Option<MovingAverageType>,
     ) -> anyhow::Result<Self> {
         Ok(Self {
             period,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/average/wma.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/average/wma.rs`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 impl Display for WeightedMovingAverage {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}({},{:?})", self.name(), self.period, self.weights)
     }
 }
 
 impl WeightedMovingAverage {
+    /// Creates a new [`WeightedMovingAverage`] instance.
     pub fn new(
         period: usize,
         weights: Vec<f64>,
         price_type: Option<PriceType>,
     ) -> anyhow::Result<Self> {
         if weights.len() != period {
             return Err(anyhow::anyhow!("Weights length must be equal to period"));
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/book/imbalance.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/book/imbalance.rs`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         self.count = 0;
         self.has_inputs = false;
         self.initialized = false;
     }
 }
 
 impl BookImbalanceRatio {
+    /// Creates a new [`BookImbalanceRatio`] instance.
     pub fn new() -> anyhow::Result<Self> {
         // Inputs don't require validation, however we return a `Result`
         // to standardize with other indicators which do need validation.
         Ok(Self {
             value: 0.0,
             count: 0,
             has_inputs: false,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/book/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/book/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/indicator.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/indicator.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines a common `Indicator` trait.
+//! A common `Indicator` trait.
 
 use std::{fmt, fmt::Debug};
 
 use nautilus_model::{
     data::{
         bar::Bar, delta::OrderBookDelta, deltas::OrderBookDeltas, depth::OrderBookDepth10,
         quote::QuoteTick, trade::TradeTick,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/lib.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/aroon.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/momentum/aroon.rs`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
         self.count = 0;
         self.has_inputs = false;
         self.initialized = false;
     }
 }
 
 impl AroonOscillator {
+    /// Creates a new [`AroonOscillator`] instance.
     pub fn new(period: usize) -> anyhow::Result<Self> {
         Ok(Self {
             period,
             high_inputs: VecDeque::with_capacity(period),
             low_inputs: VecDeque::with_capacity(period),
             aroon_up: 0.0,
             aroon_down: 0.0,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/bias.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/momentum/bias.rs`

 * *Files 5% similar despite different names*

```diff
@@ -69,22 +69,23 @@
         self.count = 0;
         self.has_inputs = false;
         self.initialized = false;
     }
 }
 
 impl Bias {
+    /// Creates a new [`Bias`] instance.
     pub fn new(period: usize, ma_type: Option<MovingAverageType>) -> anyhow::Result<Self> {
         Ok(Self {
             period,
             ma_type: ma_type.unwrap_or(MovingAverageType::Simple),
             value: 0.0,
             count: 0,
             previous_close: 0.0,
-            ma: MovingAverageFactory::create(MovingAverageType::Simple, period),
+            ma: MovingAverageFactory::create(ma_type.unwrap_or(MovingAverageType::Simple), period),
             has_inputs: false,
             initialized: false,
         })
     }
 
     pub fn update_raw(&mut self, close: f64) {
         self.ma.update_raw(close);
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/cmo.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/momentum/cmo.rs`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
         self._has_inputs = false;
         self.initialized = false;
         self._previous_close = 0.0;
     }
 }
 
 impl ChandeMomentumOscillator {
+    /// Creates a new [`ChandeMomentumOscillator`] instance.
     pub fn new(period: usize, ma_type: Option<MovingAverageType>) -> anyhow::Result<Self> {
         Ok(Self {
             period,
             ma_type: ma_type.unwrap_or(MovingAverageType::Wilder),
             _average_gain: MovingAverageFactory::create(MovingAverageType::Wilder, period),
             _average_loss: MovingAverageFactory::create(MovingAverageType::Wilder, period),
             _previous_close: 0.0,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/momentum/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -15,7 +15,8 @@
 
 //! Momentum type indicators.
 
 pub mod aroon;
 pub mod bias;
 pub mod cmo;
 pub mod rsi;
+pub mod vhf;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/momentum/rsi.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/momentum/rsi.rs`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
         self.count = 0;
         self.has_inputs = false;
         self.initialized = false;
     }
 }
 
 impl RelativeStrengthIndex {
+    /// Creates a new [`RelativeStrengthIndex`] instance.
     pub fn new(period: usize, ma_type: Option<MovingAverageType>) -> anyhow::Result<Self> {
         Ok(Self {
             period,
             ma_type: ma_type.unwrap_or(MovingAverageType::Exponential),
             value: 0.0,
             last_value: 0.0,
             count: 0,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/ama.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/ama.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/dema.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/dema.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/ema.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/ema.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/hma.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/hma.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/mod.rs`

 * *Files 14% similar despite different names*

```diff
@@ -15,8 +15,10 @@
 
 pub mod ama;
 pub mod dema;
 pub mod ema;
 pub mod hma;
 pub mod rma;
 pub mod sma;
+pub mod vidya;
+pub mod vwap;
 pub mod wma;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/rma.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/rma.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/sma.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/sma.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/vidya.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/wma.rs`

 * *Files 8% similar despite different names*

```diff
@@ -17,31 +17,31 @@
 use nautilus_model::{
     data::{bar::Bar, quote::QuoteTick, trade::TradeTick},
     enums::PriceType,
 };
 use pyo3::prelude::*;
 
 use crate::{
-    average::vidya::VariableIndexDynamicAverage,
+    average::wma::WeightedMovingAverage,
     indicator::{Indicator, MovingAverage},
 };
 
 #[pymethods]
-impl VariableIndexDynamicAverage {
+impl WeightedMovingAverage {
     #[new]
     pub fn py_new(
         period: usize,
         weights: Vec<f64>,
         price_type: Option<PriceType>,
     ) -> PyResult<Self> {
         Self::new(period, weights, price_type).map_err(to_pyvalue_err)
     }
 
     fn __repr__(&self) -> String {
-        format!("VariableIndexDynamicAverage({},{:?})", self.period, self.weights)
+        format!("WeightedMovingAverage({},{:?})", self.period, self.weights)
     }
 
     #[getter]
     #[pyo3(name = "name")]
     fn py_name(&self) -> String {
         self.name()
     }
@@ -55,44 +55,25 @@
     #[getter]
     #[pyo3(name = "count")]
     fn py_count(&self) -> usize {
         self.count()
     }
 
     #[getter]
-    #[pyo3(name = "alpha")]
-    fn py_alpha(&self) -> usize {
-        self.alpha()
-    }
-
-    #[getter]
     #[pyo3(name = "has_inputs")]
     fn py_has_inputs(&self) -> bool {
         self.has_inputs()
     }
 
     #[getter]
     #[pyo3(name = "initialized")]
     fn py_initialized(&self) -> bool {
         self.initialized
     }
 
-    #[getter]
-    #[pyo3(name = "cmo_pct")]
-    fn py_cmo_pct(&self) -> f64 {
-        self.cmo_pct
-    }
-
-    #[getter]
-    #[pyo3(name = "cmo")]
-    fn py_cmo(&self) -> ChandeMomentumOscillator {
-        self.cmo
-    }
-
-
     #[pyo3(name = "handle_quote_tick")]
     fn py_handle_quote_tick(&mut self, tick: &QuoteTick) {
         self.py_update_raw(tick.extract_price(self.price_type).into());
     }
 
     #[pyo3(name = "handle_trade_tick")]
     fn py_handle_trade_tick(&mut self, tick: &TradeTick) {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/average/wma.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/average/vidya.rs`

 * *Files 21% similar despite different names*

```diff
@@ -17,31 +17,34 @@
 use nautilus_model::{
     data::{bar::Bar, quote::QuoteTick, trade::TradeTick},
     enums::PriceType,
 };
 use pyo3::prelude::*;
 
 use crate::{
-    average::wma::WeightedMovingAverage,
+    average::{vidya::VariableIndexDynamicAverage, MovingAverageType},
     indicator::{Indicator, MovingAverage},
 };
 
 #[pymethods]
-impl WeightedMovingAverage {
+impl VariableIndexDynamicAverage {
     #[new]
     pub fn py_new(
         period: usize,
-        weights: Vec<f64>,
         price_type: Option<PriceType>,
+        cmo_ma_type: Option<MovingAverageType>,
     ) -> PyResult<Self> {
-        Self::new(period, weights, price_type).map_err(to_pyvalue_err)
+        Self::new(period, price_type, cmo_ma_type).map_err(to_pyvalue_err)
     }
 
     fn __repr__(&self) -> String {
-        format!("WeightedMovingAverage({},{:?})", self.period, self.weights)
+        format!(
+            "VariableIndexDynamicAverage({},{:?})",
+            self.period, self.price_type
+        )
     }
 
     #[getter]
     #[pyo3(name = "name")]
     fn py_name(&self) -> String {
         self.name()
     }
@@ -55,25 +58,43 @@
     #[getter]
     #[pyo3(name = "count")]
     fn py_count(&self) -> usize {
         self.count()
     }
 
     #[getter]
+    #[pyo3(name = "alpha")]
+    fn py_alpha(&self) -> f64 {
+        self.alpha
+    }
+
+    #[getter]
     #[pyo3(name = "has_inputs")]
     fn py_has_inputs(&self) -> bool {
         self.has_inputs()
     }
 
     #[getter]
     #[pyo3(name = "initialized")]
     fn py_initialized(&self) -> bool {
         self.initialized
     }
 
+    #[getter]
+    #[pyo3(name = "cmo_pct")]
+    fn py_cmo_pct(&self) -> f64 {
+        self.cmo_pct
+    }
+
+    #[getter]
+    #[pyo3(name = "value")]
+    fn py_value(&self) -> f64 {
+        self.value
+    }
+
     #[pyo3(name = "handle_quote_tick")]
     fn py_handle_quote_tick(&mut self, tick: &QuoteTick) {
         self.py_update_raw(tick.extract_price(self.price_type).into());
     }
 
     #[pyo3(name = "handle_trade_tick")]
     fn py_handle_trade_tick(&mut self, tick: &TradeTick) {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/book/imbalance.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/book/imbalance.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/book/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/book/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/mod.rs`

 * *Files 10% similar despite different names*

```diff
@@ -31,20 +31,22 @@
     m.add_class::<crate::average::ema::ExponentialMovingAverage>()?;
     m.add_class::<crate::average::sma::SimpleMovingAverage>()?;
     m.add_class::<crate::average::ama::AdaptiveMovingAverage>()?;
     m.add_class::<crate::average::dema::DoubleExponentialMovingAverage>()?;
     m.add_class::<crate::average::hma::HullMovingAverage>()?;
     m.add_class::<crate::average::rma::WilderMovingAverage>()?;
     m.add_class::<crate::average::vidya::VariableIndexDynamicAverage>()?;
+    m.add_class::<crate::average::vwap::VolumeWeightedAveragePrice>()?;
     // book
     m.add_class::<crate::book::imbalance::BookImbalanceRatio>()?;
     // ratio
     m.add_class::<crate::ratio::efficiency_ratio::EfficiencyRatio>()?;
     // momentum
     m.add_class::<crate::momentum::rsi::RelativeStrengthIndex>()?;
     m.add_class::<crate::momentum::aroon::AroonOscillator>()?;
     m.add_class::<crate::momentum::bias::Bias>()?;
     m.add_class::<crate::momentum::cmo::ChandeMomentumOscillator>()?;
+    m.add_class::<crate::momentum::vhf::VerticalHorizontalFilter>()?;
     // volatility
     m.add_class::<crate::volatility::atr::AverageTrueRange>()?;
     Ok(())
 }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/aroon.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/momentum/aroon.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/bias.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/momentum/bias.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/cmo.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/momentum/cmo.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/mod.rs` & `nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pxd`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-// -------------------------------------------------------------------------------------------------
-//  Copyright (C) 2015-2024 Nautech Systems Pty Ltd. All rights reserved.
-//  https://nautechsystems.io
-//
-//  Licensed under the GNU Lesser General Public License Version 3.0 (the "License");
-//  You may not use this file except in compliance with the License.
-//  You may obtain a copy of the License at https://www.gnu.org/licenses/lgpl-3.0.en.html
-//
-//  Unless required by applicable law or agreed to in writing, software
-//  distributed under the License is distributed on an "AS IS" BASIS,
-//  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-//  See the License for the specific language governing permissions and
-//  limitations under the License.
-// -------------------------------------------------------------------------------------------------
+# -------------------------------------------------------------------------------------------------
+#  Copyright (C) 2015-2024 Nautech Systems Pty Ltd. All rights reserved.
+#  https://nautechsystems.io
+#
+#  Licensed under the GNU Lesser General Public License Version 3.0 (the "License");
+#  You may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at https://www.gnu.org/licenses/lgpl-3.0.en.html
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+# -------------------------------------------------------------------------------------------------
 
-pub mod aroon;
-pub mod bias;
-pub mod cmo;
-pub mod rsi;
+
+cpdef enum CandleWickSize:
+    NONE = 0  # No candle wick
+    SMALL = 1
+    MEDIUM = 2
+    LARGE = 3
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/momentum/rsi.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/momentum/rsi.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/ratio/efficiency_ratio.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/ratio/efficiency_ratio.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/ratio/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/ratio/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/volatility/atr.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/volatility/atr.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/python/volatility/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/python/volatility/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/ratio/efficiency_ratio.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/ratio/efficiency_ratio.rs`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
         self.value = 0.0;
         self.inputs.clear();
         self.initialized = false;
     }
 }
 
 impl EfficiencyRatio {
+    /// Creates a new [`EfficiencyRatio`] instance.
     pub fn new(period: usize, price_type: Option<PriceType>) -> anyhow::Result<Self> {
         Ok(Self {
             period,
             price_type: price_type.unwrap_or(PriceType::Last),
             value: 0.0,
             inputs: Vec::with_capacity(period),
             deltas: Vec::with_capacity(period),
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/ratio/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/ratio/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/stubs.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/stubs.rs`

 * *Files 7% similar despite different names*

```diff
@@ -27,18 +27,21 @@
 };
 use rstest::*;
 
 use crate::{
     average::{
         ama::AdaptiveMovingAverage, dema::DoubleExponentialMovingAverage,
         ema::ExponentialMovingAverage, hma::HullMovingAverage, rma::WilderMovingAverage,
-        sma::SimpleMovingAverage, vidya::VariableIndexDynamicAverage, wma::WeightedMovingAverage,
-        MovingAverageType,
+        sma::SimpleMovingAverage, vidya::VariableIndexDynamicAverage,
+        vwap::VolumeWeightedAveragePrice, wma::WeightedMovingAverage, MovingAverageType,
+    },
+    momentum::{
+        bias::Bias, cmo::ChandeMomentumOscillator, rsi::RelativeStrengthIndex,
+        vhf::VerticalHorizontalFilter,
     },
-    momentum::{bias::Bias, cmo::ChandeMomentumOscillator, rsi::RelativeStrengthIndex},
     ratio::efficiency_ratio::EfficiencyRatio,
 };
 
 ////////////////////////////////////////////////////////////////////////////////
 // Common
 ////////////////////////////////////////////////////////////////////////////////
 #[fixture]
@@ -134,14 +137,19 @@
 #[fixture]
 pub fn indicator_vidya_10() -> VariableIndexDynamicAverage {
     VariableIndexDynamicAverage::new(10, Some(PriceType::Mid), Some(MovingAverageType::Wilder))
         .unwrap()
 }
 
 #[fixture]
+pub fn indicator_vwap() -> VolumeWeightedAveragePrice {
+    VolumeWeightedAveragePrice::new().unwrap()
+}
+
+#[fixture]
 pub fn indicator_wma_10() -> WeightedMovingAverage {
     let weights = vec![0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0];
     WeightedMovingAverage::new(10, weights, Some(PriceType::Mid)).unwrap()
 }
 
 ////////////////////////////////////////////////////////////////////////////////
 // Ratios
@@ -164,7 +172,12 @@
     ChandeMomentumOscillator::new(10, Some(MovingAverageType::Wilder)).unwrap()
 }
 
 #[fixture]
 pub fn bias_10() -> Bias {
     Bias::new(10, Some(MovingAverageType::Wilder)).unwrap()
 }
+
+#[fixture]
+pub fn vhf_10() -> VerticalHorizontalFilter {
+    VerticalHorizontalFilter::new(10, Some(MovingAverageType::Simple)).unwrap()
+}
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/testing.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/testing.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/volatility/atr.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/volatility/atr.rs`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         self.count = 0;
         self.has_inputs = false;
         self.initialized = false;
     }
 }
 
 impl AverageTrueRange {
+    /// Creates a new [`AverageTrueRange`] instance.
     pub fn new(
         period: usize,
         ma_type: Option<MovingAverageType>,
         use_previous: Option<bool>,
         value_floor: Option<f64>,
     ) -> anyhow::Result<Self> {
         Ok(Self {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/indicators/src/volatility/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/indicators/src/volatility/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/Cargo.toml` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 rmp-serde = { workspace = true }
 rust_decimal = { workspace = true }
 semver = { workspace = true }
 serde_json = { workspace = true }
 tokio = { workspace = true }
 tracing = {workspace = true }
 ustr = { workspace = true }
-redis = { version = "0.25.3", features = [
+redis = { version = "0.25.4", features = [
     "connection-manager",
     "keep-alive",
     "tls-rustls",
     "tls-rustls-webpki-roots",
     "tokio-comp",
     "tokio-rustls-comp",
 ], optional = true }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/lib.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/redis/cache.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/python/redis/cache.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::collections::HashMap;
 
-use nautilus_common::cache::database::CacheDatabase;
 use nautilus_core::{
     python::{to_pyruntime_err, to_pyvalue_err},
     uuid::UUID4,
 };
 use nautilus_model::identifiers::trader_id::TraderId;
 use pyo3::{prelude::*, types::PyBytes};
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/redis/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/python/redis/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/redis/msgbus.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/python/redis/msgbus.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/sql/cache_database.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/python/sql/cache_database.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/python/sql/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/python/sql/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/redis/cache.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/redis/cache.rs`

 * *Files 19% similar despite different names*

```diff
@@ -16,20 +16,34 @@
 use std::{
     collections::{HashMap, VecDeque},
     sync::mpsc::{channel, Receiver, Sender, TryRecvError},
     thread::{self, JoinHandle},
     time::{Duration, Instant},
 };
 
-use nautilus_common::cache::database::{CacheDatabase, DatabaseCommand, DatabaseOperation};
-use nautilus_core::{correctness::check_slice_not_empty, uuid::UUID4};
-use nautilus_model::identifiers::trader_id::TraderId;
+use nautilus_common::{
+    cache::database::CacheDatabaseAdapter, enums::SerializationEncoding,
+    interface::account::Account,
+};
+use nautilus_core::{correctness::check_slice_not_empty, nanos::UnixNanos, uuid::UUID4};
+use nautilus_model::{
+    identifiers::{
+        account_id::AccountId, client_id::ClientId, client_order_id::ClientOrderId,
+        component_id::ComponentId, instrument_id::InstrumentId, position_id::PositionId,
+        strategy_id::StrategyId, trader_id::TraderId, venue_order_id::VenueOrderId,
+    },
+    instruments::{any::InstrumentAny, synthetic::SyntheticInstrument},
+    orders::any::OrderAny,
+    position::Position,
+    types::currency::Currency,
+};
 use redis::{Commands, Connection, Pipeline};
 use serde_json::{json, Value};
 use tracing::{debug, error};
+use ustr::Ustr;
 
 use crate::redis::{create_redis_connection, get_buffer_interval};
 
 // Error constants
 const FAILED_TX_CHANNEL: &str = "Failed to send to channel";
 
 // Redis constants
@@ -59,30 +73,71 @@
 const INDEX_ORDERS_CLOSED: &str = "index:orders_closed";
 const INDEX_ORDERS_EMULATED: &str = "index:orders_emulated";
 const INDEX_ORDERS_INFLIGHT: &str = "index:orders_inflight";
 const INDEX_POSITIONS: &str = "index:positions";
 const INDEX_POSITIONS_OPEN: &str = "index:positions_open";
 const INDEX_POSITIONS_CLOSED: &str = "index:positions_closed";
 
+/// A type of database operation.
+#[derive(Clone, Debug)]
+pub enum DatabaseOperation {
+    Insert,
+    Update,
+    Delete,
+    Close,
+}
+
+/// Represents a database command to be performed which may be executed in another thread.
+#[derive(Clone, Debug)]
+pub struct DatabaseCommand {
+    /// The database operation type.
+    pub op_type: DatabaseOperation,
+    /// The primary key for the operation.
+    pub key: Option<String>,
+    /// The data payload for the operation.
+    pub payload: Option<Vec<Vec<u8>>>,
+}
+
+impl DatabaseCommand {
+    /// Creates a new [`DatabaseCommand`] instance.
+    #[must_use]
+    pub fn new(op_type: DatabaseOperation, key: String, payload: Option<Vec<Vec<u8>>>) -> Self {
+        Self {
+            op_type,
+            key: Some(key),
+            payload,
+        }
+    }
+
+    /// Initialize a `Close` database command, this is meant to close the database cache channel.
+    #[must_use]
+    pub fn close() -> Self {
+        Self {
+            op_type: DatabaseOperation::Close,
+            key: None,
+            payload: None,
+        }
+    }
+}
+
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.infrastructure")
 )]
 pub struct RedisCacheDatabase {
     pub trader_id: TraderId,
     trader_key: String,
     conn: Connection,
     tx: Sender<DatabaseCommand>,
     handle: Option<JoinHandle<()>>,
 }
 
-impl CacheDatabase for RedisCacheDatabase {
-    type DatabaseType = RedisCacheDatabase;
-
-    fn new(
+impl RedisCacheDatabase {
+    /// Creates a new [`RedisCacheDatabase`] instance.
+    pub fn new(
         trader_id: TraderId,
         instance_id: UUID4,
         config: HashMap<String, serde_json::Value>,
     ) -> anyhow::Result<RedisCacheDatabase> {
         let database_config = config
             .get("database")
             .ok_or(anyhow::anyhow!("No database config"))?;
@@ -105,45 +160,45 @@
             trader_key,
             conn,
             tx,
             handle: Some(handle),
         })
     }
 
-    fn close(&mut self) -> anyhow::Result<()> {
+    pub fn close(&mut self) -> anyhow::Result<()> {
         debug!("Closing cache database adapter");
         self.tx
             .send(DatabaseCommand::close())
             .map_err(anyhow::Error::new)?;
 
         if let Some(handle) = self.handle.take() {
             debug!("Joining `cache` thread");
             handle.join().map_err(|e| anyhow::anyhow!("{:?}", e))
         } else {
             Err(anyhow::anyhow!("Cache database already shutdown"))
         }
     }
 
-    fn flushdb(&mut self) -> anyhow::Result<()> {
+    pub fn flushdb(&mut self) -> anyhow::Result<()> {
         match redis::cmd(FLUSHDB).query::<()>(&mut self.conn) {
             Ok(_) => Ok(()),
             Err(e) => Err(e.into()),
         }
     }
 
-    fn keys(&mut self, pattern: &str) -> anyhow::Result<Vec<String>> {
+    pub fn keys(&mut self, pattern: &str) -> anyhow::Result<Vec<String>> {
         let pattern = format!("{}{DELIMITER}{}", self.trader_key, pattern);
         debug!("Querying keys: {pattern}");
         match self.conn.keys(pattern) {
             Ok(keys) => Ok(keys),
             Err(e) => Err(e.into()),
         }
     }
 
-    fn read(&mut self, key: &str) -> anyhow::Result<Vec<Vec<u8>>> {
+    pub fn read(&mut self, key: &str) -> anyhow::Result<Vec<Vec<u8>>> {
         let collection = get_collection_key(key)?;
         let key = format!("{}{DELIMITER}{}", self.trader_key, key);
 
         match collection {
             INDEX => read_index(&mut self.conn, &key),
             GENERAL => read_string(&mut self.conn, &key),
             CURRENCIES => read_string(&mut self.conn, &key),
@@ -154,31 +209,31 @@
             POSITIONS => read_list(&mut self.conn, &key),
             ACTORS => read_string(&mut self.conn, &key),
             STRATEGIES => read_string(&mut self.conn, &key),
             _ => anyhow::bail!("Unsupported operation: `read` for collection '{collection}'"),
         }
     }
 
-    fn insert(&mut self, key: String, payload: Option<Vec<Vec<u8>>>) -> anyhow::Result<()> {
+    pub fn insert(&mut self, key: String, payload: Option<Vec<Vec<u8>>>) -> anyhow::Result<()> {
         let op = DatabaseCommand::new(DatabaseOperation::Insert, key, payload);
         match self.tx.send(op) {
             Ok(_) => Ok(()),
             Err(e) => anyhow::bail!("{FAILED_TX_CHANNEL}: {e}"),
         }
     }
 
-    fn update(&mut self, key: String, payload: Option<Vec<Vec<u8>>>) -> anyhow::Result<()> {
+    pub fn update(&mut self, key: String, payload: Option<Vec<Vec<u8>>>) -> anyhow::Result<()> {
         let op = DatabaseCommand::new(DatabaseOperation::Update, key, payload);
         match self.tx.send(op) {
             Ok(_) => Ok(()),
             Err(e) => anyhow::bail!("{FAILED_TX_CHANNEL}: {e}"),
         }
     }
 
-    fn delete(&mut self, key: String, payload: Option<Vec<Vec<u8>>>) -> anyhow::Result<()> {
+    pub fn delete(&mut self, key: String, payload: Option<Vec<Vec<u8>>>) -> anyhow::Result<()> {
         let op = DatabaseCommand::new(DatabaseOperation::Delete, key, payload);
         match self.tx.send(op) {
             Ok(_) => Ok(()),
             Err(e) => anyhow::bail!("{FAILED_TX_CHANNEL}: {e}"),
         }
     }
 
@@ -616,14 +671,206 @@
             .map_err(|e| anyhow::anyhow!("Failed to deserialize msgpack `payload`: {e}")),
         "json" => serde_json::from_slice(payload)
             .map_err(|e| anyhow::anyhow!("Failed to deserialize json `payload`: {e}")),
         _ => Err(anyhow::anyhow!("Unsupported encoding: {encoding}")),
     }
 }
 
+#[allow(dead_code)] // Under development
+pub struct RedisCacheDatabaseAdapter {
+    pub encoding: SerializationEncoding,
+    database: RedisCacheDatabase,
+}
+
+#[allow(dead_code)] // Under development
+#[allow(unused)] // Under development
+impl CacheDatabaseAdapter for RedisCacheDatabaseAdapter {
+    fn close(&mut self) -> anyhow::Result<()> {
+        self.database.close()
+    }
+
+    fn flush(&mut self) -> anyhow::Result<()> {
+        self.database.flushdb()
+    }
+
+    fn load(&mut self) -> anyhow::Result<HashMap<String, Vec<u8>>> {
+        // self.database.load()
+        Ok(HashMap::new()) // TODO
+    }
+
+    fn load_currencies(&mut self) -> anyhow::Result<HashMap<Ustr, Currency>> {
+        let mut currencies = HashMap::new();
+
+        for key in self.database.keys(&format!("{CURRENCIES}*"))? {
+            let parts: Vec<&str> = key.as_str().rsplitn(2, ':').collect();
+            let currency_code = Ustr::from(parts.first().unwrap());
+            let currency = self.load_currency(&currency_code)?;
+            currencies.insert(currency_code, currency);
+        }
+
+        Ok(currencies)
+    }
+
+    fn load_instruments(&mut self) -> anyhow::Result<HashMap<InstrumentId, InstrumentAny>> {
+        todo!()
+    }
+
+    fn load_synthetics(&mut self) -> anyhow::Result<HashMap<InstrumentId, SyntheticInstrument>> {
+        todo!()
+    }
+
+    fn load_accounts(&mut self) -> anyhow::Result<HashMap<AccountId, Box<dyn Account>>> {
+        todo!()
+    }
+
+    fn load_orders(&mut self) -> anyhow::Result<HashMap<ClientOrderId, OrderAny>> {
+        todo!()
+    }
+
+    fn load_positions(&mut self) -> anyhow::Result<HashMap<PositionId, Position>> {
+        todo!()
+    }
+
+    fn load_index_order_position(&mut self) -> anyhow::Result<HashMap<ClientOrderId, Position>> {
+        todo!()
+    }
+
+    fn load_index_order_client(&mut self) -> anyhow::Result<HashMap<ClientOrderId, ClientId>> {
+        todo!()
+    }
+
+    fn load_currency(&mut self, code: &Ustr) -> anyhow::Result<Currency> {
+        todo!()
+    }
+
+    fn load_instrument(&mut self, instrument_id: &InstrumentId) -> anyhow::Result<InstrumentAny> {
+        todo!()
+    }
+
+    fn load_synthetic(
+        &mut self,
+        instrument_id: &InstrumentId,
+    ) -> anyhow::Result<SyntheticInstrument> {
+        todo!()
+    }
+
+    fn load_account(&mut self, account_id: &AccountId) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn load_order(&mut self, client_order_id: &ClientOrderId) -> anyhow::Result<OrderAny> {
+        todo!()
+    }
+
+    fn load_position(&mut self, position_id: &PositionId) -> anyhow::Result<Position> {
+        todo!()
+    }
+
+    fn load_actor(
+        &mut self,
+        component_id: &ComponentId,
+    ) -> anyhow::Result<HashMap<String, Vec<u8>>> {
+        todo!()
+    }
+
+    fn delete_actor(&mut self, component_id: &ComponentId) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn load_strategy(
+        &mut self,
+        strategy_id: &StrategyId,
+    ) -> anyhow::Result<HashMap<String, Vec<u8>>> {
+        todo!()
+    }
+
+    fn delete_strategy(&mut self, component_id: &StrategyId) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn add(&mut self, key: String, value: Vec<u8>) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn add_currency(&mut self, currency: &Currency) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn add_instrument(&mut self, instrument: &InstrumentAny) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn add_synthetic(&mut self, synthetic: &SyntheticInstrument) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn add_account(&mut self, account: &dyn Account) -> anyhow::Result<Box<dyn Account>> {
+        todo!()
+    }
+
+    fn add_order(&mut self, order: &OrderAny) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn add_position(&mut self, position: &Position) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn index_venue_order_id(
+        &mut self,
+        client_order_id: ClientOrderId,
+        venue_order_id: VenueOrderId,
+    ) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn index_order_position(
+        &mut self,
+        client_order_id: ClientOrderId,
+        position_id: PositionId,
+    ) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn update_actor(&mut self) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn update_strategy(&mut self) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn update_account(&mut self, account: &dyn Account) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn update_order(&mut self, order: &OrderAny) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn update_position(&mut self, position: &Position) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn snapshot_order_state(&mut self, order: &OrderAny) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn snapshot_position_state(&mut self, position: &Position) -> anyhow::Result<()> {
+        todo!()
+    }
+
+    fn heartbeat(&mut self, timestamp: UnixNanos) -> anyhow::Result<()> {
+        todo!()
+    }
+}
+
+////////////////////////////////////////////////////////////////////////////////
+// Tests
+////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
 mod tests {
     use std::collections::HashMap;
 
     use rstest::rstest;
     use serde_json::json;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/redis/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/redis/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/redis/msgbus.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/redis/msgbus.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/cache_database.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/cache_database.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/general.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/models/general.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/instruments.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/models/instruments.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/models/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/orders.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/models/orders.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/models/types.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/models/types.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/pg.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/pg.rs`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     pub port: u16,
     pub username: String,
     pub password: String,
     pub database: String,
 }
 
 impl PostgresConnectOptions {
+    /// Creates a new [`PostgresConnectOptions`] instance.
     pub fn new(
         host: String,
         port: u16,
         username: String,
         password: String,
         database: String,
     ) -> Self {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/src/sql/queries.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/src/sql/queries.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/infrastructure/tests/test_cache_database_postgres.rs` & `nautilus_trader-1.194.0/nautilus_core/infrastructure/tests/test_cache_database_postgres.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/Cargo.toml` & `nautilus_trader-1.194.0/nautilus_core/model/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/build.rs` & `nautilus_trader-1.194.0/nautilus_core/model/build.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/cbindgen.toml` & `nautilus_trader-1.194.0/nautilus_core/model/cbindgen.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/cbindgen_cython.toml` & `nautilus_trader-1.194.0/nautilus_core/model/cbindgen_cython.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/currencies.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/currencies.rs`

 * *Files 0% similar despite different names*

```diff
@@ -984,15 +984,15 @@
             iso4217: 0,
             name: Ustr::from("Zcash"),
             currency_type: CurrencyType::Crypto,
         })
     }
 }
 
-/// Provides a map of built-in `Currency` constants.
+/// A map of built-in `Currency` constants.
 pub static CURRENCY_MAP: Lazy<Mutex<HashMap<String, Currency>>> = Lazy::new(|| {
     let mut map = HashMap::new();
     ///////////////////////////////////////////////////////////////////////////
     // Fiat currencies
     ///////////////////////////////////////////////////////////////////////////
     map.insert(Currency::AUD().code.to_string(), Currency::AUD());
     map.insert(Currency::BRL().code.to_string(), Currency::BRL());
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/data/bar.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/data/bar.rs`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     /// The type of bar aggregation.
     pub aggregation: BarAggregation,
     /// The price type to use for aggregation.
     pub price_type: PriceType,
 }
 
 impl BarSpecification {
+    /// Creates a new [`BarSpecification`] instance.
     #[must_use]
     pub fn new(step: usize, aggregation: BarAggregation, price_type: PriceType) -> Self {
         Self {
             step,
             aggregation,
             price_type,
         }
@@ -83,14 +84,15 @@
     /// The bar types specification.
     pub spec: BarSpecification,
     /// The bar types aggregation source.
     pub aggregation_source: AggregationSource,
 }
 
 impl BarType {
+    /// Creates a new [`BarType`] instance.
     #[must_use]
     pub fn new(
         instrument_id: InstrumentId,
         spec: BarSpecification,
         aggregation_source: AggregationSource,
     ) -> Self {
         Self {
@@ -226,14 +228,15 @@
     /// The UNIX timestamp (nanoseconds) when the data event occurred.
     pub ts_event: UnixNanos,
     /// The UNIX timestamp (nanoseconds) when the struct was initialized.
     pub ts_init: UnixNanos,
 }
 
 impl Bar {
+    /// Creates a new [`Bar`] instance.
     #[must_use]
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         bar_type: BarType,
         open: Price,
         high: Price,
         low: Price,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/data/delta.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/data/delta.rs`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     /// The UNIX timestamp (nanoseconds) when the book event occurred.
     pub ts_event: UnixNanos,
     /// The UNIX timestamp (nanoseconds) when the struct was initialized.
     pub ts_init: UnixNanos,
 }
 
 impl OrderBookDelta {
+    /// Creates a new [`OrderBookDelta`] instance.
     #[allow(clippy::too_many_arguments)]
     #[must_use]
     pub fn new(
         instrument_id: InstrumentId,
         action: BookAction,
         order: BookOrder,
         flags: u8,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/data/deltas.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/data/deltas.rs`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     /// The UNIX timestamp (nanoseconds) when the book event occurred.
     pub ts_event: UnixNanos,
     /// The UNIX timestamp (nanoseconds) when the struct was initialized.
     pub ts_init: UnixNanos,
 }
 
 impl OrderBookDeltas {
+    /// Creates a new [`OrderBookDeltas`] instance.
     #[allow(clippy::too_many_arguments)]
     #[must_use]
     pub fn new(instrument_id: InstrumentId, deltas: Vec<OrderBookDelta>) -> Self {
         assert!(!deltas.is_empty(), "`deltas` cannot be empty");
         // SAFETY: We asserted `deltas` is not empty
         let last = deltas.last().unwrap();
         let flags = last.flags;
@@ -107,15 +108,15 @@
 
 impl GetTsInit for OrderBookDeltas {
     fn ts_init(&self) -> UnixNanos {
         self.ts_init
     }
 }
 
-/// Provides a C compatible Foreign Function Interface (FFI) for an underlying [`OrderBookDeltas`].
+/// C compatible Foreign Function Interface (FFI) for an underlying [`OrderBookDeltas`].
 ///
 /// This struct wraps `OrderBookDeltas` in a way that makes it compatible with C function
 /// calls, enabling interaction with `OrderBookDeltas` in a C environment.
 ///
 /// It implements the `Deref` trait, allowing instances of `OrderBookDeltas_API` to be
 /// dereferenced to `OrderBookDeltas`, providing access to `OrderBookDeltas`'s methods without
 /// having to manually access the underlying `OrderBookDeltas` instance.
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/data/depth.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/data/depth.rs`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     /// The UNIX timestamp (nanoseconds) when the book event occurred.
     pub ts_event: UnixNanos,
     /// The UNIX timestamp (nanoseconds) when the struct was initialized.
     pub ts_init: UnixNanos,
 }
 
 impl OrderBookDepth10 {
+    /// Creates a new [`OrderBookDepth10`] instance.
     #[allow(clippy::too_many_arguments)]
     #[must_use]
     pub fn new(
         instrument_id: InstrumentId,
         bids: [BookOrder; DEPTH10_LEN],
         asks: [BookOrder; DEPTH10_LEN],
         bid_counts: [u32; DEPTH10_LEN],
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/data/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/data/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines `Data` types for the trading domain model.
+//! Data types for the trading domain model.
 
 pub mod bar;
 pub mod delta;
 pub mod deltas;
 pub mod depth;
 pub mod order;
 pub mod quote;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/data/order.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/data/order.rs`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     /// The order size.
     pub size: Quantity,
     /// The order ID.
     pub order_id: OrderId,
 }
 
 impl BookOrder {
+    /// Creates a new [`BookOrder`] instance.
     #[must_use]
     pub fn new(side: OrderSide, price: Price, size: Quantity, order_id: u64) -> Self {
         Self {
             side,
             price,
             size,
             order_id,
@@ -91,14 +92,15 @@
             OrderSide::Sell => -(self.size.as_f64()),
             _ => panic!("{}", BookIntegrityError::NoOrderSide),
         }
     }
 }
 
 impl Default for BookOrder {
+    /// Creates a NULL [`BookOrder`] instance.
     fn default() -> Self {
         NULL_ORDER
     }
 }
 
 impl PartialEq for BookOrder {
     fn eq(&self, other: &Self) -> bool {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/data/quote.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/data/quote.rs`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     /// The UNIX timestamp (nanoseconds) when the quote event occurred.
     pub ts_event: UnixNanos,
     /// The UNIX timestamp (nanoseconds) when the struct was initialized.
     pub ts_init: UnixNanos,
 }
 
 impl QuoteTick {
+    /// Creates a new [`QuoteTick`] instance.
     pub fn new(
         instrument_id: InstrumentId,
         bid_price: Price,
         ask_price: Price,
         bid_size: Quantity,
         ask_size: Quantity,
         ts_event: UnixNanos,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/data/stubs.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/data/stubs.rs`

 * *Files 2% similar despite different names*

```diff
@@ -30,42 +30,45 @@
     data::order::BookOrder,
     enums::{AggregationSource, AggressorSide, BarAggregation, BookAction, OrderSide, PriceType},
     identifiers::{instrument_id::InstrumentId, symbol::Symbol, trade_id::TradeId, venue::Venue},
     types::{price::Price, quantity::Quantity},
 };
 
 impl Default for QuoteTick {
+    /// Creates a new default [`QuoteTick`] instance for testing.
     fn default() -> Self {
         Self {
             instrument_id: InstrumentId::from("AUDUSD.SIM"),
             bid_price: Price::from("1.00000"),
             ask_price: Price::from("1.00000"),
             bid_size: Quantity::from(100_000),
             ask_size: Quantity::from(100_000),
             ts_event: UnixNanos::default(),
             ts_init: UnixNanos::default(),
         }
     }
 }
 
 impl Default for TradeTick {
+    /// Creates a new default [`TradeTick`] instance for testing.
     fn default() -> Self {
         TradeTick {
             instrument_id: InstrumentId::from("AUDUSD.SIM"),
             price: Price::from("1.00000"),
             size: Quantity::from(100_000),
             aggressor_side: AggressorSide::Buyer,
             trade_id: TradeId::new("123456789").unwrap(),
             ts_event: UnixNanos::default(),
             ts_init: UnixNanos::default(),
         }
     }
 }
 
 impl Default for Bar {
+    /// Creates a new default [`Bar`] instance for testing.
     fn default() -> Self {
         Self {
             bar_type: BarType::from("AUDUSD.SIM-1-MINUTE-LAST-INTERNAL"),
             open: Price::from("1.00010"),
             high: Price::from("1.00020"),
             low: Price::from("1.00000"),
             close: Price::from("1.00010"),
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/data/trade.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/data/trade.rs`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     /// The UNIX timestamp (nanoseconds) when the trade event occurred.
     pub ts_event: UnixNanos,
     /// The UNIX timestamp (nanoseconds) when the struct was initialized.
     pub ts_init: UnixNanos,
 }
 
 impl TradeTick {
+    /// Creates a new [`TradeTick`] instance.
     #[must_use]
     pub fn new(
         instrument_id: InstrumentId,
         price: Price,
         size: Quantity,
         aggressor_side: AggressorSide,
         trade_id: TradeId,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/enums.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/enums.rs`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines enumerations for the trading domain model.
+//! Enumerations for the trading domain model.
 
 use std::str::FromStr;
 
 use serde::{Deserialize, Deserializer, Serialize, Serializer};
 use strum::{AsRefStr, Display, EnumIter, EnumString, FromRepr};
 
 use crate::enum_strum_serde;
@@ -351,17 +351,17 @@
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model.enums")
 )]
 pub enum BookType {
     /// Top-of-book best bid/ask, one level per side.
     L1_MBP = 1,
-    /// Market by price, one order per level (aggregated).
+    /// Market-by-price, one order per level (aggregated).
     L2_MBP = 2,
-    /// Market by order, multiple orders per level (full granularity).
+    /// Market-by-order, multiple orders per level (full granularity).
     L3_MBO = 3,
 }
 
 impl FromU8 for BookType {
     fn from_u8(value: u8) -> Option<Self> {
         match value {
             1 => Some(Self::L1_MBP),
@@ -928,15 +928,15 @@
 #[strum(serialize_all = "SCREAMING_SNAKE_CASE")]
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model.enums")
 )]
 #[allow(non_camel_case_types)]
 pub enum RecordFlag {
-    /// Last message in the packet from the venue for a given `instrument_id`.
+    /// Last message in the book event or packet from the venue for a given `instrument_id`.
     F_LAST = 1 << 7, // 128
     /// Top-of-book message, not an individual order.
     F_TOB = 1 << 6, // 64
     /// Message sourced from a replay, such as a snapshot server.
     F_SNAPSHOT = 1 << 5, // 32
     /// Aggregated price level message, not an individual order.
     F_MBP = 1 << 4, // 16
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/account/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/account/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/account/state.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/account/state.rs`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     pub is_reported: bool,
     pub event_id: UUID4,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
 }
 
 impl AccountState {
+    /// Creates a new [`AccountState`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         account_id: AccountId,
         account_type: AccountType,
         balances: Vec<AccountBalance>,
         margins: Vec<MarginBalance>,
         is_reported: bool,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/account/stubs.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/account/stubs.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/events/mod.rs`

 * *Files 9% similar despite different names*

```diff
@@ -9,12 +9,8 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines order, position and account events for the trading domain model.
-
-pub mod account;
 pub mod order;
-pub mod position;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/accepted.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/pending_cancel.rs`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::fmt::{Debug, Display};
 
 use derive_builder::Builder;
-use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
+use nautilus_core::{nanos::UnixNanos, serialization::from_bool_as_u8, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
     enums::{
         ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
         TriggerType,
@@ -39,97 +39,98 @@
 #[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
-pub struct OrderAccepted {
+pub struct OrderPendingCancel {
     pub trader_id: TraderId,
     pub strategy_id: StrategyId,
     pub instrument_id: InstrumentId,
     pub client_order_id: ClientOrderId,
-    pub venue_order_id: VenueOrderId,
     pub account_id: AccountId,
     pub event_id: UUID4,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
     #[serde(deserialize_with = "from_bool_as_u8")]
     pub reconciliation: u8, // TODO: Change to bool once Cython removed
+    pub venue_order_id: Option<VenueOrderId>,
 }
 
-impl OrderAccepted {
+impl OrderPendingCancel {
+    /// Creates a new [`OrderPendingCancel`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
-        venue_order_id: VenueOrderId,
         account_id: AccountId,
         event_id: UUID4,
         ts_event: UnixNanos,
         ts_init: UnixNanos,
         reconciliation: bool,
+        venue_order_id: Option<VenueOrderId>,
     ) -> anyhow::Result<Self> {
         Ok(Self {
             trader_id,
             strategy_id,
             instrument_id,
             client_order_id,
-            venue_order_id,
             account_id,
             event_id,
             ts_event,
             ts_init,
             reconciliation: u8::from(reconciliation),
+            venue_order_id,
         })
     }
 }
 
-impl Debug for OrderAccepted {
+impl Debug for OrderPendingCancel {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(f,
             "{}(trader_id={}, strategy_id={}, instrument_id={}, client_order_id={}, venue_order_id={}, account_id={}, event_id={}, ts_event={}, ts_init={})",
-            stringify!(OrderAccepted),
+            stringify!(OrderPendingCancel),
             self.trader_id,
             self.strategy_id,
             self.instrument_id,
             self.client_order_id,
-            self.venue_order_id,
+            self.venue_order_id.map_or_else(|| "None".to_string(), |venue_order_id| format!("{venue_order_id}")),
             self.account_id,
             self.event_id,
             self.ts_event,
             self.ts_init
         )
     }
 }
 
-impl Display for OrderAccepted {
+impl Display for OrderPendingCancel {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(
             f,
             "{}(instrument_id={}, client_order_id={}, venue_order_id={}, account_id={}, ts_event={})",
-            stringify!(OrderAccepted),
+            stringify!(OrderPendingCancel),
             self.instrument_id,
             self.client_order_id,
-            self.venue_order_id,
+            self.venue_order_id.map_or("None".to_string(), |venue_order_id| format!("{venue_order_id}")),
             self.account_id,
             self.ts_event
         )
     }
 }
 
-impl OrderEvent for OrderAccepted {
+impl OrderEvent for OrderPendingCancel {
     fn id(&self) -> UUID4 {
         self.event_id
     }
 
     fn kind(&self) -> &str {
-        stringify!(OrderAccepted)
+        stringify!(OrderPendingCancel)
     }
 
     fn order_type(&self) -> Option<OrderType> {
         None
     }
 
     fn order_side(&self) -> Option<OrderSide> {
@@ -261,15 +262,15 @@
     }
 
     fn exec_spawn_id(&self) -> Option<ClientOrderId> {
         None
     }
 
     fn venue_order_id(&self) -> Option<VenueOrderId> {
-        Some(self.venue_order_id)
+        self.venue_order_id
     }
 
     fn account_id(&self) -> Option<AccountId> {
         Some(self.account_id)
     }
 
     fn position_id(&self) -> Option<PositionId> {
@@ -292,19 +293,18 @@
 ////////////////////////////////////////////////////////////////////////////////
 // Tests
 ////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
 mod tests {
     use rstest::rstest;
 
-    use super::*;
-    use crate::events::order::stubs::*;
+    use crate::events::order::{pending_cancel::OrderPendingCancel, stubs::*};
 
     #[rstest]
-    fn test_order_accepted_display(order_accepted: OrderAccepted) {
-        let display = format!("{order_accepted}");
+    fn test_order_pending_cancel_display(order_pending_cancel: OrderPendingCancel) {
+        let display = format!("{order_pending_cancel}");
         assert_eq!(
             display,
-            "OrderAccepted(instrument_id=BTCUSDT.COINBASE, client_order_id=O-19700101-0000-000-001-1, venue_order_id=001, account_id=SIM-001, ts_event=0)"
+            "OrderPendingCancel(instrument_id=BTCUSDT.COINBASE, client_order_id=O-19700101-0000-000-001-1, venue_order_id=001, account_id=SIM-001, ts_event=0)"
         );
     }
 }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/cancel_rejected.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/cancel_rejected.rs`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::fmt::{Debug, Display};
 
 use derive_builder::Builder;
-use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
+use nautilus_core::{nanos::UnixNanos, serialization::from_bool_as_u8, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
     enums::{
         ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
         TriggerType,
@@ -55,14 +55,15 @@
     #[serde(deserialize_with = "from_bool_as_u8")]
     pub reconciliation: u8, // TODO: Change to bool once Cython removed
     pub venue_order_id: Option<VenueOrderId>,
     pub account_id: Option<AccountId>,
 }
 
 impl OrderCancelRejected {
+    /// Creates a new [`OrderCancelRejected`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         reason: Ustr,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/canceled.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/canceled.rs`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::fmt::{Debug, Display};
 
 use derive_builder::Builder;
-use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
+use nautilus_core::{nanos::UnixNanos, serialization::from_bool_as_u8, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
     enums::{
         ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
         TriggerType,
@@ -54,14 +54,15 @@
     #[serde(deserialize_with = "from_bool_as_u8")]
     pub reconciliation: u8, // TODO: Change to bool once Cython removed
     pub venue_order_id: Option<VenueOrderId>,
     pub account_id: Option<AccountId>,
 }
 
 impl OrderCanceled {
+    /// Creates a new [`OrderCanceled`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         event_id: UUID4,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/denied.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/denied.rs`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     pub reason: Ustr,
     pub event_id: UUID4,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
 }
 
 impl OrderDenied {
+    /// Creates a new [`OrderDenied`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         reason: Ustr,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/emulated.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/emulated.rs`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     pub client_order_id: ClientOrderId,
     pub event_id: UUID4,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
 }
 
 impl OrderEmulated {
+    /// Creates a new [`OrderEmulated`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         event_id: UUID4,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/event.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/event.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/expired.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/expired.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::fmt::{Debug, Display};
 
 use derive_builder::Builder;
-use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
+use nautilus_core::{nanos::UnixNanos, serialization::from_bool_as_u8, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
     enums::{
         ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
         TriggerType,
@@ -54,14 +54,15 @@
     #[serde(deserialize_with = "from_bool_as_u8")]
     pub reconciliation: u8, // TODO: Change to bool once Cython removed
     pub venue_order_id: Option<VenueOrderId>,
     pub account_id: Option<AccountId>,
 }
 
 impl OrderExpired {
+    /// Creates a new [`OrderExpired`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         event_id: UUID4,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/filled.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/filled.rs`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     pub ts_init: UnixNanos,
     pub reconciliation: bool,
     pub position_id: Option<PositionId>,
     pub commission: Option<Money>,
 }
 
 impl OrderFilled {
+    /// Creates a new [`OrderFilled`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         venue_order_id: VenueOrderId,
@@ -119,14 +120,15 @@
     #[must_use]
     pub fn is_sell(&self) -> bool {
         self.order_side == OrderSide::Sell
     }
 }
 
 impl Default for OrderFilled {
+    /// Creates a new default [`OrderFilled`] instance for testing.
     fn default() -> Self {
         Self {
             trader_id: TraderId::default(),
             strategy_id: StrategyId::default(),
             instrument_id: InstrumentId::default(),
             client_order_id: ClientOrderId::default(),
             venue_order_id: VenueOrderId::default(),
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/initialized.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/initialized.rs`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     pub exec_algorithm_id: Option<ExecAlgorithmId>,
     pub exec_algorithm_params: Option<HashMap<Ustr, Ustr>>,
     pub exec_spawn_id: Option<ClientOrderId>,
     pub tags: Option<Vec<Ustr>>,
 }
 
 impl Default for OrderInitialized {
+    /// Creates a new default [`OrderInitialized`] instance for testing.
     fn default() -> Self {
         Self {
             trader_id: TraderId::default(),
             strategy_id: StrategyId::default(),
             instrument_id: InstrumentId::default(),
             client_order_id: ClientOrderId::default(),
             order_side: OrderSide::Buy,
@@ -120,14 +121,15 @@
             ts_init: Default::default(),
             reconciliation: Default::default(),
         }
     }
 }
 
 impl OrderInitialized {
+    /// Creates a new [`OrderInitialized`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         order_side: OrderSide,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/modify_rejected.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/modify_rejected.rs`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::fmt::{Debug, Display};
 
 use derive_builder::Builder;
-use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
+use nautilus_core::{nanos::UnixNanos, serialization::from_bool_as_u8, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
     enums::{
         ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
         TriggerType,
@@ -55,14 +55,15 @@
     #[serde(deserialize_with = "from_bool_as_u8")]
     pub reconciliation: u8, // TODO: Change to bool once Cython removed
     pub venue_order_id: Option<VenueOrderId>,
     pub account_id: Option<AccountId>,
 }
 
 impl OrderModifyRejected {
+    /// Creates a new [`OrderModifyRejected`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         reason: Ustr,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/pending_cancel.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/triggered.rs`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::fmt::{Debug, Display};
 
 use derive_builder::Builder;
-use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
+use nautilus_core::{nanos::UnixNanos, serialization::from_bool_as_u8, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
     enums::{
         ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
         TriggerType,
@@ -39,97 +39,102 @@
 #[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
-pub struct OrderPendingCancel {
+pub struct OrderTriggered {
     pub trader_id: TraderId,
     pub strategy_id: StrategyId,
     pub instrument_id: InstrumentId,
     pub client_order_id: ClientOrderId,
-    pub account_id: AccountId,
     pub event_id: UUID4,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
     #[serde(deserialize_with = "from_bool_as_u8")]
     pub reconciliation: u8, // TODO: Change to bool once Cython removed
     pub venue_order_id: Option<VenueOrderId>,
+    pub account_id: Option<AccountId>,
 }
 
-impl OrderPendingCancel {
+impl OrderTriggered {
+    /// Creates a new [`OrderTriggered`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
-        account_id: AccountId,
         event_id: UUID4,
         ts_event: UnixNanos,
         ts_init: UnixNanos,
         reconciliation: bool,
         venue_order_id: Option<VenueOrderId>,
+        account_id: Option<AccountId>,
     ) -> anyhow::Result<Self> {
         Ok(Self {
             trader_id,
             strategy_id,
             instrument_id,
             client_order_id,
-            account_id,
             event_id,
             ts_event,
             ts_init,
             reconciliation: u8::from(reconciliation),
             venue_order_id,
+            account_id,
         })
     }
 }
 
-impl Debug for OrderPendingCancel {
+impl Debug for OrderTriggered {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(f,
             "{}(trader_id={}, strategy_id={}, instrument_id={}, client_order_id={}, venue_order_id={}, account_id={}, event_id={}, ts_event={}, ts_init={})",
-            stringify!(OrderPendingCancel),
+            stringify!(OrderTriggered),
             self.trader_id,
             self.strategy_id,
             self.instrument_id,
             self.client_order_id,
-            self.venue_order_id.map_or_else(|| "None".to_string(), |venue_order_id| format!("{venue_order_id}")),
-            self.account_id,
+            self.venue_order_id.map_or("None".to_string(), |venue_order_id| format!("{venue_order_id}")),
+            self.account_id.map_or("None".to_string(), |account_id| format!("{account_id}")),
             self.event_id,
             self.ts_event,
             self.ts_init
         )
     }
 }
 
-impl Display for OrderPendingCancel {
+impl Display for OrderTriggered {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(
             f,
             "{}(instrument_id={}, client_order_id={}, venue_order_id={}, account_id={}, ts_event={})",
-            stringify!(OrderPendingCancel),
+            stringify!(OrderTriggered),
             self.instrument_id,
             self.client_order_id,
-            self.venue_order_id.map_or("None".to_string(), |venue_order_id| format!("{venue_order_id}")),
-            self.account_id,
-            self.ts_event
+            self.venue_order_id
+                .map_or("None".to_string(), |venue_order_id| format!(
+                    "{venue_order_id}"
+                )),
+            self.account_id
+                .map_or("None".to_string(), |account_id| format!("{account_id}")),
+            self.ts_event,
         )
     }
 }
 
-impl OrderEvent for OrderPendingCancel {
+impl OrderEvent for OrderTriggered {
     fn id(&self) -> UUID4 {
         self.event_id
     }
 
     fn kind(&self) -> &str {
-        stringify!(OrderPendingCancel)
+        stringify!(OrderTriggered)
     }
 
     fn order_type(&self) -> Option<OrderType> {
         None
     }
 
     fn order_side(&self) -> Option<OrderSide> {
@@ -265,15 +270,15 @@
     }
 
     fn venue_order_id(&self) -> Option<VenueOrderId> {
         self.venue_order_id
     }
 
     fn account_id(&self) -> Option<AccountId> {
-        Some(self.account_id)
+        self.account_id
     }
 
     fn position_id(&self) -> Option<PositionId> {
         None
     }
 
     fn commission(&self) -> Option<Money> {
@@ -292,18 +297,16 @@
 ////////////////////////////////////////////////////////////////////////////////
 // Tests
 ////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
 mod tests {
     use rstest::rstest;
 
-    use crate::events::order::{pending_cancel::OrderPendingCancel, stubs::*};
+    use crate::events::order::{stubs::*, triggered::OrderTriggered};
 
     #[rstest]
-    fn test_order_pending_cancel_display(order_pending_cancel: OrderPendingCancel) {
-        let display = format!("{order_pending_cancel}");
-        assert_eq!(
-            display,
-            "OrderPendingCancel(instrument_id=BTCUSDT.COINBASE, client_order_id=O-19700101-0000-000-001-1, venue_order_id=001, account_id=SIM-001, ts_event=0)"
-        );
+    fn test_order_triggered_display(order_triggered: OrderTriggered) {
+        let display = format!("{order_triggered}");
+        assert_eq!(display, "OrderTriggered(instrument_id=BTCUSDT.COINBASE, client_order_id=O-19700101-0000-000-001-1, \
+        venue_order_id=001, account_id=SIM-001, ts_event=0)");
     }
 }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/pending_update.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/pending_update.rs`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::fmt::{Debug, Display};
 
 use derive_builder::Builder;
-use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
+use nautilus_core::{nanos::UnixNanos, serialization::from_bool_as_u8, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
     enums::{
         ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
         TriggerType,
@@ -54,14 +54,15 @@
     pub ts_init: UnixNanos,
     #[serde(deserialize_with = "from_bool_as_u8")]
     pub reconciliation: u8, // TODO: Change to bool once Cython removed
     pub venue_order_id: Option<VenueOrderId>,
 }
 
 impl OrderPendingUpdate {
+    /// Creates a new [`OrderPendingUpdate`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         account_id: AccountId,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/rejected.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/rejected.rs`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::fmt::{Debug, Display};
 
 use derive_builder::Builder;
-use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
+use nautilus_core::{nanos::UnixNanos, serialization::from_bool_as_u8, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
     enums::{
         ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
         TriggerType,
@@ -54,14 +54,15 @@
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
     #[serde(deserialize_with = "from_bool_as_u8")]
     pub reconciliation: u8, // TODO: Change to bool once Cython removed
 }
 
 impl OrderRejected {
+    /// Creates a new [`OrderRejected`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         account_id: AccountId,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/released.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/released.rs`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     pub released_price: Price,
     pub event_id: UUID4,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
 }
 
 impl OrderReleased {
+    /// Creates a new [`OrderReleased`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         released_price: Price,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/stubs.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/stubs.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/submitted.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/submitted.rs`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     pub account_id: AccountId,
     pub event_id: UUID4,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
 }
 
 impl OrderSubmitted {
+    /// Creates a new [`OrderSubmitted`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         account_id: AccountId,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/order/triggered.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/order/updated.rs`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
 use std::fmt::{Debug, Display};
 
 use derive_builder::Builder;
-use nautilus_core::{deserialization::from_bool_as_u8, nanos::UnixNanos, uuid::UUID4};
+use nautilus_core::{nanos::UnixNanos, serialization::from_bool_as_u8, uuid::UUID4};
 use serde::{Deserialize, Serialize};
 use ustr::Ustr;
 
 use crate::{
     enums::{
         ContingencyType, LiquiditySide, OrderSide, OrderType, TimeInForce, TrailingOffsetType,
         TriggerType,
@@ -39,101 +39,114 @@
 #[derive(Clone, Copy, PartialEq, Eq, Default, Serialize, Deserialize, Builder)]
 #[builder(default)]
 #[serde(tag = "type")]
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
-pub struct OrderTriggered {
+pub struct OrderUpdated {
     pub trader_id: TraderId,
     pub strategy_id: StrategyId,
     pub instrument_id: InstrumentId,
     pub client_order_id: ClientOrderId,
+    pub venue_order_id: Option<VenueOrderId>,
+    pub account_id: Option<AccountId>,
+    pub quantity: Quantity,
+    pub price: Option<Price>,
+    pub trigger_price: Option<Price>,
     pub event_id: UUID4,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
     #[serde(deserialize_with = "from_bool_as_u8")]
     pub reconciliation: u8, // TODO: Change to bool once Cython removed
-    pub venue_order_id: Option<VenueOrderId>,
-    pub account_id: Option<AccountId>,
 }
 
-impl OrderTriggered {
+impl OrderUpdated {
+    /// Creates a new [`OrderUpdated`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
+        quantity: Quantity,
         event_id: UUID4,
         ts_event: UnixNanos,
         ts_init: UnixNanos,
         reconciliation: bool,
         venue_order_id: Option<VenueOrderId>,
         account_id: Option<AccountId>,
+        price: Option<Price>,
+        trigger_price: Option<Price>,
     ) -> anyhow::Result<Self> {
         Ok(Self {
             trader_id,
             strategy_id,
             instrument_id,
             client_order_id,
+            quantity,
             event_id,
             ts_event,
             ts_init,
             reconciliation: u8::from(reconciliation),
             venue_order_id,
             account_id,
+            price,
+            trigger_price,
         })
     }
 }
 
-impl Debug for OrderTriggered {
+impl Debug for OrderUpdated {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(f,
-            "{}(trader_id={}, strategy_id={}, instrument_id={}, client_order_id={}, venue_order_id={}, account_id={}, event_id={}, ts_event={}, ts_init={})",
-            stringify!(OrderTriggered),
+            "{}(trader_id={}, strategy_id={}, instrument_id={}, client_order_id={}, \
+            venue_order_id={}, account_id={}, quantity={}, price={}, trigger_price={}, event_id={}, ts_event={}, ts_init={})",
+            stringify!(OrderUpdated),
             self.trader_id,
             self.strategy_id,
             self.instrument_id,
             self.client_order_id,
             self.venue_order_id.map_or("None".to_string(), |venue_order_id| format!("{venue_order_id}")),
             self.account_id.map_or("None".to_string(), |account_id| format!("{account_id}")),
+            self.quantity,
+            self.price.map_or("None".to_string(), |price| price.to_formatted_string()),
+            self.trigger_price.map_or("None".to_string(), |trigger_price| trigger_price.to_formatted_string()),
             self.event_id,
             self.ts_event,
             self.ts_init
         )
     }
 }
 
-impl Display for OrderTriggered {
+impl Display for OrderUpdated {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(
             f,
-            "{}(instrument_id={}, client_order_id={}, venue_order_id={}, account_id={}, ts_event={})",
-            stringify!(OrderTriggered),
+            "{}(instrument_id={}, client_order_id={}, venue_order_id={}, account_id={}, quantity={}, price={}, trigger_price={}, ts_event={})",
+            stringify!(OrderUpdated),
             self.instrument_id,
             self.client_order_id,
-            self.venue_order_id
-                .map_or("None".to_string(), |venue_order_id| format!(
-                    "{venue_order_id}"
-                )),
-            self.account_id
-                .map_or("None".to_string(), |account_id| format!("{account_id}")),
-            self.ts_event,
+            self.venue_order_id.map_or("None".to_string(), |venue_order_id| format!("{venue_order_id}")),
+            self.account_id.map_or("None".to_string(), |account_id| format!("{account_id}")),
+            self.quantity.to_formatted_string(),
+            self.price.map_or("None".to_string(), |price| price.to_formatted_string()),
+            self.trigger_price.map_or("None".to_string(), |trigger_price| trigger_price.to_formatted_string()),
+            self.ts_event
         )
     }
 }
 
-impl OrderEvent for OrderTriggered {
+impl OrderEvent for OrderUpdated {
     fn id(&self) -> UUID4 {
         self.event_id
     }
 
     fn kind(&self) -> &str {
-        stringify!(OrderTriggered)
+        stringify!(OrderUpdated)
     }
 
     fn order_type(&self) -> Option<OrderType> {
         None
     }
 
     fn order_side(&self) -> Option<OrderSide> {
@@ -165,15 +178,15 @@
     }
 
     fn reason(&self) -> Option<Ustr> {
         None
     }
 
     fn quantity(&self) -> Option<Quantity> {
-        None
+        Some(self.quantity)
     }
 
     fn time_in_force(&self) -> Option<TimeInForce> {
         None
     }
 
     fn liquidity_side(&self) -> Option<LiquiditySide> {
@@ -193,27 +206,27 @@
     }
 
     fn reconciliation(&self) -> bool {
         false
     }
 
     fn price(&self) -> Option<Price> {
-        None
+        self.price
     }
 
     fn last_px(&self) -> Option<Price> {
         None
     }
 
     fn last_qty(&self) -> Option<Quantity> {
         None
     }
 
     fn trigger_price(&self) -> Option<Price> {
-        None
+        self.trigger_price
     }
 
     fn trigger_type(&self) -> Option<TriggerType> {
         None
     }
 
     fn limit_offset(&self) -> Option<Price> {
@@ -296,16 +309,18 @@
 ////////////////////////////////////////////////////////////////////////////////
 // Tests
 ////////////////////////////////////////////////////////////////////////////////
 #[cfg(test)]
 mod tests {
     use rstest::rstest;
 
-    use crate::events::order::{stubs::*, triggered::OrderTriggered};
+    use crate::events::order::{stubs::*, updated::OrderUpdated};
 
     #[rstest]
-    fn test_order_triggered_display(order_triggered: OrderTriggered) {
-        let display = format!("{order_triggered}");
-        assert_eq!(display, "OrderTriggered(instrument_id=BTCUSDT.COINBASE, client_order_id=O-19700101-0000-000-001-1, \
-        venue_order_id=001, account_id=SIM-001, ts_event=0)");
+    fn test_order_updated_display(order_updated: OrderUpdated) {
+        let display = format!("{order_updated}");
+        assert_eq!(
+            display,
+            "OrderUpdated(instrument_id=BTCUSDT.COINBASE, client_order_id=O-19700101-0000-000-001-1, venue_order_id=001, account_id=SIM-001, quantity=100, price=22_000, trigger_price=None, ts_event=0)"
+        );
     }
 }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/position/changed.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/position/changed.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/position/closed.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/position/closed.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/position/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/position/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/position/opened.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/position/opened.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/events/position/state.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/position/state.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/bar.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/data/bar.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/delta.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/data/delta.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/deltas.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/data/deltas.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/depth.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/data/depth.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orderbook/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-pub mod bar;
-pub mod delta;
-pub mod deltas;
-pub mod depth;
-pub mod order;
-pub mod quote;
-pub mod trade;
+//! Order book components which can handle L1/L2/L3 data.
+
+pub mod aggregation;
+pub mod analysis;
+pub mod book;
+pub mod display;
+pub mod error;
+pub mod ladder;
+pub mod level;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/order.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/data/order.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/quote.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/data/quote.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/data/trade.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/data/trade.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/enums.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/enums.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/events/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/account/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-pub mod order;
+pub mod state;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/events/order.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/events/order.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/account_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/account_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/client_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/client_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/client_order_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/client_order_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/component_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/component_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/exec_algorithm_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/exec_algorithm_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/instrument_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/instrument_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/order_list_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/order_list_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/position_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/position_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/strategy_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/strategy_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/symbol.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/symbol.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/trade_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/trade_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/trader_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/trader_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/venue.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/venue.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/identifiers/venue_order_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/identifiers/venue_order_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/instruments/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/instruments/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/instruments/synthetic.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/instruments/synthetic.rs`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 use crate::{
     identifiers::{instrument_id::InstrumentId, symbol::Symbol},
     instruments::synthetic::SyntheticInstrument,
     types::price::{Price, ERROR_PRICE},
 };
 
-/// Provides a C compatible Foreign Function Interface (FFI) for an underlying
+/// C compatible Foreign Function Interface (FFI) for an underlying
 /// [`SyntheticInstrument`].
 ///
 /// This struct wraps `SyntheticInstrument` in a way that makes it compatible with C function
 /// calls, enabling interaction with `SyntheticInstrument` in a C environment.
 ///
 /// It implements the `Deref` trait, allowing instances of `SyntheticInstrument_API` to be
 /// dereferenced to `SyntheticInstrument`, providing access to `SyntheticInstruments`'s methods without
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/mod.rs` & `nautilus_trader-1.194.0/nautilus_trader/backtest/execution_client.pxd`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-// -------------------------------------------------------------------------------------------------
-//  Copyright (C) 2015-2024 Nautech Systems Pty Ltd. All rights reserved.
-//  https://nautechsystems.io
-//
-//  Licensed under the GNU Lesser General Public License Version 3.0 (the "License");
-//  You may not use this file except in compliance with the License.
-//  You may obtain a copy of the License at https://www.gnu.org/licenses/lgpl-3.0.en.html
-//
-//  Unless required by applicable law or agreed to in writing, software
-//  distributed under the License is distributed on an "AS IS" BASIS,
-//  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-//  See the License for the specific language governing permissions and
-//  limitations under the License.
-// -------------------------------------------------------------------------------------------------
+# -------------------------------------------------------------------------------------------------
+#  Copyright (C) 2015-2024 Nautech Systems Pty Ltd. All rights reserved.
+#  https://nautechsystems.io
+#
+#  Licensed under the GNU Lesser General Public License Version 3.0 (the "License");
+#  You may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at https://www.gnu.org/licenses/lgpl-3.0.en.html
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+# -------------------------------------------------------------------------------------------------
 
-//! Provides a C foreign function interface (FFI) from `cbindgen`.
+from nautilus_trader.backtest.exchange cimport SimulatedExchange
+from nautilus_trader.execution.client cimport ExecutionClient
 
-pub mod data;
-pub mod enums;
-pub mod events;
-pub mod identifiers;
-pub mod instruments;
-pub mod orderbook;
-pub mod types;
+
+cdef class BacktestExecClient(ExecutionClient):
+    cdef SimulatedExchange _exchange
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/orderbook/book.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/orderbook/book.rs`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         aggregation::{update_book_with_quote_tick, update_book_with_trade_tick},
         analysis::book_check_integrity,
         book::OrderBook,
     },
     types::{price::Price, quantity::Quantity},
 };
 
-/// Provides a C compatible Foreign Function Interface (FFI) for an underlying `OrderBook`.
+/// C compatible Foreign Function Interface (FFI) for an underlying `OrderBook`.
 ///
 /// This struct wraps `OrderBook` in a way that makes it compatible with C function
 /// calls, enabling interaction with `OrderBook` in a C environment.
 ///
 /// It implements the `Deref` trait, allowing instances of `OrderBook_API` to be
 /// dereferenced to `OrderBook`, providing access to `OrderBook`'s methods without
 /// having to manually access the underlying `OrderBook` instance.
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/orderbook/level.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/orderbook/level.rs`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 use crate::{
     data::order::BookOrder,
     enums::OrderSide,
     orderbook::{ladder::BookPrice, level::Level},
     types::price::Price,
 };
 
-/// Provides a C compatible Foreign Function Interface (FFI) for an underlying order book[`Level`].
+/// C compatible Foreign Function Interface (FFI) for an underlying order book[`Level`].
 ///
 /// This struct wraps `Level` in a way that makes it compatible with C function
 /// calls, enabling interaction with `Level` in a C environment.
 ///
 /// It implements the `Deref` trait, allowing instances of `Level_API` to be
 /// dereferenced to `Level`, providing access to `Level`'s methods without
 /// having to manually acce wss the underlying `Level` instance.
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/orderbook/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/orderbook/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/currency.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/types/currency.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/types/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/money.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/types/money.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/price.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/types/price.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/ffi/types/quantity.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/ffi/types/quantity.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/account_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/account_id.rs`

 * *Files 7% similar despite different names*

```diff
@@ -9,45 +9,46 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Represents a valid account ID.
+
 use std::{
     fmt::{Debug, Display, Formatter},
     hash::Hash,
 };
 
 use nautilus_core::correctness::{check_string_contains, check_valid_string};
 use ustr::Ustr;
 
 use super::venue::Venue;
 
 /// Represents a valid account ID.
-///
-/// Must be correctly formatted with two valid strings either side of a hyphen '-'.
-/// It is expected an account ID is the name of the issuer with an account number
-/// separated by a hyphen.
-///
-/// Example: "IB-D02851908".
 #[repr(C)]
 #[derive(Clone, Copy, Hash, PartialEq, Eq, PartialOrd, Ord)]
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
 pub struct AccountId(Ustr);
 
 impl AccountId {
-    /// Creates a new `AccountId` instance from the given identifier value.
+    /// Creates a new [`AccountId`] instance.
+    ///
+    /// Must be correctly formatted with two valid strings either side of a hyphen '-'.
+    /// It is expected an account ID is the name of the issuer with an account number
+    /// separated by a hyphen.
     ///
+    /// Example: "IB-D02851908".
     /// # Panics
     ///
-    /// Panics if the value is not a valid string, or does not contain a hyphen '-' separator.
+    /// Panics if `value` is not a valid string, or does not contain a hyphen '-' separator.
     pub fn new(value: &str) -> anyhow::Result<Self> {
         check_valid_string(value, stringify!(value))?;
         check_string_contains(value, "-", stringify!(value))?;
 
         Ok(Self(Ustr::from(value)))
     }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/client_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/client_id.rs`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Represents a system client ID.
+
 use std::{
     fmt::{Debug, Display, Formatter},
     hash::Hash,
 };
 
 use nautilus_core::correctness::check_valid_string;
 use ustr::Ustr;
@@ -27,19 +29,19 @@
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
 pub struct ClientId(Ustr);
 
 impl ClientId {
-    /// Creates a new `ClientId` instance from the given identifier value.
+    /// Creates a new [`ClientId`] instance.
     ///
     /// # Panics
     ///
-    /// Panics if the value is not a valid string.
+    /// Panics if `value` is not a valid string.
     pub fn new(value: &str) -> anyhow::Result<Self> {
         check_valid_string(value, stringify!(value))?;
 
         Ok(Self(Ustr::from(value)))
     }
 
     /// Sets the inner identifier value.
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/client_order_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/client_order_id.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Represents a valid client order ID (assigned by the Nautilus system).
+
 use std::{
     fmt::{Debug, Display, Formatter},
     hash::Hash,
 };
 
 use nautilus_core::correctness::check_valid_string;
 use ustr::Ustr;
@@ -27,19 +29,19 @@
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
 pub struct ClientOrderId(Ustr);
 
 impl ClientOrderId {
-    /// Creates a new `ClientOrderId` instance from the given identifier value.
+    /// Creates a new [`ClientOrderId`] instance.
     ///
     /// # Panics
     ///
-    /// Panics if the value is not a valid string.
+    /// Panics if `value` is not a valid string.
     pub fn new(value: &str) -> anyhow::Result<Self> {
         check_valid_string(value, stringify!(value))?;
 
         Ok(Self(Ustr::from(value)))
     }
 
     /// Sets the inner identifier value.
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/component_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/component_id.rs`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Represents a valid component ID.
+
 use std::{
     fmt::{Debug, Display, Formatter},
     hash::Hash,
 };
 
 use nautilus_core::correctness::check_valid_string;
 use ustr::Ustr;
@@ -27,19 +29,19 @@
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
 pub struct ComponentId(Ustr);
 
 impl ComponentId {
-    /// Creates a new `ComponentId` instance from the given identifier value.
+    /// Creates a new [`ComponentId`] instance.
     ///
     /// # Panics
     ///
-    /// Panics if the value is not a valid string.
+    /// Panics if `value` is not a valid string.
     pub fn new(value: &str) -> anyhow::Result<Self> {
         check_valid_string(value, stringify!(value))?;
 
         Ok(Self(Ustr::from(value)))
     }
 
     /// Sets the inner identifier value.
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/exec_algorithm_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/exec_algorithm_id.rs`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Represents a valid execution algorithm ID.
+
 use std::{
     fmt::{Debug, Display, Formatter},
     hash::Hash,
 };
 
 use nautilus_core::correctness::check_valid_string;
 use ustr::Ustr;
@@ -27,19 +29,19 @@
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
 pub struct ExecAlgorithmId(Ustr);
 
 impl ExecAlgorithmId {
-    /// Creates a new `ExecAlgorithmId` instance from the given identifier value.
+    /// Creates a new [`ExecAlgorithmId`] instance.
     ///
     /// # Panics
     ///
-    /// Panics if the value is not a valid string.
+    /// Panics if `value` is not a valid string.
     pub fn new(value: &str) -> anyhow::Result<Self> {
         check_valid_string(value, stringify!(value))?;
 
         Ok(Self(Ustr::from(value)))
     }
 
     /// Sets the inner identifier value.
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/instrument_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/instrument_id.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Represents a valid instrument ID.
+
 use std::{
     fmt::{Debug, Display, Formatter},
     hash::Hash,
     str::FromStr,
 };
 
 use serde::{Deserialize, Deserializer, Serialize};
@@ -36,15 +38,15 @@
     /// The instruments ticker symbol.
     pub symbol: Symbol,
     /// The instruments trading venue.
     pub venue: Venue,
 }
 
 impl InstrumentId {
-    /// Creates a new `InstrumentId` instance from the given `Symbol` and `Venue`.
+    /// Creates a new [`InstrumentId`] instance.
     #[must_use]
     pub fn new(symbol: Symbol, venue: Venue) -> Self {
         Self { symbol, venue }
     }
 
     #[must_use]
     pub fn is_synthetic(&self) -> bool {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/macros.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/macros.rs`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Provides macros for generating identifier functionality.
+
 macro_rules! impl_serialization_for_identifier {
     ($ty:ty) => {
         impl Serialize for $ty {
             fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
             where
                 S: Serializer,
             {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines identifiers for the trading domain models.
+//! Identifiers for the trading domain model.
 
 use std::str::FromStr;
 
 use serde::{Deserialize, Deserializer, Serialize, Serializer};
 
 #[macro_use]
 mod macros;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/order_list_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/order_list_id.rs`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Represents a valid order list ID (assigned by the Nautilus system).
+
 use std::{
     fmt::{Debug, Display, Formatter},
     hash::Hash,
 };
 
 use nautilus_core::correctness::check_valid_string;
 use ustr::Ustr;
@@ -27,19 +29,19 @@
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
 pub struct OrderListId(Ustr);
 
 impl OrderListId {
-    /// Creates a new `OrderListId` instance from the given identifier value.
+    /// Creates a new [`OrderListId`] instance.
     ///
     /// # Panics
     ///
-    /// Panics if the value is not a valid string.
+    /// Panics if `value` is not a valid string.
     pub fn new(value: &str) -> anyhow::Result<Self> {
         check_valid_string(value, stringify!(value))?;
 
         Ok(Self(Ustr::from(value)))
     }
 
     /// Sets the inner identifier value.
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/position_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/position_id.rs`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Represents a valid position ID.
+
 use std::{
     fmt::{Debug, Display, Formatter},
     hash::Hash,
 };
 
 use nautilus_core::correctness::check_valid_string;
 use ustr::Ustr;
@@ -27,19 +29,19 @@
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
 pub struct PositionId(Ustr);
 
 impl PositionId {
-    /// Creates a new `PositionId` instance from the given identifier value.
+    /// Creates a new [`PositionId`] instance.
     ///
     /// # Panics
     ///
-    /// Panics if the value is not a valid string.
+    /// Panics if `value` is not a valid string.
     pub fn new(value: &str) -> anyhow::Result<Self> {
         check_valid_string(value, stringify!(value))?;
 
         Ok(Self(Ustr::from(value)))
     }
 
     /// Sets the inner identifier value.
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/strategy_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/strategy_id.rs`

 * *Files 12% similar despite different names*

```diff
@@ -9,46 +9,48 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Represents a valid strategy ID.
+
 use std::fmt::{Debug, Display, Formatter};
 
 use nautilus_core::correctness::{check_string_contains, check_valid_string};
 use ustr::Ustr;
 
 /// The identifier for all 'external' strategy IDs (not local to this system instance).
 const EXTERNAL_STRATEGY_ID: &str = "EXTERNAL";
 
 /// Represents a valid strategy ID.
-///
-/// Must be correctly formatted with two valid strings either side of a hyphen.
-/// It is expected a strategy ID is the class name of the strategy,
-/// with an order ID tag number separated by a hyphen.
-///
-/// Example: "EMACross-001".
-///
-/// The reason for the numerical component of the ID is so that order and position IDs
-/// do not collide with those from another strategy within the node instance.
 #[repr(C)]
 #[derive(Clone, Copy, Hash, PartialEq, Eq, PartialOrd, Ord)]
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
 pub struct StrategyId(Ustr);
 
 impl StrategyId {
-    /// Creates a new `StrategyId` instance from the given identifier value.
+    /// Creates a new [`StrategyId`] instance.
+    ///
+    /// Must be correctly formatted with two valid strings either side of a hyphen.
+    /// It is expected a strategy ID is the class name of the strategy,
+    /// with an order ID tag number separated by a hyphen.
+    ///
+    /// Example: "EMACross-001".
+    ///
+    /// The reason for the numerical component of the ID is so that order and position IDs
+    /// do not collide with those from another strategy within the node instance.
     ///
     /// # Panics
     ///
-    /// Panics if the value is not a valid string, or does not contain a hyphen '-' separator.
+    /// Panics if `value` is not a valid string, or does not contain a hyphen '-' separator.
     pub fn new(value: &str) -> anyhow::Result<Self> {
         check_valid_string(value, stringify!(value))?;
         if value != EXTERNAL_STRATEGY_ID {
             check_string_contains(value, "-", stringify!(value))?;
         }
 
         Ok(Self(Ustr::from(value)))
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/stubs.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/stubs.rs`

 * *Files 20% similar despite different names*

```diff
@@ -9,79 +9,91 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Default implementations and fixture functions to provide stub identifiers for testing.
+
 use nautilus_core::uuid::UUID4;
 use rstest::fixture;
 
 use crate::identifiers::{
     account_id::AccountId, client_id::ClientId, client_order_id::ClientOrderId,
     component_id::ComponentId, exec_algorithm_id::ExecAlgorithmId, instrument_id::InstrumentId,
     order_list_id::OrderListId, position_id::PositionId, strategy_id::StrategyId, symbol::Symbol,
     trade_id::TradeId, trader_id::TraderId, venue::Venue, venue_order_id::VenueOrderId,
 };
 
 impl Default for AccountId {
+    /// Creates a new default [`AccountId`] instance for testing.
     fn default() -> Self {
         Self::from("SIM-001")
     }
 }
 
 impl Default for ClientId {
+    /// Creates a new default [`ClientId`] instance for testing.
     fn default() -> Self {
         Self::from("SIM")
     }
 }
 
 impl Default for ClientOrderId {
+    /// Creates a new default [`ClientOrderId`] instance for testing.
     fn default() -> Self {
         Self::from("O-19700101-0000-000-001-1")
     }
 }
 
 impl Default for PositionId {
+    /// Creates a new default [`PositionId`] instance for testing.
     fn default() -> Self {
         Self::from("P-001")
     }
 }
 
 impl Default for StrategyId {
+    /// Creates a new default [`StrategyId`] instance for testing.
     fn default() -> Self {
         Self::from("S-001")
     }
 }
 
 impl Default for Symbol {
+    /// Creates a new default [`Symbol`] instance for testing.
     fn default() -> Self {
         Self::from("AUD/USD")
     }
 }
 
 impl Default for TradeId {
+    /// Creates a new default [`TradeId`] instance for testing.
     fn default() -> Self {
         Self::from("1")
     }
 }
 
 impl Default for TraderId {
+    /// Creates a new default [`TraderId`] instance for testing.
     fn default() -> Self {
         Self::from("TRADER-000")
     }
 }
 
 impl Default for Venue {
+    /// Creates a new default [`Venue`] instance for testing.
     fn default() -> Self {
         Self::from("SIM")
     }
 }
 
 impl Default for VenueOrderId {
+    /// Creates a new default [`VenueOrderId`] instance for testing.
     fn default() -> Self {
         Self::from("001")
     }
 }
 
 // ---- AccountId ----
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/symbol.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/symbol.rs`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Represents a valid ticker symbol ID for a tradable instrument.
+
 use std::{
     fmt::{Debug, Display, Formatter},
     hash::Hash,
 };
 
 use nautilus_core::correctness::check_valid_string;
 use ustr::Ustr;
@@ -27,19 +29,19 @@
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
 pub struct Symbol(Ustr);
 
 impl Symbol {
-    /// Creates a new `Symbol` instance from the given identifier value.
+    /// Creates a new [`Symbol`] instance.
     ///
     /// # Panics
     ///
-    /// Panics if the value is not a valid string.
+    /// Panics if `value` is not a valid string.
     pub fn new(value: &str) -> anyhow::Result<Self> {
         check_valid_string(value, stringify!(value))?;
 
         Ok(Self(Ustr::from(value)))
     }
 
     /// Sets the inner identifier value.
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/trade_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/trade_id.rs`

 * *Files 6% similar despite different names*

```diff
@@ -9,51 +9,53 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Represents a valid trade match ID (assigned by a trading venue).
+
 use std::{
     ffi::{CStr, CString},
     fmt::{Debug, Display, Formatter},
     hash::Hash,
 };
 
 use nautilus_core::correctness::{check_in_range_inclusive_usize, check_valid_string};
 use serde::{Deserialize, Deserializer, Serialize};
 
 /// The maximum length of ASCII characters for a `TradeId` string value (including null terminator).
 const TRADE_ID_LEN: usize = 37;
 
 /// Represents a valid trade match ID (assigned by a trading venue).
 ///
-/// Maximum length is 36 characters.
-///
-/// The unique ID assigned to the trade entity once it is received or matched by
-/// the exchange or central counterparty.
-///
 /// Can correspond to the `TradeID <1003> field` of the FIX protocol.
 #[repr(C)]
 #[derive(Clone, Copy, Debug, Hash, PartialEq, Eq, PartialOrd, Ord)]
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
 pub struct TradeId {
     /// The trade match ID value as a fixed-length C string byte array (includes null terminator).
     pub(crate) value: [u8; 37], // cbindgen issue using the constant in the array
 }
 
 impl TradeId {
-    /// Creates a new `TradeId` instance from the given identifier value.
+    /// Creates a new [`TradeId`] instance.
+    ///
+    /// Maximum length is 36 characters.
+    ///
+    /// The unique ID assigned to the trade entity once it is received or matched by
+    /// the exchange or central counterparty.
     ///
     /// # Panics
     ///
-    /// Panics if the value is not a valid string, or value length is greater than 36.
+    /// Panics if `value` is not a valid string, or value length is greater than 36.
     pub fn new(value: &str) -> anyhow::Result<Self> {
         let cstr = CString::new(value).expect("`CString` conversion failed");
         Self::from_cstr(cstr)
     }
 
     pub fn from_cstr(cstr: CString) -> anyhow::Result<Self> {
         let bytes = cstr.as_bytes_with_nul();
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/trader_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/trader_id.rs`

 * *Files 12% similar despite different names*

```diff
@@ -9,43 +9,45 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Represents a valid trader ID.
+
 use std::fmt::{Debug, Display, Formatter};
 
 use nautilus_core::correctness::{check_string_contains, check_valid_string};
 use ustr::Ustr;
 
 /// Represents a valid trader ID.
-///
-/// Must be correctly formatted with two valid strings either side of a hyphen.
-/// It is expected a trader ID is the abbreviated name of the trader
-/// with an order ID tag number separated by a hyphen.
-///
-/// Example: "TESTER-001".
-
-/// The reason for the numerical component of the ID is so that order and position IDs
-/// do not collide with those from another node instance.
 #[repr(C)]
 #[derive(Clone, Copy, Hash, PartialEq, Eq, PartialOrd, Ord)]
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
 pub struct TraderId(Ustr);
 
 impl TraderId {
-    /// Creates a new `TraderId` instance from the given identifier value.
+    /// Creates a new [`TraderId`] instance.
+    ///
+    /// Must be correctly formatted with two valid strings either side of a hyphen.
+    /// It is expected a trader ID is the abbreviated name of the trader
+    /// with an order ID tag number separated by a hyphen.
+    ///
+    /// Example: "TESTER-001".
+    ///
+    /// The reason for the numerical component of the ID is so that order and position IDs
+    /// do not collide with those from another node instance.
     ///
     /// # Panics
     ///
-    /// Panics if the value is not a valid string, or does not contain a hyphen '-' separator.
+    /// Panics if `value` is not a valid string, or does not contain a hyphen '-' separator.
     pub fn new(value: &str) -> anyhow::Result<Self> {
         check_valid_string(value, stringify!(value))?;
         check_string_contains(value, "-", stringify!(value))?;
 
         Ok(Self(Ustr::from(value)))
     }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/venue.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/venue.rs`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Represents a valid trading venue ID.
+
 use std::{
     fmt::{Debug, Display, Formatter},
     hash::Hash,
 };
 
 use nautilus_core::correctness::check_valid_string;
 use ustr::Ustr;
@@ -31,19 +33,19 @@
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
 pub struct Venue(Ustr);
 
 impl Venue {
-    /// Creates a new `Venue` instance from the given identifier value.
+    /// Creates a new [`Venue`] instance.
     ///
     /// # Panics
     ///
-    /// Panics if the value is not a valid string.
+    /// Panics if `value` is not a valid string.
     pub fn new(value: &str) -> anyhow::Result<Self> {
         check_valid_string(value, stringify!(value))?;
 
         Ok(Self(Ustr::from(value)))
     }
 
     /// Sets the inner identifier value.
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/identifiers/venue_order_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/identifiers/venue_order_id.rs`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Represents a valid venue order ID (assigned by a trading venue).
+
 use std::{
     fmt::{Debug, Display, Formatter},
     hash::Hash,
 };
 
 use nautilus_core::correctness::check_valid_string;
 use ustr::Ustr;
@@ -27,19 +29,19 @@
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
 pub struct VenueOrderId(Ustr);
 
 impl VenueOrderId {
-    /// Creates a new `VenueOrderId` instance from the given identifier value.
+    /// Creates a new [`VenueOrderId`] instance.
     ///
     /// # Panics
     ///
-    /// Panics if the value is not a valid string.
+    /// Panics if `value` is not a valid string.
     pub fn new(value: &str) -> anyhow::Result<Self> {
         check_valid_string(value, stringify!(value))?;
 
         Ok(Self(Ustr::from(value)))
     }
 
     /// Sets the inner identifier value.
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/any.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/instruments/any.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/crypto_future.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/instruments/crypto_future.rs`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     pub max_price: Option<Price>,
     pub min_price: Option<Price>,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
 }
 
 impl CryptoFuture {
+    /// Creates a new [`CryptoFuture`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         id: InstrumentId,
         raw_symbol: Symbol,
         underlying: Currency,
         quote_currency: Currency,
         settlement_currency: Currency,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/crypto_perpetual.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/instruments/crypto_perpetual.rs`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     pub max_price: Option<Price>,
     pub min_price: Option<Price>,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
 }
 
 impl CryptoPerpetual {
+    /// Creates a new [`CryptoPerpetual`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         id: InstrumentId,
         raw_symbol: Symbol,
         base_currency: Currency,
         quote_currency: Currency,
         settlement_currency: Currency,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/currency_pair.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/instruments/currency_pair.rs`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     pub max_price: Option<Price>,
     pub min_price: Option<Price>,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
 }
 
 impl CurrencyPair {
+    /// Creates a new [`CurrencyPair`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         id: InstrumentId,
         raw_symbol: Symbol,
         base_currency: Currency,
         quote_currency: Currency,
         price_precision: u8,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/equity.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/instruments/equity.rs`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     pub max_price: Option<Price>,
     pub min_price: Option<Price>,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
 }
 
 impl Equity {
+    /// Creates a new [`Equity`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         id: InstrumentId,
         raw_symbol: Symbol,
         isin: Option<Ustr>,
         currency: Currency,
         price_precision: u8,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/futures_contract.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/instruments/futures_contract.rs`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     pub max_price: Option<Price>,
     pub min_price: Option<Price>,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
 }
 
 impl FuturesContract {
+    /// Creates a new [`FuturesContract`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         id: InstrumentId,
         raw_symbol: Symbol,
         asset_class: AssetClass,
         exchange: Option<Ustr>,
         underlying: Ustr,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/futures_spread.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/instruments/futures_spread.rs`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     pub max_price: Option<Price>,
     pub min_price: Option<Price>,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
 }
 
 impl FuturesSpread {
+    /// Creates a new [`FuturesSpread`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         id: InstrumentId,
         raw_symbol: Symbol,
         asset_class: AssetClass,
         exchange: Option<Ustr>,
         underlying: Ustr,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/instruments/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines instrument definitions for the trading domain models.
+//! Instrument definitions for the trading domain model.
 
 pub mod any;
 pub mod crypto_future;
 pub mod crypto_perpetual;
 pub mod currency_pair;
 pub mod equity;
 pub mod futures_contract;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/options_contract.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/instruments/options_contract.rs`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     pub max_price: Option<Price>,
     pub min_price: Option<Price>,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
 }
 
 impl OptionsContract {
+    /// Creates a new [`OptionsContract`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         id: InstrumentId,
         raw_symbol: Symbol,
         asset_class: AssetClass,
         exchange: Option<Ustr>,
         underlying: Ustr,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/options_spread.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/instruments/options_spread.rs`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     pub max_price: Option<Price>,
     pub min_price: Option<Price>,
     pub ts_event: UnixNanos,
     pub ts_init: UnixNanos,
 }
 
 impl OptionsSpread {
+    /// Creates a new [`OptionsSpread`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         id: InstrumentId,
         raw_symbol: Symbol,
         asset_class: AssetClass,
         exchange: Option<Ustr>,
         underlying: Ustr,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/stubs.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/instruments/stubs.rs`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         currency_pair::CurrencyPair, equity::Equity, futures_contract::FuturesContract,
         options_contract::OptionsContract,
     },
     types::{currency::Currency, money::Money, price::Price, quantity::Quantity},
 };
 
 impl Default for SyntheticInstrument {
+    /// Creates a new default [`SyntheticInstrument`] instance for testing.
     fn default() -> Self {
         let btc_binance = InstrumentId::from("BTC.BINANCE");
         let ltc_binance = InstrumentId::from("LTC.BINANCE");
         let formula = "(BTC.BINANCE + LTC.BINANCE) / 2.0".to_string();
         SyntheticInstrument::new(
             Symbol::new("BTC-LTC").unwrap(),
             2,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/instruments/synthetic.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/instruments/synthetic.rs`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     pub ts_init: UnixNanos,
     context: HashMapContext,
     variables: Vec<String>,
     operator_tree: Node,
 }
 
 impl SyntheticInstrument {
+    /// Creates a new [`SyntheticInstrument`] instance.
     pub fn new(
         symbol: Symbol,
         price_precision: u8,
         components: Vec<InstrumentId>,
         formula: String,
         ts_event: UnixNanos,
         ts_init: UnixNanos,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/lib.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/macros.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/python/mod.rs`

 * *Files 26% similar despite different names*

```diff
@@ -9,32 +9,29 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Model specific macros.
+//! Python bindings from `pyo3`.
 
-#[macro_export]
-macro_rules! enum_strum_serde {
-    ($type:ty) => {
-        impl Serialize for $type {
-            fn serialize<S>(&self, serializer: S) -> Result<S::Ok, S::Error>
-            where
-                S: Serializer,
-            {
-                serializer.serialize_str(&self.to_string())
-            }
-        }
+#![allow(warnings)] // non-local `impl` definition, temporary allow until pyo3 upgrade
 
-        impl<'de> Deserialize<'de> for $type {
-            fn deserialize<D>(deserializer: D) -> Result<Self, D::Error>
-            where
-                D: Deserializer<'de>,
-            {
-                let s = String::deserialize(deserializer)?;
-                <$type>::from_str(&s).map_err(serde::de::Error::custom)
-            }
-        }
-    };
+use pyo3::prelude::*;
+
+pub mod backend;
+pub mod wranglers;
+
+/// Loaded as nautilus_pyo3.persistence
+#[pymodule]
+pub fn persistence(_: Python<'_>, m: &PyModule) -> PyResult<()> {
+    m.add_class::<crate::backend::session::DataBackendSession>()?;
+    m.add_class::<crate::backend::session::DataQueryResult>()?;
+    m.add_class::<backend::session::NautilusDataType>()?;
+    m.add_class::<backend::transformer::DataTransformer>()?;
+    m.add_class::<wranglers::bar::BarDataWrangler>()?;
+    m.add_class::<wranglers::delta::OrderBookDeltaDataWrangler>()?;
+    m.add_class::<wranglers::quote::QuoteTickDataWrangler>()?;
+    m.add_class::<wranglers::trade::TradeTickDataWrangler>()?;
+    Ok(())
 }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/aggregation.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orderbook/aggregation.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Functions related to normalizing and processing top-of-book events.
+
 use nautilus_core::nanos::UnixNanos;
 
 use super::{book::OrderBook, error::InvalidBookOperation};
 use crate::{
     data::{order::BookOrder, quote::QuoteTick, trade::TradeTick},
     enums::{BookType, OrderSide, RecordFlag},
 };
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/analysis.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orderbook/analysis.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Functions related to order book analysis.
+
 use std::collections::BTreeMap;
 
 use super::{book::OrderBook, ladder::BookPrice, level::Level};
 use crate::{
     enums::{BookType, OrderSide},
     orderbook::error::BookIntegrityError,
     types::{price::Price, quantity::Quantity},
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/book.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orderbook/book.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,33 +9,35 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! A performant, generic, multi-purpose order book.
+
 use nautilus_core::nanos::UnixNanos;
 
 use super::{aggregation::pre_process_order, analysis, display::pprint_book, level::Level};
 use crate::{
     data::{
         delta::OrderBookDelta, deltas::OrderBookDeltas, depth::OrderBookDepth10, order::BookOrder,
     },
     enums::{BookAction, BookType, OrderSide, OrderSideSpecified},
     identifiers::instrument_id::InstrumentId,
     orderbook::{error::BookIntegrityError, ladder::Ladder},
     types::{price::Price, quantity::Quantity},
 };
 
-/// Provides an order book.
+/// Provides a performant, generic, multi-purpose order book.
 ///
 /// Can handle the following granularity data:
-/// - MBO (market by order) / L3
-/// - MBP (market by price) / L2 aggregated order per level
-/// - MBP (market by price) / L1 top-of-book only
+/// - MBO (market-by-order) / L3
+/// - MBP (market-by-price) / L2 aggregated order per level
+/// - MBP (market-by-price) / L1 top-of-book only
 #[derive(Clone, Debug)]
 #[cfg_attr(
     feature = "python",
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
 pub struct OrderBook {
     /// The order book type (MBP types will aggregate orders).
@@ -49,14 +51,15 @@
     /// The current count of events applied to the order book.
     pub count: u64,
     pub(crate) bids: Ladder,
     pub(crate) asks: Ladder,
 }
 
 impl OrderBook {
+    /// Creates a new [`OrderBook`] instance.
     #[must_use]
     pub fn new(book_type: BookType, instrument_id: InstrumentId) -> Self {
         Self {
             book_type,
             instrument_id,
             sequence: 0,
             ts_last: UnixNanos::default(),
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/display.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orderbook/display.rs`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Functions related to order book display.
+
 use tabled::{settings::Style, Table, Tabled};
 
 use super::{ladder::BookPrice, level::Level};
 use crate::orderbook::ladder::Ladder;
 
 #[derive(Tabled)]
 struct OrderLevelDisplay {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/error.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orderbook/error.rs`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Errors associated with order book operations and integrity.
+
 use nautilus_core::nanos::UnixNanos;
 
 use super::ladder::BookPrice;
 use crate::enums::{BookType, OrderSide};
 
 #[derive(thiserror::Error, Debug)]
 pub enum InvalidBookOperation {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/ladder.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orderbook/ladder.rs`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Represents a ladder of price levels for one side of an order book.
+
 use std::{
     cmp::Ordering,
     collections::{BTreeMap, HashMap},
     fmt::{Display, Formatter},
 };
 
 use nautilus_core::nanos::UnixNanos;
@@ -71,15 +73,15 @@
 
 impl Display for BookPrice {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.value)
     }
 }
 
-/// Represents one side of an order book as a ladder of price levels.
+/// Represents a ladder of price levels for one side of an order book.
 #[derive(Clone, Debug)]
 pub struct Ladder {
     pub side: OrderSide,
     pub levels: BTreeMap<BookPrice, Level>,
     pub cache: HashMap<u64, BookPrice>,
 }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/level.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orderbook/level.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
+//! Represents a discrete price level in an order book.
+
 use std::{cmp::Ordering, collections::BTreeMap};
 
 use nautilus_core::nanos::UnixNanos;
 
 use crate::{
     data::order::{BookOrder, OrderId},
     orderbook::{error::BookIntegrityError, ladder::BookPrice},
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orderbook/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/common/src/ffi/mod.rs`

 * *Files 13% similar despite different names*

```diff
@@ -9,16 +9,13 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides a generic order book which can handle L1/L2/L3 data.
+//! C foreign function interface (FFI) from `cbindgen`.
 
-pub mod aggregation;
-pub mod analysis;
-pub mod book;
-pub mod display;
-pub mod error;
-pub mod ladder;
-pub mod level;
+pub mod clock;
+pub mod enums;
+pub mod logging;
+pub mod timer;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orders/any.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orders/any.rs`

 * *Files 4% similar despite different names*

```diff
@@ -25,26 +25,27 @@
     market_to_limit::MarketToLimitOrder,
     stop_limit::StopLimitOrder,
     stop_market::StopMarketOrder,
     trailing_stop_limit::TrailingStopLimitOrder,
     trailing_stop_market::TrailingStopMarketOrder,
 };
 use crate::{
-    enums::{OrderSide, OrderSideSpecified, TriggerType},
+    enums::{OrderSide, OrderSideSpecified, OrderStatus, TriggerType},
     events::order::event::OrderEventAny,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
         instrument_id::InstrumentId, position_id::PositionId, strategy_id::StrategyId,
         trader_id::TraderId, venue_order_id::VenueOrderId,
     },
     polymorphism::{
         ApplyOrderEventAny, GetAccountId, GetClientOrderId, GetEmulationTrigger,
         GetExecAlgorithmId, GetExecSpawnId, GetInstrumentId, GetLimitPrice, GetOrderFilledQty,
-        GetOrderLeavesQty, GetOrderQuantity, GetOrderSide, GetOrderSideSpecified, GetPositionId,
-        GetStopPrice, GetStrategyId, GetTraderId, GetVenueOrderId, IsClosed, IsInflight, IsOpen,
+        GetOrderLeavesQty, GetOrderQuantity, GetOrderSide, GetOrderSideSpecified, GetOrderStatus,
+        GetPositionId, GetStopPrice, GetStrategyId, GetTraderId, GetVenueOrderId, IsClosed,
+        IsInflight, IsOpen,
     },
     types::{price::Price, quantity::Quantity},
 };
 
 #[derive(Clone, Debug, Serialize, Deserialize)]
 pub enum OrderAny {
     Limit(LimitOrder),
@@ -308,14 +309,30 @@
             Self::StopMarket(order) => order.quantity,
             Self::TrailingStopLimit(order) => order.quantity,
             Self::TrailingStopMarket(order) => order.quantity,
         }
     }
 }
 
+impl GetOrderStatus for OrderAny {
+    fn status(&self) -> OrderStatus {
+        match self {
+            Self::Limit(order) => order.status,
+            Self::LimitIfTouched(order) => order.status,
+            Self::Market(order) => order.status,
+            Self::MarketIfTouched(order) => order.status,
+            Self::MarketToLimit(order) => order.status,
+            Self::StopLimit(order) => order.status,
+            Self::StopMarket(order) => order.status,
+            Self::TrailingStopLimit(order) => order.status,
+            Self::TrailingStopMarket(order) => order.status,
+        }
+    }
+}
+
 impl GetOrderFilledQty for OrderAny {
     fn filled_qty(&self) -> Quantity {
         match self {
             Self::Limit(order) => order.filled_qty(),
             Self::LimitIfTouched(order) => order.filled_qty(),
             Self::Market(order) => order.filled_qty(),
             Self::MarketIfTouched(order) => order.filled_qty(),
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orders/base.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orders/base.rs`

 * *Files 1% similar despite different names*

```diff
@@ -311,32 +311,38 @@
                 | OrderStatus::Canceled
                 | OrderStatus::Expired
                 | OrderStatus::Filled
         )
     }
 
     fn is_inflight(&self) -> bool {
-        self.emulation_trigger().is_none()
-            && matches!(
-                self.status(),
-                OrderStatus::Submitted | OrderStatus::PendingCancel | OrderStatus::PendingUpdate
-            )
+        if let Some(emulation_trigger) = self.emulation_trigger() {
+            if emulation_trigger != TriggerType::NoTrigger {
+                return false;
+            }
+        }
+
+        matches!(
+            self.status(),
+            OrderStatus::Submitted | OrderStatus::PendingCancel | OrderStatus::PendingUpdate
+        )
     }
 
     fn is_pending_update(&self) -> bool {
         self.status() == OrderStatus::PendingUpdate
     }
 
     fn is_pending_cancel(&self) -> bool {
         self.status() == OrderStatus::PendingCancel
     }
 
     fn is_spawned(&self) -> bool {
-        self.exec_algorithm_id().is_some()
-            && self.exec_spawn_id().unwrap() != self.client_order_id()
+        self.exec_spawn_id().map_or(false, |exec_spawn_id| {
+            exec_spawn_id != self.client_order_id()
+        })
     }
 }
 
 impl<T> From<&T> for OrderInitialized
 where
     T: Order,
 {
@@ -417,14 +423,15 @@
     pub slippage: Option<f64>,
     pub init_id: UUID4,
     pub ts_init: UnixNanos,
     pub ts_last: UnixNanos,
 }
 
 impl OrderCore {
+    /// Creates a new [`OrderCore`] instance.
     pub fn new(init: OrderInitialized) -> anyhow::Result<Self> {
         let events: Vec<OrderEventAny> = vec![OrderEventAny::Initialized(init.clone())];
         Ok(Self {
             events,
             commissions: HashMap::new(),
             venue_order_ids: Vec::new(),
             trade_ids: Vec::new(),
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orders/default.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orders/default.rs`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     identifiers::{
         client_order_id::ClientOrderId, instrument_id::InstrumentId, strategy_id::StrategyId,
         trader_id::TraderId,
     },
     types::{price::Price, quantity::Quantity},
 };
 
-/// Provides a default [`LimitOrder`] used for testing.
 impl Default for LimitOrder {
+    /// Creates a new default [`LimitOrder`] instance for testing.
     fn default() -> Self {
         Self::new(
             TraderId::default(),
             StrategyId::default(),
             InstrumentId::default(),
             ClientOrderId::default(),
             OrderSide::Buy,
@@ -60,16 +60,16 @@
             UUID4::default(),
             UnixNanos::default(),
         )
         .unwrap() // SAFETY: Valid default values are used
     }
 }
 
-/// Provides a default [`LimitIfTouchedOrder`] used for testing.
 impl Default for LimitIfTouchedOrder {
+    /// Creates a new default [`LimitIfTouchedOrder`] instance for testing.
     fn default() -> Self {
         Self::new(
             TraderId::default(),
             StrategyId::default(),
             InstrumentId::default(),
             ClientOrderId::default(),
             OrderSide::Buy,
@@ -96,16 +96,16 @@
             UUID4::default(),
             UnixNanos::default(),
         )
         .unwrap() // SAFETY: Valid default values are used
     }
 }
 
-/// Provides a default [`MarketOrder`] used for testing.
 impl Default for MarketOrder {
+    /// Creates a new default [`MarketOrder`] instance for testing.
     fn default() -> Self {
         Self::new(
             TraderId::default(),
             StrategyId::default(),
             InstrumentId::default(),
             ClientOrderId::default(),
             OrderSide::Buy,
@@ -124,16 +124,16 @@
             None,
             None,
         )
         .unwrap() // SAFETY: Valid default values are used
     }
 }
 
-/// Provides a default [`MarketIfTouchedOrder`] used for testing.
 impl Default for MarketIfTouchedOrder {
+    /// Creates a new default [`MarketIfTouchedOrder`] instance for testing.
     fn default() -> Self {
         Self::new(
             TraderId::default(),
             StrategyId::default(),
             InstrumentId::default(),
             ClientOrderId::default(),
             OrderSide::Buy,
@@ -158,16 +158,16 @@
             UUID4::default(),
             UnixNanos::default(),
         )
         .unwrap() // SAFETY: Valid default values are used
     }
 }
 
-/// Provides a default [`MarketToLimitOrder`] used for testing.
 impl Default for MarketToLimitOrder {
+    /// Creates a new default [`MarketToLimitOrder`] instance for testing.
     fn default() -> Self {
         Self::new(
             TraderId::default(),
             StrategyId::default(),
             InstrumentId::default(),
             ClientOrderId::default(),
             OrderSide::Buy,
@@ -189,16 +189,16 @@
             UUID4::default(),
             UnixNanos::default(),
         )
         .unwrap() // SAFETY: Valid default values are used
     }
 }
 
-/// Provides a default [`StopLimitOrder`] used for testing.
 impl Default for StopLimitOrder {
+    /// Creates a new default [`StopLimitOrder`] instance for testing.
     fn default() -> Self {
         Self::new(
             TraderId::default(),
             StrategyId::default(),
             InstrumentId::default(),
             ClientOrderId::default(),
             OrderSide::Buy,
@@ -225,16 +225,16 @@
             UUID4::default(),
             UnixNanos::default(),
         )
         .unwrap() // SAFETY: Valid default values are used
     }
 }
 
-/// Provides a default [`StopMarketOrder`] used for testing.
 impl Default for StopMarketOrder {
+    /// Creates a new default [`StopMarketOrder`] instance for testing.
     fn default() -> Self {
         Self::new(
             TraderId::default(),
             StrategyId::default(),
             InstrumentId::default(),
             ClientOrderId::default(),
             OrderSide::Buy,
@@ -259,16 +259,16 @@
             UUID4::default(),
             UnixNanos::default(),
         )
         .unwrap() // SAFETY: Valid default values are used
     }
 }
 
-/// Provides a default [`TrailingStopLimitOrder`] used for testing.
 impl Default for TrailingStopLimitOrder {
+    /// Creates a new default [`TrailingStopLimitOrder`] instance for testing.
     fn default() -> Self {
         Self::new(
             TraderId::default(),
             StrategyId::default(),
             InstrumentId::default(),
             ClientOrderId::default(),
             OrderSide::Buy,
@@ -298,16 +298,16 @@
             UUID4::default(),
             UnixNanos::default(),
         )
         .unwrap() // SAFETY: Valid default values are used
     }
 }
 
-/// Provides a default [`TrailingStopMarketOrder`] used for testing.
 impl Default for TrailingStopMarketOrder {
+    /// Creates a new default [`TrailingStopMarketOrder`] instance for testing.
     fn default() -> Self {
         Self::new(
             TraderId::default(),
             StrategyId::default(),
             InstrumentId::default(),
             ClientOrderId::default(),
             OrderSide::Buy,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orders/limit.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orders/limit.rs`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     pub expire_time: Option<UnixNanos>,
     pub is_post_only: bool,
     pub display_qty: Option<Quantity>,
     pub trigger_instrument_id: Option<InstrumentId>,
 }
 
 impl LimitOrder {
+    /// Creates a new [`LimitOrder`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         order_side: OrderSide,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orders/limit_if_touched.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orders/limit_if_touched.rs`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     pub trigger_instrument_id: Option<InstrumentId>,
     pub is_triggered: bool,
     pub ts_triggered: Option<UnixNanos>,
     core: OrderCore,
 }
 
 impl LimitIfTouchedOrder {
+    /// Creates a new [`LimitIfTouchedOrder`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         order_side: OrderSide,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orders/list.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orders/list.rs`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     pub instrument_id: InstrumentId,
     pub strategy_id: StrategyId,
     pub orders: Vec<OrderAny>,
     pub ts_init: UnixNanos,
 }
 
 impl OrderList {
+    /// Creates a new [`OrderList`] instance.
     pub fn new(
         order_list_id: OrderListId,
         instrument_id: InstrumentId,
         strategy_id: StrategyId,
         orders: Vec<OrderAny>,
         ts_init: UnixNanos,
     ) -> anyhow::Result<Self> {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orders/market.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orders/market.rs`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     pyo3::pyclass(module = "nautilus_trader.core.nautilus_pyo3.model")
 )]
 pub struct MarketOrder {
     core: OrderCore,
 }
 
 impl MarketOrder {
+    /// Creates a new [`MarketOrder`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         order_side: OrderSide,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orders/market_if_touched.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orders/market_if_touched.rs`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     pub trigger_instrument_id: Option<InstrumentId>,
     pub is_triggered: bool,
     pub ts_triggered: Option<UnixNanos>,
     core: OrderCore,
 }
 
 impl MarketIfTouchedOrder {
+    /// Creates a new [`MarketIfTouchedOrder`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         order_side: OrderSide,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orders/market_to_limit.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orders/market_to_limit.rs`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     pub price: Option<Price>,
     pub expire_time: Option<UnixNanos>,
     pub is_post_only: bool,
     pub display_qty: Option<Quantity>,
 }
 
 impl MarketToLimitOrder {
+    /// Creates a new [`MarketToLimitOrder`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         order_side: OrderSide,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orders/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orders/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines order types for the trading domain model.
+//! Order types for the trading domain model.
 
 #![allow(dead_code)]
 
 pub mod any;
 pub mod base;
 pub mod default;
 pub mod limit;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orders/stop_limit.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orders/stop_limit.rs`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     pub trigger_instrument_id: Option<InstrumentId>,
     pub is_triggered: bool,
     pub ts_triggered: Option<UnixNanos>,
     core: OrderCore,
 }
 
 impl StopLimitOrder {
+    /// Creates a new [`StopLimitOrder`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         order_side: OrderSide,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orders/stop_market.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orders/stop_market.rs`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     pub trigger_instrument_id: Option<InstrumentId>,
     pub is_triggered: bool,
     pub ts_triggered: Option<UnixNanos>,
     core: OrderCore,
 }
 
 impl StopMarketOrder {
+    /// Creates a new [`StopMarketOrder`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         order_side: OrderSide,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orders/stubs.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orders/stubs.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orders/trailing_stop_limit.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orders/trailing_stop_limit.rs`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     pub display_qty: Option<Quantity>,
     pub trigger_instrument_id: Option<InstrumentId>,
     pub is_triggered: bool,
     pub ts_triggered: Option<UnixNanos>,
 }
 
 impl TrailingStopLimitOrder {
+    /// Creates a new [`TrailingStopLimitOrder`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         order_side: OrderSide,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/orders/trailing_stop_market.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/orders/trailing_stop_market.rs`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     pub display_qty: Option<Quantity>,
     pub trigger_instrument_id: Option<InstrumentId>,
     pub is_triggered: bool,
     pub ts_triggered: Option<UnixNanos>,
 }
 
 impl TrailingStopMarketOrder {
+    /// Creates a new [`TrailingStopMarketOrder`] instance.
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         trader_id: TraderId,
         strategy_id: StrategyId,
         instrument_id: InstrumentId,
         client_order_id: ClientOrderId,
         order_side: OrderSide,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/polymorphism.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/polymorphism.rs`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines traits to faciliate polymorphism.
+//! Traits to faciliate polymorphism.
 
 use nautilus_core::nanos::UnixNanos;
 
 use crate::{
-    enums::{OrderSide, OrderSideSpecified, TriggerType},
+    enums::{OrderSide, OrderSideSpecified, OrderStatus, TriggerType},
     events::order::event::OrderEventAny,
     identifiers::{
         account_id::AccountId, client_order_id::ClientOrderId, exec_algorithm_id::ExecAlgorithmId,
         instrument_id::InstrumentId, position_id::PositionId, strategy_id::StrategyId,
         trader_id::TraderId, venue_order_id::VenueOrderId,
     },
     orders::base::OrderError,
@@ -73,14 +73,18 @@
     fn order_side(&self) -> OrderSide;
 }
 
 pub trait GetOrderQuantity {
     fn quantity(&self) -> Quantity;
 }
 
+pub trait GetOrderStatus {
+    fn status(&self) -> OrderStatus;
+}
+
 pub trait GetOrderFilledQty {
     fn filled_qty(&self) -> Quantity;
 }
 
 pub trait GetOrderLeavesQty {
     fn leaves_qty(&self) -> Quantity;
 }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/position.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/position.rs`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines a `Position` for the trading domain model.
+//! A `Position` for the trading domain model.
 
 use std::{
     collections::{HashMap, HashSet},
     fmt::Display,
     hash::{Hash, Hasher},
 };
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/common.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/common.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/data/bar.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/data/bar.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/data/delta.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/data/delta.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/data/deltas.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/data/deltas.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/data/depth.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/data/depth.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/data/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/data/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines data types for the trading domain model.
+//! Data types for the trading domain model.
 
 pub mod bar;
 pub mod delta;
 pub mod deltas;
 pub mod depth;
 pub mod order;
 pub mod quote;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/data/order.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/data/order.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/data/quote.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/data/quote.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/data/trade.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/data/trade.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/enums.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/enums.rs`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines enumerations for the trading domain model.
+//! Enumerations for the trading domain model.
 
 use std::str::FromStr;
 
 use nautilus_core::python::to_pyvalue_err;
 use pyo3::{prelude::*, types::PyType, PyTypeInfo};
 
 use crate::{
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/account/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/orderbook/mod.rs`

 * *Files 10% similar despite different names*

```diff
@@ -9,8 +9,11 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-pub mod state;
+//! Provides a generic L1/L2/L3 order book the trading domain model.
+
+pub mod book;
+pub mod level;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/account/state.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/account/state.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines events for the trading domain model.
+//! Events for the trading domain model.
 
 pub mod account;
 pub mod order;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/accepted.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/accepted.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/cancel_rejected.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/cancel_rejected.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/canceled.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/canceled.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/denied.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/denied.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/emulated.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/emulated.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/expired.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/expired.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/filled.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/filled.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/initialized.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/initialized.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/modify_rejected.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/modify_rejected.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/pending_cancel.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/pending_cancel.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/pending_update.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/pending_update.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/rejected.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/rejected.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/released.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/released.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/submitted.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/submitted.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/triggered.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/triggered.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/events/order/updated.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/events/order/updated.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/identifiers/instrument_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/identifiers/instrument_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/identifiers/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/identifiers/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines identifiers the trading domain model.
+//! Identifiers for the trading domain model.
 
 use std::str::FromStr;
 
 use nautilus_core::python::to_pyvalue_err;
 use pyo3::{
     prelude::*,
     pyclass::CompareOp,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/identifiers/trade_id.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/identifiers/trade_id.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/crypto_future.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/crypto_future.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/crypto_perpetual.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/crypto_perpetual.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/currency_pair.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/currency_pair.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/equity.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/equity.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/futures_contract.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/futures_contract.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/futures_spread.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/futures_spread.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines instrument definitions the trading domain model.
+//! Instrument definitions the trading domain model.
 
 use nautilus_core::python::to_pyvalue_err;
 use pyo3::{IntoPy, PyObject, PyResult, Python};
 
 use crate::instruments::{
     any::InstrumentAny, crypto_future::CryptoFuture, crypto_perpetual::CryptoPerpetual,
     currency_pair::CurrencyPair, equity::Equity, futures_contract::FuturesContract,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/options_contract.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/options_contract.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/instruments/options_spread.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/instruments/options_spread.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/macros.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/macros.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/orderbook/book.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/orderbook/book.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/orderbook/level.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/orderbook/level.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/orderbook/mod.rs` & `nautilus_trader-1.194.0/nautilus_trader/core/asynchronous.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,31 @@
-// -------------------------------------------------------------------------------------------------
-//  Copyright (C) 2015-2024 Nautech Systems Pty Ltd. All rights reserved.
-//  https://nautechsystems.io
-//
-//  Licensed under the GNU Lesser General Public License Version 3.0 (the "License");
-//  You may not use this file except in compliance with the License.
-//  You may obtain a copy of the License at https://www.gnu.org/licenses/lgpl-3.0.en.html
-//
-//  Unless required by applicable law or agreed to in writing, software
-//  distributed under the License is distributed on an "AS IS" BASIS,
-//  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-//  See the License for the specific language governing permissions and
-//  limitations under the License.
-// -------------------------------------------------------------------------------------------------
+# -------------------------------------------------------------------------------------------------
+#  Copyright (C) 2015-2024 Nautech Systems Pty Ltd. All rights reserved.
+#  https://nautechsystems.io
+#
+#  Licensed under the GNU Lesser General Public License Version 3.0 (the "License");
+#  You may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at https://www.gnu.org/licenses/lgpl-3.0.en.html
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+# -------------------------------------------------------------------------------------------------
 
-//! Provides a generic L1/L2/L3 order book the trading domain model.
+import types
 
-pub mod book;
-pub mod level;
+
+@types.coroutine
+def sleep0():
+    """
+    Skip one event loop run cycle.
+
+    This is equivalent to `asyncio.sleep(0)` however avoids the overhead of the Python
+    function call and integer comparison <= 0.
+
+    Uses a bare 'yield' expression (which Task.__step knows how to handle) instead of
+    creating a Future object.
+
+    """
+    yield
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/limit.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/limit.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/limit_if_touched.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/limit_if_touched.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/market.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/market.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/market_if_touched.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/market_if_touched.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/market_to_limit.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/market_to_limit.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/stop_limit.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/stop_limit.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/stop_market.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/stop_market.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/trailing_stop_limit.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/trailing_stop_limit.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/orders/trailing_stop_market.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/orders/trailing_stop_market.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/position.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/position.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/types/balance.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/types/balance.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/types/currency.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/types/currency.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/types/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/types/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines value types such as `Price`, `Quantity` and `Money` for the trading domain model.
+//! Value types such as `Price`, `Quantity` and `Money` for the trading domain model.
 
 pub mod balance;
 pub mod currency;
 pub mod money;
 pub mod price;
 pub mod quantity;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/types/money.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/types/money.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/types/price.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/types/price.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/python/types/quantity.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/python/types/quantity.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/stubs.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/stubs.rs`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             size_precision,
         )
         .unwrap();
         let order = BookOrder::new(
             OrderSide::Buy,
             price,
             size,
-            0, // order_id not applicable for MBP (market by price) books
+            0, // order_id not applicable for MBP (market-by-price) books
         );
         book.add(order, 0, 1, 2.into());
     }
 
     // Generate asks
     for i in 0..num_levels {
         let price = Price::new(
@@ -171,14 +171,14 @@
             size_precision,
         )
         .unwrap();
         let order = BookOrder::new(
             OrderSide::Sell,
             price,
             size,
-            0, // order_id not applicable for MBP (market by price) books
+            0, // order_id not applicable for MBP (market-by-price) books
         );
         book.add(order, 0, 1, 2.into());
     }
 
     book
 }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/types/balance.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/types/balance.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/types/currency.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/types/currency.rs`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     pub precision: u8,
     pub iso4217: u16,
     pub name: Ustr,
     pub currency_type: CurrencyType,
 }
 
 impl Currency {
+    /// Creates a new [`Currency`] instance.
     pub fn new(
         code: &str,
         precision: u8,
         iso4217: u16,
         name: &str,
         currency_type: CurrencyType,
     ) -> anyhow::Result<Self> {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/types/fixed.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/types/fixed.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/types/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/types/mod.rs`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Defines value types for the trading domain model such as `Price`, `Quantity` and `Money`.
+//! Value types for the trading domain model such as `Price`, `Quantity` and `Money`.
 
 pub mod balance;
 pub mod currency;
 pub mod fixed;
 pub mod money;
 pub mod price;
 pub mod quantity;
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/types/money.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/types/money.rs`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 )]
 pub struct Money {
     pub raw: i64,
     pub currency: Currency,
 }
 
 impl Money {
+    /// Creates a new [`Money`] instance.
     pub fn new(amount: f64, currency: Currency) -> anyhow::Result<Self> {
         check_in_range_inclusive_f64(amount, MONEY_MIN, MONEY_MAX, "amount")?;
 
         Ok(Self {
             raw: f64_to_fixed_i64(amount, currency.precision),
             currency,
         })
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/types/price.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/types/price.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/types/quantity.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/types/quantity.rs`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 )]
 pub struct Quantity {
     pub raw: u64,
     pub precision: u8,
 }
 
 impl Quantity {
+    /// Creates a new [`Quantity`] instance.
     pub fn new(value: f64, precision: u8) -> anyhow::Result<Self> {
         check_in_range_inclusive_f64(value, QUANTITY_MIN, QUANTITY_MAX, "value")?;
         check_fixed_precision(precision)?;
 
         Ok(Self {
             raw: f64_to_fixed_u64(value, precision),
             precision,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/types/stubs.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/types/stubs.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/model/src/venues.rs` & `nautilus_trader-1.194.0/nautilus_core/model/src/venues.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/Cargo.toml` & `nautilus_trader-1.194.0/nautilus_core/network/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/benches/test_client.rs` & `nautilus_trader-1.194.0/nautilus_core/network/benches/test_client.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/benches/test_server.rs` & `nautilus_trader-1.194.0/nautilus_core/network/benches/test_server.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/src/http.rs` & `nautilus_trader-1.194.0/nautilus_core/network/src/http.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides a high-performance HTTP client implementation.
+//! A high-performance HTTP client implementation.
 
 use std::{
     collections::{hash_map::DefaultHasher, HashMap},
     hash::{Hash, Hasher},
     sync::Arc,
 };
 
@@ -27,15 +27,15 @@
     header::{HeaderMap, HeaderName},
     Method, Response, Url,
 };
 use tracing::trace;
 
 use crate::ratelimiter::{clock::MonotonicClock, quota::Quota, RateLimiter};
 
-/// Provides a high-performance `HttpClient` for HTTP requests.
+/// A high-performance `HttpClient` for HTTP requests.
 ///
 /// The client is backed by a hyper Client which keeps connections alive and
 /// can be cloned cheaply. The client also has a list of header fields to
 /// extract from the response.
 ///
 /// The client returns an [`HttpResponse`]. The client filters only the key value
 /// for the give `header_keys`.
@@ -144,14 +144,15 @@
     pub status: u16,
     #[pyo3(get)]
     headers: HashMap<String, String>,
     body: Vec<u8>,
 }
 
 impl Default for InnerHttpClient {
+    /// Creates a new default [`InnerHttpClient`] instance.
     fn default() -> Self {
         let client = reqwest::Client::new();
         Self {
             client,
             header_keys: Default::default(),
         }
     }
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/src/lib.rs` & `nautilus_trader-1.194.0/nautilus_core/network/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/src/python/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/network/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/clock.rs` & `nautilus_trader-1.194.0/nautilus_core/network/src/ratelimiter/clock.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/gcra.rs` & `nautilus_trader-1.194.0/nautilus_core/network/src/ratelimiter/gcra.rs`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     pub(crate) time_of_measurement: Nanos,
 
     /// The next time a cell is expected to arrive
     pub(crate) tat: Nanos,
 }
 
 impl StateSnapshot {
+    /// Creates a new [`StateSnapshot`] instance.
     #[inline]
     pub(crate) fn new(t: Nanos, tau: Nanos, time_of_measurement: Nanos, tat: Nanos) -> Self {
         Self {
             t,
             tau,
             time_of_measurement,
             tat,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/network/src/ratelimiter/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/nanos.rs` & `nautilus_trader-1.194.0/nautilus_core/network/src/ratelimiter/nanos.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/src/ratelimiter/quota.rs` & `nautilus_trader-1.194.0/nautilus_core/network/src/ratelimiter/quota.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/src/socket.rs` & `nautilus_trader-1.194.0/nautilus_core/network/src/socket.rs`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides a high-performance raw TCP client implementation with TLS capability.
+//! A high-performance raw TCP client implementation with TLS capability.
 
 use std::{sync::Arc, time::Duration};
 
 use nautilus_core::python::to_pyruntime_err;
 use pyo3::prelude::*;
 use tokio::{
     io::{split, AsyncReadExt, AsyncWriteExt, ReadHalf, WriteHalf},
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/src/websocket.rs` & `nautilus_trader-1.194.0/nautilus_core/network/src/websocket.rs`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 //  Unless required by applicable law or agreed to in writing, software
 //  distributed under the License is distributed on an "AS IS" BASIS,
 //  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //  See the License for the specific language governing permissions and
 //  limitations under the License.
 // -------------------------------------------------------------------------------------------------
 
-//! Provides a high-performance WebSocket client implementation.
+//! A high-performance WebSocket client implementation.
 
 use std::{str::FromStr, sync::Arc, time::Duration};
 
 use futures_util::{
     stream::{SplitSink, SplitStream},
     SinkExt, StreamExt,
 };
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/CHANGELOG.md` & `nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 - Update dependencies (underlying `tungstenite` core).
 
 # 0.17.2
 
 - Make `Origin` header case-sensitive (to keep compatibility with poorely-written servers that don't accept lowercase `Origin` header).
 - Make semantics of the reading form the `WebSocketStream` more reasonable (return `None` instead of an error when the stream is normally closed).
-- Imrpove the way `poll_close()` works by properly driving the close of the stream till completion.
+- Improve the way `poll_close()` works by properly driving the close of the stream till completion.
 
 # 0.17.1
 
 - Update the `tungstenite` dependency (fixes a panic in `tungstenite` and MSRV), see [`tungstenite`'s changelog for more details](https://github.com/snapview/tungstenite-rs/blob/master/CHANGELOG.md#0172).
 
 # 0.17.0
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/Cargo.toml` & `nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/LICENSE` & `nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/LICENSE`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/README.md` & `nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/README.md`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/compat.rs` & `nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/src/compat.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/connect.rs` & `nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/src/connect.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/handshake.rs` & `nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/src/handshake.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/lib.rs` & `nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/stream.rs` & `nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/src/stream.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/network/tokio-tungstenite/src/tls.rs` & `nautilus_trader-1.194.0/nautilus_core/network/tokio-tungstenite/src/tls.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/Cargo.toml` & `nautilus_trader-1.194.0/nautilus_core/persistence/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/benches/bench_persistence.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/benches/bench_persistence.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/bar.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/arrow/bar.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/delta.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/arrow/delta.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/depth.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/arrow/depth.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/arrow/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/quote.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/arrow/quote.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/arrow/trade.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/arrow/trade.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/backend/kmerge_batch.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/backend/kmerge_batch.rs`

 * *Files 0% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 }
 
 impl<I, T, C> KMerge<I, T, C>
 where
     I: Iterator<Item = IntoIter<T>>,
     C: Compare<ElementBatchIter<I, T>>,
 {
+    /// Creates a new [`KMerge`] instance.
     pub fn new(cmp: C) -> Self {
         Self {
             heap: BinaryHeap::from_vec_cmp(Vec::new(), cmp),
         }
     }
 
     pub fn push_iter(&mut self, s: I) {
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/backend/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/backend/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/backend/session.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/backend/session.rs`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     pub chunk_size: usize,
     pub runtime: Arc<tokio::runtime::Runtime>,
     session_ctx: SessionContext,
     batch_streams: Vec<EagerStream<IntoIter<Data>>>,
 }
 
 impl DataBackendSession {
+    /// Creates a new [`DataBackendSession`] instance.
     #[must_use]
     pub fn new(chunk_size: usize) -> Self {
         let runtime = tokio::runtime::Builder::new_multi_thread()
             .enable_all()
             .build()
             .unwrap();
         Self {
@@ -179,14 +180,15 @@
     pub chunk: Option<CVec>,
     pub result: QueryResult,
     pub acc: Vec<Data>,
     pub size: usize,
 }
 
 impl DataQueryResult {
+    /// Creates a new [`DataQueryResult`] instance.
     #[must_use]
     pub fn new(result: QueryResult, size: usize) -> Self {
         Self {
             chunk: None,
             result,
             acc: Vec::new(),
             size,
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/lib.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/backend/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/python/backend/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/backend/session.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/python/backend/session.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/backend/transformer.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/python/backend/transformer.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/mod.rs` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/schemas/wallet.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,31 @@
-// -------------------------------------------------------------------------------------------------
-//  Copyright (C) 2015-2024 Nautech Systems Pty Ltd. All rights reserved.
-//  https://nautechsystems.io
-//
-//  Licensed under the GNU Lesser General Public License Version 3.0 (the "License");
-//  You may not use this file except in compliance with the License.
-//  You may obtain a copy of the License at https://www.gnu.org/licenses/lgpl-3.0.en.html
-//
-//  Unless required by applicable law or agreed to in writing, software
-//  distributed under the License is distributed on an "AS IS" BASIS,
-//  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-//  See the License for the specific language governing permissions and
-//  limitations under the License.
-// -------------------------------------------------------------------------------------------------
-
-//! Python bindings from `pyo3`.
-
-#![allow(warnings)] // non-local `impl` definition, temporary allow until pyo3 upgrade
-
-use pyo3::prelude::*;
-
-pub mod backend;
-pub mod wranglers;
-
-/// Loaded as nautilus_pyo3.persistence
-#[pymodule]
-pub fn persistence(_: Python<'_>, m: &PyModule) -> PyResult<()> {
-    m.add_class::<crate::backend::session::DataBackendSession>()?;
-    m.add_class::<crate::backend::session::DataQueryResult>()?;
-    m.add_class::<backend::session::NautilusDataType>()?;
-    m.add_class::<backend::transformer::DataTransformer>()?;
-    m.add_class::<wranglers::bar::BarDataWrangler>()?;
-    m.add_class::<wranglers::delta::OrderBookDeltaDataWrangler>()?;
-    m.add_class::<wranglers::quote::QuoteTickDataWrangler>()?;
-    m.add_class::<wranglers::trade::TradeTickDataWrangler>()?;
-    Ok(())
-}
+# -------------------------------------------------------------------------------------------------
+#  Copyright (C) 2015-2024 Nautech Systems Pty Ltd. All rights reserved.
+#  https://nautechsystems.io
+#
+#  Licensed under the GNU Lesser General Public License Version 3.0 (the "License");
+#  You may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at https://www.gnu.org/licenses/lgpl-3.0.en.html
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+# -------------------------------------------------------------------------------------------------
+
+import msgspec
+
+
+################################################################################
+# HTTP responses
+################################################################################
+
+
+class BinanceSpotTradeFee(msgspec.Struct, frozen=True):
+    """
+    Schema of a single `Binance Spot/Margin` tradeFee.
+    """
+
+    symbol: str
+    makerCommission: str
+    takerCommission: str
```

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/bar.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/python/wranglers/bar.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/delta.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/python/wranglers/delta.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/mod.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/python/wranglers/mod.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/quote.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/python/wranglers/quote.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/src/python/wranglers/trade.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/src/python/wranglers/trade.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/tests/test_catalog.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/tests/test_catalog.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/persistence/tests/test_util.rs` & `nautilus_trader-1.194.0/nautilus_core/persistence/tests/test_util.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/pyo3/Cargo.toml` & `nautilus_trader-1.194.0/nautilus_core/pyo3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_core/pyo3/src/lib.rs` & `nautilus_trader-1.194.0/nautilus_core/pyo3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/accounting/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/accounting/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/base.pxd` & `nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/base.pyx` & `nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/betting.pxd` & `nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/betting.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/betting.pyx` & `nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/betting.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/cash.pxd` & `nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/cash.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/cash.pyx` & `nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/cash.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/margin.pxd` & `nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/margin.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/accounts/margin.pyx` & `nautilus_trader-1.194.0/nautilus_trader/accounting/accounts/margin.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/calculators.pxd` & `nautilus_trader-1.194.0/nautilus_trader/accounting/calculators.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/calculators.pyx` & `nautilus_trader-1.194.0/nautilus_trader/accounting/calculators.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/error.py` & `nautilus_trader-1.194.0/nautilus_trader/accounting/error.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/factory.pxd` & `nautilus_trader-1.194.0/nautilus_trader/accounting/factory.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/factory.pyx` & `nautilus_trader-1.194.0/nautilus_trader/accounting/factory.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/manager.pxd` & `nautilus_trader-1.194.0/nautilus_trader/accounting/manager.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/accounting/manager.pyx` & `nautilus_trader-1.194.0/nautilus_trader/accounting/manager.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/_template/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/_template/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/_template/core.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/_template/core.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/_template/data.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/_template/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/_template/execution.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/_template/execution.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/_template/providers.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/_template/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/client.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/client.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/common.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/common.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/config.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/constants.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/constants.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/data.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/data_types.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/data_types.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/execution.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/execution.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/factories.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/factories.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/orderbook.pxd` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/orderbook.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/orderbook.pyx` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/orderbook.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/common.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/parsing/common.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/core.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/parsing/core.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/requests.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/parsing/requests.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/parsing/streaming.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/parsing/streaming.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/providers.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/betfair/sockets.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/betfair/sockets.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/constants.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/constants.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/credentials.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/credentials.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/data.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/enums.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/execution.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/execution.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/schemas/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/schemas/account.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/schemas/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/schemas/market.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/schemas/market.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/schemas/user.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/symbol.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/symbol.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/types.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/types.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/common/urls.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/common/urls.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/config.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/factories.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/factories.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/data.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/enums.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/execution.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/execution.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/http/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/account.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/http/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/market.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/http/market.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/user.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/http/user.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/http/wallet.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/http/wallet.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/providers.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,16 +247,16 @@
             }
             price_filter: BinanceSymbolFilter = filters.get(BinanceSymbolFilterType.PRICE_FILTER)
             lot_size_filter: BinanceSymbolFilter = filters.get(BinanceSymbolFilterType.LOT_SIZE)
             min_notional_filter: BinanceSymbolFilter = filters.get(
                 BinanceSymbolFilterType.MIN_NOTIONAL,
             )
 
-            tick_size = price_filter.tickSize.rstrip("0")
-            step_size = lot_size_filter.stepSize.rstrip("0")
+            tick_size = price_filter.tickSize
+            step_size = lot_size_filter.stepSize
             PyCondition.in_range(float(tick_size), PRICE_MIN, PRICE_MAX, "tick_size")
             PyCondition.in_range(float(step_size), QUANTITY_MIN, QUANTITY_MAX, "step_size")
 
             price_precision = abs(int(Decimal(tick_size).as_tuple().exponent))
             size_precision = abs(int(Decimal(step_size).as_tuple().exponent))
             price_increment = Price.from_str(tick_size)
             size_increment = Quantity.from_str(step_size)
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/account.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/schemas/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/market.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/schemas/market.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/user.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/schemas/user.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/schemas/wallet.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/schemas/wallet.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/futures/types.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/futures/types.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/http/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/account.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/http/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/client.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/http/client.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/endpoint.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/http/endpoint.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/error.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/http/error.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/market.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/http/market.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/http/user.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/http/user.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/data.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/enums.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/execution.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/execution.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/http/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/account.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/http/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/market.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/http/market.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/user.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/http/user.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/http/wallet.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/http/wallet.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/providers.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,16 +233,16 @@
             price_filter: BinanceSymbolFilter = filters.get(BinanceSymbolFilterType.PRICE_FILTER)
             lot_size_filter: BinanceSymbolFilter = filters.get(BinanceSymbolFilterType.LOT_SIZE)
             min_notional_filter: BinanceSymbolFilter = filters.get(
                 BinanceSymbolFilterType.MIN_NOTIONAL,
             )
             # market_lot_size_filter = symbol_filters.get("MARKET_LOT_SIZE")
 
-            tick_size = price_filter.tickSize.rstrip("0")
-            step_size = lot_size_filter.stepSize.rstrip("0")
+            tick_size = price_filter.tickSize
+            step_size = lot_size_filter.stepSize
             PyCondition.in_range(float(tick_size), PRICE_MIN, PRICE_MAX, "tick_size")
             PyCondition.in_range(float(step_size), QUANTITY_MIN, QUANTITY_MAX, "step_size")
 
             price_precision = abs(int(Decimal(tick_size).as_tuple().exponent))
             size_precision = abs(int(Decimal(step_size).as_tuple().exponent))
             price_increment = Price.from_str(tick_size)
             size_increment = Quantity.from_str(step_size)
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/account.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/schemas/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/market.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/schemas/market.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/user.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/spot/schemas/user.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/spot/schemas/wallet.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,24 +8,11 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
-
-import msgspec
-
-
-################################################################################
-# HTTP responses
-################################################################################
-
-
-class BinanceSpotTradeFee(msgspec.Struct, frozen=True):
-    """
-    Schema of a single `Binance Spot/Margin` tradeFee.
-    """
-
-    symbol: str
-    makerCommission: str
-    takerCommission: str
+"""
+The `analysis` subpackage groups components relating to trading performance statistics
+and analysis.
+"""
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/websocket/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/binance/websocket/client.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/binance/websocket/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -492,15 +492,15 @@
 
         await self._client.send_text(json.dumps(message))
         for stream in self._streams:
             self._log.debug(f"Subscribed to {stream}")
 
     async def _unsubscribe(self, stream: str) -> None:
         if stream not in self._streams:
-            self._log.warning(f"Cannot unsubscribe from {stream}: never subscribed")
+            self._log.warning(f"Cannot unsubscribe from {stream}: not subscribed")
             return  # Not subscribed
 
         self._streams.remove(stream)
 
         if self._client is None:
             self._log.error(f"Cannot unsubscribe from {stream}: not connected")
             return
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/constants.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/common/constants.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/credentials.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/common/credentials.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/enums.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/common/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/error.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/common/error.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/parsing.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/common/parsing.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     values: tuple[Price, Quantity],
     side: OrderSide,
     update_id: int,
     sequence: int,
     ts_event: int,
     ts_init: int,
     is_snapshot: bool,
+    flags: int = 0,
 ) -> OrderBookDelta:
     price = values[0]
     size = values[1]
     if is_snapshot:
         action = BookAction.ADD
     else:
         action = BookAction.DELETE if size == 0 else BookAction.UPDATE
@@ -60,15 +61,15 @@
         action=action,
         order=BookOrder(
             side=side,
             price=price,
             size=size,
             order_id=update_id,
         ),
-        flags=0,  # Not applicable
+        flags=flags,
         sequence=sequence,
         ts_event=ts_event,
         ts_init=ts_init,
     )
 
 
 def get_interval_from_bar_type(bar_type: BarType) -> str:
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/symbol.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/common/symbol.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/common/urls.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/common/urls.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/config.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/data.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,22 +287,23 @@
                 f"for Bybit {product_type.value} products, "
                 f"available depths are {depths_available}",
             )
             return
 
         if instrument_id in self._tob_quotes:
             if depth == 1:
-                self._log.debug(
+                self._log.warning(
                     f"Already subscribed to {instrument_id} top-of-book",
                     LogColor.MAGENTA,
                 )
                 return  # Already subscribed
-            raise RuntimeError(
-                "Cannot subscribe to both top-of-book quotes and order book",
-            )
+
+        if instrument_id in self._depths:
+            self._log.warning(f"Already subscribed to {instrument_id} order book deltas")
+            return
 
         self._depths[instrument_id] = depth
         ws_client = self._ws_clients[bybit_symbol.product_type]
         await ws_client.subscribe_order_book(bybit_symbol.raw_symbol, depth=depth)
 
     def _is_subscribed_to_order_book(self, instrument_id: InstrumentId) -> bool:
         return (
@@ -572,37 +573,37 @@
             if ws_message.success is False:
                 self._log.error(f"WebSocket error: {ws_message}")
                 return
             if not ws_message.topic:
                 return
 
             if "orderbook" in ws_message.topic:
-                self._handle_orderbook(product_type, raw)
+                self._handle_orderbook(product_type, raw, ws_message.topic)
             elif "publicTrade" in ws_message.topic:
                 self._handle_trade(product_type, raw)
             elif "tickers" in ws_message.topic:
                 self._handle_ticker(product_type, raw)
             elif "kline" in ws_message.topic:
                 self._handle_kline(raw)
             else:
                 self._log.error(f"Unknown websocket message topic: {ws_message.topic}")
         except Exception as e:
             self._log.error(f"Failed to parse websocket message: {raw.decode()} with error {e}")
 
-    def _handle_orderbook(self, product_type: BybitProductType, raw: bytes) -> None:
+    def _handle_orderbook(self, product_type: BybitProductType, raw: bytes, topic: str) -> None:
         msg = self._decoder_ws_orderbook.decode(raw)
         symbol = msg.data.s + f"-{product_type.value.upper()}"
         instrument_id: InstrumentId = self._get_cached_instrument_id(symbol)
 
         instrument = self._cache.instrument(instrument_id)
         if instrument is None:
             self._log.error(f"Cannot parse order book data: no instrument for {instrument_id}")
             return
 
-        if instrument_id in self._tob_quotes:
+        if instrument_id in self._tob_quotes and topic.startswith("orderbook.1."):
             quote = msg.data.parse_to_quote_tick(
                 instrument_id=instrument_id,
                 last_quote=self._last_quotes.get(instrument_id),
                 price_precision=instrument.price_precision,
                 size_precision=instrument.size_precision,
                 ts_event=millis_to_nanos(msg.ts),
                 ts_init=self._clock.timestamp_ns(),
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/account/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/account/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/account/fee_rate.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/account/fee_rate.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/account/position_info.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/account/position_info.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/account/wallet_balance.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/account/wallet_balance.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/asset/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/asset/coin_info.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/asset/coin_info.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/endpoint.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/endpoint.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/market/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/instruments_info.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/market/instruments_info.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/klines.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/market/klines.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/server_time.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/market/server_time.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/tickers.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/market/tickers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/market/trades.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/market/trades.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/amend_order.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/amend_order.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_amend_order.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_amend_order.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_cancel_order.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_cancel_order.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_place_order.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/batch_place_order.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/cancel_all_orders.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/cancel_all_orders.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/cancel_order.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/cancel_order.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/open_orders.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/open_orders.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/order_history.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/order_history.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/place_order.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/place_order.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/endpoints/trade/trade_history.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/endpoints/trade/trade_history.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/execution.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/execution.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/factories.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/factories.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/http/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/account.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/http/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/asset.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/http/asset.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/client.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/http/client.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/errors.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/http/errors.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/market.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/http/market.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/http/user.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/http/user.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/providers.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/account/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/account/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/account/balance.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/account/balance.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/account/fee_rate.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/account/fee_rate.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/asset/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/asset/coin_info.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/asset/coin_info.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/common.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/common.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/instrument.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/instrument.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/market/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/kline.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/market/kline.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/orderbook.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/risk_limit.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/market/risk_limit.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/server_time.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/market/server_time.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/ticker.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/market/ticker.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/market/trades.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/market/trades.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/order.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/order.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/position.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/position.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/trade.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/trade.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/schemas/ws.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/schemas/ws.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from nautilus_trader.model.data import BarType
 from nautilus_trader.model.data import OrderBookDelta
 from nautilus_trader.model.data import OrderBookDeltas
 from nautilus_trader.model.data import QuoteTick
 from nautilus_trader.model.data import TradeTick
 from nautilus_trader.model.enums import AggressorSide
 from nautilus_trader.model.enums import OrderSide
+from nautilus_trader.model.enums import RecordFlag
 from nautilus_trader.model.identifiers import AccountId
 from nautilus_trader.model.identifiers import ClientOrderId
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.identifiers import TradeId
 from nautilus_trader.model.identifiers import VenueOrderId
 from nautilus_trader.model.objects import Price
 from nautilus_trader.model.objects import Quantity
@@ -168,38 +169,56 @@
         clear = OrderBookDelta.clear(
             instrument_id=instrument_id,
             sequence=self.seq,
             ts_event=ts_event,
             ts_init=ts_init,
         )
         deltas.append(clear)
+        num_bids_raw = len(bids_raw)
+        num_asks_raw = len(asks_raw)
+
+        for bid_id, bid in enumerate(bids_raw):
+            flags = 0
+
+            if bid_id == num_bids_raw - 1 and num_asks_raw == 0:
+                # F_LAST, 1 << 7
+                # Last message in the packet from the venue for a given `instrument_id`
+                flags = RecordFlag.F_LAST
 
-        for bid in bids_raw:
             delta = parse_bybit_delta(
                 instrument_id=instrument_id,
                 values=bid,
                 side=OrderSide.BUY,
                 update_id=self.u,
                 sequence=self.seq,
                 ts_event=ts_event,
                 ts_init=ts_init,
                 is_snapshot=True,
+                flags=flags,
             )
             deltas.append(delta)
 
-        for ask in asks_raw:
+        for ask_id, ask in enumerate(asks_raw):
+            flags = 0
+
+            if ask_id == num_asks_raw - 1:
+                # F_LAST, 1 << 7
+                # Last message in the packet from the venue for a given `instrument_id`
+                flags = RecordFlag.F_LAST
+
             delta = parse_bybit_delta(
                 instrument_id=instrument_id,
                 values=ask,
                 side=OrderSide.SELL,
                 update_id=self.u,
                 sequence=self.seq,
                 ts_event=ts_event,
                 ts_init=ts_init,
                 is_snapshot=True,
+                flags=flags,
             )
             deltas.append(delta)
 
         return OrderBookDeltas(instrument_id=instrument_id, deltas=deltas)
 
     def parse_to_deltas(
         self,
@@ -220,39 +239,56 @@
             (
                 Price(float(d[0]), price_precision),
                 Quantity(float(d[1]), size_precision),
             )
             for d in self.a
         ]
         deltas: list[OrderBookDelta] = []
+        num_bids_raw = len(bids_raw)
+        num_asks_raw = len(asks_raw)
+
+        for bid_id, bid in enumerate(bids_raw):
+            flags = 0
+
+            if bid_id == num_bids_raw - 1 and num_asks_raw == 0:
+                # F_LAST, 1 << 7
+                # Last message in the packet from the venue for a given `instrument_id`
+                flags = RecordFlag.F_LAST
 
-        for bid in bids_raw:
             delta = parse_bybit_delta(
                 instrument_id=instrument_id,
                 values=bid,
                 side=OrderSide.BUY,
                 update_id=self.u,
                 sequence=self.seq,
                 ts_event=ts_event,
                 ts_init=ts_init,
                 is_snapshot=False,
+                flags=flags,
             )
             deltas.append(delta)
-            deltas.append(delta)
 
-        for ask in asks_raw:
+        for ask_id, ask in enumerate(asks_raw):
+            flags = 0
+
+            if ask_id == num_asks_raw - 1:
+                # F_LAST, 1 << 7
+                # Last message in the packet from the venue for a given `instrument_id`
+                flags = RecordFlag.F_LAST
+
             delta = parse_bybit_delta(
                 instrument_id=instrument_id,
                 values=ask,
                 side=OrderSide.SELL,
                 update_id=self.u,
                 sequence=self.seq,
                 ts_event=ts_event,
                 ts_init=ts_init,
                 is_snapshot=False,
+                flags=flags,
             )
             deltas.append(delta)
 
         return OrderBookDeltas(instrument_id=instrument_id, deltas=deltas)
 
     def parse_to_quote_tick(
         self,
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/websocket/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/bybit/websocket/client.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/bybit/websocket/client.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/databento/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/common.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/databento/common.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/config.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/databento/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/constants.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/databento/constants.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/data.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/databento/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/enums.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/databento/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/factories.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/databento/factories.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/loaders.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/databento/loaders.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/providers.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/databento/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/publishers.json` & `nautilus_trader-1.194.0/nautilus_trader/adapters/databento/publishers.json`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/databento/types.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/databento/types.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/env.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/env.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/account.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/account.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/client.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/client.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/common.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/common.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/connection.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/connection.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/contract.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/contract.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/error.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/error.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/market_data.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/market_data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/order.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/order.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/client/wrapper.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/client/wrapper.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/common.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/common.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/config.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/data.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/execution.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/execution.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/factories.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/factories.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/gateway.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/gateway.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/historic/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/historic/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/historic/client.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/historic/client.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/parsing/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/parsing/data.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/parsing/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/parsing/execution.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/parsing/execution.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/parsing/instruments.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/parsing/instruments.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/providers.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/interactive_brokers/web.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/interactive_brokers/web.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/sandbox/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/sandbox/config.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/sandbox/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/sandbox/execution.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/sandbox/execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 import asyncio
-from typing import ClassVar
 
 import pandas as pd
 
 from nautilus_trader.adapters.sandbox.config import SandboxExecutionClientConfig
 from nautilus_trader.backtest.exchange import SimulatedExchange
 from nautilus_trader.backtest.execution_client import BacktestExecClient
 from nautilus_trader.backtest.models import FillModel
@@ -43,15 +42,14 @@
 from nautilus_trader.model.enums import book_type_from_str
 from nautilus_trader.model.enums import oms_type_from_str
 from nautilus_trader.model.identifiers import ClientId
 from nautilus_trader.model.identifiers import ClientOrderId
 from nautilus_trader.model.identifiers import InstrumentId
 from nautilus_trader.model.identifiers import Venue
 from nautilus_trader.model.identifiers import VenueOrderId
-from nautilus_trader.model.instruments import Instrument
 from nautilus_trader.model.objects import Currency
 from nautilus_trader.model.objects import Money
 from nautilus_trader.portfolio.base import PortfolioFacade
 
 
 class SandboxExecutionClient(LiveExecutionClient):
     """
@@ -68,16 +66,14 @@
     cache : Cache
         The cache for the client.
     clock : LiveClock
         The clock for the client.
 
     """
 
-    INSTRUMENTS: ClassVar[list[Instrument]] = []
-
     def __init__(
         self,
         loop: asyncio.AbstractEventLoop,
         portfolio: PortfolioFacade,
         msgbus: MessageBus,
         cache: Cache,
         clock: LiveClock,
@@ -107,15 +103,14 @@
             venue=sandbox_venue,
             oms_type=oms_type,
             account_type=account_type,
             starting_balances=[Money.from_str(b) for b in config.starting_balances],
             base_currency=base_currency,
             default_leverage=config.default_leverage,
             leverages=config.leverages or {},
-            instruments=self.INSTRUMENTS,
             modules=[],
             portfolio=portfolio,
             msgbus=self._msgbus,
             cache=cache,
             clock=self.test_clock,
             fill_model=FillModel(),
             fee_model=MakerTakerFeeModel(),
@@ -125,15 +120,17 @@
             bar_execution=config.bar_execution,
             reject_stop_orders=config.reject_stop_orders,
             support_gtd_orders=config.support_gtd_orders,
             support_contingent_orders=config.support_contingent_orders,
             use_position_ids=config.use_position_ids,
             use_random_ids=config.use_random_ids,
             use_reduce_only=config.use_reduce_only,
+            use_message_queue=False,  # Do not use internal message queue for real-time
         )
+
         self._client = BacktestExecClient(
             exchange=self.exchange,
             msgbus=msgbus,
             cache=cache,
             clock=self.test_clock,
         )
         self.exchange.register_client(self._client)
@@ -141,14 +138,19 @@
 
     def connect(self) -> None:
         """
         Connect the client.
         """
         self._log.info("Connecting...")
         self._msgbus.subscribe("data.*", handler=self.on_data)
+
+        # Load all instruments for venue
+        for instrument in self.exchange.cache.instruments(venue=self.venue):
+            self.exchange.add_instrument(instrument)
+
         self._client._set_connected(True)
         self._set_connected(True)
         self._log.info("Connected")
 
     def disconnect(self) -> None:
         """
         Disconnect the client.
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/sandbox/factory.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/sandbox/factory.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/tardis/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/tardis/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/adapters/tardis/loaders.py` & `nautilus_trader-1.194.0/nautilus_trader/adapters/tardis/loaders.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pyx`

 * *Files 8% similar despite different names*

```diff
@@ -8,11 +8,12 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
-"""
-The `analysis` subpackage groups components relating to trading performance statistics
-and analysis.
-"""
+
+from nautilus_trader.indicators.fuzzy_enums.candle_size cimport CandleSize
+
+
+__all__ = ["CandleSize"]
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/analyzer.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/analyzer.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/reporter.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/reporter.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistic.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistic.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/expectancy.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/expectancy.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/long_ratio.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/long_ratio.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/loser_avg.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/loser_avg.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/loser_max.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/loser_max.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/loser_min.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/loser_min.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/profit_factor.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/profit_factor.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/returns_avg.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/returns_avg.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/returns_avg_loss.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/returns_avg_loss.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/returns_avg_win.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/returns_avg_win.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/returns_volatility.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/returns_volatility.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/risk_return_ratio.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/risk_return_ratio.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/sharpe_ratio.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/sharpe_ratio.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/sortino_ratio.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/sortino_ratio.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/win_rate.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/win_rate.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/winner_avg.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/winner_avg.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/winner_max.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/winner_max.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/analysis/statistics/winner_min.py` & `nautilus_trader-1.194.0/nautilus_trader/analysis/statistics/winner_min.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/backtest/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/backtest/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/__main__.py` & `nautilus_trader-1.194.0/nautilus_trader/backtest/__main__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/auction.py` & `nautilus_trader-1.194.0/nautilus_trader/backtest/auction.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/config.py` & `nautilus_trader-1.194.0/nautilus_trader/backtest/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/data_client.pxd` & `nautilus_trader-1.194.0/nautilus_trader/backtest/data_client.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/data_client.pyx` & `nautilus_trader-1.194.0/nautilus_trader/backtest/data_client.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/engine.pxd` & `nautilus_trader-1.194.0/nautilus_trader/backtest/engine.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/engine.pyx` & `nautilus_trader-1.194.0/nautilus_trader/backtest/engine.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -461,15 +461,14 @@
             venue=venue,
             oms_type=oms_type,
             account_type=account_type,
             starting_balances=starting_balances,
             base_currency=base_currency,
             default_leverage=default_leverage,
             leverages=leverages or {},
-            instruments=[],
             modules=modules,
             portfolio=self.kernel.portfolio,
             msgbus=self.kernel.msgbus,
             cache=self.kernel.cache,
             fill_model=fill_model,
             fee_model=fee_model,
             latency_model=latency_model,
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/exchange.pxd` & `nautilus_trader-1.194.0/nautilus_trader/backtest/exchange.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,16 @@
     """If contingent orders will be supported/respected by the venue.\n\n:returns: `bool`"""
     cdef readonly bint use_position_ids
     """If venue position IDs will be generated on order fills.\n\n:returns: `bool`"""
     cdef readonly bint use_random_ids
     """If venue order and position IDs will be randomly generated UUID4s.\n\n:returns: `bool`"""
     cdef readonly bint use_reduce_only
     """If the `reduce_only` option on orders will be honored.\n\n:returns: `bool`"""
+    cdef readonly bint use_message_queue
+    """If an internal message queue is being used to sequentially process incoming trading commands.\n\n:returns: `bool`"""
     cdef readonly list modules
     """The simulation modules registered with the exchange.\n\n:returns: `list[SimulationModule]`"""
     cdef readonly dict instruments
     """The exchange instruments.\n\n:returns: `dict[InstrumentId, Instrument]`"""
 
     cdef dict _matching_engines
     cdef object _message_queue
@@ -137,10 +139,12 @@
     cpdef void process_trade_tick(self, TradeTick tick)
     cpdef void process_bar(self, Bar bar)
     cpdef void process_venue_status(self, VenueStatus data)
     cpdef void process_instrument_status(self, InstrumentStatus data)
     cpdef void process(self, uint64_t ts_now)
     cpdef void reset(self)
 
+    cdef void _process_trading_command(self, TradingCommand command)
+
 # -- EVENT GENERATORS -----------------------------------------------------------------------------
 
     cdef void _generate_fresh_account_state(self)
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/exchange.pyx` & `nautilus_trader-1.194.0/nautilus_trader/backtest/exchange.pyx`

 * *Files 9% similar despite different names*

```diff
@@ -78,47 +78,54 @@
         The starting balances for the exchange.
     base_currency : Currency, optional
         The account base currency for the client. Use ``None`` for multi-currency accounts.
     default_leverage : Decimal
         The account default leverage (for margin accounts).
     leverages : dict[InstrumentId, Decimal]
         The instrument specific leverage configuration (for margin accounts).
+    modules : list[SimulatedModule]
+        The simulation modules for the exchange.
     portfolio : PortfolioFacade
         The read-only portfolio for the exchange.
     msgbus : MessageBus
         The message bus for the exchange.
     cache : CacheFacade
         The read-only cache for the exchange.
+    clock : TestClock
+        The clock for the exchange.
     fill_model : FillModel
         The fill model for the exchange.
     fee_model : FeeModel
         The fee model for the exchange.
     latency_model : LatencyModel, optional
         The latency model for the exchange.
-    clock : TestClock
-        The clock for the exchange.
     book_type : BookType
         The order book type for the exchange.
     frozen_account : bool, default False
         If the account for this exchange is frozen (balances will not change).
     bar_execution : bool, default True
         If bars should be processed by the matching engine(s) (and move the market).
     reject_stop_orders : bool, default True
         If stop orders are rejected on submission if in the market.
     support_gtd_orders : bool, default True
-        If orders with GTD time in force will be supported by the venue.
+        If orders with GTD time in force will be supported by the exchange.
     support_contingent_orders : bool, default True
-        If contingent orders will be supported/respected by the venue.
+        If contingent orders will be supported/respected by the exchange.
         If False then its expected the strategy will be managing any contingent orders.
     use_position_ids : bool, default True
         If venue position IDs will be generated on order fills.
     use_random_ids : bool, default False
-        If all venue generated identifiers will be random UUID4's.
+        If all exchange generated identifiers will be random UUID4's.
     use_reduce_only : bool, default True
         If the `reduce_only` execution instruction on orders will be honored.
+    use_message_queue : bool, default True
+        If an internal message queue should be used to process trading commands in sequence after
+        they have initially arrived. Setting this to False would be appropriate for real-time
+        sandbox environments, where we don't want to introduce additional latency of waiting for
+        the next data event before processing the trading command.
 
     Raises
     ------
     ValueError
         If `instruments` is empty.
     ValueError
         If `instruments` contains a type other than `Instrument`.
@@ -126,26 +133,26 @@
         If `starting_balances` is empty.
     ValueError
         If `starting_balances` contains a type other than `Money`.
     ValueError
         If `base_currency` and multiple starting balances.
     ValueError
         If `modules` contains a type other than `SimulationModule`.
+
     """
 
     def __init__(
         self,
         Venue venue not None,
         OmsType oms_type,
         AccountType account_type,
         list starting_balances not None,
         Currency base_currency: Currency | None,
         default_leverage not None: Decimal,
         leverages not None: dict[InstrumentId, Decimal],
-        list instruments not None,
         list modules not None,
         PortfolioFacade portfolio not None,
         MessageBus msgbus not None,
         CacheFacade cache not None,
         TestClock clock not None,
         FillModel fill_model not None,
         FeeModel fee_model not None,
@@ -155,16 +162,16 @@
         bint bar_execution = True,
         bint reject_stop_orders = True,
         bint support_gtd_orders = True,
         bint support_contingent_orders = True,
         bint use_position_ids = True,
         bint use_random_ids = False,
         bint use_reduce_only = True,
+        bint use_message_queue = True,
     ) -> None:
-        Condition.list_type(instruments, Instrument, "instruments", "Instrument")
         Condition.not_empty(starting_balances, "starting_balances")
         Condition.list_type(starting_balances, Money, "starting_balances")
         Condition.list_type(modules, SimulationModule, "modules", "SimulationModule")
         if base_currency:
             Condition.true(len(starting_balances) == 1, "single-currency account has multiple starting currencies")
         if default_leverage and default_leverage > 1 or leverages:
             Condition.true(account_type == AccountType.MARGIN, "leverages defined when account type is not `MARGIN`")
@@ -193,14 +200,15 @@
         self.bar_execution = bar_execution
         self.reject_stop_orders = reject_stop_orders
         self.support_gtd_orders = support_gtd_orders
         self.support_contingent_orders = support_contingent_orders
         self.use_position_ids = use_position_ids
         self.use_random_ids = use_random_ids
         self.use_reduce_only = use_reduce_only
+        self.use_message_queue = use_message_queue
         self.fill_model = fill_model
         self.fee_model = fee_model
         self.latency_model = latency_model
 
         # Load modules
         self.modules = []
         for module in modules:
@@ -212,24 +220,20 @@
                 cache=cache,
                 clock=clock,
             )
             self.modules.append(module)
             self._log.info(f"Loaded {module}")
 
         # Markets
-        self._matching_engines: dict[InstrumentId, OrderMatchingEngine] = {}
-
-        # Load instruments
         self.instruments: dict[InstrumentId, Instrument] = {}
-        for instrument in instruments:
-            self.add_instrument(instrument)
+        self._matching_engines: dict[InstrumentId, OrderMatchingEngine] = {}
 
         self._message_queue = deque()
         self._inflight_queue: list[tuple[(uint64_t, uint64_t), TradingCommand]] = []
-        self._inflight_counter: dict[uint64_t, int] = {}
+        self._inflight_counter: dict[uint64_t, uint64_t] = {}
 
     def __repr__(self) -> str:
         return (
             f"{type(self).__name__}("
             f"id={self.id}, "
             f"oms_type={oms_type_to_str(self.oms_type)}, "
             f"account_type={account_type_to_str(self.account_type)})"
@@ -290,22 +294,21 @@
         self.latency_model = latency_model
 
         self._log.info("Changed latency model")
 
     cpdef void initialize_account(self):
         """
         Initialize the account to the starting balances.
+
         """
         self._generate_fresh_account_state()
 
     cpdef void add_instrument(self, Instrument instrument):
         """
-        Add the given instrument to the venue.
-
-        A random and unique 32-bit unsigned integer raw ID will be generated.
+        Add the given instrument to the exchange.
 
         Parameters
         ----------
         instrument : Instrument
             The instrument to add.
 
         Raises
@@ -617,15 +620,17 @@
         ----------
         command : TradingCommand
             The command to send.
 
         """
         Condition.not_none(command, "command")
 
-        if self.latency_model is None:
+        if not self.use_message_queue:
+            self._process_trading_command(command)
+        elif self.latency_model is None:
             self._message_queue.appendleft(command)
         else:
             heappush(self._inflight_queue, self.generate_inflight_command(command))
 
     cdef tuple generate_inflight_command(self, TradingCommand command):
         cdef uint64_t ts
         if isinstance(command, (SubmitOrder, SubmitOrderList)):
@@ -656,15 +661,19 @@
 
         cdef SimulationModule module
         for module in self.modules:
             module.pre_process(delta)
 
         cdef OrderMatchingEngine matching_engine = self._matching_engines.get(delta.instrument_id)
         if matching_engine is None:
-            raise RuntimeError(f"No matching engine found for {delta.instrument_id}")
+            instrument = self.cache.instrument(delta.instrument_id)
+            if instrument is None:
+                raise RuntimeError(f"No matching engine found for {delta.instrument_id}")
+            self.add_instrument(instrument)
+            matching_engine = self._matching_engines[delta.instrument_id]
 
         matching_engine.process_order_book_delta(delta)
 
     cpdef void process_order_book_deltas(self, OrderBookDeltas deltas):
         """
         Process the exchanges market for the given order book deltas.
 
@@ -678,15 +687,19 @@
 
         cdef SimulationModule module
         for module in self.modules:
             module.pre_process(deltas)
 
         cdef OrderMatchingEngine matching_engine = self._matching_engines.get(deltas.instrument_id)
         if matching_engine is None:
-            raise RuntimeError(f"No matching engine found for {deltas.instrument_id}")
+            instrument = self.cache.instrument(deltas.instrument_id)
+            if instrument is None:
+                raise RuntimeError(f"No matching engine found for {deltas.instrument_id}")
+            self.add_instrument(instrument)
+            matching_engine = self._matching_engines[deltas.instrument_id]
 
         matching_engine.process_order_book_deltas(deltas)
 
     cpdef void process_quote_tick(self, QuoteTick tick):
         """
         Process the exchanges market for the given quote tick.
 
@@ -702,15 +715,19 @@
 
         cdef SimulationModule module
         for module in self.modules:
             module.pre_process(tick)
 
         cdef OrderMatchingEngine matching_engine = self._matching_engines.get(tick.instrument_id)
         if matching_engine is None:
-            raise RuntimeError(f"No matching engine found for {tick.instrument_id}")
+            instrument = self.cache.instrument(tick.instrument_id)
+            if instrument is None:
+                raise RuntimeError(f"No matching engine found for {tick.instrument_id}")
+            self.add_instrument(instrument)
+            matching_engine = self._matching_engines[tick.instrument_id]
 
         matching_engine.process_quote_tick(tick)
 
     cpdef void process_trade_tick(self, TradeTick tick):
         """
         Process the exchanges market for the given trade tick.
 
@@ -726,15 +743,19 @@
 
         cdef SimulationModule module
         for module in self.modules:
             module.pre_process(tick)
 
         cdef OrderMatchingEngine matching_engine = self._matching_engines.get(tick.instrument_id)
         if matching_engine is None:
-            raise RuntimeError(f"No matching engine found for {tick.instrument_id}")
+            instrument = self.cache.instrument(tick.instrument_id)
+            if instrument is None:
+                raise RuntimeError(f"No matching engine found for {tick.instrument_id}")
+            self.add_instrument(instrument)
+            matching_engine = self._matching_engines[tick.instrument_id]
 
         matching_engine.process_trade_tick(tick)
 
     cpdef void process_bar(self, Bar bar):
         """
         Process the exchanges market for the given bar.
 
@@ -750,15 +771,19 @@
 
         cdef SimulationModule module
         for module in self.modules:
             module.pre_process(bar)
 
         cdef OrderMatchingEngine matching_engine = self._matching_engines.get(bar.bar_type.instrument_id)
         if matching_engine is None:
-            raise RuntimeError(f"No matching engine found for {bar.bar_type.instrument_id}")
+            instrument = self.cache.instrument(bar.bar_type.instrument_id)
+            if instrument is None:
+                raise RuntimeError(f"No matching engine found for {bar.bar_type.instrument_id}")
+            self.add_instrument(instrument)
+            matching_engine = self._matching_engines[bar.bar_type.instrument_id]
 
         matching_engine.process_bar(bar)
 
     cpdef void process_venue_status(self, VenueStatus data):
         """
         Process the exchange for the given status.
 
@@ -792,21 +817,25 @@
 
         cdef SimulationModule module
         for module in self.modules:
             module.pre_process(data)
 
         cdef OrderMatchingEngine matching_engine = self._matching_engines.get(data.instrument_id)
         if matching_engine is None:
-            raise RuntimeError(f"No matching engine found for {data.instrument_id}")
+            instrument = self.cache.instrument(data.instrument_id)
+            if instrument is None:
+                raise RuntimeError(f"No matching engine found for {data.instrument_id}")
+            self.add_instrument(instrument)
+            matching_engine = self._matching_engines[data.instrument_id]
 
         matching_engine.process_status(data.status)
 
     cpdef void process(self, uint64_t ts_now):
         """
-        Process the exchange to the gives time.
+        Process the exchange to the given time.
 
         All pending commands will be processed along with all simulation modules.
 
         Parameters
         ----------
         ts_now : uint64_t
             The current UNIX timestamp (nanoseconds).
@@ -822,33 +851,18 @@
             if ts <= ts_now:
                 # Place message on queue to be processed
                 self._message_queue.appendleft(self._inflight_queue.pop(0)[1])
                 self._inflight_counter.pop(ts, None)
             else:
                 break
 
-        cdef:
-            TradingCommand command
-            Order order
-            list orders
+        cdef TradingCommand command
         while self._message_queue:
             command = self._message_queue.pop()
-            if isinstance(command, SubmitOrder):
-                self._matching_engines[command.instrument_id].process_order(command.order, self.exec_client.account_id)
-            elif isinstance(command, SubmitOrderList):
-                for order in command.order_list.orders:
-                    self._matching_engines[command.instrument_id].process_order(order, self.exec_client.account_id)
-            elif isinstance(command, ModifyOrder):
-                self._matching_engines[command.instrument_id].process_modify(command, self.exec_client.account_id)
-            elif isinstance(command, CancelOrder):
-                self._matching_engines[command.instrument_id].process_cancel(command, self.exec_client.account_id)
-            elif isinstance(command, CancelAllOrders):
-                self._matching_engines[command.instrument_id].process_cancel_all(command, self.exec_client.account_id)
-            elif isinstance(command, BatchCancelOrders):
-                self._matching_engines[command.instrument_id].process_batch_cancel(command, self.exec_client.account_id)
+            self._process_trading_command(command)
 
         # Iterate over modules
         cdef SimulationModule module
         for module in self.modules:
             module.process(ts_now)
 
     cpdef void reset(self):
@@ -869,14 +883,36 @@
 
         self._message_queue = deque()
         self._inflight_queue.clear()
         self._inflight_counter.clear()
 
         self._log.info("Reset")
 
+    cdef void _process_trading_command(self, TradingCommand command):
+        cdef OrderMatchingEngine matching_engine = self._matching_engines.get(command.instrument_id)
+        if matching_engine is None:
+            raise RuntimeError(f"Cannot process command: no matching engine for {command.instrument_id}")
+
+        cdef:
+            Order order
+            list[Order] orders
+        if isinstance(command, SubmitOrder):
+            matching_engine.process_order(command.order, self.exec_client.account_id)
+        elif isinstance(command, SubmitOrderList):
+            for order in command.order_list.orders:
+                matching_engine.process_order(order, self.exec_client.account_id)
+        elif isinstance(command, ModifyOrder):
+            matching_engine.process_modify(command, self.exec_client.account_id)
+        elif isinstance(command, CancelOrder):
+            matching_engine.process_cancel(command, self.exec_client.account_id)
+        elif isinstance(command, CancelAllOrders):
+            matching_engine.process_cancel_all(command, self.exec_client.account_id)
+        elif isinstance(command, BatchCancelOrders):
+            matching_engine.process_batch_cancel(command, self.exec_client.account_id)
+
 # -- EVENT GENERATORS -----------------------------------------------------------------------------
 
     cdef void _generate_fresh_account_state(self):
         cdef list balances = [
             AccountBalance(
                 total=money,
                 locked=Money(0, money.currency),
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/execution_client.pxd` & `nautilus_trader-1.194.0/nautilus_trader/portfolio/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
+"""
+The `portfolio` subpackage provides portfolio management functionality.
+"""
 
-from nautilus_trader.backtest.exchange cimport SimulatedExchange
-from nautilus_trader.execution.client cimport ExecutionClient
+from nautilus_trader.portfolio.base import PortfolioFacade
+from nautilus_trader.portfolio.portfolio import Portfolio
 
 
-cdef class BacktestExecClient(ExecutionClient):
-    cdef SimulatedExchange _exchange
+__all__ = [
+    "Portfolio",
+    "PortfolioFacade",
+]
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/execution_client.pyx` & `nautilus_trader-1.194.0/nautilus_trader/backtest/execution_client.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/matching_engine.pxd` & `nautilus_trader-1.194.0/nautilus_trader/backtest/matching_engine.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/matching_engine.pyx` & `nautilus_trader-1.194.0/nautilus_trader/backtest/matching_engine.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/models.pxd` & `nautilus_trader-1.194.0/nautilus_trader/backtest/models.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/models.pyx` & `nautilus_trader-1.194.0/nautilus_trader/backtest/models.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/modules.pxd` & `nautilus_trader-1.194.0/nautilus_trader/backtest/modules.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/modules.pyx` & `nautilus_trader-1.194.0/nautilus_trader/backtest/modules.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/node.py` & `nautilus_trader-1.194.0/nautilus_trader/backtest/node.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/backtest/results.py` & `nautilus_trader-1.194.0/nautilus_trader/backtest/results.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/cache/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/cache/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/cache/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/cache/base.pxd` & `nautilus_trader-1.194.0/nautilus_trader/cache/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/cache/base.pyx` & `nautilus_trader-1.194.0/nautilus_trader/cache/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/cache/cache.pxd` & `nautilus_trader-1.194.0/nautilus_trader/cache/cache.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/cache/cache.pyx` & `nautilus_trader-1.194.0/nautilus_trader/cache/cache.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/cache/config.py` & `nautilus_trader-1.194.0/nautilus_trader/cache/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/cache/database.pxd` & `nautilus_trader-1.194.0/nautilus_trader/cache/database.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/cache/database.pyx` & `nautilus_trader-1.194.0/nautilus_trader/cache/database.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/cache/facade.pxd` & `nautilus_trader-1.194.0/nautilus_trader/cache/facade.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/cache/facade.pyx` & `nautilus_trader-1.194.0/nautilus_trader/cache/facade.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/cache/postgres/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/cache/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/cache/postgres/adapter.py` & `nautilus_trader-1.194.0/nautilus_trader/cache/postgres/adapter.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/cache/postgres/transformers.py` & `nautilus_trader-1.194.0/nautilus_trader/cache/postgres/transformers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/common/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/common/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/common/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/common/actor.pxd` & `nautilus_trader-1.194.0/nautilus_trader/common/actor.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/common/actor.pyx` & `nautilus_trader-1.194.0/nautilus_trader/common/actor.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/common/component.pxd` & `nautilus_trader-1.194.0/nautilus_trader/common/component.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/common/component.pyx` & `nautilus_trader-1.194.0/nautilus_trader/common/component.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/common/config.py` & `nautilus_trader-1.194.0/nautilus_trader/common/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,15 @@
     use_instance_id : bool, default False
         If the traders instance ID is used for stream names.
     streams_prefix : str, default 'streams'
         The prefix for externally published stream names (must have a `database` config).
         If `use_trader_id` and `use_instance_id` are *both* false, then it becomes possible for
         many traders to be configured to write to the same streams.
     types_filter : list[type], optional
-        A list of serializable types *not* to publish externally.
+        A list of serializable types **not** to publish externally.
 
     """
 
     database: DatabaseConfig | None = None
     encoding: str = "msgpack"
     timestamps_as_iso8601: bool = False
     buffer_interval_ms: PositiveInt | None = None
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/common/enums.py` & `nautilus_trader-1.194.0/nautilus_trader/common/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/common/executor.py` & `nautilus_trader-1.194.0/nautilus_trader/common/executor.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/common/factories.pxd` & `nautilus_trader-1.194.0/nautilus_trader/common/factories.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/common/factories.pyx` & `nautilus_trader-1.194.0/nautilus_trader/common/factories.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/common/functions.py` & `nautilus_trader-1.194.0/nautilus_trader/common/functions.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/common/generators.pxd` & `nautilus_trader-1.194.0/nautilus_trader/common/generators.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/common/generators.pyx` & `nautilus_trader-1.194.0/nautilus_trader/common/generators.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/common/messages.pxd` & `nautilus_trader-1.194.0/nautilus_trader/common/messages.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/common/messages.pyx` & `nautilus_trader-1.194.0/nautilus_trader/common/messages.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/common/providers.py` & `nautilus_trader-1.194.0/nautilus_trader/common/providers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/config/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/core/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/core/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/asynchronous.py` & `nautilus_trader-1.194.0/nautilus_trader/indicators/bias.pxd`

 * *Files 20% similar despite different names*

```diff
@@ -9,23 +9,21 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-import types
+from nautilus_trader.indicators.average.moving_average cimport MovingAverage
+from nautilus_trader.indicators.base.indicator cimport Indicator
 
 
-@types.coroutine
-def sleep0():
-    """
-    Skip one event loop run cycle.
+cdef class Bias(Indicator):
+    cdef MovingAverage _ma
 
-    This is equivalent to `asyncio.sleep(0)` however avoids the overhead of the Python
-    function call and integer comparison <= 0.
+    cdef readonly int period
+    """The window period.\n\n:returns: `int`"""
+    cdef readonly double value
+    """The current value.\n\n:returns: `double`"""
 
-    Uses a bare 'yield' expression (which Task.__step knows how to handle) instead of
-    creating a Future object.
-
-    """
-    yield
+    cpdef void update_raw(self, double close)
+    cdef void _check_initialized(self)
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/correctness.pxd` & `nautilus_trader-1.194.0/nautilus_trader/core/correctness.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/correctness.pyx` & `nautilus_trader-1.194.0/nautilus_trader/core/correctness.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -694,14 +694,17 @@
         double end,
         str param,
         ex_type = None,
     ):
         """
         Check the real number value is within the specified range (inclusive).
 
+        This function accounts for potential floating-point precision issues by using a small
+        epsilon value of 1e-15.
+
         Parameters
         ----------
         value : scalar
             The value to check.
         start : scalar
             The start of the range.
         end : scalar
@@ -713,15 +716,16 @@
 
         Raises
         -------
         ValueError
               If `value` is not within the range (inclusive of the end points).
 
         """
-        if start <= value <= end:
+        cdef double epsilon = 1e-15  # Epsilon to account for floating-point precision issues
+        if start - epsilon <= value <= end + epsilon:
             return  # Check passed
 
         raise make_exception(
             ex_default=ValueError,
             ex_type=ex_type,
             msg=(f"The \'{param}\' was out of range [{start:_}, {end:_}]"
                  f", was {value:_}"),
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/data.pxd` & `nautilus_trader-1.194.0/nautilus_trader/core/data.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/data.pyx` & `nautilus_trader-1.194.0/nautilus_trader/core/data.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/datetime.pxd` & `nautilus_trader-1.194.0/nautilus_trader/core/datetime.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/datetime.pyx` & `nautilus_trader-1.194.0/nautilus_trader/core/datetime.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/fsm.pxd` & `nautilus_trader-1.194.0/nautilus_trader/core/fsm.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/fsm.pyx` & `nautilus_trader-1.194.0/nautilus_trader/core/fsm.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/includes/algorithms.h` & `nautilus_trader-1.194.0/nautilus_trader/core/includes/algorithms.h`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/includes/backtest.h` & `nautilus_trader-1.194.0/nautilus_trader/core/includes/backtest.h`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/includes/common.h` & `nautilus_trader-1.194.0/nautilus_trader/core/includes/common.h`

 * *Files 2% similar despite different names*

```diff
@@ -189,51 +189,61 @@
     WARNING = 30,
     /**
      * The **ERROR** error log level.
      */
     ERROR = 40,
 } LogLevel;
 
+/**
+ * A real-time clock which uses system time.
+ *
+ * Timestamps are guaranteed to be unique and monotonically increasing.
+ */
 typedef struct LiveClock LiveClock;
 
 typedef struct LogGuard LogGuard;
 
+/**
+ * A static test clock.
+ *
+ * Stores the current timestamp internally which can be advanced.
+ */
 typedef struct TestClock TestClock;
 
 /**
- * Provides a C compatible Foreign Function Interface (FFI) for an underlying [`TestClock`].
+ * C compatible Foreign Function Interface (FFI) for an underlying [`TestClock`].
  *
  * This struct wraps `TestClock` in a way that makes it compatible with C function
  * calls, enabling interaction with `TestClock` in a C environment.
  *
  * It implements the `Deref` trait, allowing instances of `TestClock_API` to be
  * dereferenced to `TestClock`, providing access to `TestClock`'s methods without
  * having to manually access the underlying `TestClock` instance.
  */
 typedef struct TestClock_API {
     struct TestClock *_0;
 } TestClock_API;
 
 /**
- * Provides a C compatible Foreign Function Interface (FFI) for an underlying [`LiveClock`].
+ * C compatible Foreign Function Interface (FFI) for an underlying [`LiveClock`].
  *
  * This struct wraps `LiveClock` in a way that makes it compatible with C function
  * calls, enabling interaction with `LiveClock` in a C environment.
  *
  * It implements the `Deref` and `DerefMut` traits, allowing instances of `LiveClock_API` to be
  * dereferenced to `LiveClock`, providing access to `LiveClock`'s methods without
  * having to manually access the underlying `LiveClock` instance. This includes
  * both mutable and immutable access.
  */
 typedef struct LiveClock_API {
     struct LiveClock *_0;
 } LiveClock_API;
 
 /**
- * Provides a C compatible Foreign Function Interface (FFI) for an underlying [`LogGuard`].
+ * C compatible Foreign Function Interface (FFI) for an underlying [`LogGuard`].
  *
  * This struct wraps `LogGuard` in a way that makes it compatible with C function
  * calls, enabling interaction with `LogGuard` in a C environment.
  *
  * It implements the `Deref` trait, allowing instances of `LogGuard_API` to be
  * dereferenced to `LogGuard`, providing access to `LogGuard`'s methods without
  * having to manually access the underlying `LogGuard` instance.
@@ -265,15 +275,15 @@
 } TimeEvent_t;
 
 /**
  * Represents a time event and its associated handler.
  */
 typedef struct TimeEventHandler_t {
     /**
-     * The event.
+     * The time event.
      */
     struct TimeEvent_t event;
     /**
      * The callable raw pointer.
      */
     char *callback_ptr;
 } TimeEventHandler_t;
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/includes/core.h` & `nautilus_trader-1.194.0/nautilus_trader/core/includes/core.h`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/includes/model.h` & `nautilus_trader-1.194.0/nautilus_trader/core/includes/model.h`

 * *Files 1% similar despite different names*

```diff
@@ -134,19 +134,19 @@
  */
 typedef enum BookType {
     /**
      * Top-of-book best bid/ask, one level per side.
      */
     L1_MBP = 1,
     /**
-     * Market by price, one order per level (aggregated).
+     * Market-by-price, one order per level (aggregated).
      */
     L2_MBP = 2,
     /**
-     * Market by order, multiple orders per level (full granularity).
+     * Market-by-order, multiple orders per level (full granularity).
      */
     L3_MBO = 3,
 } BookType;
 
 /**
  * The order contigency type which specifies the behavior of linked orders.
  *
@@ -543,15 +543,15 @@
 } PriceType;
 
 /**
  * A record flag bit field, indicating event end and data information.
  */
 typedef enum RecordFlag {
     /**
-     * Last message in the packet from the venue for a given `instrument_id`.
+     * Last message in the book event or packet from the venue for a given `instrument_id`.
      */
     F_LAST = (1 << 7),
     /**
      * Top-of-book message, not an individual order.
      */
     F_TOB = (1 << 6),
     /**
@@ -701,20 +701,20 @@
  *
  * The level maintains a collection of orders as well as tracking insertion order
  * to preserve FIFO queue dynamics.
  */
 typedef struct Level Level;
 
 /**
- * Provides an order book.
+ * Provides a performant, generic, multi-purpose order book.
  *
  * Can handle the following granularity data:
- * - MBO (market by order) / L3
- * - MBP (market by price) / L2 aggregated order per level
- * - MBP (market by price) / L1 top-of-book only
+ * - MBO (market-by-order) / L3
+ * - MBP (market-by-price) / L2 aggregated order per level
+ * - MBP (market-by-price) / L1 top-of-book only
  */
 typedef struct OrderBook OrderBook;
 
 /**
  * Represents a grouped batch of `OrderBookDelta` updates for an `OrderBook`.
  *
  * This type cannot be `repr(C)` due to the `deltas` vec.
@@ -820,15 +820,15 @@
     /**
      * The UNIX timestamp (nanoseconds) when the struct was initialized.
      */
     uint64_t ts_init;
 } OrderBookDelta_t;
 
 /**
- * Provides a C compatible Foreign Function Interface (FFI) for an underlying [`OrderBookDeltas`].
+ * C compatible Foreign Function Interface (FFI) for an underlying [`OrderBookDeltas`].
  *
  * This struct wraps `OrderBookDeltas` in a way that makes it compatible with C function
  * calls, enabling interaction with `OrderBookDeltas` in a C environment.
  *
  * It implements the `Deref` trait, allowing instances of `OrderBookDeltas_API` to be
  * dereferenced to `OrderBookDeltas`, providing access to `OrderBookDeltas`'s methods without
  * having to manually access the underlying `OrderBookDeltas` instance.
@@ -920,19 +920,14 @@
      */
     uint64_t ts_init;
 } QuoteTick_t;
 
 /**
  * Represents a valid trade match ID (assigned by a trading venue).
  *
- * Maximum length is 36 characters.
- *
- * The unique ID assigned to the trade entity once it is received or matched by
- * the exchange or central counterparty.
- *
  * Can correspond to the `TradeID <1003> field` of the FIX protocol.
  */
 typedef struct TradeId_t {
     /**
      * The trade match ID value as a fixed-length C string byte array (includes null terminator).
      */
     uint8_t value[37];
@@ -1085,38 +1080,21 @@
             struct Bar_t bar;
         };
     };
 } Data_t;
 
 /**
  * Represents a valid trader ID.
- *
- * Must be correctly formatted with two valid strings either side of a hyphen.
- * It is expected a trader ID is the abbreviated name of the trader
- * with an order ID tag number separated by a hyphen.
- *
- * Example: "TESTER-001".
- * The reason for the numerical component of the ID is so that order and position IDs
- * do not collide with those from another node instance.
  */
 typedef struct TraderId_t {
     char* _0;
 } TraderId_t;
 
 /**
  * Represents a valid strategy ID.
- *
- * Must be correctly formatted with two valid strings either side of a hyphen.
- * It is expected a strategy ID is the class name of the strategy,
- * with an order ID tag number separated by a hyphen.
- *
- * Example: "EMACross-001".
- *
- * The reason for the numerical component of the ID is so that order and position IDs
- * do not collide with those from another strategy within the node instance.
  */
 typedef struct StrategyId_t {
     char* _0;
 } StrategyId_t;
 
 /**
  * Represents a valid client order ID (assigned by the Nautilus system).
@@ -1155,20 +1133,14 @@
     UUID4_t event_id;
     uint64_t ts_event;
     uint64_t ts_init;
 } OrderReleased_t;
 
 /**
  * Represents a valid account ID.
- *
- * Must be correctly formatted with two valid strings either side of a hyphen '-'.
- * It is expected an account ID is the name of the issuer with an account number
- * separated by a hyphen.
- *
- * Example: "IB-D02851908".
  */
 typedef struct AccountId_t {
     char* _0;
 } AccountId_t;
 
 typedef struct OrderSubmitted_t {
     struct TraderId_t trader_id;
@@ -1246,44 +1218,44 @@
  * Represents a valid position ID.
  */
 typedef struct PositionId_t {
     char* _0;
 } PositionId_t;
 
 /**
- * Provides a C compatible Foreign Function Interface (FFI) for an underlying
+ * C compatible Foreign Function Interface (FFI) for an underlying
  * [`SyntheticInstrument`].
  *
  * This struct wraps `SyntheticInstrument` in a way that makes it compatible with C function
  * calls, enabling interaction with `SyntheticInstrument` in a C environment.
  *
  * It implements the `Deref` trait, allowing instances of `SyntheticInstrument_API` to be
  * dereferenced to `SyntheticInstrument`, providing access to `SyntheticInstruments`'s methods without
  * having to manually access the underlying instance.
  */
 typedef struct SyntheticInstrument_API {
     struct SyntheticInstrument *_0;
 } SyntheticInstrument_API;
 
 /**
- * Provides a C compatible Foreign Function Interface (FFI) for an underlying `OrderBook`.
+ * C compatible Foreign Function Interface (FFI) for an underlying `OrderBook`.
  *
  * This struct wraps `OrderBook` in a way that makes it compatible with C function
  * calls, enabling interaction with `OrderBook` in a C environment.
  *
  * It implements the `Deref` trait, allowing instances of `OrderBook_API` to be
  * dereferenced to `OrderBook`, providing access to `OrderBook`'s methods without
  * having to manually access the underlying `OrderBook` instance.
  */
 typedef struct OrderBook_API {
     struct OrderBook *_0;
 } OrderBook_API;
 
 /**
- * Provides a C compatible Foreign Function Interface (FFI) for an underlying order book[`Level`].
+ * C compatible Foreign Function Interface (FFI) for an underlying order book[`Level`].
  *
  * This struct wraps `Level` in a way that makes it compatible with C function
  * calls, enabling interaction with `Level` in a C environment.
  *
  * It implements the `Deref` trait, allowing instances of `Level_API` to be
  * dereferenced to `Level`, providing access to `Level`'s methods without
  * having to manually acce wss the underlying `Level` instance.
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/inspect.py` & `nautilus_trader-1.194.0/nautilus_trader/core/inspect.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/message.pxd` & `nautilus_trader-1.194.0/nautilus_trader/core/message.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/message.pyx` & `nautilus_trader-1.194.0/nautilus_trader/core/message.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/nautilus_pyo3.pyi` & `nautilus_trader-1.194.0/nautilus_trader/core/nautilus_pyo3.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2660,14 +2660,50 @@
     def cmo_pct(self) -> float: ...
     def update_raw(self, value: float) -> None: ...
     def handle_quote_tick(self, quote: QuoteTick) -> None: ...
     def handle_trade_tick(self, trade: TradeTick) -> None: ...
     def handle_bar(self, bar: Bar) -> None: ...
     def reset(self) -> None: ...
 
+class VolumeWeightedAveragePrice:
+    def __init__(
+        self
+    ) -> None: ...
+    @property
+    def name(self) -> str: ...
+    @property
+    def initialized(self) -> bool: ...
+    @property
+    def has_inputs(self) -> bool: ...
+    @property
+    def value(self) -> float: ...
+    def update_raw(self, price: float, volume: float, timestamp: float ) -> None: ...
+    def handle_bar(self, bar: Bar) -> None: ...
+    def reset(self) -> None: ...
+
+class VerticalHorizontalFilter:
+    def __init__(
+        self,
+        period: int,
+        ma_type: MovingAverageType = ...,
+    ) -> None: ...
+    @property
+    def name(self) -> str: ...
+    @property
+    def period(self) -> int: ...
+    @property
+    def initialized(self) -> bool: ...
+    @property
+    def has_inputs(self) -> bool: ...
+    @property
+    def value(self) -> float: ...
+    def update_raw(self, close: float) -> None: ...
+    def handle_bar(self, bar: Bar) -> None: ...
+    def reset(self) -> None: ...
+
 class ChandeMomentumOscillator:
     def __init__(
         self,
         period: int,
     ) -> None: ...
     @property
     def name(self) -> str: ...
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/rust/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/core/rust/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/rust/algorithms.pxd` & `nautilus_trader-1.194.0/nautilus_trader/core/rust/algorithms.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/rust/backtest.pxd` & `nautilus_trader-1.194.0/nautilus_trader/core/rust/backtest.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/rust/common.pxd` & `nautilus_trader-1.194.0/nautilus_trader/core/rust/common.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -97,47 +97,53 @@
         # The **INFO** info log level.
         INFO # = 20,
         # The **WARNING** warning log level.
         WARNING # = 30,
         # The **ERROR** error log level.
         ERROR # = 40,
 
+    # A real-time clock which uses system time.
+    #
+    # Timestamps are guaranteed to be unique and monotonically increasing.
     cdef struct LiveClock:
         pass
 
     cdef struct LogGuard:
         pass
 
+    # A static test clock.
+    #
+    # Stores the current timestamp internally which can be advanced.
     cdef struct TestClock:
         pass
 
-    # Provides a C compatible Foreign Function Interface (FFI) for an underlying [`TestClock`].
+    # C compatible Foreign Function Interface (FFI) for an underlying [`TestClock`].
     #
     # This struct wraps `TestClock` in a way that makes it compatible with C function
     # calls, enabling interaction with `TestClock` in a C environment.
     #
     # It implements the `Deref` trait, allowing instances of `TestClock_API` to be
     # dereferenced to `TestClock`, providing access to `TestClock`'s methods without
     # having to manually access the underlying `TestClock` instance.
     cdef struct TestClock_API:
         TestClock *_0;
 
-    # Provides a C compatible Foreign Function Interface (FFI) for an underlying [`LiveClock`].
+    # C compatible Foreign Function Interface (FFI) for an underlying [`LiveClock`].
     #
     # This struct wraps `LiveClock` in a way that makes it compatible with C function
     # calls, enabling interaction with `LiveClock` in a C environment.
     #
     # It implements the `Deref` and `DerefMut` traits, allowing instances of `LiveClock_API` to be
     # dereferenced to `LiveClock`, providing access to `LiveClock`'s methods without
     # having to manually access the underlying `LiveClock` instance. This includes
     # both mutable and immutable access.
     cdef struct LiveClock_API:
         LiveClock *_0;
 
-    # Provides a C compatible Foreign Function Interface (FFI) for an underlying [`LogGuard`].
+    # C compatible Foreign Function Interface (FFI) for an underlying [`LogGuard`].
     #
     # This struct wraps `LogGuard` in a way that makes it compatible with C function
     # calls, enabling interaction with `LogGuard` in a C environment.
     #
     # It implements the `Deref` trait, allowing instances of `LogGuard_API` to be
     # dereferenced to `LogGuard`, providing access to `LogGuard`'s methods without
     # having to manually access the underlying `LogGuard` instance.
@@ -153,15 +159,15 @@
         # The message category
         uint64_t ts_event;
         # The UNIX timestamp (nanoseconds) when the object was initialized.
         uint64_t ts_init;
 
     # Represents a time event and its associated handler.
     cdef struct TimeEventHandler_t:
-        # The event.
+        # The time event.
         TimeEvent_t event;
         # The callable raw pointer.
         char *callback_ptr;
 
     # Returns whether the core logger is enabled.
     uint8_t logging_is_initialized();
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/rust/common.pyx` & `nautilus_trader-1.194.0/nautilus_trader/core/rust/common.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/rust/core.pxd` & `nautilus_trader-1.194.0/nautilus_trader/core/rust/core.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/rust/model.pxd` & `nautilus_trader-1.194.0/nautilus_trader/core/rust/model.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -76,17 +76,17 @@
         # The state of the order book is cleared.
         CLEAR # = 4,
 
     # The order book type, representing the type of levels granularity and delta updating heuristics.
     cpdef enum BookType:
         # Top-of-book best bid/ask, one level per side.
         L1_MBP # = 1,
-        # Market by price, one order per level (aggregated).
+        # Market-by-price, one order per level (aggregated).
         L2_MBP # = 2,
-        # Market by order, multiple orders per level (full granularity).
+        # Market-by-order, multiple orders per level (full granularity).
         L3_MBO # = 3,
 
     # The order contigency type which specifies the behavior of linked orders.
     #
     # [FIX 5.0 SP2 : ContingencyType <1385> field](https://www.onixs.biz/fix-dictionary/5.0.sp2/tagnum_1385.html).
     cpdef enum ContingencyType:
         # Not a contingent order.
@@ -292,15 +292,15 @@
         # The midpoint between the bid and ask prices.
         MID # = 3,
         # The last price at which a trade was made for an instrument.
         LAST # = 4,
 
     # A record flag bit field, indicating event end and data information.
     cpdef enum RecordFlag:
-        # Last message in the packet from the venue for a given `instrument_id`.
+        # Last message in the book event or packet from the venue for a given `instrument_id`.
         F_LAST # = (1 << 7),
         # Top-of-book message, not an individual order.
         F_TOB # = (1 << 6),
         # Message sourced from a replay, such as a snapshot server.
         F_SNAPSHOT # = (1 << 5),
         # Aggregated price level message, not an individual order.
         F_MBP # = (1 << 4),
@@ -374,20 +374,20 @@
     # Represents a discrete price level in an order book.
     #
     # The level maintains a collection of orders as well as tracking insertion order
     # to preserve FIFO queue dynamics.
     cdef struct Level:
         pass
 
-    # Provides an order book.
+    # Provides a performant, generic, multi-purpose order book.
     #
     # Can handle the following granularity data:
-    # - MBO (market by order) / L3
-    # - MBP (market by price) / L2 aggregated order per level
-    # - MBP (market by price) / L1 top-of-book only
+    # - MBO (market-by-order) / L3
+    # - MBP (market-by-price) / L2 aggregated order per level
+    # - MBP (market-by-price) / L1 top-of-book only
     cdef struct OrderBook:
         pass
 
     # Represents a grouped batch of `OrderBookDelta` updates for an `OrderBook`.
     #
     # This type cannot be `repr(C)` due to the `deltas` vec.
     cdef struct OrderBookDeltas_t:
@@ -447,15 +447,15 @@
         # The message sequence number assigned at the venue.
         uint64_t sequence;
         # The UNIX timestamp (nanoseconds) when the book event occurred.
         uint64_t ts_event;
         # The UNIX timestamp (nanoseconds) when the struct was initialized.
         uint64_t ts_init;
 
-    # Provides a C compatible Foreign Function Interface (FFI) for an underlying [`OrderBookDeltas`].
+    # C compatible Foreign Function Interface (FFI) for an underlying [`OrderBookDeltas`].
     #
     # This struct wraps `OrderBookDeltas` in a way that makes it compatible with C function
     # calls, enabling interaction with `OrderBookDeltas` in a C environment.
     #
     # It implements the `Deref` trait, allowing instances of `OrderBookDeltas_API` to be
     # dereferenced to `OrderBookDeltas`, providing access to `OrderBookDeltas`'s methods without
     # having to manually access the underlying `OrderBookDeltas` instance.
@@ -506,19 +506,14 @@
         # The UNIX timestamp (nanoseconds) when the quote event occurred.
         uint64_t ts_event;
         # The UNIX timestamp (nanoseconds) when the struct was initialized.
         uint64_t ts_init;
 
     # Represents a valid trade match ID (assigned by a trading venue).
     #
-    # Maximum length is 36 characters.
-    #
-    # The unique ID assigned to the trade entity once it is received or matched by
-    # the exchange or central counterparty.
-    #
     # Can correspond to the `TradeID <1003> field` of the FIX protocol.
     cdef struct TradeId_t:
         # The trade match ID value as a fixed-length C string byte array (includes null terminator).
         uint8_t value[37];
 
     # Represents a single trade tick in a market.
     cdef struct TradeTick_t:
@@ -594,35 +589,18 @@
         OrderBookDeltas_API deltas;
         OrderBookDepth10_t depth10;
         QuoteTick_t quote;
         TradeTick_t trade;
         Bar_t bar;
 
     # Represents a valid trader ID.
-    #
-    # Must be correctly formatted with two valid strings either side of a hyphen.
-    # It is expected a trader ID is the abbreviated name of the trader
-    # with an order ID tag number separated by a hyphen.
-    #
-    # Example: "TESTER-001".
-    # The reason for the numerical component of the ID is so that order and position IDs
-    # do not collide with those from another node instance.
     cdef struct TraderId_t:
         char* _0;
 
     # Represents a valid strategy ID.
-    #
-    # Must be correctly formatted with two valid strings either side of a hyphen.
-    # It is expected a strategy ID is the class name of the strategy,
-    # with an order ID tag number separated by a hyphen.
-    #
-    # Example: "EMACross-001".
-    #
-    # The reason for the numerical component of the ID is so that order and position IDs
-    # do not collide with those from another strategy within the node instance.
     cdef struct StrategyId_t:
         char* _0;
 
     # Represents a valid client order ID (assigned by the Nautilus system).
     cdef struct ClientOrderId_t:
         char* _0;
 
@@ -652,20 +630,14 @@
         ClientOrderId_t client_order_id;
         Price_t released_price;
         UUID4_t event_id;
         uint64_t ts_event;
         uint64_t ts_init;
 
     # Represents a valid account ID.
-    #
-    # Must be correctly formatted with two valid strings either side of a hyphen '-'.
-    # It is expected an account ID is the name of the issuer with an account number
-    # separated by a hyphen.
-    #
-    # Example: "IB-D02851908".
     cdef struct AccountId_t:
         char* _0;
 
     cdef struct OrderSubmitted_t:
         TraderId_t trader_id;
         StrategyId_t strategy_id;
         InstrumentId_t instrument_id;
@@ -719,38 +691,38 @@
     cdef struct OrderListId_t:
         char* _0;
 
     # Represents a valid position ID.
     cdef struct PositionId_t:
         char* _0;
 
-    # Provides a C compatible Foreign Function Interface (FFI) for an underlying
+    # C compatible Foreign Function Interface (FFI) for an underlying
     # [`SyntheticInstrument`].
     #
     # This struct wraps `SyntheticInstrument` in a way that makes it compatible with C function
     # calls, enabling interaction with `SyntheticInstrument` in a C environment.
     #
     # It implements the `Deref` trait, allowing instances of `SyntheticInstrument_API` to be
     # dereferenced to `SyntheticInstrument`, providing access to `SyntheticInstruments`'s methods without
     # having to manually access the underlying instance.
     cdef struct SyntheticInstrument_API:
         SyntheticInstrument *_0;
 
-    # Provides a C compatible Foreign Function Interface (FFI) for an underlying `OrderBook`.
+    # C compatible Foreign Function Interface (FFI) for an underlying `OrderBook`.
     #
     # This struct wraps `OrderBook` in a way that makes it compatible with C function
     # calls, enabling interaction with `OrderBook` in a C environment.
     #
     # It implements the `Deref` trait, allowing instances of `OrderBook_API` to be
     # dereferenced to `OrderBook`, providing access to `OrderBook`'s methods without
     # having to manually access the underlying `OrderBook` instance.
     cdef struct OrderBook_API:
         OrderBook *_0;
 
-    # Provides a C compatible Foreign Function Interface (FFI) for an underlying order book[`Level`].
+    # C compatible Foreign Function Interface (FFI) for an underlying order book[`Level`].
     #
     # This struct wraps `Level` in a way that makes it compatible with C function
     # calls, enabling interaction with `Level` in a C environment.
     #
     # It implements the `Deref` trait, allowing instances of `Level_API` to be
     # dereferenced to `Level`, providing access to `Level`'s methods without
     # having to manually acce wss the underlying `Level` instance.
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/rust/model.pyx` & `nautilus_trader-1.194.0/nautilus_trader/core/rust/model.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/stats.pxd` & `nautilus_trader-1.194.0/nautilus_trader/core/stats.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/stats.pyx` & `nautilus_trader-1.194.0/nautilus_trader/core/stats.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/string.pxd` & `nautilus_trader-1.194.0/nautilus_trader/core/string.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/uuid.pxd` & `nautilus_trader-1.194.0/nautilus_trader/core/uuid.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/core/uuid.pyx` & `nautilus_trader-1.194.0/nautilus_trader/core/uuid.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/data/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/data/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/data/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/data/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/data/aggregation.pxd` & `nautilus_trader-1.194.0/nautilus_trader/data/aggregation.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/data/aggregation.pyx` & `nautilus_trader-1.194.0/nautilus_trader/data/aggregation.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/data/client.pxd` & `nautilus_trader-1.194.0/nautilus_trader/data/client.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/data/client.pyx` & `nautilus_trader-1.194.0/nautilus_trader/data/client.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/data/config.py` & `nautilus_trader-1.194.0/nautilus_trader/data/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,17 +31,20 @@
         If False then will timestamp on bar open.
     time_bars_interval_type : str, default 'left-open'
         Determines the type of interval used for time aggregation.
         - 'left-open': start time is excluded and end time is included (default).
         - 'right-open': start time is included and end time is excluded.
     validate_data_sequence : bool, default False
         If data objects timestamp sequencing will be validated and handled.
+    buffer_deltas : bool, default False
+        If order book deltas should be buffered until the F_LAST flag is set for a delta.
     debug : bool, default False
         If debug mode is active (will provide extra debug logging).
 
     """
 
     time_bars_build_with_no_updates: bool = True
     time_bars_timestamp_on_close: bool = True
     time_bars_interval_type: str = "left-open"
     validate_data_sequence: bool = False
+    buffer_deltas: bool = False
     debug: bool = False
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/data/engine.pxd` & `nautilus_trader-1.194.0/nautilus_trader/data/engine.pxd`

 * *Files 0% similar despite different names*

```diff
@@ -53,18 +53,20 @@
     cdef readonly dict[Venue, DataClient] _routing_map
     cdef readonly dict _order_book_intervals
     cdef readonly dict[BarType, BarAggregator] _bar_aggregators
     cdef readonly dict[InstrumentId, list[SyntheticInstrument]] _synthetic_quote_feeds
     cdef readonly dict[InstrumentId, list[SyntheticInstrument]] _synthetic_trade_feeds
     cdef readonly list[InstrumentId] _subscribed_synthetic_quotes
     cdef readonly list[InstrumentId] _subscribed_synthetic_trades
+    cdef readonly dict[InstrumentId, list[OrderBookDelta]] _buffered_deltas_map
     cdef readonly bint _time_bars_build_with_no_updates
     cdef readonly bint _time_bars_timestamp_on_close
     cdef readonly str _time_bars_interval_type
     cdef readonly bint _validate_data_sequence
+    cdef readonly bint _buffer_deltas
 
     cdef readonly bint debug
     """If debug mode is active (will provide extra debug logging).\n\n:returns: `bool`"""
     cdef readonly int command_count
     """The total count of data commands received by the engine.\n\n:returns: `int`"""
     cdef readonly int request_count
     """The total count of data requests received by the engine.\n\n:returns: `int`"""
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/data/engine.pyx` & `nautilus_trader-1.194.0/nautilus_trader/data/engine.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 from nautilus_trader.model.identifiers cimport ClientId
 from nautilus_trader.model.identifiers cimport ComponentId
 from nautilus_trader.model.identifiers cimport InstrumentId
 from nautilus_trader.model.instruments.base cimport Instrument
 from nautilus_trader.model.instruments.synthetic cimport SyntheticInstrument
 from nautilus_trader.model.objects cimport Price
 from nautilus_trader.model.objects cimport Quantity
+from nautilus_trader.model.enums import RecordFlag
 
 
 cdef class DataEngine(Component):
     """
     Provides a high-performance data engine for managing many `DataClient`
     instances, for the asynchronous ingest of data.
 
@@ -133,21 +134,23 @@
         self._catalog: ParquetDataCatalog | None = None
         self._order_book_intervals: dict[(InstrumentId, int), list[Callable[[Bar], None]]] = {}
         self._bar_aggregators: dict[BarType, BarAggregator] = {}
         self._synthetic_quote_feeds: dict[InstrumentId, list[SyntheticInstrument]] = {}
         self._synthetic_trade_feeds: dict[InstrumentId, list[SyntheticInstrument]] = {}
         self._subscribed_synthetic_quotes: list[InstrumentId] = []
         self._subscribed_synthetic_trades: list[InstrumentId] = []
+        self._buffered_deltas_map: dict[InstrumentId, list[OrderBookDelta]] = {}
 
         # Settings
         self.debug = config.debug
         self._time_bars_build_with_no_updates = config.time_bars_build_with_no_updates
         self._time_bars_timestamp_on_close = config.time_bars_timestamp_on_close
         self._time_bars_interval_type = config.time_bars_interval_type
         self._validate_data_sequence = config.validate_data_sequence
+        self._buffer_deltas = config.buffer_deltas
 
         # Counters
         self.command_count = 0
         self.data_count = 0
         self.request_count = 0
         self.response_count = 0
 
@@ -527,14 +530,15 @@
 
         self._order_book_intervals.clear()
         self._bar_aggregators.clear()
         self._synthetic_quote_feeds.clear()
         self._synthetic_trade_feeds.clear()
         self._subscribed_synthetic_quotes.clear()
         self._subscribed_synthetic_trades.clear()
+        self._buffered_deltas_map.clear()
 
         self._clock.cancel_timers()
         self.command_count = 0
         self.data_count = 0
         self.request_count = 0
         self.response_count = 0
 
@@ -1051,27 +1055,29 @@
         MarketDataClient client,
         InstrumentId instrument_id,
     ):
         Condition.not_none(client, "client")
 
         if instrument_id is None:
             if not self._msgbus.has_subscribers(f"data.instrument.{client.id.value}.*"):
-                client.unsubscribe_instruments()
+                if client.subscribed_instruments():
+                    client.unsubscribe_instruments()
             return
         else:
             if instrument_id.is_synthetic():
                 self._log.error("Cannot unsubscribe from synthetic instrument `Instrument` data")
                 return
 
             if not self._msgbus.has_subscribers(
                 f"data.instrument"
                 f".{instrument_id.venue}"
                 f".{instrument_id.symbol}",
             ):
-                client.unsubscribe_instrument(instrument_id)
+                if instrument_id in client.subscribed_instruments():
+                    client.unsubscribe_instrument(instrument_id)
 
     cpdef void _handle_unsubscribe_order_book_deltas(
         self,
         MarketDataClient client,
         InstrumentId instrument_id,
         dict metadata,
     ):
@@ -1084,15 +1090,16 @@
             return
 
         if not self._msgbus.has_subscribers(
             f"data.book.deltas"
             f".{instrument_id.venue}"
             f".{instrument_id.symbol}",
         ):
-            client.unsubscribe_order_book_deltas(instrument_id)
+            if instrument_id in client.subscribed_order_book_deltas():
+                client.unsubscribe_order_book_deltas(instrument_id)
 
     cpdef void _handle_unsubscribe_order_book_snapshots(
         self,
         MarketDataClient client,
         InstrumentId instrument_id,
         dict metadata,
     ):
@@ -1105,45 +1112,48 @@
             return
 
         if not self._msgbus.has_subscribers(
             f"data.book.snapshots"
             f".{instrument_id.venue}"
             f".{instrument_id.symbol}",
         ):
-            client.unsubscribe_order_book_snapshots(instrument_id)
+            if instrument_id in client.subscribed_order_book_snapshots():
+                client.unsubscribe_order_book_snapshots(instrument_id)
 
     cpdef void _handle_unsubscribe_quote_ticks(
         self,
         MarketDataClient client,
         InstrumentId instrument_id,
     ):
         Condition.not_none(client, "client")
         Condition.not_none(instrument_id, "instrument_id")
 
         if not self._msgbus.has_subscribers(
             f"data.quotes"
             f".{instrument_id.venue}"
             f".{instrument_id.symbol}",
         ):
-            client.unsubscribe_quote_ticks(instrument_id)
+            if instrument_id in client.subscribed_quote_ticks():
+                client.unsubscribe_quote_ticks(instrument_id)
 
     cpdef void _handle_unsubscribe_trade_ticks(
         self,
         MarketDataClient client,
         InstrumentId instrument_id,
     ):
         Condition.not_none(client, "client")
         Condition.not_none(instrument_id, "instrument_id")
 
         if not self._msgbus.has_subscribers(
             f"data.trades"
             f".{instrument_id.venue}"
             f".{instrument_id.symbol}",
         ):
-            client.unsubscribe_trade_ticks(instrument_id)
+            if instrument_id in client.subscribed_trade_ticks():
+                client.unsubscribe_trade_ticks(instrument_id)
 
     cpdef void _handle_unsubscribe_bars(
         self,
         MarketDataClient client,
         BarType bar_type,
     ):
         Condition.not_none(client, "client")
@@ -1167,15 +1177,16 @@
         DataType data_type,
     ):
         Condition.not_none(client, "client")
         Condition.not_none(data_type, "data_type")
 
         try:
             if not self._msgbus.has_subscribers(f"data.{data_type}"):
-                client.unsubscribe(data_type)
+                if data_type in client.subscribed_custom_data():
+                    client.unsubscribe(data_type)
         except NotImplementedError:
             self._log.error(
                 f"Cannot unsubscribe: {client.id.value} "
                 f"has not implemented data type {data_type} subscriptions",
             )
             return
 
@@ -1370,32 +1381,87 @@
             topic=f"data.instrument"
                   f".{instrument.id.venue}"
                   f".{instrument.id.symbol}",
             msg=instrument,
         )
 
     cpdef void _handle_order_book_delta(self, OrderBookDelta delta):
-        cdef OrderBookDeltas deltas = OrderBookDeltas(
-            instrument_id=delta.instrument_id,
-            deltas=[delta]
-        )
-        self._msgbus.publish_c(
-            topic=f"data.book.deltas"
-                  f".{deltas.instrument_id.venue}"
-                  f".{deltas.instrument_id.symbol}",
-            msg=deltas,
-        )
+        cdef OrderBookDeltas deltas = None
+        cdef list[OrderBookDelta] buffer_deltas = None
+        cdef bint is_last_delta = False
+
+        if self._buffer_deltas:
+            buffer_deltas = self._buffered_deltas_map.get(delta.instrument_id)
+
+            if buffer_deltas is None:
+                buffer_deltas = []
+                self._buffered_deltas_map[delta.instrument_id] = buffer_deltas
+
+            buffer_deltas.append(delta)
+            is_last_delta = delta.flags == RecordFlag.F_LAST
+
+            if is_last_delta:
+                deltas = OrderBookDeltas(
+                    instrument_id=delta.instrument_id,
+                    deltas=buffer_deltas
+                )
+                self._msgbus.publish_c(
+                    topic=f"data.book.deltas"
+                        f".{deltas.instrument_id.venue}"
+                        f".{deltas.instrument_id.symbol}",
+                    msg=deltas,
+                )
+                buffer_deltas.clear()
+        else:
+            deltas = OrderBookDeltas(
+                instrument_id=delta.instrument_id,
+                deltas=[delta]
+            )
+            self._msgbus.publish_c(
+                 topic=f"data.book.deltas"
+                    f".{deltas.instrument_id.venue}"
+                    f".{deltas.instrument_id.symbol}",
+                msg=deltas,
+            )
 
     cpdef void _handle_order_book_deltas(self, OrderBookDeltas deltas):
-        self._msgbus.publish_c(
-            topic=f"data.book.deltas"
-                  f".{deltas.instrument_id.venue}"
-                  f".{deltas.instrument_id.symbol}",
-            msg=deltas,
-        )
+        cdef OrderBookDeltas deltas_to_publish = None
+        cdef list[OrderBookDelta] buffer_deltas = None
+        cdef bint is_last_delta = False
+
+        if self._buffer_deltas:
+            buffer_deltas = self._buffered_deltas_map.get(deltas.instrument_id)
+
+            if buffer_deltas is None:
+                buffer_deltas = []
+                self._buffered_deltas_map[deltas.instrument_id] = buffer_deltas
+
+            for delta in deltas.deltas:
+                buffer_deltas.append(delta)
+                is_last_delta = delta.flags == RecordFlag.F_LAST
+
+                if is_last_delta:
+                    deltas_to_publish = OrderBookDeltas(
+                        instrument_id=deltas.instrument_id,
+                        deltas=buffer_deltas,
+                    )
+                    self._msgbus.publish_c(
+                        topic=f"data.book.deltas"
+                            f".{deltas.instrument_id.venue}"
+                            f".{deltas.instrument_id.symbol}",
+                        msg=deltas_to_publish,
+                    )
+                    buffer_deltas.clear()
+        else:
+            self._msgbus.publish_c(
+                topic=f"data.book.deltas"
+                    f".{deltas.instrument_id.venue}"
+                    f".{deltas.instrument_id.symbol}",
+                msg=deltas,
+            )
 
     cpdef void _handle_order_book_depth(self, OrderBookDepth10 depth):
         self._msgbus.publish_c(
             topic=f"data.book.depth"
                   f".{depth.instrument_id.venue}"
                   f".{depth.instrument_id.symbol}",
             msg=depth,
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/data/messages.pxd` & `nautilus_trader-1.194.0/nautilus_trader/data/messages.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/data/messages.pyx` & `nautilus_trader-1.194.0/nautilus_trader/data/messages.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/algorithms/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/algorithms/blank.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/algorithms/blank.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/algorithms/twap.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/algorithms/twap.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/blank.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/blank.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/ema_cross.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_bracket.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/ema_cross_bracket.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_bracket_algo.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/ema_cross_bracket_algo.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_cython.pyx` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/ema_cross_cython.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_long_only.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/ema_cross_long_only.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_stop_entry.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/ema_cross_stop_entry.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_trailing_stop.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/ema_cross_trailing_stop.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/ema_cross_twap.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/ema_cross_twap.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/market_maker.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/market_maker.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/orderbook_imbalance.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/orderbook_imbalance.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/orderbook_imbalance_rust.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/orderbook_imbalance_rust.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/signal_strategy.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/signal_strategy.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/subscribe.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/subscribe.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/talib_strategy.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/talib_strategy.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/examples/strategies/volatility_market_maker.py` & `nautilus_trader-1.194.0/nautilus_trader/examples/strategies/volatility_market_maker.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/execution/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/algorithm.pxd` & `nautilus_trader-1.194.0/nautilus_trader/execution/algorithm.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/algorithm.pyx` & `nautilus_trader-1.194.0/nautilus_trader/execution/algorithm.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/client.pxd` & `nautilus_trader-1.194.0/nautilus_trader/execution/client.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/client.pyx` & `nautilus_trader-1.194.0/nautilus_trader/execution/client.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/config.py` & `nautilus_trader-1.194.0/nautilus_trader/execution/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/emulator.pxd` & `nautilus_trader-1.194.0/nautilus_trader/execution/emulator.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/emulator.pyx` & `nautilus_trader-1.194.0/nautilus_trader/execution/emulator.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/engine.pxd` & `nautilus_trader-1.194.0/nautilus_trader/execution/engine.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/engine.pyx` & `nautilus_trader-1.194.0/nautilus_trader/execution/engine.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/manager.pxd` & `nautilus_trader-1.194.0/nautilus_trader/execution/manager.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/manager.pyx` & `nautilus_trader-1.194.0/nautilus_trader/execution/manager.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/matching_core.pxd` & `nautilus_trader-1.194.0/nautilus_trader/execution/matching_core.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/matching_core.pyx` & `nautilus_trader-1.194.0/nautilus_trader/execution/matching_core.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/messages.pxd` & `nautilus_trader-1.194.0/nautilus_trader/execution/messages.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/messages.pyx` & `nautilus_trader-1.194.0/nautilus_trader/execution/messages.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/reports.py` & `nautilus_trader-1.194.0/nautilus_trader/execution/reports.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/trailing.pxd` & `nautilus_trader-1.194.0/nautilus_trader/execution/trailing.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/execution/trailing.pyx` & `nautilus_trader-1.194.0/nautilus_trader/execution/trailing.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/amat.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/amat.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/amat.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/amat.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/aroon.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/aroon.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/aroon.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/aroon.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/atr.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/atr.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/atr.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/atr.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/ama.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/ama.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/ama.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/ama.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/dema.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/dema.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/dema.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/dema.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/ema.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/ema.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/ema.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/ema.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/hma.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/hma.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/hma.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/hma.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/ma_factory.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/ma_factory.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/moving_average.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/moving_average.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/moving_average.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/moving_average.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/rma.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/rma.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/rma.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/rma.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/sma.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/sma.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/sma.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/sma.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/vidya.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/vidya.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/vidya.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/vidya.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/wma.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/wma.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/average/wma.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/average/wma.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/base/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/base/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/base/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/indicators/base/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/base/indicator.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/base/indicator.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/base/indicator.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/base/indicator.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/bias.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/keltner_position.pxd`

 * *Files 11% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-from nautilus_trader.indicators.average.moving_average cimport MovingAverage
 from nautilus_trader.indicators.base.indicator cimport Indicator
+from nautilus_trader.indicators.keltner_channel cimport KeltnerChannel
 
 
-cdef class Bias(Indicator):
-    cdef MovingAverage _ma
+cdef class KeltnerPosition(Indicator):
+    cdef KeltnerChannel _kc
 
     cdef readonly int period
     """The window period.\n\n:returns: `int`"""
+    cdef readonly double k_multiplier
+    """The K multiplier.\n\n:returns: `double`"""
     cdef readonly double value
     """The current value.\n\n:returns: `double`"""
 
-    cpdef void update_raw(self, double close)
-    cdef void _check_initialized(self)
+    cpdef void update_raw(self, double high, double low, double close)
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/bias.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/bias.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/bollinger_bands.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/bollinger_bands.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/bollinger_bands.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/bollinger_bands.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/cci.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/cci.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/cci.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/cci.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/cmo.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/cmo.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/cmo.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/cmo.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/dm.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/dm.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/dm.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/dm.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/donchian_channel.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/donchian_channel.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/donchian_channel.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/donchian_channel.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/efficiency_ratio.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/efficiency_ratio.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/efficiency_ratio.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/efficiency_ratio.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_candlesticks.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_candlesticks.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_candlesticks.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_candlesticks.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enum.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enum.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/candle_body.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/candle_direction.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_size.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-from nautilus_trader.indicators.fuzzy_enums.candle_size cimport CandleSize
+from nautilus_trader.indicators.fuzzy_enums.candle_wick cimport CandleWickSize
 
 
-__all__ = ["CandleSize"]
+__all__ = ["CandleWickSize"]
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/ta_lib/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,7 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
-
-
-cpdef enum CandleWickSize:
-    NONE = 0  # No candle wick
-    SMALL = 1
-    MEDIUM = 2
-    LARGE = 3
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/fuzzy_enums/candle_wick.pyx` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,12 +8,11 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
-
-from nautilus_trader.indicators.fuzzy_enums.candle_wick cimport CandleWickSize
-
-
-__all__ = ["CandleWickSize"]
+"""
+The test kit contains test doubles and helpers to support the NautilusTrader test suite,
+as well as supporting testing for downstream projects and packages.
+"""
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/keltner_channel.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/keltner_channel.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/keltner_channel.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/keltner_channel.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/keltner_position.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/roc.pxd`

 * *Files 17% similar despite different names*

```diff
@@ -10,21 +10,19 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
 from nautilus_trader.indicators.base.indicator cimport Indicator
-from nautilus_trader.indicators.keltner_channel cimport KeltnerChannel
 
 
-cdef class KeltnerPosition(Indicator):
-    cdef KeltnerChannel _kc
+cdef class RateOfChange(Indicator):
+    cdef bint _use_log
+    cdef object _prices
 
     cdef readonly int period
     """The window period.\n\n:returns: `int`"""
-    cdef readonly double k_multiplier
-    """The K multiplier.\n\n:returns: `double`"""
     cdef readonly double value
     """The current value.\n\n:returns: `double`"""
 
-    cpdef void update_raw(self, double high, double low, double close)
+    cpdef void update_raw(self, double price)
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/keltner_position.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/keltner_position.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/kvo.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/kvo.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/kvo.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/kvo.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/linear_regression.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/linear_regression.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/linear_regression.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/linear_regression.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/macd.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/macd.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/macd.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/macd.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/obv.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/obv.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/obv.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/obv.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/pressure.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/pressure.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/pressure.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/pressure.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/psl.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/psl.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/psl.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/psl.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/roc.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/volatility_ratio.pxd`

 * *Files 11% similar despite different names*

```diff
@@ -9,20 +9,24 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
+from nautilus_trader.indicators.atr cimport AverageTrueRange
 from nautilus_trader.indicators.base.indicator cimport Indicator
 
 
-cdef class RateOfChange(Indicator):
-    cdef bint _use_log
-    cdef object _prices
+cdef class VolatilityRatio(Indicator):
+    cdef AverageTrueRange _atr_fast
+    cdef AverageTrueRange _atr_slow
 
-    cdef readonly int period
-    """The window period.\n\n:returns: `int`"""
+    cdef readonly int fast_period
+    """The period of the fast ATR.\n\n:returns: `int`"""
+    cdef readonly int slow_period
+    """The period of the slow ATR.\n\n:returns: `int`"""
     cdef readonly double value
     """The current value.\n\n:returns: `double`"""
 
-    cpdef void update_raw(self, double price)
+    cpdef void update_raw(self, double high, double low, double close)
+    cdef void _check_initialized(self)
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/roc.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/roc.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/rsi.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/rsi.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/rsi.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/rsi.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/rvi.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/rvi.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/rvi.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/rvi.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/spread_analyzer.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/spread_analyzer.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/spread_analyzer.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/spread_analyzer.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/stochastics.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/stochastics.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/stochastics.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/stochastics.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/swings.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/swings.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/swings.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/swings.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/ta_lib/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/model/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/ta_lib/common.py` & `nautilus_trader-1.194.0/nautilus_trader/indicators/ta_lib/common.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/ta_lib/manager.py` & `nautilus_trader-1.194.0/nautilus_trader/indicators/ta_lib/manager.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/vhf.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/vhf.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/vhf.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/vhf.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/volatility_ratio.pxd` & `nautilus_trader-1.194.0/nautilus_trader/indicators/vwap.pxd`

 * *Files 17% similar despite different names*

```diff
@@ -9,24 +9,21 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-from nautilus_trader.indicators.atr cimport AverageTrueRange
+from cpython.datetime cimport datetime
+
 from nautilus_trader.indicators.base.indicator cimport Indicator
 
 
-cdef class VolatilityRatio(Indicator):
-    cdef AverageTrueRange _atr_fast
-    cdef AverageTrueRange _atr_slow
-
-    cdef readonly int fast_period
-    """The period of the fast ATR.\n\n:returns: `int`"""
-    cdef readonly int slow_period
-    """The period of the slow ATR.\n\n:returns: `int`"""
+cdef class VolumeWeightedAveragePrice(Indicator):
+    cdef int _day
+    cdef double _price_volume
+    cdef double _volume_total
+
     cdef readonly double value
     """The current value.\n\n:returns: `double`"""
 
-    cpdef void update_raw(self, double high, double low, double close)
-    cdef void _check_initialized(self)
+    cpdef void update_raw(self, double price, double volume, datetime timestamp)
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/volatility_ratio.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/volatility_ratio.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/vwap.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/implementations/tiered.pxd`

 * *Files 18% similar despite different names*

```diff
@@ -9,21 +9,26 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-from cpython.datetime cimport datetime
+cimport numpy as np
 
-from nautilus_trader.indicators.base.indicator cimport Indicator
+from nautilus_trader.model.objects cimport Price
+from nautilus_trader.model.tick_scheme.base cimport TickScheme
 
 
-cdef class VolumeWeightedAveragePrice(Indicator):
-    cdef int _day
-    cdef double _price_volume
-    cdef double _volume_total
+cdef class TieredTickScheme(TickScheme):
+    cdef list tiers
+    cdef int max_ticks_per_tier
+    cdef int price_precision
+    cdef int tick_count
 
-    cdef readonly double value
-    """The current value.\n\n:returns: `double`"""
+    cdef readonly np.ndarray ticks
 
-    cpdef void update_raw(self, double price, double volume, datetime timestamp)
+    cpdef _build_ticks(self)
+
+    cpdef int find_tick_index(self, double value)
+    cpdef Price next_ask_price(self, double value, int n=*)
+    cpdef Price next_bid_price(self, double value, int n=*)
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/indicators/vwap.pyx` & `nautilus_trader-1.194.0/nautilus_trader/indicators/vwap.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/live/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/live/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/live/__main__.py` & `nautilus_trader-1.194.0/nautilus_trader/live/__main__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/live/config.py` & `nautilus_trader-1.194.0/nautilus_trader/live/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/live/data_client.py` & `nautilus_trader-1.194.0/nautilus_trader/live/data_client.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/live/data_engine.py` & `nautilus_trader-1.194.0/nautilus_trader/live/data_engine.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/live/execution_client.py` & `nautilus_trader-1.194.0/nautilus_trader/live/execution_client.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/live/execution_engine.py` & `nautilus_trader-1.194.0/nautilus_trader/live/execution_engine.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/live/factories.py` & `nautilus_trader-1.194.0/nautilus_trader/live/factories.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/live/node.py` & `nautilus_trader-1.194.0/nautilus_trader/live/node.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/live/node_builder.py` & `nautilus_trader-1.194.0/nautilus_trader/live/node_builder.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/live/risk_engine.py` & `nautilus_trader-1.194.0/nautilus_trader/live/risk_engine.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/events/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/model/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/book.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/book.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/book.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/book.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/currencies.py` & `nautilus_trader-1.194.0/nautilus_trader/model/currencies.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/data.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/data.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/data.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/data.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/enums.py` & `nautilus_trader-1.194.0/nautilus_trader/model/enums.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/events/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/events/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/model/events/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/events/account.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/events/account.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/events/account.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/events/account.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/events/order.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/events/order.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/events/order.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/events/order.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/events/position.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/events/position.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/events/position.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/events/position.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/functions.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/functions.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/functions.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/functions.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/identifiers.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/identifiers.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/identifiers.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/identifiers.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/base.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/base.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/base.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -446,18 +446,22 @@
         Returns
         -------
         Price
 
         Raises
         ------
         ValueError
-            If tick scheme is not registered.
+            If a tick scheme is not initialized.
 
         """
-        Condition.not_none(self._tick_scheme, "self._tick_scheme")
+        if self._tick_scheme is None:
+            raise ValueError(
+                f"No tick scheme for instrument {self.id.to_str()}. "
+                "You can specify a tick scheme by passing a `tick_scheme_name` at initialization."
+            )
 
         return self._tick_scheme.next_bid_price(value=value, n=num_ticks)
 
     cpdef Price next_ask_price(self, double value, int num_ticks=0):
         """
         Return the price `n` ask ticks away from value.
 
@@ -473,18 +477,22 @@
         Returns
         -------
         Price
 
         Raises
         ------
         ValueError
-            If tick scheme is not registered.
+            If a tick scheme is not initialized.
 
         """
-        Condition.not_none(self._tick_scheme, "self._tick_scheme")
+        if self._tick_scheme is None:
+            raise ValueError(
+                f"No tick scheme for instrument {self.id.to_str()}. "
+                "You can specify a tick scheme by passing a `tick_scheme_name` at initialization."
+            )
 
         return self._tick_scheme.next_ask_price(value=value, n=num_ticks)
 
     cpdef Quantity make_qty(self, value):
         """
         Return a new quantity from the given value using the instruments size
         precision.
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/betting.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/betting.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/betting.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/betting.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/cfd.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/cfd.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/cfd.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/cfd.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/commodity.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/commodity.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/commodity.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/commodity.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/crypto_future.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/crypto_future.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/crypto_future.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/crypto_future.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/crypto_perpetual.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/crypto_perpetual.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/crypto_perpetual.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/crypto_perpetual.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/currency_pair.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/currency_pair.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/currency_pair.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/currency_pair.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/equity.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/equity.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/equity.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/equity.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/futures_contract.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/futures_contract.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/futures_contract.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/futures_contract.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/futures_spread.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/futures_spread.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/futures_spread.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/futures_spread.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/options_contract.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/options_contract.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/options_contract.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/options_contract.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/options_spread.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/options_spread.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/options_spread.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/options_spread.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/synthetic.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/synthetic.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/instruments/synthetic.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/instruments/synthetic.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/objects.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/objects.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/objects.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/objects.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/base.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/base.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/limit.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/limit.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/limit.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/limit.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/limit_if_touched.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/limit_if_touched.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/limit_if_touched.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/limit_if_touched.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/list.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/list.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/list.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/list.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/market.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/market.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/market.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/market.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/market_if_touched.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/market_if_touched.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/market_if_touched.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/market_if_touched.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/market_to_limit.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/market_to_limit.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/market_to_limit.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/market_to_limit.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/stop_limit.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/stop_limit.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/stop_limit.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/stop_limit.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/stop_market.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/stop_market.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/stop_market.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/stop_market.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/trailing_stop_limit.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/trailing_stop_limit.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/trailing_stop_limit.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/trailing_stop_limit.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/trailing_stop_market.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/trailing_stop_market.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/trailing_stop_market.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/trailing_stop_market.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/unpacker.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/unpacker.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/orders/unpacker.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/orders/unpacker.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/position.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/position.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/position.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/position.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/portfolio/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/base.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/base.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/fixed.pxd` & `nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/implementations/fixed.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/fixed.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/implementations/fixed.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/tiered.pxd` & `nautilus_trader-1.194.0/nautilus_trader/persistence/catalog/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-cimport numpy as np
+from __future__ import annotations
 
-from nautilus_trader.model.objects cimport Price
-from nautilus_trader.model.tick_scheme.base cimport TickScheme
+from dataclasses import dataclass
 
+from nautilus_trader.core.data import Data
+from nautilus_trader.model.identifiers import ClientId
+from nautilus_trader.model.instruments import Instrument
 
-cdef class TieredTickScheme(TickScheme):
-    cdef list tiers
-    cdef int max_ticks_per_tier
-    cdef int price_precision
-    cdef int tick_count
 
-    cdef readonly np.ndarray ticks
+@dataclass(frozen=True)
+class CatalogDataResult:
+    """
+    Represents a catalog data query result.
+    """
 
-    cpdef _build_ticks(self)
-
-    cpdef int find_tick_index(self, double value)
-    cpdef Price next_ask_price(self, double value, int n=*)
-    cpdef Price next_bid_price(self, double value, int n=*)
+    data_cls: type
+    data: list[Data]
+    instrument: Instrument | None = None
+    client_id: ClientId | None = None
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/tick_scheme/implementations/tiered.pyx` & `nautilus_trader-1.194.0/nautilus_trader/model/tick_scheme/implementations/tiered.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/model/venues.py` & `nautilus_trader-1.194.0/nautilus_trader/model/venues.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/persistence/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/persistence/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/base.py` & `nautilus_trader-1.194.0/nautilus_trader/persistence/catalog/base.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/parquet.py` & `nautilus_trader-1.194.0/nautilus_trader/persistence/catalog/parquet.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/singleton.py` & `nautilus_trader-1.194.0/nautilus_trader/persistence/catalog/singleton.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/persistence/catalog/types.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/mocks/controller.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
 
-from __future__ import annotations
-
-from dataclasses import dataclass
-
-from nautilus_trader.core.data import Data
-from nautilus_trader.model.identifiers import ClientId
-from nautilus_trader.model.instruments import Instrument
-
-
-@dataclass(frozen=True)
-class CatalogDataResult:
-    """
-    Represents a catalog data query result.
-    """
-
-    data_cls: type
-    data: list[Data]
-    instrument: Instrument | None = None
-    client_id: ClientId | None = None
+from nautilus_trader.config import ActorConfig
+from nautilus_trader.examples.strategies.signal_strategy import SignalStrategy
+from nautilus_trader.examples.strategies.signal_strategy import SignalStrategyConfig
+from nautilus_trader.trading.controller import Controller
+
+
+class ControllerConfig(ActorConfig, frozen=True):
+    pass
+
+
+class MyController(Controller):
+    def start(self):
+        """
+        Dynamically add a new strategy after startup.
+        """
+        instruments = self.cache.instruments()
+        strategy_config = SignalStrategyConfig(instrument_id=instruments[0].id)
+        strategy = SignalStrategy(strategy_config)
+        self.create_strategy(strategy)
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/persistence/config.py` & `nautilus_trader-1.194.0/nautilus_trader/persistence/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         The `fsspec` storage options.
     flush_interval_ms : int, optional
         The flush interval (milliseconds) for writing chunks.
     replace_existing: bool, default False
         If any existing feather files should be replaced.
     include_types : list[type], optional
         A list of Arrow serializable types to write.
-        If this is specified then *only* the included types will be written.
+        If this is specified then **only** the included types will be written.
 
     """
 
     catalog_path: str
     fs_protocol: str | None = None
     fs_storage_options: dict | None = None
     flush_interval_ms: int | None = None
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/persistence/funcs.py` & `nautilus_trader-1.194.0/nautilus_trader/persistence/funcs.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/persistence/loaders.py` & `nautilus_trader-1.194.0/nautilus_trader/persistence/loaders.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/persistence/wranglers.pxd` & `nautilus_trader-1.194.0/nautilus_trader/persistence/wranglers.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/persistence/wranglers.pyx` & `nautilus_trader-1.194.0/nautilus_trader/persistence/wranglers.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/persistence/wranglers_v2.py` & `nautilus_trader-1.194.0/nautilus_trader/persistence/wranglers_v2.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/persistence/writer.py` & `nautilus_trader-1.194.0/nautilus_trader/persistence/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         The `fsspec` file system protocol.
     flush_interval_ms : int, optional
         The flush interval (milliseconds) for writing chunks.
     replace : bool, default False
         If existing files at the given `path` should be replaced.
     include_types : list[type], optional
         A list of Arrow serializable types to write.
-        If this is specified then *only* the included types will be written.
+        If this is specified then **only** the included types will be written.
 
     """
 
     def __init__(
         self,
         path: str,
         fs_protocol: str | None = "file",
@@ -85,18 +85,17 @@
 
         self._schemas = list_schemas()
         self.logger = Logger(type(self).__name__)
         self._files: dict[object, TextIOWrapper | BinaryIO | AbstractBufferedFile] = {}
         self._writers: dict[str, RecordBatchStreamWriter] = {}
         self._instrument_writers: dict[tuple[str, str], RecordBatchStreamWriter] = {}
         self._per_instrument_writers = {
-            "trade_tick",
-            "quote_tick",
             "order_book_delta",
-            "ticker",
+            "quote_tick",
+            "trade_tick",
         }
         self._instruments: dict[InstrumentId, Instrument] = {}
         self._create_writers()
 
         self.flush_interval_ms = datetime.timedelta(milliseconds=flush_interval_ms or 1000)
         self._last_flush = datetime.datetime(1970, 1, 1)  # Default value to begin
         self.missing_writers: set[type] = set()
@@ -129,14 +128,16 @@
         full_path = f"{self.path}/{table_name}.feather"
 
         self.fs.makedirs(self.fs._parent(full_path), exist_ok=True)
         f = self.fs.open(full_path, "wb")
         self._files[table_name] = f
         self._writers[table_name] = pa.ipc.new_stream(f, schema)
 
+        self.logger.info(f"Created writer for table '{table_name}'")
+
     def _create_writers(self) -> None:
         for cls in self._schemas:
             self._create_writer(cls=cls)
 
     def _create_instrument_writer(self, cls: type, obj: Any) -> None:
         # Check if an include types filter has been specified
         if self.include_types is not None and cls not in self.include_types:
@@ -152,14 +153,16 @@
         self.fs.makedirs(folder, exist_ok=True)
 
         full_path = f"{folder}/{urisafe_instrument_id(obj.instrument_id.value)}.feather"
         f = self.fs.open(full_path, "wb")
         self._files[key] = f
         self._instrument_writers[key] = pa.ipc.new_stream(f, schema)
 
+        self.logger.info(f"Created writer for table '{table_name}'")
+
     def _extract_obj_metadata(
         self,
         obj: TradeTick | QuoteTick | Bar | OrderBookDelta,
     ) -> dict[bytes, bytes]:
         instrument = self._instruments[obj.instrument_id]
         metadata = {b"instrument_id": obj.instrument_id.value.encode()}
         if isinstance(obj, OrderBookDelta):
@@ -224,35 +227,39 @@
 
         table = class_to_filename(cls)
         if isinstance(obj, Bar):
             bar: Bar = obj
             table += f"_{str(bar.bar_type).lower()}"
 
         if table not in self._writers:
+            self.logger.debug(f"Writer not setup for table '{table}'")
             if table.startswith("custom_signal"):
                 self._create_writer(cls=cls)
-            elif table.startswith("bar"):
+            elif table.startswith(("bar", "binance_bar")):
                 self._create_writer(cls=cls, table_name=table)
             elif table in self._per_instrument_writers:
                 key = (table, obj.instrument_id.value)  # type: ignore
                 if key not in self._instrument_writers:
                     self._create_instrument_writer(cls=cls, obj=obj)
             elif cls not in self.missing_writers:
                 self.logger.warning(f"Can't find writer for cls: {cls}")
                 self.missing_writers.add(cls)
                 return
             else:
                 return
+
         if table in self._per_instrument_writers:
             writer: RecordBatchStreamWriter = self._instrument_writers[(table, obj.instrument_id.value)]  # type: ignore
         else:
             writer: RecordBatchStreamWriter = self._writers[table]  # type: ignore
+
         serialized = ArrowSerializer.serialize_batch([obj], data_cls=cls)
         if not serialized:
             return
+
         try:
             writer.write_table(serialized)
             self.check_flush()
         except Exception as e:
             self.logger.error(f"Failed to serialize {cls=}")
             self.logger.error(f"ERROR = `{e}`")
             self.logger.debug(f"data = {obj}")
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/portfolio/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/risk/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/portfolio/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/serialization/serializer.pxd`

 * *Files 23% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # -------------------------------------------------------------------------------------------------
-"""
-The `portfolio` subpackage provides portfolio management functionality.
-"""
 
-from nautilus_trader.portfolio.base import PortfolioFacade
-from nautilus_trader.portfolio.portfolio import Portfolio
+from nautilus_trader.serialization.base cimport Serializer
 
 
-__all__ = [
-    "Portfolio",
-    "PortfolioFacade",
-]
+cdef class MsgSpecSerializer(Serializer):
+    cdef object _encode
+    cdef object _decode
+
+    cdef readonly bint timestamps_as_str
+    """If the serializer converts timestamp `int64_t` to integer strings.\n\n:returns: `bool`"""
+    cdef readonly bint timestamps_as_iso8601
+    """If the serializer converts timestamp `int64_t` to ISO 8601 strings.\n\n:returns: `bool`"""
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/portfolio/base.pxd` & `nautilus_trader-1.194.0/nautilus_trader/portfolio/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/portfolio/base.pyx` & `nautilus_trader-1.194.0/nautilus_trader/portfolio/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/portfolio/portfolio.pxd` & `nautilus_trader-1.194.0/nautilus_trader/portfolio/portfolio.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/portfolio/portfolio.pyx` & `nautilus_trader-1.194.0/nautilus_trader/portfolio/portfolio.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/risk/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/serialization/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/risk/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/risk/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/risk/config.py` & `nautilus_trader-1.194.0/nautilus_trader/risk/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/risk/engine.pxd` & `nautilus_trader-1.194.0/nautilus_trader/risk/engine.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/risk/engine.pyx` & `nautilus_trader-1.194.0/nautilus_trader/risk/engine.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/risk/sizing.pxd` & `nautilus_trader-1.194.0/nautilus_trader/risk/sizing.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/risk/sizing.pyx` & `nautilus_trader-1.194.0/nautilus_trader/risk/sizing.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/serialization/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/serialization/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/system/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/account_state.py` & `nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/implementations/account_state.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/component_events.py` & `nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/implementations/component_events.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/instruments.py` & `nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/implementations/instruments.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/order_events.py` & `nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/implementations/order_events.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/implementations/position_events.py` & `nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/implementations/position_events.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/schema.py` & `nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/schema.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/serialization/arrow/serializer.py` & `nautilus_trader-1.194.0/nautilus_trader/serialization/arrow/serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,18 @@
     @staticmethod
     def _unpack_container_objects(data_cls: type, data: list[Any]) -> list[Data]:
         if data_cls == OrderBookDeltas:
             return [delta for deltas in data for delta in deltas.deltas]
         return data
 
     @staticmethod
-    def rust_defined_to_record_batch(data: list[Data], data_cls: type) -> pa.Table | pa.RecordBatch:
+    def rust_defined_to_record_batch(  # noqa: C901 (too complex)
+        data: list[Data],
+        data_cls: type,
+    ) -> pa.Table | pa.RecordBatch:
         data = sorted(data, key=lambda x: x.ts_init)
         data = ArrowSerializer._unpack_container_objects(data_cls, data)
 
         match data_cls:
             case nautilus_pyo3.OrderBookDelta:
                 batch_bytes = DataTransformer.pyo3_order_book_deltas_to_record_batch_bytes(data)
             case nautilus_pyo3.OrderBookDepth10:
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/serialization/base.pxd` & `nautilus_trader-1.194.0/nautilus_trader/serialization/base.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/serialization/base.pyx` & `nautilus_trader-1.194.0/nautilus_trader/serialization/base.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/serialization/serializer.pyx` & `nautilus_trader-1.194.0/nautilus_trader/serialization/serializer.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/system/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/mocks/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/system/config.py` & `nautilus_trader-1.194.0/nautilus_trader/system/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/system/kernel.py` & `nautilus_trader-1.194.0/nautilus_trader/system/kernel.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/__init__.py` & `nautilus_trader-1.194.0/nautilus_core/core/src/ffi/mod.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-# -------------------------------------------------------------------------------------------------
-#  Copyright (C) 2015-2024 Nautech Systems Pty Ltd. All rights reserved.
-#  https://nautechsystems.io
-#
-#  Licensed under the GNU Lesser General Public License Version 3.0 (the "License");
-#  You may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at https://www.gnu.org/licenses/lgpl-3.0.en.html
-#
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
-# -------------------------------------------------------------------------------------------------
-"""
-The test kit contains test doubles and helpers to support the NautilusTrader test suite,
-as well as supporting testing for downstream projects and packages.
-"""
+// -------------------------------------------------------------------------------------------------
+//  Copyright (C) 2015-2024 Nautech Systems Pty Ltd. All rights reserved.
+//  https://nautechsystems.io
+//
+//  Licensed under the GNU Lesser General Public License Version 3.0 (the "License");
+//  You may not use this file except in compliance with the License.
+//  You may obtain a copy of the License at https://www.gnu.org/licenses/lgpl-3.0.en.html
+//
+//  Unless required by applicable law or agreed to in writing, software
+//  distributed under the License is distributed on an "AS IS" BASIS,
+//  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+//  See the License for the specific language governing permissions and
+//  limitations under the License.
+// -------------------------------------------------------------------------------------------------
+
+//! C foreign function interface (FFI) from `cbindgen`.
+
+pub mod cvec;
+pub mod datetime;
+pub mod parsing;
+pub mod string;
+pub mod uuid;
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/functions.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/functions.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/rust/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/actors.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/mocks/actors.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/cache_database.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/mocks/cache_database.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/data.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/mocks/data.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/engines.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/mocks/engines.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/exec_clients.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/mocks/exec_clients.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/mocks/strategies.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/mocks/strategies.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/providers.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -646,15 +646,15 @@
 
     days_to_add = (4 - first_day_weekday + 7) % 7 + 14
     third_friday = first_day + dt.timedelta(days=days_to_add)
 
     return third_friday
 
 
-def get_contract_month_code(expiry_month: int) -> str:
+def get_contract_month_code(expiry_month: int) -> str:  # noqa: C901 (too complex)
     match expiry_month:
         case 1:
             return "F"
         case 2:
             return "G"
         case 3:
             return "H"
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/accounting_pyo3.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/rust/accounting_pyo3.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/data_pyo3.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/rust/data_pyo3.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/events_pyo3.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/rust/events_pyo3.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/identifiers_pyo3.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/rust/identifiers_pyo3.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/instruments_pyo3.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/rust/instruments_pyo3.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/orders_pyo3.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/rust/orders_pyo3.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/rust/types_pyo3.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/rust/types_pyo3.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/trading/__init__.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/commands.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/commands.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/component.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/component.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/config.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/data.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,18 +423,19 @@
             ts_init=0,
         )
 
     @staticmethod
     def order_book_deltas(
         instrument_id: InstrumentId | None = None,
         deltas: list[OrderBookDelta] | None = None,
+        flags: int = 0,
     ) -> OrderBookDeltas:
         return OrderBookDeltas(
             instrument_id=instrument_id or TestIdStubs.audusd_id(),
-            deltas=deltas or [TestDataStubs.order_book_delta()],
+            deltas=deltas or [TestDataStubs.order_book_delta(flags=flags)],
         )
 
     @staticmethod
     def make_book(
         instrument: Instrument,
         book_type: BookType,
         bids: list[tuple] | None = None,
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/events.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/events.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/execution.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/execution.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/identifiers.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/identifiers.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/test_kit/stubs/persistence.py` & `nautilus_trader-1.194.0/nautilus_trader/test_kit/stubs/persistence.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/trading/__init__.pxd` & `nautilus_trader-1.194.0/nautilus_core/model/src/events/mod.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,20 @@
-# -------------------------------------------------------------------------------------------------
-#  Copyright (C) 2015-2024 Nautech Systems Pty Ltd. All rights reserved.
-#  https://nautechsystems.io
-#
-#  Licensed under the GNU Lesser General Public License Version 3.0 (the "License");
-#  You may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at https://www.gnu.org/licenses/lgpl-3.0.en.html
-#
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
-# -------------------------------------------------------------------------------------------------
+// -------------------------------------------------------------------------------------------------
+//  Copyright (C) 2015-2024 Nautech Systems Pty Ltd. All rights reserved.
+//  https://nautechsystems.io
+//
+//  Licensed under the GNU Lesser General Public License Version 3.0 (the "License");
+//  You may not use this file except in compliance with the License.
+//  You may obtain a copy of the License at https://www.gnu.org/licenses/lgpl-3.0.en.html
+//
+//  Unless required by applicable law or agreed to in writing, software
+//  distributed under the License is distributed on an "AS IS" BASIS,
+//  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+//  See the License for the specific language governing permissions and
+//  limitations under the License.
+// -------------------------------------------------------------------------------------------------
+
+//! Events for the trading domain model.
+
+pub mod account;
+pub mod order;
+pub mod position;
```

### Comparing `nautilus_trader-1.193.0/nautilus_trader/trading/__init__.py` & `nautilus_trader-1.194.0/nautilus_trader/trading/__init__.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/trading/config.py` & `nautilus_trader-1.194.0/nautilus_trader/trading/config.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/trading/controller.py` & `nautilus_trader-1.194.0/nautilus_trader/trading/controller.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/trading/filters.py` & `nautilus_trader-1.194.0/nautilus_trader/trading/filters.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/trading/strategy.pxd` & `nautilus_trader-1.194.0/nautilus_trader/trading/strategy.pxd`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/trading/strategy.pyx` & `nautilus_trader-1.194.0/nautilus_trader/trading/strategy.pyx`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/nautilus_trader/trading/trader.py` & `nautilus_trader-1.194.0/nautilus_trader/trading/trader.py`

 * *Files identical despite different names*

### Comparing `nautilus_trader-1.193.0/pyproject.toml` & `nautilus_trader-1.194.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautilus_trader"
-version = "1.193.0"
+version = "1.194.0"
 description = "A high-performance algorithmic trading platform and event-driven backtester"
 authors = ["Nautech Systems <info@nautechsystems.io>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://nautilustrader.io"
 repository = "https://github.com/nautechsystems/nautilus_trader"
 classifiers = [
@@ -79,24 +79,24 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.4.2"
 docformatter = "^1.7.5"
 mypy = "^1.10.0"
 pandas-stubs = "^2.2.2"
 pre-commit = "^3.7.1"
-ruff = "^0.4.5"
+ruff = "^0.4.6"
 types-pytz = "^2023.3"
 types-requests = "^2.31"
 types-toml = "^0.10.2"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-coverage = "^7.5.1"
+coverage = "^7.5.3"
 pytest = "^7.4.4"
 pytest-aiohttp = "^1.0.5"
 pytest-asyncio = "==0.21.1"  # Pinned due Cython: cannot set '__pytest_asyncio_scoped_event_loop' attribute of immutable type
 pytest-benchmark = "^4.0.0"
 pytest-cov = "^4.1.0"
 pytest-mock = "^3.14.0"
 pytest-xdist = { version = "^3.6.1", extras = ["psutil"] }
```

### Comparing `nautilus_trader-1.193.0/PKG-INFO` & `nautilus_trader-1.194.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautilus_trader
-Version: 1.193.0
+Version: 1.194.0
 Summary: A high-performance algorithmic trading platform and event-driven backtester
 Home-page: https://nautilustrader.io
 License: LGPL-3.0-or-later
 Author: Nautech Systems
 Author-email: info@nautechsystems.io
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
@@ -85,38 +85,38 @@
 
 The platform is also universal and asset class agnostic - with any REST, WebSocket or FIX API able to be integrated via modular
 adapters. Thus, it can handle high-frequency trading operations for any asset classes
 including FX, Equities, Futures, Options, CFDs, Crypto and Betting - across multiple venues simultaneously.
 
 ## Features
 
-- **Fast** - Core written in Rust with asynchronous networking using [tokio](https://crates.io/crates/tokio)
-- **Reliable** - Type safety and thread safety through Rust. Redis backed performant state persistence
-- **Portable** - OS independent, runs on Linux, macOS, Windows. Deploy using Docker
-- **Flexible** - Modular adapters mean any REST, WebSocket, or FIX API can be integrated
-- **Advanced** - Time in force `IOC`, `FOK`, `GTD`, `AT_THE_OPEN`, `AT_THE_CLOSE`, advanced order types and conditional triggers. Execution instructions `post-only`, `reduce-only`, and icebergs. Contingency order lists including `OCO`, `OTO`
-- **Customizable** - Add user defined custom components, or assemble entire systems from scratch leveraging the cache and message bus
-- **Backtesting** - Run with multiple venues, instruments and strategies simultaneously using historical quote tick, trade tick, bar, order book and custom data with nanosecond resolution
-- **Live** - Use identical strategy implementations between backtesting and live deployments
-- **Multi-venue** - Multiple venue capabilities facilitate market making and statistical arbitrage strategies
-- **AI Agent Training** - Backtest engine fast enough to be used to train AI trading agents (RL/ES)
+- **Fast:** Core written in Rust with asynchronous networking using [tokio](https://crates.io/crates/tokio)
+- **Reliable:** Type safety and thread safety through Rust. Redis backed performant state persistence
+- **Portable:** OS independent, runs on Linux, macOS, Windows. Deploy using Docker
+- **Flexible:** Modular adapters mean any REST, WebSocket, or FIX API can be integrated
+- **Advanced:** Time in force `IOC`, `FOK`, `GTD`, `AT_THE_OPEN`, `AT_THE_CLOSE`, advanced order types and conditional triggers. Execution instructions `post-only`, `reduce-only`, and icebergs. Contingency order lists including `OCO`, `OTO`
+- **Customizable:** Add user defined custom components, or assemble entire systems from scratch leveraging the cache and message bus
+- **Backtesting:** Run with multiple venues, instruments and strategies simultaneously using historical quote tick, trade tick, bar, order book and custom data with nanosecond resolution
+- **Live:** Use identical strategy implementations between backtesting and live deployments
+- **Multi-venue:** Multiple venue capabilities facilitate market making and statistical arbitrage strategies
+- **AI Training:** Backtest engine fast enough to be used to train AI trading agents (RL/ES)
 
 ![Alt text](https://github.com/nautechsystems/nautilus_trader/blob/develop/docs/_images/nautilus-art.png?raw=true "nautilus")
 
 > _nautilus - from ancient Greek 'sailor' and naus 'ship'._
 >
 > _The nautilus shell consists of modular chambers with a growth factor which approximates a logarithmic spiral.
 > The idea is that this can be translated to the aesthetics of design and architecture._
 
 ## Why NautilusTrader?
 
-- **Highly performant event-driven Python** - native binary core components
-- **Parity between backtesting and live trading** - identical strategy code
-- **Reduced operational risk** - risk management functionality, logical correctness and type safety
-- **Highly extendable** - message bus, custom components and actors, custom data, custom adapters
+- **Highly performant event-driven Python:** Native binary core components
+- **Parity between backtesting and live trading:** Identical strategy code
+- **Reduced operational risk:** Risk management functionality, logical correctness and type safety
+- **Highly extendable:** Message bus, custom components and actors, custom data, custom adapters
 
 Traditionally, trading strategy research and backtesting might be conducted in Python (or other suitable language)
 using vectorized methods, with the strategy then needing to be reimplemented in a more event-drive way
 using C++, C#, Java or other statically typed language(s). The reasoning here is that vectorized backtesting code cannot
 express the granular time and event dependent complexity of real-time trading, where compiled languages have
 proven to be more suitable due to their inherently higher performance, and type safety.
 
@@ -171,16 +171,16 @@
 | [Binance](https://binance.com)                            | `BINANCE`             | Crypto Exchange (CEX)   | ![status](https://img.shields.io/badge/stable-green)    | [Guide](https://docs.nautilustrader.io/integrations/binance.html)   |
 | [Binance US](https://binance.us)                          | `BINANCE`             | Crypto Exchange (CEX)   | ![status](https://img.shields.io/badge/stable-green)    | [Guide](https://docs.nautilustrader.io/integrations/binance.html)   |
 | [Binance Futures](https://www.binance.com/en/futures)     | `BINANCE`             | Crypto Exchange (CEX)   | ![status](https://img.shields.io/badge/stable-green)    | [Guide](https://docs.nautilustrader.io/integrations/binance.html)   |
 | [Bybit](https://www.bybit.com)                            | `BYBIT`               | Crypto Exchange (CEX)   | ![status](https://img.shields.io/badge/beta-yellow)     | [Guide](https://docs.nautilustrader.io/integrations/bybit.html)     |
 | [Databento](https://databento.com)                        | `DATABENTO`           | Data Provider           | ![status](https://img.shields.io/badge/beta-yellow)     | [Guide](https://docs.nautilustrader.io/integrations/databento.html) |
 | [Interactive Brokers](https://www.interactivebrokers.com) | `INTERACTIVE_BROKERS` | Brokerage (multi-venue) | ![status](https://img.shields.io/badge/stable-green)    | [Guide](https://docs.nautilustrader.io/integrations/ib.html)        |
 
-- `ID:` The default client ID for the integrations adapter clients
-- `Type:` The type of integration (often the venue type)
+- **ID:** The default client ID for the integrations adapter clients
+- **Type:** The type of integration (often the venue type)
 
 ### Status
 - `building` - Under construction and likely not in a usable state
 - `beta` - Completed to a minimally working state and in a 'beta' testing phase
 - `stable` - Stabilized feature set and API, the integration has been tested by both developers and users to a reasonable level (some bugs may still remain)
 
 Refer to the [Integrations](https://docs.nautilustrader.io/integrations/index.html) documentation for further details.
@@ -238,27 +238,31 @@
    cd nautilus_trader
    poetry install --only main --all-extras
 
 Refer to the [Installation Guide](https://docs.nautilustrader.io/getting_started/installation.html) for other options and further details.
 
 ## Versioning and releases
 
-NautilusTrader is currently following a bi-weekly beta release schedule.
+NautilusTrader is currently targeting a weekly release schedule, occasionally there may be experimental
+or larger features which will delay a release by several weeks.
+
 The API is becoming more stable, however breaking changes are still possible between releases.
 Documentation of these changes in the release notes are made on a best-effort basis.
 
 ### Branches
 
+We aim to maintain a stable passing build on all branches.
+
 - `master` branch will always reflect the source code for the latest released version
 - `nightly` branch may contain experimental features and is generally merged from `develop` branch daily, and also when required
-- `develop` branch is normally very active with frequent commits and may contain experimental features. We aim to maintain a stable
-  passing build on this branch
+- `develop` branch is normally very active with frequent commits and may contain experimental features
 
-The current roadmap has a goal of achieving a stable API for a `2.x` version. From this
-point we will follow a formal process for releases, with deprecation periods for any API changes.
+The current roadmap has a goal of achieving a stable API for a `2.x` version (likely post Rust port).
+From this point we will follow a formal process for releases, with deprecation periods for any API changes.
+This allows us to maintain a maximum pace of development for now.
 
 ## Makefile
 
 A `Makefile` is provided to automate most installation and build tasks for development. It provides the following targets:
 
 - `make install` -- Installs in `release` build mode with `main`, `dev` and `test` dependencies then installs the package using poetry (default)
 - `make install-debug` -- Same as `make install` but with `debug` build mode
```

