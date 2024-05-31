# Comparing `tmp/glean_sdk-60.2.0.tar.gz` & `tmp/glean_sdk-60.3.0.tar.gz`

## Comparing `glean_sdk-60.2.0.tar` & `glean_sdk-60.3.0.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0     1001     1002     1893 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/Cargo.toml
--rw-r--r--   0     1001     1002    16725 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/LICENSE
--rw-r--r--   0     1001     1002     1699 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/README.md
--rw-r--r--   0     1001     1002       76 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/build.rs
--rw-r--r--   0     1001     1002     4699 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/common_metric_data.rs
--rw-r--r--   0     1001     1002    37130 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/core/mod.rs
--rw-r--r--   0     1001     1002     7409 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/core_metrics.rs
--rw-r--r--   0     1001     1002     1776 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/coverage.rs
--rw-r--r--   0     1001     1002    66424 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/database/mod.rs
--rw-r--r--   0     1001     1002    10907 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/debug.rs
--rw-r--r--   0     1001     1002     7202 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/dispatcher/global.rs
--rw-r--r--   0     1001     1002    19263 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/dispatcher/mod.rs
--rw-r--r--   0     1001     1002     4755 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/error.rs
--rw-r--r--   0     1001     1002     8335 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/error_recording.rs
--rw-r--r--   0     1001     1002    48891 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/event_database/mod.rs
--rw-r--r--   0     1001     1002     2603 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/fd_logger.rs
--rw-r--r--   0     1001     1002    18756 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/glean.udl
--rw-r--r--   0     1001     1002      899 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/glean_metrics.rs
--rw-r--r--   0     1001     1002     6938 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/histogram/exponential.rs
--rw-r--r--   0     1001     1002     5764 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/histogram/functional.rs
--rw-r--r--   0     1001     1002     5770 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/histogram/linear.rs
--rw-r--r--   0     1001     1002     3930 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/histogram/mod.rs
--rw-r--r--   0     1001     1002    10750 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/internal_metrics.rs
--rw-r--r--   0     1001     1002     2534 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/internal_pings.rs
--rw-r--r--   0     1001     1002    47787 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/lib.rs
--rw-r--r--   0     1001     1002    41878 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/lib_unit_tests.rs
--rw-r--r--   0     1001     1002     4061 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/boolean.rs
--rw-r--r--   0     1001     1002     5241 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/counter.rs
--rw-r--r--   0     1001     1002     8437 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/custom_distribution.rs
--rw-r--r--   0     1001     1002    10449 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/datetime.rs
--rw-r--r--   0     1001     1002     4572 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/denominator.rs
--rw-r--r--   0     1001     1002     7478 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/event.rs
--rw-r--r--   0     1001     1002     9850 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/experiment.rs
--rw-r--r--   0     1001     1002     9862 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/labeled.rs
--rw-r--r--   0     1001     1002     9793 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/memory_distribution.rs
--rw-r--r--   0     1001     1002     1809 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/memory_unit.rs
--rw-r--r--   0     1001     1002    12047 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/mod.rs
--rw-r--r--   0     1001     1002     2959 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/numerator.rs
--rw-r--r--   0     1001     1002     5239 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/object.rs
--rw-r--r--   0     1001     1002    11699 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/ping.rs
--rw-r--r--   0     1001     1002     3818 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/quantity.rs
--rw-r--r--   0     1001     1002     5963 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/rate.rs
--rw-r--r--   0     1001     1002     1573 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/recorded_experiment.rs
--rw-r--r--   0     1001     1002     1797 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/remote_settings_config.rs
--rw-r--r--   0     1001     1002     5363 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/string.rs
--rw-r--r--   0     1001     1002     6514 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/string_list.rs
--rw-r--r--   0     1001     1002     5544 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/text.rs
--rw-r--r--   0     1001     1002     3768 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/time_unit.rs
--rw-r--r--   0     1001     1002    10380 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/timespan.rs
--rw-r--r--   0     1001     1002    21230 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/timing_distribution.rs
--rw-r--r--   0     1001     1002    10222 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/url.rs
--rw-r--r--   0     1001     1002     5063 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/metrics/uuid.rs
--rw-r--r--   0     1001     1002    15471 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/ping/mod.rs
--rw-r--r--   0     1001     1002    23631 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/scheduler.rs
--rw-r--r--   0     1001     1002     9495 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/storage/mod.rs
--rw-r--r--   0     1001     1002     2856 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/system.rs
--rw-r--r--   0     1001     1002     1380 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/boolean.rs
--rw-r--r--   0     1001     1002     1497 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/counter.rs
--rw-r--r--   0     1001     1002     2615 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/custom_distribution.rs
--rw-r--r--   0     1001     1002     1759 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/datetime.rs
--rw-r--r--   0     1001     1002     3788 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/event.rs
--rw-r--r--   0     1001     1002     1519 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/labeled.rs
--rw-r--r--   0     1001     1002     1804 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/memory_distribution.rs
--rw-r--r--   0     1001     1002     1642 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/mod.rs
--rw-r--r--   0     1001     1002     1584 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/numerator.rs
--rw-r--r--   0     1001     1002     1730 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/object.rs
--rw-r--r--   0     1001     1002      665 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/ping.rs
--rw-r--r--   0     1001     1002     1481 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/quantity.rs
--rw-r--r--   0     1001     1002     1823 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/rate.rs
--rw-r--r--   0     1001     1002     1574 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/string.rs
--rw-r--r--   0     1001     1002     1971 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/string_list.rs
--rw-r--r--   0     1001     1002     1568 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/text.rs
--rw-r--r--   0     1001     1002     2403 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/timespan.rs
--rw-r--r--   0     1001     1002     6069 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/timing_distribution.rs
--rw-r--r--   0     1001     1002     1645 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/url.rs
--rw-r--r--   0     1001     1002     1528 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/traits/uuid.rs
--rw-r--r--   0     1001     1002    16472 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/upload/directory.rs
--rw-r--r--   0     1001     1002    68645 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/upload/mod.rs
--rw-r--r--   0     1001     1002     3830 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/upload/policy.rs
--rw-r--r--   0     1001     1002    10852 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/upload/request.rs
--rw-r--r--   0     1001     1002     3150 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/upload/result.rs
--rw-r--r--   0     1001     1002    10750 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/src/util.rs
--rw-r--r--   0     1001     1002     2829 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/boolean.rs
--rw-r--r--   0     1001     1002     5373 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/common/mod.rs
--rw-r--r--   0     1001     1002     5294 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/counter.rs
--rw-r--r--   0     1001     1002    13398 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/custom_distribution.rs
--rw-r--r--   0     1001     1002     5974 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/datetime.rs
--rw-r--r--   0     1001     1002    16375 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/event.rs
--rw-r--r--   0     1001     1002    14418 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/labeled.rs
--rw-r--r--   0     1001     1002     5865 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/memory_distribution.rs
--rw-r--r--   0     1001     1002     3195 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/object.rs
--rw-r--r--   0     1001     1002     8742 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/ping.rs
--rw-r--r--   0     1001     1002    10630 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/ping_maker.rs
--rw-r--r--   0     1001     1002     3611 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/quantity.rs
--rw-r--r--   0     1001     1002     4058 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/rate.rs
--rw-r--r--   0     1001     1002     3314 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/storage.rs
--rw-r--r--   0     1001     1002     3730 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/string.rs
--rw-r--r--   0     1001     1002     7423 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/string_list.rs
--rw-r--r--   0     1001     1002     3470 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/text.rs
--rw-r--r--   0     1001     1002    10155 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/timespan.rs
--rw-r--r--   0     1001     1002    12973 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/timing_distribution.rs
--rw-r--r--   0     1001     1002     3375 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/tests/uuid.rs
--rw-r--r--   0     1001     1002      205 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/uniffi.toml
--rw-r--r--   0     1001     1002      299 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/tools/embedded-uniffi-bindgen/Cargo.toml
--rw-r--r--   0     1001     1002     1902 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/tools/embedded-uniffi-bindgen/README.md
--rw-r--r--   0     1001     1002       67 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/tools/embedded-uniffi-bindgen/src/lib.rs
--rw-r--r--   0     1001     1002     2571 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/tools/embedded-uniffi-bindgen/src/main.rs
--rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 glean_sdk-60.2.0/glean-core/bundle/Cargo.toml
--rw-r--r--   0     1001     1002    18756 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/bundle/src/glean.udl
--rw-r--r--   0     1001     1002      973 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/bundle/src/lib.rs
--rw-r--r--   0     1001     1002      205 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/bundle/uniffi.toml
--rw-r--r--   0     1001     1002    32669 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/Cargo.lock
--rw-r--r--   0        0        0      208 1970-01-01 00:00:00.000000 glean_sdk-60.2.0/Cargo.toml
--rw-r--r--   0     1001     1002     1209 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/pyproject.toml
--rw-r--r--   0     1001     1002     1479 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/__init__.py
--rw-r--r--   0     1001     1002      585 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/_builtins.py
--rw-r--r--   0     1001     1002     1698 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/_ffi.py
--rw-r--r--   0     1001     1002    12757 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/_loader.py
--rw-r--r--   0     1001     1002     5161 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/_process_dispatcher.py
--rw-r--r--   0     1001     1002      199 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/_subprocess/__init__.py
--rw-r--r--   0     1001     1002     1336 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/_subprocess/_process_dispatcher_helper.py
--rw-r--r--   0     1001     1002     1502 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/_util.py
--rw-r--r--   0     1001     1002     4278 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/config.py
--rw-r--r--   0     1001     1002    16012 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/glean.py
--rw-r--r--   0     1001     1002    23717 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics.yaml
--rw-r--r--   0     1001     1002     2034 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/__init__.py
--rw-r--r--   0     1001     1002     3803 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/datetime.py
--rw-r--r--   0     1001     1002     3289 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/event.py
--rw-r--r--   0     1001     1002     3225 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/labeled.py
--rw-r--r--   0     1001     1002     3402 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/object.py
--rw-r--r--   0     1001     1002     2408 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/ping.py
--rw-r--r--   0     1001     1002     1576 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/string.py
--rw-r--r--   0     1001     1002     4395 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/timespan.py
--rw-r--r--   0     1001     1002     5030 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/timing_distribution.py
--rw-r--r--   0     1001     1002     1628 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/url.py
--rw-r--r--   0     1001     1002     1757 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/metrics/uuid.py
--rw-r--r--   0     1001     1002      522 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/net/__init__.py
--rw-r--r--   0     1001     1002     1569 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/net/base_uploader.py
--rw-r--r--   0     1001     1002     3211 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/net/http_client.py
--rw-r--r--   0     1001     1002     5230 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/net/ping_upload_worker.py
--rw-r--r--   0     1001     1002     1068 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/net/ping_uploader.py
--rw-r--r--   0     1001     1002     5383 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/pings.yaml
--rw-r--r--   0     1001     1002     2883 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/glean-core/python/glean/testing/__init__.py
--rw-r--r--   0     1001     1002     3773 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/README.md
--rw-r--r--   0     1001     1002    16725 2024-05-23 16:56:35.000000 glean_sdk-60.2.0/LICENSE
--rw-r--r--   0        0        0     4703 1970-01-01 00:00:00.000000 glean_sdk-60.2.0/PKG-INFO
+-rw-r--r--   0     1001     1002      299 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/tools/embedded-uniffi-bindgen/Cargo.toml
+-rw-r--r--   0     1001     1002     1902 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/tools/embedded-uniffi-bindgen/README.md
+-rw-r--r--   0     1001     1002       67 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/tools/embedded-uniffi-bindgen/src/lib.rs
+-rw-r--r--   0     1001     1002     2571 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/tools/embedded-uniffi-bindgen/src/main.rs
+-rw-r--r--   0     1001     1002     1893 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/Cargo.toml
+-rw-r--r--   0     1001     1002    16725 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/LICENSE
+-rw-r--r--   0     1001     1002     1699 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/README.md
+-rw-r--r--   0     1001     1002       76 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/build.rs
+-rw-r--r--   0     1001     1002     4699 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/common_metric_data.rs
+-rw-r--r--   0     1001     1002    37130 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/core/mod.rs
+-rw-r--r--   0     1001     1002     7409 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/core_metrics.rs
+-rw-r--r--   0     1001     1002     1776 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/coverage.rs
+-rw-r--r--   0     1001     1002    68925 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/database/mod.rs
+-rw-r--r--   0     1001     1002    10907 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/debug.rs
+-rw-r--r--   0     1001     1002     7202 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/dispatcher/global.rs
+-rw-r--r--   0     1001     1002    19263 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/dispatcher/mod.rs
+-rw-r--r--   0     1001     1002     4755 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/error.rs
+-rw-r--r--   0     1001     1002     8335 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/error_recording.rs
+-rw-r--r--   0     1001     1002    48891 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/event_database/mod.rs
+-rw-r--r--   0     1001     1002     2603 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/fd_logger.rs
+-rw-r--r--   0     1001     1002    18802 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/glean.udl
+-rw-r--r--   0     1001     1002      899 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/glean_metrics.rs
+-rw-r--r--   0     1001     1002     6938 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/histogram/exponential.rs
+-rw-r--r--   0     1001     1002     5764 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/histogram/functional.rs
+-rw-r--r--   0     1001     1002     5770 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/histogram/linear.rs
+-rw-r--r--   0     1001     1002     3930 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/histogram/mod.rs
+-rw-r--r--   0     1001     1002    10750 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/internal_metrics.rs
+-rw-r--r--   0     1001     1002     2534 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/internal_pings.rs
+-rw-r--r--   0     1001     1002    47996 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/lib.rs
+-rw-r--r--   0     1001     1002    41878 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/lib_unit_tests.rs
+-rw-r--r--   0     1001     1002     4061 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/boolean.rs
+-rw-r--r--   0     1001     1002     5241 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/counter.rs
+-rw-r--r--   0     1001     1002     8437 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/custom_distribution.rs
+-rw-r--r--   0     1001     1002    10449 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/datetime.rs
+-rw-r--r--   0     1001     1002     4572 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/denominator.rs
+-rw-r--r--   0     1001     1002     7478 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/event.rs
+-rw-r--r--   0     1001     1002     9850 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/experiment.rs
+-rw-r--r--   0     1001     1002     9862 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/labeled.rs
+-rw-r--r--   0     1001     1002     9793 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/memory_distribution.rs
+-rw-r--r--   0     1001     1002     1809 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/memory_unit.rs
+-rw-r--r--   0     1001     1002    12047 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/mod.rs
+-rw-r--r--   0     1001     1002     2959 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/numerator.rs
+-rw-r--r--   0     1001     1002     5239 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/object.rs
+-rw-r--r--   0     1001     1002    11699 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/ping.rs
+-rw-r--r--   0     1001     1002     3818 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/quantity.rs
+-rw-r--r--   0     1001     1002     5963 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/rate.rs
+-rw-r--r--   0     1001     1002     1573 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/recorded_experiment.rs
+-rw-r--r--   0     1001     1002     1797 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/remote_settings_config.rs
+-rw-r--r--   0     1001     1002     5363 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/string.rs
+-rw-r--r--   0     1001     1002     6514 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/string_list.rs
+-rw-r--r--   0     1001     1002     5544 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/text.rs
+-rw-r--r--   0     1001     1002     3768 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/time_unit.rs
+-rw-r--r--   0     1001     1002    10380 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/timespan.rs
+-rw-r--r--   0     1001     1002    21230 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/timing_distribution.rs
+-rw-r--r--   0     1001     1002    10222 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/url.rs
+-rw-r--r--   0     1001     1002     5063 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/metrics/uuid.rs
+-rw-r--r--   0     1001     1002    15471 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/ping/mod.rs
+-rw-r--r--   0     1001     1002    23631 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/scheduler.rs
+-rw-r--r--   0     1001     1002     9495 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/storage/mod.rs
+-rw-r--r--   0     1001     1002     2856 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/system.rs
+-rw-r--r--   0     1001     1002     1380 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/boolean.rs
+-rw-r--r--   0     1001     1002     1497 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/counter.rs
+-rw-r--r--   0     1001     1002     2615 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/custom_distribution.rs
+-rw-r--r--   0     1001     1002     1759 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/datetime.rs
+-rw-r--r--   0     1001     1002     3788 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/event.rs
+-rw-r--r--   0     1001     1002     1519 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/labeled.rs
+-rw-r--r--   0     1001     1002     1804 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/memory_distribution.rs
+-rw-r--r--   0     1001     1002     1642 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/mod.rs
+-rw-r--r--   0     1001     1002     1584 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/numerator.rs
+-rw-r--r--   0     1001     1002     1730 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/object.rs
+-rw-r--r--   0     1001     1002      665 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/ping.rs
+-rw-r--r--   0     1001     1002     1481 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/quantity.rs
+-rw-r--r--   0     1001     1002     1823 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/rate.rs
+-rw-r--r--   0     1001     1002     1574 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/string.rs
+-rw-r--r--   0     1001     1002     1971 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/string_list.rs
+-rw-r--r--   0     1001     1002     1568 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/text.rs
+-rw-r--r--   0     1001     1002     2403 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/timespan.rs
+-rw-r--r--   0     1001     1002     6069 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/timing_distribution.rs
+-rw-r--r--   0     1001     1002     1645 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/url.rs
+-rw-r--r--   0     1001     1002     1528 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/traits/uuid.rs
+-rw-r--r--   0     1001     1002    16472 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/upload/directory.rs
+-rw-r--r--   0     1001     1002    68645 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/upload/mod.rs
+-rw-r--r--   0     1001     1002     3830 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/upload/policy.rs
+-rw-r--r--   0     1001     1002    10852 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/upload/request.rs
+-rw-r--r--   0     1001     1002     3150 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/upload/result.rs
+-rw-r--r--   0     1001     1002    10750 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/src/util.rs
+-rw-r--r--   0     1001     1002     2829 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/boolean.rs
+-rw-r--r--   0     1001     1002     5373 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/common/mod.rs
+-rw-r--r--   0     1001     1002     5294 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/counter.rs
+-rw-r--r--   0     1001     1002    13398 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/custom_distribution.rs
+-rw-r--r--   0     1001     1002     5974 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/datetime.rs
+-rw-r--r--   0     1001     1002    16375 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/event.rs
+-rw-r--r--   0     1001     1002    14418 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/labeled.rs
+-rw-r--r--   0     1001     1002     5865 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/memory_distribution.rs
+-rw-r--r--   0     1001     1002     3195 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/object.rs
+-rw-r--r--   0     1001     1002     8742 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/ping.rs
+-rw-r--r--   0     1001     1002    10630 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/ping_maker.rs
+-rw-r--r--   0     1001     1002     3611 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/quantity.rs
+-rw-r--r--   0     1001     1002     4058 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/rate.rs
+-rw-r--r--   0     1001     1002     3314 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/storage.rs
+-rw-r--r--   0     1001     1002     3730 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/string.rs
+-rw-r--r--   0     1001     1002     7423 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/string_list.rs
+-rw-r--r--   0     1001     1002     3470 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/text.rs
+-rw-r--r--   0     1001     1002    10155 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/timespan.rs
+-rw-r--r--   0     1001     1002    12973 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/timing_distribution.rs
+-rw-r--r--   0     1001     1002     3375 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/tests/uuid.rs
+-rw-r--r--   0     1001     1002      205 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/uniffi.toml
+-rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 glean_sdk-60.3.0/glean-core/bundle/Cargo.toml
+-rw-r--r--   0     1001     1002    18802 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/bundle/src/glean.udl
+-rw-r--r--   0     1001     1002      973 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/bundle/src/lib.rs
+-rw-r--r--   0     1001     1002      205 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/bundle/uniffi.toml
+-rw-r--r--   0     1001     1002    32669 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/Cargo.lock
+-rw-r--r--   0        0        0      208 1970-01-01 00:00:00.000000 glean_sdk-60.3.0/Cargo.toml
+-rw-r--r--   0     1001     1002     1209 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/pyproject.toml
+-rw-r--r--   0     1001     1002     1479 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/__init__.py
+-rw-r--r--   0     1001     1002      585 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/_builtins.py
+-rw-r--r--   0     1001     1002     1698 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/_ffi.py
+-rw-r--r--   0     1001     1002    12757 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/_loader.py
+-rw-r--r--   0     1001     1002     5161 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/_process_dispatcher.py
+-rw-r--r--   0     1001     1002      199 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/_subprocess/__init__.py
+-rw-r--r--   0     1001     1002     1336 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/_subprocess/_process_dispatcher_helper.py
+-rw-r--r--   0     1001     1002     1502 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/_util.py
+-rw-r--r--   0     1001     1002     4278 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/config.py
+-rw-r--r--   0     1001     1002    16012 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/glean.py
+-rw-r--r--   0     1001     1002    23717 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/metrics.yaml
+-rw-r--r--   0     1001     1002     2034 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/metrics/__init__.py
+-rw-r--r--   0     1001     1002     3803 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/metrics/datetime.py
+-rw-r--r--   0     1001     1002     3289 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/metrics/event.py
+-rw-r--r--   0     1001     1002     3225 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/metrics/labeled.py
+-rw-r--r--   0     1001     1002     3402 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/metrics/object.py
+-rw-r--r--   0     1001     1002     2408 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/metrics/ping.py
+-rw-r--r--   0     1001     1002     1576 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/metrics/string.py
+-rw-r--r--   0     1001     1002     4395 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/metrics/timespan.py
+-rw-r--r--   0     1001     1002     5030 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/metrics/timing_distribution.py
+-rw-r--r--   0     1001     1002     1628 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/metrics/url.py
+-rw-r--r--   0     1001     1002     1757 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/metrics/uuid.py
+-rw-r--r--   0     1001     1002      522 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/net/__init__.py
+-rw-r--r--   0     1001     1002     1569 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/net/base_uploader.py
+-rw-r--r--   0     1001     1002     3211 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/net/http_client.py
+-rw-r--r--   0     1001     1002     5230 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/net/ping_upload_worker.py
+-rw-r--r--   0     1001     1002     1068 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/net/ping_uploader.py
+-rw-r--r--   0     1001     1002     5383 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/pings.yaml
+-rw-r--r--   0     1001     1002     2883 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/glean-core/python/glean/testing/__init__.py
+-rw-r--r--   0     1001     1002     3773 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/README.md
+-rw-r--r--   0     1001     1002    16725 2024-05-31 12:11:27.000000 glean_sdk-60.3.0/LICENSE
+-rw-r--r--   0        0        0     4703 1970-01-01 00:00:00.000000 glean_sdk-60.3.0/PKG-INFO
```

### Comparing `glean_sdk-60.2.0/glean-core/Cargo.toml` & `glean_sdk-60.3.0/glean-core/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "glean-core"
-version = "60.2.0"
+version = "60.3.0"
 authors = ["Jan-Erik Rediger <jrediger@mozilla.com>", "The Glean Team <glean-team@mozilla.com>"]
 description = "A modern Telemetry library"
 repository = "https://github.com/mozilla/glean"
 readme = "README.md"
 license = "MPL-2.0"
 edition = "2021"
 keywords = ["telemetry"]
```

### Comparing `glean_sdk-60.2.0/glean-core/LICENSE` & `glean_sdk-60.3.0/glean-core/LICENSE`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/README.md` & `glean_sdk-60.3.0/glean-core/README.md`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/common_metric_data.rs` & `glean_sdk-60.3.0/glean-core/src/common_metric_data.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/core/mod.rs` & `glean_sdk-60.3.0/glean-core/src/core/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/core_metrics.rs` & `glean_sdk-60.3.0/glean-core/src/core_metrics.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/coverage.rs` & `glean_sdk-60.3.0/glean-core/src/coverage.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/database/mod.rs` & `glean_sdk-60.3.0/glean-core/src/database/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 use std::collections::btree_map::Entry;
 use std::collections::BTreeMap;
 use std::fs;
 use std::io;
 use std::num::NonZeroU64;
 use std::path::Path;
 use std::str;
+#[cfg(target_os = "android")]
+use std::sync::atomic::{AtomicUsize, Ordering};
 use std::sync::RwLock;
 
 use crate::ErrorKind;
 
 use rkv::migrator::Migrator;
 use rkv::{MigrateError, StoreError, StoreOptions};
 
@@ -163,14 +165,21 @@
 
 use crate::common_metric_data::CommonMetricDataInternal;
 use crate::metrics::Metric;
 use crate::Glean;
 use crate::Lifetime;
 use crate::Result;
 
+/// The number of writes we accept writes to the ping-lifetime in-memory map
+/// before data is flushed to disk.
+///
+/// Only considered if `delay_ping_lifetime_io` is set to `true`.
+#[cfg(target_os = "android")]
+const PING_LIFETIME_THRESHOLD: usize = 1000;
+
 pub struct Database {
     /// Handle to the database environment.
     rkv: Rkv,
 
     /// Handles to the "lifetime" stores.
     ///
     /// A "store" is a handle to the underlying database.
@@ -180,14 +189,22 @@
     application_store: SingleStore,
 
     /// If the `delay_ping_lifetime_io` Glean config option is `true`,
     /// we will save metrics with 'ping' lifetime data in a map temporarily
     /// so as to persist them to disk using rkv in bulk on demand.
     ping_lifetime_data: Option<RwLock<BTreeMap<String, Metric>>>,
 
+    /// A count of how many database writes have been done since the last ping-lifetime flush.
+    ///
+    /// A ping-lifetime flush is automatically done after `PING_LIFETIME_THRESHOLD` writes.
+    ///
+    /// Only relevant if `delay_ping_lifetime_io` is set to `true`,
+    #[cfg(target_os = "android")]
+    ping_lifetime_count: AtomicUsize,
+
     /// Initial file size when opening the database.
     file_size: Option<NonZeroU64>,
 
     /// RKV load state
     rkv_load_state: RkvLoadState,
 }
 
@@ -259,14 +276,16 @@
 
         let db = Self {
             rkv,
             user_store,
             ping_store,
             application_store,
             ping_lifetime_data,
+            #[cfg(target_os = "android")]
+            ping_lifetime_count: AtomicUsize::new(0),
             file_size,
             rkv_load_state,
         };
 
         db.load_ping_lifetime_data();
 
         Ok(db)
@@ -524,14 +543,17 @@
         // Glean has `delay_ping_lifetime_io` set to true
         if lifetime == Lifetime::Ping {
             if let Some(ping_lifetime_data) = &self.ping_lifetime_data {
                 let mut data = ping_lifetime_data
                     .write()
                     .expect("Can't read ping lifetime data");
                 data.insert(final_key, metric.clone());
+
+                // flush ping lifetime
+                self.persist_ping_lifetime_data_if_full(&data)?;
                 return Ok(());
             }
         }
 
         let encoded = bincode::serialize(&metric).expect("IMPOSSIBLE: Serializing metric failed");
         let value = rkv::Value::Blob(&encoded);
 
@@ -605,14 +627,17 @@
                         entry.insert(transform(None));
                     }
                     Entry::Occupied(mut entry) => {
                         let old_value = entry.get().clone();
                         entry.insert(transform(Some(old_value)));
                     }
                 }
+
+                // flush ping lifetime
+                self.persist_ping_lifetime_data_if_full(&data)?;
                 return Ok(());
             }
         }
 
         let mut writer = self.rkv.write()?;
         let store = self.get_store(lifetime);
         let new_value: Metric = {
@@ -798,14 +823,18 @@
     /// * This function will **not** panic on database errors.
     pub fn persist_ping_lifetime_data(&self) -> Result<()> {
         if let Some(ping_lifetime_data) = &self.ping_lifetime_data {
             let data = ping_lifetime_data
                 .read()
                 .expect("Can't read ping lifetime data");
 
+            // We can reset the write-counter. Current data has been persisted.
+            #[cfg(target_os = "android")]
+            self.ping_lifetime_count.store(0, Ordering::Release);
+
             self.write_with_store(Lifetime::Ping, |mut writer, store| {
                 for (key, value) in data.iter() {
                     let encoded =
                         bincode::serialize(&value).expect("IMPOSSIBLE: Serializing metric failed");
                     // There is no need for `get_storage_key` here because
                     // the key is already formatted from when it was saved
                     // to ping_lifetime_data.
@@ -813,14 +842,50 @@
                 }
                 writer.commit()?;
                 Ok(())
             })?;
         }
         Ok(())
     }
+
+    pub fn persist_ping_lifetime_data_if_full(
+        &self,
+        data: &BTreeMap<String, Metric>,
+    ) -> Result<()> {
+        #[cfg(target_os = "android")]
+        {
+            self.ping_lifetime_count.fetch_add(1, Ordering::Release);
+
+            let write_count = self.ping_lifetime_count.load(Ordering::Relaxed);
+            if write_count < PING_LIFETIME_THRESHOLD {
+                return Ok(());
+            }
+
+            self.ping_lifetime_count.store(0, Ordering::Release);
+            let write_result = self.write_with_store(Lifetime::Ping, |mut writer, store| {
+                for (key, value) in data.iter() {
+                    let encoded =
+                        bincode::serialize(&value).expect("IMPOSSIBLE: Serializing metric failed");
+                    // There is no need for `get_storage_key` here because
+                    // the key is already formatted from when it was saved
+                    // to ping_lifetime_data.
+                    store.put(&mut writer, key, &rkv::Value::Blob(&encoded))?;
+                }
+                writer.commit()?;
+                Ok(())
+            });
+
+            return write_result;
+        }
+        #[cfg(not(target_os = "android"))]
+        {
+            _ = data; // suppress unused_variables warning.
+            Ok(())
+        }
+    }
 }
 
 #[cfg(test)]
 mod test {
     use super::*;
     use crate::tests::new_glean;
     use std::collections::HashMap;
```

### Comparing `glean_sdk-60.2.0/glean-core/src/debug.rs` & `glean_sdk-60.3.0/glean-core/src/debug.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/dispatcher/global.rs` & `glean_sdk-60.3.0/glean-core/src/dispatcher/global.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/dispatcher/mod.rs` & `glean_sdk-60.3.0/glean-core/src/dispatcher/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/error.rs` & `glean_sdk-60.3.0/glean-core/src/error.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/error_recording.rs` & `glean_sdk-60.3.0/glean-core/src/error_recording.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/event_database/mod.rs` & `glean_sdk-60.3.0/glean-core/src/event_database/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/fd_logger.rs` & `glean_sdk-60.3.0/glean-core/src/fd_logger.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/glean.udl` & `glean_sdk-60.3.0/glean-core/src/glean.udl`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,16 @@
     // Server Knobs API
     void glean_apply_server_knobs_config(string json);
 
     boolean glean_set_debug_view_tag(string tag);
     boolean glean_set_source_tags(sequence<string> tags);
     void glean_set_log_pings(boolean value);
 
+    void glean_persist_ping_lifetime_data();
+
     void glean_handle_client_active();
     void glean_handle_client_inactive();
 
     void glean_submit_ping_by_name(string ping_name, optional string? reason = null);
     boolean glean_submit_ping_by_name_sync(string ping_name, optional string? reason = null);
 
     void glean_set_test_mode(boolean enabled);
```

### Comparing `glean_sdk-60.2.0/glean-core/src/glean_metrics.rs` & `glean_sdk-60.3.0/glean-core/src/glean_metrics.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/histogram/exponential.rs` & `glean_sdk-60.3.0/glean-core/src/histogram/exponential.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/histogram/functional.rs` & `glean_sdk-60.3.0/glean-core/src/histogram/functional.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/histogram/linear.rs` & `glean_sdk-60.3.0/glean-core/src/histogram/linear.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/histogram/mod.rs` & `glean_sdk-60.3.0/glean-core/src/histogram/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/internal_metrics.rs` & `glean_sdk-60.3.0/glean-core/src/internal_metrics.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/internal_pings.rs` & `glean_sdk-60.3.0/glean-core/src/internal_pings.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/lib.rs` & `glean_sdk-60.3.0/glean-core/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -693,15 +693,15 @@
     });
 }
 
 /// Asks the database to persist ping-lifetime data to disk. Probably expensive to call.
 /// Only has effect when Glean is configured with `delay_ping_lifetime_io: true`.
 /// If Glean hasn't been initialized this will dispatch and return Ok(()),
 /// otherwise it will block until the persist is done and return its Result.
-pub fn persist_ping_lifetime_data() {
+pub fn glean_persist_ping_lifetime_data() {
     // This is async, we can't get the Error back to the caller.
     crate::launch_with_glean(|glean| {
         let _ = glean.persist_ping_lifetime_data();
     });
 }
 
 fn initialize_core_metrics(glean: &Glean, client_info: &ClientInfoMetrics) {
@@ -1125,16 +1125,22 @@
         // Just because initialize was called doesn't mean it's done.
         join_init();
 
         dispatcher::reset_dispatcher();
 
         // Only useful if Glean initialization finished successfully
         // and set up the storage.
-        let has_storage =
-            core::with_opt_glean(|glean| glean.storage_opt().is_some()).unwrap_or(false);
+        let has_storage = core::with_opt_glean(|glean| {
+            // We need to flush the ping lifetime data before a full shutdown.
+            glean
+                .storage_opt()
+                .map(|storage| storage.persist_ping_lifetime_data())
+                .is_some()
+        })
+        .unwrap_or(false);
         if has_storage {
             uploader_shutdown();
         }
 
         if core::global_glean().is_some() {
             core::with_glean_mut(|glean| {
                 if clear_stores {
```

### Comparing `glean_sdk-60.2.0/glean-core/src/lib_unit_tests.rs` & `glean_sdk-60.3.0/glean-core/src/lib_unit_tests.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/boolean.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/boolean.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/counter.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/counter.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/custom_distribution.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/custom_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/datetime.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/datetime.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/denominator.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/denominator.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/event.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/event.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/experiment.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/experiment.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/labeled.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/labeled.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/memory_distribution.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/memory_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/memory_unit.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/memory_unit.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/mod.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/numerator.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/numerator.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/object.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/object.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/ping.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/ping.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/quantity.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/quantity.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/rate.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/rate.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/recorded_experiment.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/recorded_experiment.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/remote_settings_config.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/remote_settings_config.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/string.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/string.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/string_list.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/string_list.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/text.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/text.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/time_unit.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/time_unit.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/timespan.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/timespan.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/timing_distribution.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/timing_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/url.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/url.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/metrics/uuid.rs` & `glean_sdk-60.3.0/glean-core/src/metrics/uuid.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/ping/mod.rs` & `glean_sdk-60.3.0/glean-core/src/ping/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/scheduler.rs` & `glean_sdk-60.3.0/glean-core/src/scheduler.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/storage/mod.rs` & `glean_sdk-60.3.0/glean-core/src/storage/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/system.rs` & `glean_sdk-60.3.0/glean-core/src/system.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/boolean.rs` & `glean_sdk-60.3.0/glean-core/src/traits/boolean.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/counter.rs` & `glean_sdk-60.3.0/glean-core/src/traits/counter.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/custom_distribution.rs` & `glean_sdk-60.3.0/glean-core/src/traits/custom_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/datetime.rs` & `glean_sdk-60.3.0/glean-core/src/traits/datetime.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/event.rs` & `glean_sdk-60.3.0/glean-core/src/traits/event.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/labeled.rs` & `glean_sdk-60.3.0/glean-core/src/traits/labeled.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/memory_distribution.rs` & `glean_sdk-60.3.0/glean-core/src/traits/memory_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/mod.rs` & `glean_sdk-60.3.0/glean-core/src/traits/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/numerator.rs` & `glean_sdk-60.3.0/glean-core/src/traits/numerator.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/object.rs` & `glean_sdk-60.3.0/glean-core/src/traits/object.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/ping.rs` & `glean_sdk-60.3.0/glean-core/src/traits/ping.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/quantity.rs` & `glean_sdk-60.3.0/glean-core/src/traits/quantity.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/rate.rs` & `glean_sdk-60.3.0/glean-core/src/traits/rate.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/string.rs` & `glean_sdk-60.3.0/glean-core/src/traits/string.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/string_list.rs` & `glean_sdk-60.3.0/glean-core/src/traits/string_list.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/text.rs` & `glean_sdk-60.3.0/glean-core/src/traits/text.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/timespan.rs` & `glean_sdk-60.3.0/glean-core/src/traits/timespan.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/timing_distribution.rs` & `glean_sdk-60.3.0/glean-core/src/traits/timing_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/url.rs` & `glean_sdk-60.3.0/glean-core/src/traits/url.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/traits/uuid.rs` & `glean_sdk-60.3.0/glean-core/src/traits/uuid.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/upload/directory.rs` & `glean_sdk-60.3.0/glean-core/src/upload/directory.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/upload/mod.rs` & `glean_sdk-60.3.0/glean-core/src/upload/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/upload/policy.rs` & `glean_sdk-60.3.0/glean-core/src/upload/policy.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/upload/request.rs` & `glean_sdk-60.3.0/glean-core/src/upload/request.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/upload/result.rs` & `glean_sdk-60.3.0/glean-core/src/upload/result.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/src/util.rs` & `glean_sdk-60.3.0/glean-core/src/util.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/boolean.rs` & `glean_sdk-60.3.0/glean-core/tests/boolean.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/common/mod.rs` & `glean_sdk-60.3.0/glean-core/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/counter.rs` & `glean_sdk-60.3.0/glean-core/tests/counter.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/custom_distribution.rs` & `glean_sdk-60.3.0/glean-core/tests/custom_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/datetime.rs` & `glean_sdk-60.3.0/glean-core/tests/datetime.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/event.rs` & `glean_sdk-60.3.0/glean-core/tests/event.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/labeled.rs` & `glean_sdk-60.3.0/glean-core/tests/labeled.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/memory_distribution.rs` & `glean_sdk-60.3.0/glean-core/tests/memory_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/object.rs` & `glean_sdk-60.3.0/glean-core/tests/object.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/ping.rs` & `glean_sdk-60.3.0/glean-core/tests/ping.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/ping_maker.rs` & `glean_sdk-60.3.0/glean-core/tests/ping_maker.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/quantity.rs` & `glean_sdk-60.3.0/glean-core/tests/quantity.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/rate.rs` & `glean_sdk-60.3.0/glean-core/tests/rate.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/storage.rs` & `glean_sdk-60.3.0/glean-core/tests/storage.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/string.rs` & `glean_sdk-60.3.0/glean-core/tests/string.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/string_list.rs` & `glean_sdk-60.3.0/glean-core/tests/string_list.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/text.rs` & `glean_sdk-60.3.0/glean-core/tests/text.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/timespan.rs` & `glean_sdk-60.3.0/glean-core/tests/timespan.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/timing_distribution.rs` & `glean_sdk-60.3.0/glean-core/tests/timing_distribution.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/tests/uuid.rs` & `glean_sdk-60.3.0/glean-core/tests/uuid.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/tools/embedded-uniffi-bindgen/README.md` & `glean_sdk-60.3.0/tools/embedded-uniffi-bindgen/README.md`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/tools/embedded-uniffi-bindgen/src/main.rs` & `glean_sdk-60.3.0/tools/embedded-uniffi-bindgen/src/main.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/bundle/Cargo.toml` & `glean_sdk-60.3.0/glean-core/bundle/Cargo.toml`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/bundle/src/glean.udl` & `glean_sdk-60.3.0/glean-core/bundle/src/glean.udl`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,16 @@
     // Server Knobs API
     void glean_apply_server_knobs_config(string json);
 
     boolean glean_set_debug_view_tag(string tag);
     boolean glean_set_source_tags(sequence<string> tags);
     void glean_set_log_pings(boolean value);
 
+    void glean_persist_ping_lifetime_data();
+
     void glean_handle_client_active();
     void glean_handle_client_inactive();
 
     void glean_submit_ping_by_name(string ping_name, optional string? reason = null);
     boolean glean_submit_ping_by_name_sync(string ping_name, optional string? reason = null);
 
     void glean_set_test_mode(boolean enabled);
```

### Comparing `glean_sdk-60.2.0/glean-core/bundle/src/lib.rs` & `glean_sdk-60.3.0/glean-core/bundle/src/lib.rs`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/Cargo.lock` & `glean_sdk-60.3.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "glean"
-version = "60.2.0"
+version = "60.3.0"
 dependencies = [
  "crossbeam-channel",
  "env_logger",
  "flate2",
  "glean-core",
  "inherent",
  "jsonschema-valid",
@@ -355,15 +355,15 @@
 version = "1.0.0"
 dependencies = [
  "glean-core",
 ]
 
 [[package]]
 name = "glean-core"
-version = "60.2.0"
+version = "60.3.0"
 dependencies = [
  "android_logger",
  "bincode",
  "chrono",
  "crossbeam-channel",
  "ctor",
  "env_logger",
```

### Comparing `glean_sdk-60.2.0/pyproject.toml` & `glean_sdk-60.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "glean-sdk"
-version = "60.2.0"
+version = "60.3.0"
 requires-python = ">=3.8"
 classifiers = [
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: 3",
```

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/__init__.py` & `glean_sdk-60.3.0/glean-core/python/glean/__init__.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/_builtins.py` & `glean_sdk-60.3.0/glean-core/python/glean/_builtins.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/_ffi.py` & `glean_sdk-60.3.0/glean-core/python/glean/_ffi.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/_loader.py` & `glean_sdk-60.3.0/glean-core/python/glean/_loader.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/_process_dispatcher.py` & `glean_sdk-60.3.0/glean-core/python/glean/_process_dispatcher.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/_subprocess/_process_dispatcher_helper.py` & `glean_sdk-60.3.0/glean-core/python/glean/_subprocess/_process_dispatcher_helper.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/_util.py` & `glean_sdk-60.3.0/glean-core/python/glean/_util.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/config.py` & `glean_sdk-60.3.0/glean-core/python/glean/config.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/glean.py` & `glean_sdk-60.3.0/glean-core/python/glean/glean.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/metrics.yaml` & `glean_sdk-60.3.0/glean-core/python/glean/metrics.yaml`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/metrics/__init__.py` & `glean_sdk-60.3.0/glean-core/python/glean/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/metrics/datetime.py` & `glean_sdk-60.3.0/glean-core/python/glean/metrics/datetime.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/metrics/event.py` & `glean_sdk-60.3.0/glean-core/python/glean/metrics/event.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/metrics/labeled.py` & `glean_sdk-60.3.0/glean-core/python/glean/metrics/labeled.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/metrics/object.py` & `glean_sdk-60.3.0/glean-core/python/glean/metrics/object.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/metrics/ping.py` & `glean_sdk-60.3.0/glean-core/python/glean/metrics/ping.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/metrics/string.py` & `glean_sdk-60.3.0/glean-core/python/glean/metrics/string.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/metrics/timespan.py` & `glean_sdk-60.3.0/glean-core/python/glean/metrics/timespan.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/metrics/timing_distribution.py` & `glean_sdk-60.3.0/glean-core/python/glean/metrics/timing_distribution.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/metrics/url.py` & `glean_sdk-60.3.0/glean-core/python/glean/metrics/url.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/metrics/uuid.py` & `glean_sdk-60.3.0/glean-core/python/glean/metrics/uuid.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/net/__init__.py` & `glean_sdk-60.3.0/glean-core/python/glean/net/__init__.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/net/base_uploader.py` & `glean_sdk-60.3.0/glean-core/python/glean/net/base_uploader.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/net/http_client.py` & `glean_sdk-60.3.0/glean-core/python/glean/net/http_client.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/net/ping_upload_worker.py` & `glean_sdk-60.3.0/glean-core/python/glean/net/ping_upload_worker.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/net/ping_uploader.py` & `glean_sdk-60.3.0/glean-core/python/glean/net/ping_uploader.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/pings.yaml` & `glean_sdk-60.3.0/glean-core/python/glean/pings.yaml`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/glean-core/python/glean/testing/__init__.py` & `glean_sdk-60.3.0/glean-core/python/glean/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/README.md` & `glean_sdk-60.3.0/README.md`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/LICENSE` & `glean_sdk-60.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glean_sdk-60.2.0/PKG-INFO` & `glean_sdk-60.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: glean-sdk
-Version: 60.2.0
+Version: 60.3.0
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: semver >=2.13.0
 Requires-Dist: glean-parser ~=14.0
```

